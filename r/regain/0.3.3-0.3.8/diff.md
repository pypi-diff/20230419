# Comparing `tmp/regain-0.3.3.tar.gz` & `tmp/regain-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/regain-0.3.3.tar", last modified: Wed Jun 23 11:52:14 2021, max compression
+gzip compressed data, was "regain-0.3.8.tar", last modified: Wed Apr 19 10:38:40 2023, max compression
```

## Comparing `regain-0.3.3.tar` & `regain-0.3.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2021-06-23 11:50:10.000000 regain-0.3.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2021-06-23 11:50:10.000000 regain-0.3.3/AUTHORS.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2021-06-23 11:52:14.000000 regain-0.3.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5248 2021-06-23 11:50:10.000000 regain-0.3.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2021-06-23 11:52:14.000000 regain-0.3.3/regain.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-23 11:52:14.000000 regain-0.3.3/regain.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-06-23 11:52:14.000000 regain-0.3.3/regain.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2333 2021-06-23 11:52:14.000000 regain-0.3.3/regain.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2021-06-23 11:52:14.000000 regain-0.3.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1514 2021-06-23 11:50:10.000000 regain-0.3.3/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7790 2021-06-23 11:50:10.000000 regain-0.3.3/regain/discriminant_analysis.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/bayesian/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12233 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/wishart_process_.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3427 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/_laplace_approximation.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8907 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/wishart_distribution_.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15577 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/gwishart_inference.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9478 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/sampling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/gaussian_process_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3241 2021-06-23 11:50:10.000000 regain-0.3.3/regain/bayesian/stats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3154 2021-06-23 11:50:10.000000 regain-0.3.3/regain/clustering.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/generalized_linear_model/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9576 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/glm_poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25237 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/glm_time_ising.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6481 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/glm_gaussian.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1610 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10701 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/glm_ising.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25516 2021-06-23 11:50:10.000000 regain-0.3.3/regain/generalized_linear_model/glm_time_poisson.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1535 2021-06-23 11:50:10.000000 regain-0.3.3/regain/data/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2021-06-23 11:50:10.000000 regain-0.3.3/regain/data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/model_selection/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26850 2021-06-23 11:50:10.000000 regain-0.3.3/regain/model_selection/stability_optimization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10577 2021-06-23 11:50:10.000000 regain-0.3.3/regain/model_selection/_bayesian_optimization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2021-06-23 11:50:10.000000 regain-0.3.3/regain/model_selection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2511 2021-06-23 11:50:10.000000 regain-0.3.3/regain/norm.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/forward_backward/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5262 2021-06-23 11:50:10.000000 regain-0.3.3/regain/forward_backward/forward_backward.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18723 2021-06-23 11:50:10.000000 regain-0.3.3/regain/forward_backward/time_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1780 2021-06-23 11:50:10.000000 regain-0.3.3/regain/forward_backward/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2099 2021-06-23 11:50:10.000000 regain-0.3.3/regain/update_rules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20021 2021-06-23 11:50:10.000000 regain-0.3.3/regain/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/covariance/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16468 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/latent_time_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5755 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/infimal_convolution_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11364 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15147 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/latent_time_matrix_decomposition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18380 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/time_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10667 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/missing_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29328 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/kernel_latent_time_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1781 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10411 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/latent_graphical_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26753 2021-06-23 11:50:10.000000 regain-0.3.3/regain/covariance/kernel_time_graphical_lasso_.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/linear_model/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19554 2021-06-23 11:50:10.000000 regain-0.3.3/regain/linear_model/group_lasso_overlap_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5612 2021-06-23 11:50:10.000000 regain-0.3.3/regain/linear_model/_group_lasso_overlap_old_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4802 2021-06-23 11:50:10.000000 regain-0.3.3/regain/linear_model/lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5173 2021-06-23 11:50:10.000000 regain-0.3.3/regain/linear_model/group_lasso_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1642 2021-06-23 11:50:10.000000 regain-0.3.3/regain/linear_model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4617 2021-06-23 11:50:10.000000 regain-0.3.3/regain/validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11425 2021-06-23 11:50:10.000000 regain-0.3.3/regain/prox.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/plotting/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3096 2021-06-23 11:50:10.000000 regain-0.3.3/regain/plotting/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4062 2021-06-23 11:50:10.000000 regain-0.3.3/regain/plotting/covariance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2021-06-23 11:50:10.000000 regain-0.3.3/regain/plotting/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7514 2021-06-23 11:50:10.000000 regain-0.3.3/regain/plotting/results.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11999 2021-06-23 11:50:10.000000 regain-0.3.3/regain/plotting/plotly.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1583 2021-06-23 11:50:10.000000 regain-0.3.3/regain/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/datasets/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11777 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/ising.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23068 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/gaussian.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9356 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23439 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/kernels.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9742 2021-06-23 11:50:10.000000 regain-0.3.3/regain/datasets/multi_class.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/wrapper/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 11:52:14.000000 regain-0.3.3/regain/wrapper/paspal/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8148 2021-06-23 11:50:10.000000 regain-0.3.3/regain/wrapper/paspal/glopridu.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-23 11:50:10.000000 regain-0.3.3/regain/wrapper/paspal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5139 2021-06-23 11:50:10.000000 regain-0.3.3/regain/wrapper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-06-23 11:50:10.000000 regain-0.3.3/regain/scores.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2021-06-23 11:50:10.000000 regain-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 10:38:27.000000 regain-0.3.8/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-19 10:38:27.000000 regain-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 10:38:27.000000 regain-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-19 10:38:40.615666 regain-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-19 10:38:27.000000 regain-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.595665 regain-0.3.8/regain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-19 10:38:27.000000 regain-0.3.8/regain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.599665 regain-0.3.8/regain/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3427 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/gaussian_process_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15577 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/gwishart_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8907 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/wishart_distribution_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/wishart_process_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-19 10:38:27.000000 regain-0.3.8/regain/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.603665 regain-0.3.8/regain/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/infimal_convolution_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/kernel_latent_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28021 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/kernel_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_time_matrix_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/missing_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/time_graphical_lasso_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.603665 regain-0.3.8/regain/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-19 10:38:27.000000 regain-0.3.8/regain/data/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.607665 regain-0.3.8/regain/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23461 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/multi_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-19 10:38:27.000000 regain-0.3.8/regain/discriminant_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.607665 regain-0.3.8/regain/forward_backward/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/forward_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/time_graphical_lasso_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/generalized_linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_time_ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26895 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_time_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/_group_lasso_overlap_old_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/group_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/group_lasso_overlap_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/lasso_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/_bayesian_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/stability_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-19 10:38:27.000000 regain-0.3.8/regain/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-19 10:38:27.000000 regain-0.3.8/regain/prox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-19 10:38:27.000000 regain-0.3.8/regain/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 10:38:27.000000 regain-0.3.8/regain/update_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-19 10:38:27.000000 regain-0.3.8/regain/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-19 10:38:27.000000 regain-0.3.8/regain/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/wrapper/paspal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/paspal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/paspal/glopridu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.599665 regain-0.3.8/regain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-19 10:38:40.615666 regain-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 10:38:27.000000 regain-0.3.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `regain-0.3.3/PKG-INFO` & `regain-0.3.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: regain
-Version: 0.3.3
+Version: 0.3.8
 Summary: REGAIN (Regularised Graph Inference)
 Home-page: https://github.com/fdtomasi/regain
+Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.8.tar.gz
 Author: Federico Tomasi
 Author-email: fdtomasi@gmail.com
 Maintainer: Federico Tomasi
 Maintainer-email: fdtomasi@gmail.com
 License: FreeBSD
-Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.3.tar.gz
 Keywords: graph inference,latent variables
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
-Requires: numpy (>=1.11)
-Requires: scipy (>=0.16.1,>=1.0)
-Requires: sklearn (>=0.17)
-Requires: six
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/regain/) [![Requirements Status](https://requires.io/github/fdtomasi/regain/requirements.svg?branch=master)](https://requires.io/github/fdtomasi/regain/requirements/?branch=master)
+[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
@@ -133,9 +128,7 @@
   month = 	 {11--14 Sep},
   publisher = 	 {PMLR},
   pdf = 	 {http://proceedings.mlr.press/v72/tomasi18a/tomasi18a.pdf},
   url = 	 {http://proceedings.mlr.press/v72/tomasi18a.html},
   abstract = 	 {Gaussian graphical models have received much attention in the last years, due to their flexibility and expression power. However, the optimisation of such complex models suffer from computational issues both in terms of convergence rates and memory requirements. Here, we present a forward-backward splitting (FBS) procedure for Gaussian graphical modelling of multivariate time-series which relies on recent theoretical studies ensuring convergence under mild assumptions. Our experiments show that a FBS-based implementation achieves, with very fast convergence rates, optimal results with respect to ground truth and standard methods for dynamical network inference. Optimisation algorithms which are usually exploited for network inference suffer from drawbacks when considering large sets of unknowns. Particularly for increasing data sets and model complexity, we argue for the use of fast and theoretically sound optimisation algorithms to be significant to the graphical modelling community.}
 }
 ```
-
-
```

### Comparing `regain-0.3.3/README.md` & `regain-0.3.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/regain/) [![Requirements Status](https://requires.io/github/fdtomasi/regain/requirements.svg?branch=master)](https://requires.io/github/fdtomasi/regain/requirements/?branch=master)
+[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
```

### Comparing `regain-0.3.3/regain.egg-info/PKG-INFO` & `regain-0.3.8/regain.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: regain
-Version: 0.3.3
+Version: 0.3.8
 Summary: REGAIN (Regularised Graph Inference)
 Home-page: https://github.com/fdtomasi/regain
+Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.8.tar.gz
 Author: Federico Tomasi
 Author-email: fdtomasi@gmail.com
 Maintainer: Federico Tomasi
 Maintainer-email: fdtomasi@gmail.com
 License: FreeBSD
-Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.3.tar.gz
 Keywords: graph inference,latent variables
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
-Requires: numpy (>=1.11)
-Requires: scipy (>=0.16.1,>=1.0)
-Requires: sklearn (>=0.17)
-Requires: six
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/regain/) [![Requirements Status](https://requires.io/github/fdtomasi/regain/requirements.svg?branch=master)](https://requires.io/github/fdtomasi/regain/requirements/?branch=master)
+[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
@@ -133,9 +128,7 @@
   month = 	 {11--14 Sep},
   publisher = 	 {PMLR},
   pdf = 	 {http://proceedings.mlr.press/v72/tomasi18a/tomasi18a.pdf},
   url = 	 {http://proceedings.mlr.press/v72/tomasi18a.html},
   abstract = 	 {Gaussian graphical models have received much attention in the last years, due to their flexibility and expression power. However, the optimisation of such complex models suffer from computational issues both in terms of convergence rates and memory requirements. Here, we present a forward-backward splitting (FBS) procedure for Gaussian graphical modelling of multivariate time-series which relies on recent theoretical studies ensuring convergence under mild assumptions. Our experiments show that a FBS-based implementation achieves, with very fast convergence rates, optimal results with respect to ground truth and standard methods for dynamical network inference. Optimisation algorithms which are usually exploited for network inference suffer from drawbacks when considering large sets of unknowns. Particularly for increasing data sets and model complexity, we argue for the use of fast and theoretically sound optimisation algorithms to be significant to the graphical modelling community.}
 }
 ```
-
-
```

### Comparing `regain-0.3.3/regain.egg-info/SOURCES.txt` & `regain-0.3.8/regain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/LICENSE` & `regain-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/discriminant_analysis.py` & `regain-0.3.8/regain/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/wishart_process_.py` & `regain-0.3.8/regain/bayesian/wishart_process_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/_laplace_approximation.py` & `regain-0.3.8/regain/bayesian/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/wishart_distribution_.py` & `regain-0.3.8/regain/bayesian/wishart_distribution_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/gwishart_inference.py` & `regain-0.3.8/regain/bayesian/gwishart_inference.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/sampling.py` & `regain-0.3.8/regain/bayesian/sampling.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/__init__.py` & `regain-0.3.8/regain/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/gaussian_process_.py` & `regain-0.3.8/regain/bayesian/gaussian_process_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/bayesian/stats.py` & `regain-0.3.8/regain/bayesian/stats.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/clustering.py` & `regain-0.3.8/regain/clustering.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/generalized_linear_model/glm_poisson.py` & `regain-0.3.8/regain/generalized_linear_model/glm_poisson.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/generalized_linear_model/glm_time_ising.py` & `regain-0.3.8/regain/generalized_linear_model/glm_time_ising.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,16 @@
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_X_y
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 
 from sklearn.utils.validation import check_is_fitted
 
-from regain.generalized_linear_model.ising import _fit
-from regain.generalized_linear_model.ising import loss
 from regain.covariance.time_graphical_lasso_ import init_precision
+from regain.generalized_linear_model.glm_ising import _fit, loss
 from regain.norm import l1_od_norm
 from regain.utils import convergence
 from regain.update_rules import update_rho
 from regain.validation import check_norm_prox
 
 
 def loss_ising(X, K, n_samples=None):
@@ -194,15 +193,17 @@
 
         # other Zs
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             A_L = K[:-m] + U_L
             A_R = K[m:] + U_R
             if not psi_node_penalty:
-                prox_e = prox_psi(A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho)
+                prox_e = prox_psi(
+                    A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho
+                )
                 Z_L = 0.5 * (A_L + A_R - prox_e)
                 Z_R = 0.5 * (A_L + A_R + prox_e)
             else:
                 Z_L, Z_R = prox_psi(
                     np.concatenate((A_L, A_R), axis=1),
                     lamda=0.5 * np.diag(kernel, m)[:, None, None] / rho,
                     rho=rho,
@@ -214,54 +215,81 @@
 
             # update other residuals
             U_L += K[:-m] - Z_L
             U_R += K[m:] - Z_R
 
         # diagnostics, reporting, termination checks
         rnorm = np.sqrt(
-            sum(squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1]) for m in range(1, n_times))
+            sum(
+                squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1])
+                for m in range(1, n_times)
+            )
         )
 
         snorm = rho * np.sqrt(
             sum(
-                squared_norm(Z_M[m][0] - Z_M_old[m][0]) + squared_norm(Z_M[m][1] - Z_M_old[m][1])
+                squared_norm(Z_M[m][0] - Z_M_old[m][0])
+                + squared_norm(Z_M[m][1] - Z_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
         obj = objective(X, K, Z_M, alpha, kernel, psi) if compute_objective else np.nan
 
         check = convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
-                np.sqrt(sum(squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1]) for m in range(1, n_times))),
-                np.sqrt(squared_norm(K) + sum(squared_norm(K[:-m]) + squared_norm(K[m:]) for m in range(1, n_times))),
+                np.sqrt(
+                    sum(
+                        squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1])
+                        for m in range(1, n_times)
+                    )
+                ),
+                np.sqrt(
+                    squared_norm(K)
+                    + sum(
+                        squared_norm(K[:-m]) + squared_norm(K[m:])
+                        for m in range(1, n_times)
+                    )
+                ),
             ),
             e_dual=n_features * n_times * tol
-            + rtol * rho * np.sqrt(sum(squared_norm(U_M[m][0]) + squared_norm(U_M[m][1]) for m in range(1, n_times))),
+            + rtol
+            * rho
+            * np.sqrt(
+                sum(
+                    squared_norm(U_M[m][0]) + squared_norm(U_M[m][1])
+                    for m in range(1, n_times)
+                )
+            ),
         )
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(
+                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
+                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
+            )
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         # U_0 *= rho / rho_new
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             U_L *= rho / rho_new
             U_R *= rho / rho_new
         rho = rho_new
@@ -385,21 +413,31 @@
         self.n_cores = n_cores
 
     def get_precision(self):
         return self.precision_
 
     def fit(self, X, y):
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         self.classes_, n_samples = np.unique(y, return_counts=True)
         self.data = X.copy()
         if np.unique(self.data).size != 2:
             raise ValueError(
-                "Using the ising distribution your data has " "to contain only two values, either 0 and 1 " "or -1, 1"
+                "Using the ising distribution your data has "
+                "to contain only two values, either 0 and 1 "
+                "or -1, 1"
             )
         X = np.array([X[y == cl] for cl in self.classes_])
 
         if self.ker_param == "auto":
             from scipy.optimize import minimize_scalar
 
             if not callable(self.kernel):
@@ -408,15 +446,20 @@
             # initialise precision matrices, as warm start
             self.precision_ = init_precision(X, mode=self.init)
             theta_old = 0
             for i in range(self.max_iter_ext):
                 # E step - discover best kernel parameter
                 theta = minimize_scalar(
                     objective_kernel,
-                    args=(self.precision_, self.psi, self.kernel, self.classes_[:, None]),
+                    args=(
+                        self.precision_,
+                        self.psi,
+                        self.kernel,
+                        self.classes_[:, None],
+                    ),
                     bounds=(0, X.shape[0]),
                     method="bounded",
                 ).x
 
                 if i > 0 and abs(theta_old - theta) < 1e-5:
                     break
                 else:
@@ -453,24 +496,30 @@
             else:
                 print("warning: theta not converged")
 
         else:
             if callable(self.kernel):
                 try:
                     # this works if it is a ExpSineSquared or RBF kernel
-                    kernel = self.kernel(length_scale=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(length_scale=self.ker_param)(
+                        self.classes_[:, None]
+                    )
                 except TypeError:
                     # maybe it's a ConstantKernel
-                    kernel = self.kernel(constant_value=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(constant_value=self.ker_param)(
+                        self.classes_[:, None]
+                    )
             else:
                 kernel = self.kernel
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
-                        "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                        "got {} classes and kernel has shape {}".format(
+                            self.classes_.size, kernel.shape[0]
+                        )
                     )
             out = _fit_time_ising_model(
                 X,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
                 tol=self.tol,
@@ -504,26 +553,36 @@
         Returns
         -------
         res : float
             The likelihood of the data set with `self.covariance_` as an
             estimator of its covariance matrix.
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         # TO THINK
         return -99999999
 
 
 def precision_similarity(precision, psi=None):
     from regain.norm import l1_od_norm
     from scipy.spatial.distance import squareform
     from itertools import combinations
 
-    distances = squareform([l1_od_norm(t1 - t2) for t1, t2 in combinations(precision, 2)])
+    distances = squareform(
+        [l1_od_norm(t1 - t2) for t1, t2 in combinations(precision, 2)]
+    )
     print(distances)
     distances /= np.max(distances)
     return 1 - distances
 
 
 class SimilarityTemporalIsingModel(TemporalIsingModel):
     """Learn how to relate different adjacencies matrices across times.
@@ -618,28 +677,40 @@
         self.beta = beta
         self.kernel = kernel
         self.max_iter_ext = max_iter_ext
         self.eps = eps
         self.n_clusters = n_clusters
 
     def fit(self, X, y):
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         self.classes_, n_samples = np.unique(y, return_counts=True)
         self.data = X.copy()
         if np.unique(self.data).size != 2:
             raise ValueError(
-                "Using the ising distribution your data has " "to contain only two values, either 0 and 1 " "or -1, 1"
+                "Using the ising distribution your data has "
+                "to contain only two values, either 0 and 1 "
+                "or -1, 1"
             )
         X = np.array([X[y == cl] for cl in self.classes_])
         if self.kernel is None:
             # from scipy.optimize import minimize
             # discover best kernel parameter via EM
             # initialise precision matrices, as warm start
-            self.precision_ = np.random.rand(self.classes_.shape[0], X.shape[1], X.shape[1])
+            self.precision_ = np.random.rand(
+                self.classes_.shape[0], X.shape[1], X.shape[1]
+            )
             n_times = self.precision_.shape[0]
             kernel = np.eye(n_times)
 
             psi, _, _ = check_norm_prox(self.psi)
             if self.n_clusters is None:
                 self.n_clusters = n_times
             labels_pred_old = 0
@@ -661,35 +732,43 @@
                 if self.return_history:
                     (self.precision_, self.history_, self.n_iter_) = out
                 else:
                     self.precision_, self.n_iter_ = out
                 theta = precision_similarity(self.precision_, psi)
                 kernel = theta
                 labels_pred = AgglomerativeClustering(
-                    n_clusters=self.n_clusters, affinity="precomputed", linkage="complete"
+                    n_clusters=self.n_clusters,
+                    affinity="precomputed",
+                    linkage="complete",
                 ).fit_predict(kernel)
 
-                if i > 0 and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size < self.eps:
+                if (
+                    i > 0
+                    and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size
+                    < self.eps
+                ):
                     break
-                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(self.beta)(
-                    np.arange(n_times)[:, None]
-                )
+                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(
+                    self.beta
+                )(np.arange(n_times)[:, None])
                 print(kernel)
                 labels_pred_old = labels_pred
 
             else:
                 warnings.warn("theta did not converge.")
             self.similarity_matrix_ = kernel
 
         else:
             kernel = self.kernel
             if kernel.shape[0] != self.classes_.size:
                 raise ValueError(
                     "Kernel size does not match classes of samples, "
-                    "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                    "got {} classes and kernel has shape {}".format(
+                        self.classes_.size, kernel.shape[0]
+                    )
                 )
 
             out = _fit_time_ising_model(
                 X,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
```

### Comparing `regain-0.3.3/regain/generalized_linear_model/glm_gaussian.py` & `regain-0.3.8/regain/generalized_linear_model/glm_gaussian.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
-
-
 from sklearn.utils import check_array
 
-
-from regain.generalized_linear_model.base import GLM_GM, convergence, build_adjacency_matrix
+from regain.generalized_linear_model.base import (
+    GLM_GM,
+    build_adjacency_matrix,
+    convergence,
+)
 from regain.prox import soft_thresholding
 
 
 def objective(X, theta, n, r, selector, alpha):
     XXT = X[:, r].T.dot(X[:, selector]).dot(theta)
     TXXT = theta.T.dot(X[:, selector].T).dot(X[:, selector]).dot(theta)
     return -(1 / n) * XXT + (1 / (2 * n)) * TXXT + alpha * np.linalg.norm(theta, 1)
@@ -73,20 +74,25 @@
         theta = soft_thresholding(theta_new, alpha * gamma)
         thetas.append(theta)
 
         check = convergence(
             iter=iter_,
             obj=objective(X, theta, n, ix, selector, alpha),
             iter_norm=np.linalg.norm(thetas[-2] - thetas[-1]),
-            iter_r_norm=(np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-1])),
+            iter_r_norm=(
+                np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-1])
+            ),
         )
         checks.append(check)
         # if adjust_gamma: # TODO multiply or divide
         if verbose:
-            print("Iter: %d, objective: %.4f, iter_norm %.4f" % (check[0], check[1], check[2]))
+            print(
+                "Iter: %d, objective: %.4f, iter_norm %.4f"
+                % (check[0], check[1], check[2])
+            )
 
         if check[-2] < tol:
             break
 
     return_list = [thetas[-1]]
     if return_history:
         return_list.append(thetas)
@@ -160,15 +166,22 @@
         max_iter=100,
         verbose=False,
         return_history=True,
         return_n_iter=False,
         compute_objective=True,
     ):
         super(Gaussian_GLM_GM, self).__init__(
-            alpha, tol, rtol, max_iter, verbose, return_history, return_n_iter, compute_objective
+            alpha,
+            tol,
+            rtol,
+            max_iter,
+            verbose,
+            return_history,
+            return_n_iter,
+            compute_objective,
         )
         self.reconstruction = reconstruction
 
     def get_precision(self):
         return self.precision_
 
     def fit(self, X, y=None, gamma=1e-3):
```

### Comparing `regain-0.3.3/regain/generalized_linear_model/base.py` & `regain-0.3.8/regain/generalized_linear_model/base.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/generalized_linear_model/glm_ising.py` & `regain-0.3.8/regain/generalized_linear_model/glm_ising.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/generalized_linear_model/glm_time_poisson.py` & `regain-0.3.8/regain/generalized_linear_model/glm_time_poisson.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,27 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import warnings
 
 import numpy as np
-
 from six.moves import map, range, zip
-
 from sklearn.base import BaseEstimator
-from sklearn.utils.extmath import squared_norm
-from sklearn.utils.validation import check_X_y
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
+from sklearn.utils.extmath import squared_norm
+from sklearn.utils.validation import check_X_y, check_is_fitted
 
-from sklearn.utils.validation import check_is_fitted
-
-from regain.generalized_linear_model.poisson import fit_each_variable
-from regain.generalized_linear_model.poisson import loss
-from regain.generalized_linear_model.base import build_adjacency_matrix
 from regain.covariance.kernel_time_graphical_lasso_ import precision_similarity
+from regain.generalized_linear_model.base import build_adjacency_matrix
+from regain.generalized_linear_model.glm_poisson import fit_each_variable, loss
 from regain.norm import l1_od_norm
-from regain.utils import convergence
 from regain.update_rules import update_rho
+from regain.utils import convergence
 from regain.validation import check_norm_prox
 
 
 def loss_poisson(X, K, n_samples=None):
     """Loss function for time-varying poisson model."""
     if n_samples is None:
         n_samples = np.ones(X.shape[0])
@@ -86,14 +81,15 @@
     rtol=1e-4,
     return_history=False,
     return_n_iter=True,
     compute_objective=True,
     stop_at=None,
     stop_when=1e-4,
     n_cores=-1,
+    update_rho_options=None,
 ):
     """Time-varying graphical model solver.
 
     Solves the following problem via ADMM:
         min sum_{i=1}^T -n_i log_likelihood(K_i, X_i) + alpha ||K_i||_{od,1}
             + sum_{s>t}^T k(s,t) Psi(K_s - K_t)
 
@@ -171,27 +167,36 @@
         # K_new = np.zeros_like(K)
 
         for t in range(n_times):
             thetas_pred = []
             for v in range(n_features):
                 inner_verbose = max(0, verbose - 1)
                 res = fit_each_variable(
-                    X[t, :, :], v, alpha, tol=tol, verbose=inner_verbose, A=A[t, :, :], T=n_times, rho=rho
+                    X[t, :, :],
+                    v,
+                    alpha,
+                    tol=tol,
+                    verbose=inner_verbose,
+                    A=A[t, :, :],
+                    T=n_times,
+                    rho=rho,
                 )
                 thetas_pred.append(res[0])
 
             K[t, :, :] = build_adjacency_matrix(thetas_pred, "union")
 
         # other Zs
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             A_L = K[:-m] + U_L
             A_R = K[m:] + U_R
             if not psi_node_penalty:
-                prox_e = prox_psi(A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho)
+                prox_e = prox_psi(
+                    A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho
+                )
                 Z_L = 0.5 * (A_L + A_R - prox_e)
                 Z_R = 0.5 * (A_L + A_R + prox_e)
             else:
                 Z_L, Z_R = prox_psi(
                     np.concatenate((A_L, A_R), axis=1),
                     lamda=0.5 * np.diag(kernel, m)[:, None, None] / rho,
                     rho=rho,
@@ -203,54 +208,81 @@
 
             # update other residuals
             U_L += K[:-m] - Z_L
             U_R += K[m:] - Z_R
 
         # diagnostics, reporting, termination checks
         rnorm = np.sqrt(
-            sum(squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1]) for m in range(1, n_times))
+            sum(
+                squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1])
+                for m in range(1, n_times)
+            )
         )
 
         snorm = rho * np.sqrt(
             sum(
-                squared_norm(Z_M[m][0] - Z_M_old[m][0]) + squared_norm(Z_M[m][1] - Z_M_old[m][1])
+                squared_norm(Z_M[m][0] - Z_M_old[m][0])
+                + squared_norm(Z_M[m][1] - Z_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
         obj = objective(X, K, Z_M, alpha, kernel, psi) if compute_objective else np.nan
 
         check = convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
-                np.sqrt(sum(squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1]) for m in range(1, n_times))),
-                np.sqrt(squared_norm(K) + sum(squared_norm(K[:-m]) + squared_norm(K[m:]) for m in range(1, n_times))),
+                np.sqrt(
+                    sum(
+                        squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1])
+                        for m in range(1, n_times)
+                    )
+                ),
+                np.sqrt(
+                    squared_norm(K)
+                    + sum(
+                        squared_norm(K[:-m]) + squared_norm(K[m:])
+                        for m in range(1, n_times)
+                    )
+                ),
             ),
             e_dual=n_features * n_times * tol
-            + rtol * rho * np.sqrt(sum(squared_norm(U_M[m][0]) + squared_norm(U_M[m][1]) for m in range(1, n_times))),
+            + rtol
+            * rho
+            * np.sqrt(
+                sum(
+                    squared_norm(U_M[m][0]) + squared_norm(U_M[m][1])
+                    for m in range(1, n_times)
+                )
+            ),
         )
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(
+                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
+                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
+            )
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         # U_0 *= rho / rho_new
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             U_L *= rho / rho_new
             U_R *= rho / rho_new
         rho = rho_new
@@ -374,36 +406,51 @@
         self.n_cores = n_cores
 
     def get_precision(self):
         return self.precision_
 
     def fit(self, X, y):
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         self.classes_, n_samples = np.unique(y, return_counts=True)
         X = np.around(X)  # to ensure discreteness
         self.data = X.copy()
         if np.any(self.data) < 0:
-            raise ValueError("Using the poisson distribution your data has " "to be positive")
+            raise ValueError(
+                "Using the poisson distribution your data has " "to be positive"
+            )
         X = np.array([X[y == cl] for cl in self.classes_])
 
         if self.ker_param == "auto":
             from scipy.optimize import minimize_scalar
 
             if not callable(self.kernel):
                 raise ValueError("kernel should be a function if ker_param=='auto'")
             # discover best kernel parameter via alternating minimization
             # initialise precision matrices, as warm start
             theta_old = 0
             for i in range(self.max_iter_ext):
                 # E step - discover best kernel parameter
                 theta = minimize_scalar(
                     objective_kernel,
-                    args=(self.precision_, self.psi, self.kernel, self.classes_[:, None]),
+                    args=(
+                        self.precision_,
+                        self.psi,
+                        self.kernel,
+                        self.classes_[:, None],
+                    ),
                     bounds=(0, X.shape[0]),
                     method="bounded",
                 ).x
 
                 if i > 0 and abs(theta_old - theta) < 1e-5:
                     break
                 else:
@@ -441,24 +488,30 @@
             else:
                 print("warning: theta not converged")
 
         else:
             if callable(self.kernel):
                 try:
                     # this works if it is a ExpSineSquared or RBF kernel
-                    kernel = self.kernel(length_scale=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(length_scale=self.ker_param)(
+                        self.classes_[:, None]
+                    )
                 except TypeError:
                     # maybe it's a ConstantKernel
-                    kernel = self.kernel(constant_value=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(constant_value=self.ker_param)(
+                        self.classes_[:, None]
+                    )
             else:
                 kernel = self.kernel
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
-                        "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                        "got {} classes and kernel has shape {}".format(
+                            self.classes_.size, kernel.shape[0]
+                        )
                     )
             out = _fit_time_poisson_model(
                 X,
                 gamma=self.gamma,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
@@ -493,15 +546,23 @@
         Returns
         -------
         res : float
             The likelihood of the data set with `self.covariance_` as an
             estimator of its covariance matrix.
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         # TO THINK
         return -99999999
 
 
 class SimilarityTemporalPoissonModel(TemporalPoissonModel):
     """Learn how to relate different adjacencies matrices across times.
@@ -609,21 +670,31 @@
         self.beta = beta
         self.kernel = kernel
         self.max_iter_ext = max_iter_ext
         self.eps = eps
         self.n_clusters = n_clusters
 
     def fit(self, X, y):
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         self.classes_, n_samples = np.unique(y, return_counts=True)
         self.data = X.copy()
         if np.unique(self.data).size != 2:
             raise ValueError(
-                "Using the ising distribution your data has " "to contain only two values, either 0 and 1 " "or -1, 1"
+                "Using the ising distribution your data has "
+                "to contain only two values, either 0 and 1 "
+                "or -1, 1"
             )
         X = np.array([X[y == cl] for cl in self.classes_])
         print(X.shape)
         if self.kernel is None:
             # from scipy.optimize import minimize
             # discover best kernel parameter via EM
             # initialise precision matrices, as warm start
@@ -635,21 +706,27 @@
             if self.n_clusters is None:
                 self.n_clusters = n_times
             labels_pred_old = 0
             for i in range(self.max_iter_ext):
                 theta = precision_similarity(self.precision_, psi)
                 kernel = theta
                 labels_pred = AgglomerativeClustering(
-                    n_clusters=self.n_clusters, affinity="precomputed", linkage="complete"
+                    n_clusters=self.n_clusters,
+                    affinity="precomputed",
+                    linkage="complete",
                 ).fit_predict(kernel)
-                if i > 0 and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size < self.eps:
+                if (
+                    i > 0
+                    and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size
+                    < self.eps
+                ):
                     break
-                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(self.beta)(
-                    np.arange(n_times)[:, None]
-                )
+                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(
+                    self.beta
+                )(np.arange(n_times)[:, None])
 
                 out = _fit_time_poisson_model(
                     X,
                     alpha=self.alpha,
                     rho=self.rho,
                     kernel=kernel,
                     tol=self.tol,
@@ -675,15 +752,17 @@
             self.similarity_matrix_ = kernel
 
         else:
             kernel = self.kernel
             if kernel.shape[0] != self.classes_.size:
                 raise ValueError(
                     "Kernel size does not match classes of samples, "
-                    "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                    "got {} classes and kernel has shape {}".format(
+                        self.classes_.size, kernel.shape[0]
+                    )
                 )
 
             out = _fit_time_poisson_model(
                 X,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
```

### Comparing `regain-0.3.3/regain/data/base.py` & `regain-0.3.8/regain/data/base.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/data/__init__.py` & `regain-0.3.8/regain/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from .base import load_webkb, load_food_search_trends
+from .base import make_dataset
```

### Comparing `regain-0.3.3/regain/model_selection/stability_optimization.py` & `regain-0.3.8/regain/model_selection/stability_optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,23 @@
 from collections import defaultdict
 from functools import partial
 from itertools import product
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+from numpy.ma import MaskedArray
 from scipy.special import binom
 from scipy.stats import rankdata
 from sklearn.base import clone, is_classifier
-from sklearn.metrics.scorer import _check_multimetric_scoring
-from sklearn.model_selection import GridSearchCV, ParameterGrid, ShuffleSplit, StratifiedShuffleSplit
+from sklearn.metrics._scorer import _check_multimetric_scoring
+from sklearn.model_selection import GridSearchCV, StratifiedShuffleSplit
 from sklearn.model_selection._split import check_cv
 from sklearn.model_selection._validation import _aggregate_score_dicts, _fit_and_score
-from sklearn.utils import deprecated
 from sklearn.utils._joblib import Parallel, delayed
-from sklearn.utils.fixes import MaskedArray
 from sklearn.utils.validation import indexable
 
 warnings.simplefilter("ignore")
 
 
 def global_instability(estimators):
     """Computes instability of the graphs inferred from estimators.
@@ -77,15 +76,17 @@
         mean_connectivity = np.zeros_like(precisions[0])[triu_idx]
         for c in precisions:
             mean_connectivity += (c[triu_idx].copy() != 0).astype(int)
     else:
         # for tri dimensional matrices
         n_times = precisions[0].shape[0]
         triu_idx = np.triu_indices_from(precisions[0][0], 1)
-        mean_connectivity = np.array([np.zeros_like(precisions[0][0])[triu_idx] for i in range(n_times)])
+        mean_connectivity = np.array(
+            [np.zeros_like(precisions[0][0])[triu_idx] for i in range(n_times)]
+        )
         for c in precisions:
             for i in range(n_times):
                 mean_connectivity[i] += (c[i][triu_idx].copy() != 0).astype(int)
 
     mean_connectivity /= len(estimators)
     xi_matrix = 2 * mean_connectivity * (1 - mean_connectivity)
     return np.sum(xi_matrix) / (binom(precisions[0].shape[1], 2) * n_times)
@@ -115,27 +116,33 @@
     n = len(estimators)
     precisions = [estimator.get_precision() for estimator in estimators]
 
     if precisions[0].ndim == 2:
         gdvs = []
         for p in precisions:
             g = nx.from_numpy_array(p - np.diag(np.diag(p)))
-            gdvs.append(graphlet_degree_vectors(list(g.nodes), list(g.edges), graphlet_size=4))
+            gdvs.append(
+                graphlet_degree_vectors(list(g.nodes), list(g.edges), graphlet_size=4)
+            )
         distances = []
         for i in range(len(gdvs)):
             for j in range(i + 1, len(gdvs)):
                 distances.append(GCD(gdvs[i], gdvs[j])[1])
     else:
         n_times = precisions[0].shape[0]
         gdvs = []
         for p in precisions:
             times = []
             for t in range(n_times):
                 g = nx.from_numpy_array(p[t] - np.diag(np.diag(p[t])))
-                times.append(graphlet_degree_vectors(list(g.nodes), list(g.edges), graphlet_size=4))
+                times.append(
+                    graphlet_degree_vectors(
+                        list(g.nodes), list(g.edges), graphlet_size=4
+                    )
+                )
             gdvs.append(times)
 
         distances = []
         for i in range(len(gdvs)):
             for j in range(i + 1, len(gdvs)):
                 distance = 0
                 for t in range(n_times):
@@ -152,24 +159,30 @@
         mean_connectivity = np.zeros_like(precisions[0])[triu_idx]
         for c in precisions:
             mean_connectivity += (c[triu_idx].copy() != 0).astype(int)
     else:
         # for tri-dimensional matrices
         n_times = precisions[0].shape[0]
         triu_idx = np.triu_indices_from(precisions[0][0], 1)
-        mean_connectivity = np.array([np.zeros_like(precisions[0][0])[triu_idx] for i in range(n_times)])
+        mean_connectivity = np.array(
+            [np.zeros_like(precisions[0][0])[triu_idx] for i in range(n_times)]
+        )
         for c in precisions:
             for i in range(n_times):
                 mean_connectivity[i] += (c[i][triu_idx].copy() != 0).astype(int)
     mean_connectivity /= len(estimators)
     xi_matrix = 2 * mean_connectivity * (1 - mean_connectivity)
 
     p = precisions[0].shape[1]
     theta_hat = np.sum(xi_matrix)
-    theta_hat = theta_hat / (p * (p - 1) / 2) if precisions[0].ndim == 2 else theta_hat / (n_times * p * (p - 1) / 2)
+    theta_hat = (
+        theta_hat / (p * (p - 1) / 2)
+        if precisions[0].ndim == 2
+        else theta_hat / (n_times * p * (p - 1) / 2)
+    )
     return 4 * theta_hat * (1 - theta_hat)
 
 
 def _check_param_order(param_grid):
     """Ensure that the parameters are in descending order.
 
     This is required for stability to be correctly computed.
@@ -307,37 +320,44 @@
         **fit_params : dict of string -> object
             Parameters passed to the ``fit`` method of the estimator
         """
         estimator = self.estimator
 
         if self.sampling_size is None:
             self.sampling_size = int(min(10 * np.sqrt(X.shape[0]), X.shape[0] - 10))
-            self.cv = StratifiedShuffleSplit(train_size=self.sampling_size, n_splits=self.n_repetitions)
+            self.cv = StratifiedShuffleSplit(
+                train_size=self.sampling_size, n_splits=self.n_repetitions
+            )
         if y is not None:
             n_classes = np.unique(y).shape[0]
             if self.sampling_size % n_classes != 0:
-                warnings.warn("Changing sampling size, divisible for the " "number of classes.")
+                warnings.warn(
+                    "Changing sampling size, divisible for the " "number of classes."
+                )
                 self.sampling_size = (self.sampling_size // n_classes) * n_classes
                 self.cv = StratifiedShuffleSplit(
                     n_splits=self.n_repetitions,
                     train_size=self.sampling_size,
                     test_size=X.shape[0] - self.sampling_size,
                 )
         else:
             y = np.ones(X.shape[0])
         cv = check_cv(self.cv, y, classifier=is_classifier(estimator))
 
-        scorers, self.multimetric_ = _check_multimetric_scoring(self.estimator, scoring=self.scoring)
+        scorers, self.multimetric_ = _check_multimetric_scoring(
+            self.estimator, scoring=self.scoring
+        )
 
         if self.multimetric_:
             if (
                 self.refit is not False
                 and (
                     not isinstance(self.refit, str)
-                    or self.refit not in scorers  # This will work for both dict / list (tuple)
+                    or self.refit
+                    not in scorers  # This will work for both dict / list (tuple)
                 )
                 and not callable(self.refit)
             ):
                 raise ValueError(
                     "For multi-metric scoring, the parameter "
                     "refit must be set to a scorer key or a "
                     "callable to refit an estimator with the "
@@ -353,15 +373,17 @@
             # refit_metric = 'score'
             refit_metric = "instability"
 
         X, y, groups = indexable(X, y, groups)
         n_splits = cv.get_n_splits(X, y, groups)
         base_estimator = clone(self.estimator)
 
-        parallel = Parallel(n_jobs=self.n_jobs, verbose=self.verbose, pre_dispatch=self.pre_dispatch)
+        parallel = Parallel(
+            n_jobs=self.n_jobs, verbose=self.verbose, pre_dispatch=self.pre_dispatch
+        )
 
         fit_and_score_kwargs = dict(
             scorer=scorers,
             fit_params=fit_params,
             return_train_score=self.return_train_score,
             return_n_test_samples=True,
             return_times=True,
@@ -378,46 +400,54 @@
             def evaluate_candidates(candidate_params):
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
                     print(
                         "Fitting {0} folds for each of {1} candidates,"
-                        " totalling {2} fits".format(n_splits, n_candidates, n_candidates * n_splits)
+                        " totalling {2} fits".format(
+                            n_splits, n_candidates, n_candidates * n_splits
+                        )
                     )
 
                 out = parallel(
                     delayed(_fit_and_score)(
                         clone(base_estimator),
                         X,
                         y,
                         train=train,
                         test=test,
                         parameters=parameters,
                         **fit_and_score_kwargs
                     )
-                    for parameters, (train, test) in product(candidate_params, cv.split(X, y, groups))
+                    for parameters, (train, test) in product(
+                        candidate_params, cv.split(X, y, groups)
+                    )
                 )
 
                 if len(out) < 1:
                     raise ValueError(
-                        "No fits were performed. " "Was the CV iterator empty? " "Were there no candidates?"
+                        "No fits were performed. "
+                        "Was the CV iterator empty? "
+                        "Were there no candidates?"
                     )
                 elif len(out) != n_candidates * n_splits:
                     raise ValueError(
                         "cv.split and cv.get_n_splits returned "
                         "inconsistent results. Expected {} "
                         "splits, got {}".format(n_splits, len(out) // n_candidates)
                     )
 
                 all_candidate_params.extend(candidate_params)
                 all_out.extend(out)
 
                 nonlocal results
-                results = self._format_results(all_candidate_params, scorers, n_splits, all_out)
+                results = self._format_results(
+                    all_candidate_params, scorers, n_splits, all_out
+                )
                 return results
 
             self._run_search(evaluate_candidates)
 
         # For multi-metric evaluation, store the best_index_, best_params_ and
         # best_score_ iff refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
@@ -429,15 +459,17 @@
                 if not isinstance(self.best_index_, (int, np.integer)):
                     raise TypeError("best_index_ returned is not an integer")
                 if self.best_index_ < 0 or self.best_index_ >= len(results["params"]):
                     raise IndexError("best_index_ index out of range")
             else:
                 self.best_index_ = results["rank_test_%s" % refit_metric].argmin()
                 print(self.best_index_)
-                self.best_score_ = results["mean_test_%s" % refit_metric][self.best_index_]
+                self.best_score_ = results["mean_test_%s" % refit_metric][
+                    self.best_index_
+                ]
             self.best_params_ = results["params"][self.best_index_]
 
         if self.refit:
             self.best_estimator_ = clone(base_estimator).set_params(**self.best_params_)
             refit_start_time = time.time()
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
@@ -455,17 +487,30 @@
         return self
 
     def _format_results(self, candidate_params, scorers, n_splits, out):
         n_candidates = len(candidate_params)
 
         # if one choose to see train score, "out" will contain train score info
         if self.return_train_score:
-            (train_score_dicts, test_score_dicts, test_sample_counts, fit_time, score_time, estimators) = zip(*out)
+            (
+                train_score_dicts,
+                test_score_dicts,
+                test_sample_counts,
+                fit_time,
+                score_time,
+                estimators,
+            ) = zip(*out)
         else:
-            (test_score_dicts, test_sample_counts, fit_time, score_time, estimators) = zip(*out)
+            (
+                test_score_dicts,
+                test_sample_counts,
+                fit_time,
+                score_time,
+                estimators,
+            ) = zip(*out)
 
         # test_score_dicts and train_score dicts are lists of dictionaries and
         # we make them into dict of lists
         test_scores = _aggregate_score_dicts(test_score_dicts)
         if self.return_train_score:
             train_scores = _aggregate_score_dicts(train_score_dicts)
 
@@ -480,19 +525,25 @@
                 for split_i in range(n_splits):
                     # Uses closure to alter the results
                     results["split%d_%s" % (split_i, key_name)] = array[:, split_i]
 
             array_means = np.average(array, axis=1, weights=weights)
             results["mean_%s" % key_name] = array_means
             # Weighted std is not directly available in numpy
-            array_stds = np.sqrt(np.average((array - array_means[:, np.newaxis]) ** 2, axis=1, weights=weights))
+            array_stds = np.sqrt(
+                np.average(
+                    (array - array_means[:, np.newaxis]) ** 2, axis=1, weights=weights
+                )
+            )
             results["std_%s" % key_name] = array_stds
 
             if rank:
-                results["rank_%s" % key_name] = np.asarray(rankdata(-array_means, method="min"), dtype=np.int32)
+                results["rank_%s" % key_name] = np.asarray(
+                    rankdata(-array_means, method="min"), dtype=np.int32
+                )
 
         _store("fit_time", fit_time)
         _store("score_time", score_time)
         # Use one MaskedArray and mask all the places where the param is not
         # applicable for that candidate. Use defaultdict as each candidate may
         # not contain all the params
         param_results = defaultdict(
@@ -517,15 +568,17 @@
         results["params"] = candidate_params
 
         # NOTE test_sample counts (weights) remain the same for all candidates
         test_sample_counts = np.array(test_sample_counts[:n_splits], dtype=np.int)
 
         if self.iid != "deprecated":
             warnings.warn(
-                "The parameter 'iid' is deprecated in 0.22 and will be " "removed in 0.24.", DeprecationWarning
+                "The parameter 'iid' is deprecated in 0.22 and will be "
+                "removed in 0.24.",
+                DeprecationWarning,
             )
             iid = self.iid
         else:
             iid = False
 
         for scorer_name in scorers.keys():
             # Computed the (weighted) mean and std for test scores alone
@@ -541,38 +594,46 @@
 
         estimators = np.asarray(estimators).reshape(n_candidates, n_splits)
         array_means = np.array([global_instability(e_split) for e_split in estimators])
 
         # monotonize instabilities - require ordered parameters,
         # from high sparsity to low
 
-        monotonized_instabilities = [array_means[0]] + [np.max(array_means[:i]) for i in range(1, array_means.size)]
+        monotonized_instabilities = [array_means[0]] + [
+            np.max(array_means[:i]) for i in range(1, array_means.size)
+        ]
         monotonized_instabilities = np.array(monotonized_instabilities)
         self.monotonized_instabilities = np.copy(monotonized_instabilities)
 
         if self.mode.lower() == "gstars":
-            graphlets_stability = np.array([graphlet_instability(e_split) for e_split in estimators])
+            graphlets_stability = np.array(
+                [graphlet_instability(e_split) for e_split in estimators]
+            )
             self.graphlets_instabilities = np.copy(graphlets_stability)
 
             upper_bounds = np.array([upper_bound(e_split) for e_split in estimators])
-            upper_bounds = [upper_bounds[0]] + [np.max(upper_bounds[:i]) for i in range(1, upper_bounds.size)]
+            upper_bounds = [upper_bounds[0]] + [
+                np.max(upper_bounds[:i]) for i in range(1, upper_bounds.size)
+            ]
             self.upper_bounds = np.array(upper_bounds)
             lb = np.where(np.array(monotonized_instabilities) <= 0.05)[0]
             ub = np.where(np.array(upper_bounds) <= 0.05)[0]
             lb = lb[-1] if lb.size != 0 else len(monotonized_instabilities)
             ub = ub[-1] if ub.size != 0 else 0
             self.lower_bound = lb
             self.upper_bound = ub
             graphlets_stability[0:ub] = np.inf
             graphlets_stability[lb + 1 :] = np.inf
 
             key_name = "test_instability"
             results["raw_%s" % key_name] = array_means
             results["mean_%s" % key_name] = monotonized_instabilities
-            results["rank_%s" % key_name] = np.asarray(rankdata(graphlets_stability, method="min"), dtype=np.int32)
+            results["rank_%s" % key_name] = np.asarray(
+                rankdata(graphlets_stability, method="min"), dtype=np.int32
+            )
         else:
             # discard high values
             monotonized_instabilities[monotonized_instabilities > 0.05] = -np.inf
             key_name = "test_instability"
             results["raw_%s" % key_name] = array_means
             results["mean_%s" % key_name] = monotonized_instabilities
             results["rank_%s" % key_name] = np.asarray(
```

### Comparing `regain-0.3.3/regain/model_selection/_bayesian_optimization.py` & `regain-0.3.8/regain/model_selection/_bayesian_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Deprecated.
 
 This module to port GPyOpt in a `sklearn-usable` way has been deprecated
 in favor of scikit-optimize, which natively offer a Bayesian replacement
 for the GridSearchCV.
 """
-import numpy as np
 from functools import partial
-from sklearn.base import is_classifier, clone
-from sklearn.metrics.scorer import _check_multimetric_scoring
+
+import numpy as np
+from sklearn.base import clone, is_classifier
+from sklearn.metrics._scorer import _check_multimetric_scoring
 from sklearn.model_selection import cross_val_score
-from sklearn.model_selection._split import check_cv
 from sklearn.model_selection._search import BaseSearchCV
+from sklearn.model_selection._split import check_cv
 from sklearn.utils import deprecated
 
 try:
     import GPyOpt
     from GPyOpt.core.task.objective import SingleObjective
     from GPyOpt.core.task.cost import CostModel
     from GPyOpt.core.task.space import Design_space
@@ -139,32 +140,37 @@
 
         # --- CHOOSE the model type. If an instance of a GPyOpt model is passed (possibly user defined), it is used.
         # note that this 2 options are not used with the predefined model
         self.model_type = model_type
         self.exact_feval = exact_feval
         self.normalize_Y = normalize_Y
 
-        if "model" in self.kwargs and isinstance(kwargs["model"], GPyOpt.models.base.BOModel):
+        if "model" in self.kwargs and isinstance(
+            kwargs["model"], GPyOpt.models.base.BOModel
+        ):
             self.model = kwargs["model"]
             self.model_type = "User defined model used."
             if self.verbose:
                 print("Using a model defined by the used.")
         else:
             self.model = self._model_chooser()
 
         # --- CHOOSE the acquisition optimizer_type
         # This states how the discrete variables are handled (exact search or rounding)
         self.acquisition_optimizer_type = acquisition_optimizer_type
         self.acquisition_optimizer = AcquisitionOptimizer(
             self.space, self.acquisition_optimizer_type, model=self.model
         )
 
-        # --- CHOOSE acquisition function. If an instance of an acquisition is passed (possibly user defined), it is used.
+        # --- CHOOSE acquisition function.
+        # If an instance of an acquisition is passed (possibly user defined), it is used.
         self.acquisition_type = acquisition_type
-        if "acquisition" in self.kwargs and isinstance(kwargs["acquisition"], GPyOpt.acquisitions.AcquisitionBase):
+        if "acquisition" in self.kwargs and isinstance(
+            kwargs["acquisition"], GPyOpt.acquisitions.AcquisitionBase
+        ):
             self.acquisition = kwargs["acquisition"]
             self.acquisition_type = "User defined acquisition used."
             if self.verbose:
                 print("Using an acquisition defined by the used.")
         else:
             self.acquisition = self._acquisition_chooser()
 
@@ -207,15 +213,17 @@
 
         **fit_params : dict of string -> object
             Parameters passed to the ``fit`` method of the estimator
 
         """
         cv = check_cv(self.cv, y, classifier=is_classifier(self.estimator))
 
-        scorers, self.multimetric_ = _check_multimetric_scoring(self.estimator, scoring=self.scoring)
+        scorers, self.multimetric_ = _check_multimetric_scoring(
+            self.estimator, scoring=self.scoring
+        )
 
         score_function = partial(
             cross_val_score,
             X=X,
             y=y,
             groups=groups,
             scoring=self.scoring,
@@ -260,8 +268,13 @@
         super(_BayesianOptimization, self).plot_acquisition()
         # restore original X and Y
         self.X, self.Y = old_X, old_Y
 
 
 def _fit_score(x, score_function, mdl=None, param_names=None):
     x = 10 ** np.atleast_2d(x)
-    return -np.array([np.mean(score_function(mdl.set_params(**dict(zip(param_names, pars))))) for pars in x])[:, None]
+    return -np.array(
+        [
+            np.mean(score_function(mdl.set_params(**dict(zip(param_names, pars)))))
+            for pars in x
+        ]
+    )[:, None]
```

### Comparing `regain-0.3.3/regain/model_selection/__init__.py` & `regain-0.3.8/regain/data/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/norm.py` & `regain-0.3.8/regain/norm.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/forward_backward/forward_backward.py` & `regain-0.3.8/regain/forward_backward/forward_backward.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/forward_backward/time_graphical_lasso_.py` & `regain-0.3.8/regain/forward_backward/time_graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 
 import warnings
 from functools import partial
 
 import numpy as np
 from scipy import linalg
 from six.moves import map, range, zip
-from sklearn.covariance.graph_lasso_ import alpha_max
+from sklearn.covariance._graph_lasso import alpha_max  # noqa
 from sklearn.utils.extmath import squared_norm
 
-from regain.covariance.time_graphical_lasso_ import TimeGraphicalLasso, init_precision
-from regain.covariance.time_graphical_lasso_ import loss as loss_tgl
+from regain.covariance.time_graphical_lasso_ import (
+    TimeGraphicalLasso,
+    init_precision,
+    loss as loss_tgl,
+)
 from regain.norm import l1_od_norm, vector_p_norm
 from regain.prox import prox_FL, soft_thresholding_od
 from regain.utils import convergence
-
 from .forward_backward import _scalar_product, choose_gamma, choose_lamda, upper_diag_3d
 
 
 def loss(S, K, n_samples=None, vareps=0):
     """Loss function for time-varying graphical lasso."""
     loss_ = loss_tgl(S, K, n_samples=n_samples)
     loss_ += vareps / 2.0 * _scalar_product(K, K)
@@ -71,15 +73,17 @@
 def penalty(precision, alpha, beta, psi):
     """Penalty for time-varying graphical lasso."""
     if isinstance(alpha, np.ndarray):
         obj = sum(a[0][0] * m for a, m in zip(alpha, map(l1_od_norm, precision)))
     else:
         obj = alpha * sum(map(l1_od_norm, precision))
     if isinstance(beta, np.ndarray):
-        obj += sum(b[0][0] * m for b, m in zip(beta, map(psi, precision[1:] - precision[:-1])))
+        obj += sum(
+            b[0][0] * m for b, m in zip(beta, map(psi, precision[1:] - precision[:-1]))
+        )
     else:
         obj += beta * psi(precision[1:] - precision[:-1])
     return obj
 
 
 def objective(n_samples, emp_cov, precision, alpha, beta, psi, vareps=0):
     """Objective function for time-varying graphical lasso."""
@@ -118,15 +122,17 @@
         obj = alpha * sum(map(l1_od_norm, precision))
     # obj += beta * psi(precision[1:] - precision[:-1])
     return obj
 
 
 def objective_laplacian(n_samples, emp_cov, precision, alpha, beta, vareps=0):
     """Objective function for TGL with Laplacian penalty."""
-    obj = loss_laplacian(emp_cov, precision, beta=beta, n_samples=n_samples, vareps=vareps)
+    obj = loss_laplacian(
+        emp_cov, precision, beta=beta, n_samples=n_samples, vareps=vareps
+    )
     obj += penalty_laplacian(precision, alpha)
     return obj
 
 
 def _J(x, beta, alpha, gamma, lamda, S, n_samples, p=1, x_inv=None, grad=None):
     """Grad + prox + line search for the new point."""
     prox = prox_FL(x - gamma * grad, beta * gamma, alpha * gamma, p=p, symmetric=True)
@@ -218,33 +224,54 @@
         If return_history, then also a structure that contains the
         objective value, the primal and dual residual norms, and tolerances
         for the primal and dual residual norms at each iteration.
 
     """
     available_choose = ("gamma", "lamda", "fixed", "both")
     if choose not in available_choose:
-        raise ValueError("`choose` parameter must be one of %s." % available_choose)
+        raise ValueError(f"`choose` parameter must be one of {available_choose}.")
 
     n_times, _, n_features = emp_cov.shape
     K = init_precision(emp_cov, mode=init)
 
     if laplacian_penalty:
         obj_partial = partial(
-            objective_laplacian, n_samples=n_samples, emp_cov=emp_cov, alpha=alpha, beta=beta, vareps=vareps
+            objective_laplacian,
+            n_samples=n_samples,
+            emp_cov=emp_cov,
+            alpha=alpha,
+            beta=beta,
+            vareps=vareps,
+        )
+        function_f = partial(
+            loss_laplacian, beta=beta, n_samples=n_samples, S=emp_cov, vareps=vareps
+        )
+        gradient_f = partial(
+            grad_loss_laplacian,
+            emp_cov=emp_cov,
+            beta=beta,
+            n_samples=n_samples,
+            vareps=vareps,
         )
-        function_f = partial(loss_laplacian, beta=beta, n_samples=n_samples, S=emp_cov, vareps=vareps)
-        gradient_f = partial(grad_loss_laplacian, emp_cov=emp_cov, beta=beta, n_samples=n_samples, vareps=vareps)
         function_g = partial(penalty_laplacian, alpha=alpha)
     else:
         psi = partial(vector_p_norm, p=time_norm)
         obj_partial = partial(
-            objective, n_samples=n_samples, emp_cov=emp_cov, alpha=alpha, beta=beta, psi=psi, vareps=vareps
+            objective,
+            n_samples=n_samples,
+            emp_cov=emp_cov,
+            alpha=alpha,
+            beta=beta,
+            psi=psi,
+            vareps=vareps,
         )
         function_f = partial(loss, n_samples=n_samples, S=emp_cov, vareps=vareps)
-        gradient_f = partial(grad_loss, emp_cov=emp_cov, n_samples=n_samples, vareps=vareps)
+        gradient_f = partial(
+            grad_loss, emp_cov=emp_cov, n_samples=n_samples, vareps=vareps
+        )
         function_g = partial(penalty, alpha=alpha, beta=beta, psi=psi)
 
     max_residual = -np.inf
     n_linesearch = 0
     checks = [convergence(obj=obj_partial(precision=K))]
     for iteration_ in range(max_iter):
         k_previous = K.copy()
@@ -270,15 +297,17 @@
             )
 
         x_hat = K - gamma * grad
         if choose not in ["gamma", "both"]:
             if laplacian_penalty:
                 y = soft_thresholding_od(x_hat, alpha * gamma)
             else:
-                y = prox_FL(x_hat, beta * gamma, alpha * gamma, p=time_norm, symmetric=True)
+                y = prox_FL(
+                    x_hat, beta * gamma, alpha * gamma, p=time_norm, symmetric=True
+                )
 
         if choose in ("lamda", "both"):
             lamda, n_ls = choose_lamda(
                 min(lamda / eps if iteration_ > 0 else lamda, 1),
                 K,
                 function_f=function_f,
                 objective_f=obj_partial,
@@ -298,22 +327,31 @@
 
         K = K + min(max(lamda, 0), 1) * (y - K)
         # K, t = fista_step(Y, Y - Y_old, t)
 
         check = convergence(
             obj=obj_partial(precision=K),
             rnorm=np.linalg.norm(upper_diag_3d(K) - upper_diag_3d(k_previous)),
-            snorm=np.linalg.norm(obj_partial(precision=K) - obj_partial(precision=k_previous)),
+            snorm=np.linalg.norm(
+                obj_partial(precision=K) - obj_partial(precision=k_previous)
+            ),
             e_pri=np.sqrt(upper_diag_3d(K).size) * tol
-            + tol * max(np.linalg.norm(upper_diag_3d(K)), np.linalg.norm(upper_diag_3d(k_previous))),
+            + tol
+            * max(
+                np.linalg.norm(upper_diag_3d(K)),
+                np.linalg.norm(upper_diag_3d(k_previous)),
+            ),
             e_dual=tol,
         )
 
         if verbose and iteration_ % (50 if verbose < 2 else 1) == 0:
-            print("obj: %.4f, rnorm: %.7f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(
+                "obj: %.4f, rnorm: %.7f, snorm: %.4f,"
+                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
+            )
 
         if return_history:
             checks.append(check)
 
         if np.isnan(check.rnorm) or np.isnan(check.snorm):
             warnings.warn("precision is not positive definite.")
 
@@ -518,16 +556,27 @@
             stop_when=self.stop_when,
             init=self.init,
             laplacian_penalty=self.laplacian_penalty,
         )
 
         if self.return_history:
             if self.return_n_linesearch:
-                self.precision_, self.covariance_, self.history_, self.n_iter_, self.n_linesearch_ = out
+                (
+                    self.precision_,
+                    self.covariance_,
+                    self.history_,
+                    self.n_iter_,
+                    self.n_linesearch_,
+                ) = out
             else:
                 self.precision_, self.covariance_, self.history_, self.n_iter_ = out
         else:
             if self.return_n_linesearch:
-                self.precision_, self.covariance_, self.n_iter_, self.n_linesearch_ = out
+                (
+                    self.precision_,
+                    self.covariance_,
+                    self.n_iter_,
+                    self.n_linesearch_,
+                ) = out
             else:
                 self.precision_, self.covariance_, self.n_iter_ = out
         return self
```

### Comparing `regain-0.3.3/regain/forward_backward/__init__.py` & `regain-0.3.8/regain/forward_backward/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/update_rules.py` & `regain-0.3.8/regain/update_rules.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/utils.py` & `regain-0.3.8/regain/utils.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/latent_time_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/latent_time_graphical_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/infimal_convolution_.py` & `regain-0.3.8/regain/covariance/infimal_convolution_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/graphical_lasso_.py` & `regain-0.3.8/regain/covariance/graphical_lasso_.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,29 +35,24 @@
 from __future__ import division
 
 import warnings
 
 import numpy as np
 from scipy import linalg
 from six.moves import range
+from sklearn.covariance import GraphicalLasso as GraphLasso
 from sklearn.covariance import empirical_covariance
 from sklearn.utils.extmath import fast_logdet
 from sklearn.utils.validation import check_array
 
 from regain.norm import l1_od_norm
 from regain.prox import prox_logdet, soft_thresholding_od
 from regain.update_rules import update_rho
 from regain.utils import convergence
 
-try:
-    # sklean >= 0.20
-    from sklearn.covariance import GraphicalLasso as GraphLasso
-except ImportError:
-    # sklearn < 0.20
-    from sklearn.covariance import GraphLasso
 
 
 def logl(emp_cov, precision):
     """Gaussian log-likelihood without constant term."""
     return fast_logdet(precision) - np.sum(emp_cov * precision)
```

### Comparing `regain-0.3.3/regain/covariance/latent_time_matrix_decomposition.py` & `regain-0.3.8/regain/covariance/latent_time_matrix_decomposition.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/time_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/time_graphical_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/missing_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/missing_graphical_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/kernel_latent_time_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/kernel_latent_time_graphical_lasso_.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,29 @@
 from scipy import linalg
 from six.moves import map, range, zip
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_is_fitted
 
-from regain.covariance.kernel_time_graphical_lasso_ import KernelTimeGraphicalLasso, init_precision
-from regain.covariance.kernel_time_graphical_lasso_ import objective as obj_ktgl
-from regain.covariance.kernel_time_graphical_lasso_ import precision_similarity
+from regain.covariance.kernel_time_graphical_lasso_ import (
+    KernelTimeGraphicalLasso,
+    init_precision,
+    objective as obj_ktgl,
+    precision_similarity,
+)
 from regain.prox import prox_logdet, prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
 from regain.utils import convergence
 from regain.validation import check_norm_prox
 
 
-def objective(S, n_samples, R, Z_0, Z_M, W_0, W_M, alpha, tau, kernel_psi, kernel_phi, psi, phi):
+def objective(
+    S, n_samples, R, Z_0, Z_M, W_0, W_M, alpha, tau, kernel_psi, kernel_phi, psi, phi
+):
     """Objective function for latent variable time-varying graphical lasso."""
     obj = obj_ktgl(n_samples, S, R, Z_0, Z_M, alpha, kernel_psi, psi)
     if isinstance(tau, np.ndarray):
         obj += sum(np.linalg.norm(t * w, ord="nuc") for t, w in zip(tau, W_0))
     else:
         obj += tau * sum(map(partial(np.linalg.norm, ord="nuc"), W_0))
 
@@ -203,26 +208,30 @@
             A[:-m] += W_M[m][0] - U_M[m][0]
             A[m:] += W_M[m][1] - U_M[m][1]
 
         A /= n_times
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
-        W_0 = np.array([prox_trace_indicator(a, lamda=tau / (rho * n_times)) for a in A])
+        W_0 = np.array(
+            [prox_trace_indicator(a, lamda=tau / (rho * n_times)) for a in A]
+        )
 
         # update residuals
         X_0 += R - Z_0 + W_0
 
         for m in range(1, n_times):
             # other Zs
             Y_L, Y_R = Y_M[m]
             A_L = Z_0[:-m] + Y_L
             A_R = Z_0[m:] + Y_R
             if not psi_node_penalty:
-                prox_e = prox_psi(A_R - A_L, lamda=2.0 * np.diag(kernel_psi, m)[:, None, None] / rho)
+                prox_e = prox_psi(
+                    A_R - A_L, lamda=2.0 * np.diag(kernel_psi, m)[:, None, None] / rho
+                )
                 Z_L = 0.5 * (A_L + A_R - prox_e)
                 Z_R = 0.5 * (A_L + A_R + prox_e)
             else:
                 Z_L, Z_R = prox_psi(
                     np.concatenate((A_L, A_R), axis=1),
                     lamda=0.5 * np.diag(kernel_psi, m)[:, None, None] / rho,
                     rho=rho,
@@ -237,15 +246,17 @@
             Y_R += Z_0[m:] - Z_R
 
             # other Ws
             U_L, U_R = U_M[m]
             A_L = W_0[:-m] + U_L
             A_R = W_0[m:] + U_R
             if not phi_node_penalty:
-                prox_e = prox_phi(A_R - A_L, lamda=2.0 * np.diag(kernel_phi, m)[:, None, None] / rho)
+                prox_e = prox_phi(
+                    A_R - A_L, lamda=2.0 * np.diag(kernel_phi, m)[:, None, None] / rho
+                )
                 W_L = 0.5 * (A_L + A_R - prox_e)
                 W_R = 0.5 * (A_L + A_R + prox_e)
             else:
                 W_L, W_R = prox_phi(
                     np.concatenate((A_L, A_R), axis=1),
                     lamda=0.5 * np.diag(kernel_phi, m)[:, None, None] / rho,
                     rho=rho,
@@ -279,15 +290,29 @@
                 + squared_norm(W_M[m][0] - W_M_old[m][0])
                 + squared_norm(W_M[m][1] - W_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
         obj = (
-            objective(emp_cov, n_samples, R, Z_0, Z_M, W_0, W_M, alpha, tau, kernel_psi, kernel_phi, psi, phi)
+            objective(
+                emp_cov,
+                n_samples,
+                R,
+                Z_0,
+                Z_M,
+                W_0,
+                W_M,
+                alpha,
+                tau,
+                kernel_psi,
+                kernel_phi,
+                psi,
+                phi,
+            )
             if compute_objective
             else np.nan
         )
 
         check = convergence(
             obj=obj,
             rnorm=rnorm,
@@ -304,15 +329,18 @@
                         + squared_norm(W_M[m][1])
                         for m in range(1, n_times)
                     )
                 ),
                 np.sqrt(
                     squared_norm(Z_0 - W_0)
                     + sum(
-                        squared_norm(Z_0[:-m]) + squared_norm(Z_0[m:]) + squared_norm(W_0[:-m]) + squared_norm(W_0[m:])
+                        squared_norm(Z_0[:-m])
+                        + squared_norm(Z_0[m:])
+                        + squared_norm(W_0[:-m])
+                        + squared_norm(W_0[m:])
                         for m in range(1, n_times)
                     )
                 ),
             ),
             e_dual=n_features * np.sqrt(n_times * (2 * n_times - 1)) * tol
             + rtol
             * rho
@@ -330,21 +358,26 @@
 
         R_old = R.copy()
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
             W_M_old[m] = (W_M[m][0].copy(), W_M[m][1].copy())
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(
+                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
+                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
+            )
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         X_0 *= rho / rho_new
         for m in range(1, n_times):
             Y_L, Y_R = Y_M[m]
             Y_L *= rho / rho_new
             Y_R *= rho / rho_new
 
@@ -491,39 +524,51 @@
         return self.precision_ - self.latent_
 
     def _fit(self, emp_cov, n_samples):
         # TODO auto discover parameter
         if callable(self.kernel_phi):
             try:
                 # this works if it is a ExpSineSquared or RBF kernel
-                kernel_phi = self.kernel_phi(length_scale=self.ker_phi_param)(self.classes_[:, None])
+                kernel_phi = self.kernel_phi(length_scale=self.ker_phi_param)(
+                    self.classes_[:, None]
+                )
             except TypeError:
                 # maybe it's a ConstantKernel
-                kernel_phi = self.kernel_phi(constant_value=self.ker_phi_param)(self.classes_[:, None])
+                kernel_phi = self.kernel_phi(constant_value=self.ker_phi_param)(
+                    self.classes_[:, None]
+                )
 
         else:
             kernel_phi = self.kernel_phi
             if kernel_phi.shape[0] != self.classes_.size:
                 raise ValueError(
                     "kernel_phi size does not match classes of samples, "
-                    "got {} classes and kernel_phi has shape {}".format(self.classes_.size, kernel_phi.shape[0])
+                    "got {} classes and kernel_phi has shape {}".format(
+                        self.classes_.size, kernel_phi.shape[0]
+                    )
                 )
         if callable(self.kernel_psi):
             try:
                 # this works if it is a ExpSineSquared kernel
-                kernel_psi = self.kernel_psi(length_scale=self.ker_psi_param)(self.classes_[:, None])
+                kernel_psi = self.kernel_psi(length_scale=self.ker_psi_param)(
+                    self.classes_[:, None]
+                )
             except TypeError:
                 # maybe it's a ConstantKernel
-                kernel_psi = self.kernel_psi(constant_value=self.ker_psi_param)(self.classes_[:, None])
+                kernel_psi = self.kernel_psi(constant_value=self.ker_psi_param)(
+                    self.classes_[:, None]
+                )
         else:
             kernel_psi = self.kernel_psi
             if kernel_psi.shape[0] != self.classes_.size:
                 raise ValueError(
                     "kernel_psi size does not match classes of samples, "
-                    "got {} classes and kernel_psi has shape {}".format(self.classes_.size, kernel_psi.shape[0])
+                    "got {} classes and kernel_psi has shape {}".format(
+                        self.classes_.size, kernel_psi.shape[0]
+                    )
                 )
 
         out = kernel_latent_time_graphical_lasso(
             emp_cov,
             alpha=self.alpha,
             tau=self.tau,
             rho=self.rho,
@@ -538,15 +583,21 @@
             return_n_iter=True,
             return_history=self.return_history,
             update_rho_options=self.update_rho_options,
             compute_objective=self.compute_objective,
             init=self.init,
         )
         if self.return_history:
-            self.precision_, self.latent_, self.covariance_, self.history_, self.n_iter_ = out
+            (
+                self.precision_,
+                self.latent_,
+                self.covariance_,
+                self.history_,
+                self.n_iter_,
+            ) = out
         else:
             self.precision_, self.latent_, self.covariance_, self.n_iter_ = out
 
         return self
 
 
 class SimilarityLatentTimeGraphicalLasso(KernelLatentTimeGraphicalLasso):
@@ -702,33 +753,39 @@
             self.latent_ = np.zeros_like(self.precision_)
             theta_old = np.zeros(n_times * (n_times - 1) // 2)
             kernel_psi = np.eye(n_times)
 
             psi, _, _ = check_norm_prox(self.psi)
             if self.n_clusters is None:
                 self.n_clusters = n_times
-
+            labels_pred_old = None
             for i in range(self.max_iter_ext):
                 # E step - discover best kernel
                 theta = precision_similarity(self.get_precision(), psi)
 
                 # if i > 0 and np.linalg.norm(theta_old -
                 #                             theta) / theta.size < self.eps:
                 #     break
 
                 # kernel_psi = theta * self.beta
                 kernel_psi = theta
                 labels_pred = AgglomerativeClustering(
-                    n_clusters=self.n_clusters, affinity="precomputed", linkage="complete"
+                    n_clusters=self.n_clusters,
+                    affinity="precomputed",
+                    linkage="complete",
                 ).fit_predict(kernel_psi)
-                if i > 0 and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size < self.eps:
+                if (
+                    i > 0
+                    and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size
+                    < self.eps
+                ):
                     break
-                kernel_psi = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(self.beta)(
-                    np.arange(n_times)[:, None]
-                )
+                kernel_psi = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(
+                    self.beta
+                )(np.arange(n_times)[:, None])
 
                 # M step - fix the kernel matrix
                 out = kernel_latent_time_graphical_lasso(
                     emp_cov,
                     alpha=self.alpha,
                     tau=self.tau,
                     rho=self.rho,
@@ -744,51 +801,74 @@
                     return_history=self.return_history,
                     update_rho_options=self.update_rho_options,
                     compute_objective=self.compute_objective,
                     init=self.precision_,
                 )
 
                 if self.return_history:
-                    (self.precision_, self.latent_, self.covariance_, self.history_, self.n_iter_) = out
+                    (
+                        self.precision_,
+                        self.latent_,
+                        self.covariance_,
+                        self.history_,
+                        self.n_iter_,
+                    ) = out
                 else:
-                    (self.precision_, self.latent_, self.covariance_, self.n_iter_) = out
+                    (
+                        self.precision_,
+                        self.latent_,
+                        self.covariance_,
+                        self.n_iter_,
+                    ) = out
                 theta_old = theta
                 labels_pred_old = labels_pred
             else:
                 warnings.warn("theta did not converge.")
             self.similarity_matrix_ = kernel_psi
         else:
             if callable(self.kernel_phi):
                 try:
                     # this works if it is a ExpSineSquared or RBF kernel
-                    kernel_phi = self.kernel_phi(length_scale=self.ker_phi_param)(self.classes_[:, None])
+                    kernel_phi = self.kernel_phi(length_scale=self.ker_phi_param)(
+                        self.classes_[:, None]
+                    )
                 except TypeError:
                     # maybe it's a ConstantKernel
-                    kernel_phi = self.kernel_phi(constant_value=self.ker_phi_param)(self.classes_[:, None])
+                    kernel_phi = self.kernel_phi(constant_value=self.ker_phi_param)(
+                        self.classes_[:, None]
+                    )
 
             else:
                 kernel_phi = self.kernel_phi
                 if kernel_phi.shape[0] != self.classes_.size:
                     raise ValueError(
                         "kernel_phi size does not match classes of samples, "
-                        "got {} classes and kernel_phi has shape {}".format(self.classes_.size, kernel_phi.shape[0])
+                        "got {} classes and kernel_phi has shape {}".format(
+                            self.classes_.size, kernel_phi.shape[0]
+                        )
                     )
             if callable(self.kernel_psi):
                 try:
                     # this works if it is a ExpSineSquared kernel
-                    kernel_psi = self.kernel_psi(length_scale=self.ker_psi_param)(self.classes_[:, None])
+                    kernel_psi = self.kernel_psi(length_scale=self.ker_psi_param)(
+                        self.classes_[:, None]
+                    )
                 except TypeError:
                     # maybe it's a ConstantKernel
-                    kernel_psi = self.kernel_psi(constant_value=self.ker_psi_param)(self.classes_[:, None])
+                    kernel_psi = self.kernel_psi(constant_value=self.ker_psi_param)(
+                        self.classes_[:, None]
+                    )
             else:
                 kernel_psi = self.kernel_psi
                 if kernel_psi.shape[0] != self.classes_.size:
                     raise ValueError(
                         "kernel_psi size does not match classes of samples, "
-                        "got {} classes and kernel_psi has shape {}".format(self.classes_.size, kernel_psi.shape[0])
+                        "got {} classes and kernel_psi has shape {}".format(
+                            self.classes_.size, kernel_psi.shape[0]
+                        )
                     )
 
             out = kernel_latent_time_graphical_lasso(
                 emp_cov,
                 alpha=self.alpha,
                 tau=self.tau,
                 rho=self.rho,
@@ -803,15 +883,21 @@
                 return_n_iter=True,
                 return_history=self.return_history,
                 update_rho_options=self.update_rho_options,
                 compute_objective=self.compute_objective,
                 init=self.init,
             )
             if self.return_history:
-                (self.precision_, self.latent_, self.covariance_, self.history_, self.n_iter_) = out
+                (
+                    self.precision_,
+                    self.latent_,
+                    self.covariance_,
+                    self.history_,
+                    self.n_iter_,
+                ) = out
             else:
                 (self.precision_, self.latent_, self.covariance_, self.n_iter_) = out
 
         return self
 
     def transform(self, X, y=None):
         """Possibility to add in a Pipeline."""
```

### Comparing `regain-0.3.3/regain/covariance/__init__.py` & `regain-0.3.8/regain/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/latent_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/latent_graphical_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/covariance/kernel_time_graphical_lasso_.py` & `regain-0.3.8/regain/covariance/kernel_time_graphical_lasso_.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 from scipy import linalg
 from six.moves import map, range, zip
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_is_fitted
 
-from regain.covariance.time_graphical_lasso_ import TimeGraphicalLasso, init_precision, loss
+from regain.covariance.time_graphical_lasso_ import (
+    TimeGraphicalLasso,
+    init_precision,
+    loss,
+)
 from regain.norm import l1_od_norm
 from regain.prox import prox_logdet, soft_thresholding
 from regain.update_rules import update_rho
 from regain.utils import convergence
 from regain.validation import check_norm_prox
 
 # from regain.clustering import graph_k_means
@@ -154,15 +158,19 @@
         Z_L_old = np.zeros_like(Z_L)
         Z_R_old = np.zeros_like(Z_R)
         Z_M_old[m] = (Z_L_old, Z_R_old)
 
     if n_samples is None:
         n_samples = np.ones(n_times)
 
-    checks = [convergence(obj=objective(n_samples, emp_cov, Z_0, Z_0, Z_M, alpha, kernel, psi))]
+    checks = [
+        convergence(
+            obj=objective(n_samples, emp_cov, Z_0, Z_0, Z_M, alpha, kernel, psi)
+        )
+    ]
     for iteration_ in range(max_iter):
         # update K
         A = Z_0 - U_0
         for m in range(1, n_times):
             A[:-m] += Z_M[m][0] - U_M[m][0]
             A[m:] += Z_M[m][1] - U_M[m][1]
 
@@ -171,15 +179,17 @@
         # K = np.array(map(soft_thresholding_, A))
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
         A *= -rho * n_times / n_samples[:, None, None]
         A += emp_cov
 
-        K = np.array([prox_logdet(a, lamda=ni / (rho * n_times)) for a, ni in zip(A, n_samples)])
+        K = np.array(
+            [prox_logdet(a, lamda=ni / (rho * n_times)) for a, ni in zip(A, n_samples)]
+        )
 
         # update Z_0
         A = K + U_0
         A += A.transpose(0, 2, 1)
         A /= 2.0
         Z_0 = soft_thresholding(A, lamda=alpha / rho)
 
@@ -188,15 +198,17 @@
 
         # other Zs
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             A_L = K[:-m] + U_L
             A_R = K[m:] + U_R
             if not psi_node_penalty:
-                prox_e = prox_psi(A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho)
+                prox_e = prox_psi(
+                    A_R - A_L, lamda=2.0 * np.diag(kernel, m)[:, None, None] / rho
+                )
                 Z_L = 0.5 * (A_L + A_R - prox_e)
                 Z_R = 0.5 * (A_L + A_R + prox_e)
             else:
                 Z_L, Z_R = prox_psi(
                     np.concatenate((A_L, A_R), axis=1),
                     lamda=0.5 * np.diag(kernel, m)[:, None, None] / rho,
                     rho=rho,
@@ -209,63 +221,89 @@
             # update other residuals
             U_L += K[:-m] - Z_L
             U_R += K[m:] - Z_R
 
         # diagnostics, reporting, termination checks
         rnorm = np.sqrt(
             squared_norm(K - Z_0)
-            + sum(squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1]) for m in range(1, n_times))
+            + sum(
+                squared_norm(K[:-m] - Z_M[m][0]) + squared_norm(K[m:] - Z_M[m][1])
+                for m in range(1, n_times)
+            )
         )
 
         snorm = rho * np.sqrt(
             squared_norm(Z_0 - Z_0_old)
             + sum(
-                squared_norm(Z_M[m][0] - Z_M_old[m][0]) + squared_norm(Z_M[m][1] - Z_M_old[m][1])
+                squared_norm(Z_M[m][0] - Z_M_old[m][0])
+                + squared_norm(Z_M[m][1] - Z_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
-        obj = objective(n_samples, emp_cov, Z_0, K, Z_M, alpha, kernel, psi) if compute_objective else np.nan
+        obj = (
+            objective(n_samples, emp_cov, Z_0, K, Z_M, alpha, kernel, psi)
+            if compute_objective
+            else np.nan
+        )
 
         check = convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
                 np.sqrt(
                     squared_norm(Z_0)
-                    + sum(squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1]) for m in range(1, n_times))
+                    + sum(
+                        squared_norm(Z_M[m][0]) + squared_norm(Z_M[m][1])
+                        for m in range(1, n_times)
+                    )
+                ),
+                np.sqrt(
+                    squared_norm(K)
+                    + sum(
+                        squared_norm(K[:-m]) + squared_norm(K[m:])
+                        for m in range(1, n_times)
+                    )
                 ),
-                np.sqrt(squared_norm(K) + sum(squared_norm(K[:-m]) + squared_norm(K[m:]) for m in range(1, n_times))),
             ),
             e_dual=n_features * n_times * tol
             + rtol
             * rho
             * np.sqrt(
-                squared_norm(U_0) + sum(squared_norm(U_M[m][0]) + squared_norm(U_M[m][1]) for m in range(1, n_times))
+                squared_norm(U_0)
+                + sum(
+                    squared_norm(U_M[m][0]) + squared_norm(U_M[m][1])
+                    for m in range(1, n_times)
+                )
             ),
         )
         Z_0_old = Z_0.copy()
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(
+                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
+                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
+            )
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         U_0 *= rho / rho_new
         for m in range(1, n_times):
             U_L, U_R = U_M[m]
             U_L *= rho / rho_new
             U_R *= rho / rho_new
         rho = rho_new
@@ -440,15 +478,20 @@
             # initialise precision matrices, as warm start
             self.precision_ = init_precision(emp_cov, mode=self.init)
             theta_old = 0
             for i in range(self.max_iter_ext):
                 # E step - discover best kernel parameter
                 theta = minimize_scalar(
                     objective_kernel,
-                    args=(self.precision_, self.psi, self.kernel, self.classes_[:, None]),
+                    args=(
+                        self.precision_,
+                        self.psi,
+                        self.kernel,
+                        self.classes_[:, None],
+                    ),
                     bounds=(0, emp_cov.shape[0]),
                     method="bounded",
                 ).x
 
                 if i > 0 and abs(theta_old - theta) < 1e-5:
                     break
                 else:
@@ -476,35 +519,46 @@
                     return_n_iter=True,
                     return_history=self.return_history,
                     update_rho_options=self.update_rho_options,
                     compute_objective=self.compute_objective,
                     init=self.precision_,
                 )
                 if self.return_history:
-                    (self.precision_, self.covariance_, self.history_, self.n_iter_) = out
+                    (
+                        self.precision_,
+                        self.covariance_,
+                        self.history_,
+                        self.n_iter_,
+                    ) = out
                 else:
                     self.precision_, self.covariance_, self.n_iter_ = out
                 theta_old = theta
             else:
                 print("warning: theta not converged")
 
         else:
             if callable(self.kernel):
                 try:
                     # this works if it is a ExpSineSquared or RBF kernel
-                    kernel = self.kernel(length_scale=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(length_scale=self.ker_param)(
+                        self.classes_[:, None]
+                    )
                 except TypeError:
                     # maybe it's a ConstantKernel
-                    kernel = self.kernel(constant_value=self.ker_param)(self.classes_[:, None])
+                    kernel = self.kernel(constant_value=self.ker_param)(
+                        self.classes_[:, None]
+                    )
             else:
                 kernel = self.kernel
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
-                        "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                        "got {} classes and kernel has shape {}".format(
+                            self.classes_.size, kernel.shape[0]
+                        )
                     )
 
             out = kernel_time_graphical_lasso(
                 emp_cov,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
@@ -646,14 +700,15 @@
             # idx = np.triu_indices(n_times, 1)
             kernel = np.eye(n_times)
 
             psi, _, _ = check_norm_prox(self.psi)
             if self.n_clusters is None:
                 self.n_clusters = n_times
 
+            labels_pred_old = None
             for i in range(self.max_iter_ext):
                 # E step - discover best kernel
                 # , method='bounded'bounds=[(0, None)]*theta_old.size
                 # theta = minimize(
                 #     objective_similarity, theta_old,
                 #     args=(self.precision_, self.classes_[:, None], psi)
                 #     ).x
@@ -666,21 +721,27 @@
                 #     break
 
                 # kernel[idx] = theta
                 # kernel[idx[::-1]] = theta
                 kernel = theta
 
                 labels_pred = AgglomerativeClustering(
-                    n_clusters=self.n_clusters, affinity="precomputed", linkage="complete"
+                    n_clusters=self.n_clusters,
+                    affinity="precomputed",
+                    linkage="complete",
                 ).fit_predict(kernel)
-                if i > 0 and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size < self.eps:
+                if (
+                    i > 0
+                    and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size
+                    < self.eps
+                ):
                     break
-                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(self.beta)(
-                    np.arange(n_times)[:, None]
-                )
+                kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(
+                    self.beta
+                )(np.arange(n_times)[:, None])
 
                 # normalize_matrix(kernel_sum)
                 # kernel += kerne * self.beta
 
                 # M step - fix the kernel matrix
                 out = kernel_time_graphical_lasso(
                     emp_cov,
@@ -697,15 +758,20 @@
                     return_history=self.return_history,
                     update_rho_options=self.update_rho_options,
                     compute_objective=self.compute_objective,
                     init=self.precision_,
                 )
 
                 if self.return_history:
-                    (self.precision_, self.covariance_, self.history_, self.n_iter_) = out
+                    (
+                        self.precision_,
+                        self.covariance_,
+                        self.history_,
+                        self.n_iter_,
+                    ) = out
                 else:
                     self.precision_, self.covariance_, self.n_iter_ = out
                 theta_old = theta
                 labels_pred_old = labels_pred
                 # kernel = graph_k_means(
                 #   list(self.precision_), 3, max_iter=100)
                 # self.similarity_matrix = kernel
@@ -718,15 +784,17 @@
             self.similarity_matrix_ = kernel
 
         else:
             kernel = self.kernel
             if kernel.shape[0] != self.classes_.size:
                 raise ValueError(
                     "Kernel size does not match classes of samples, "
-                    "got {} classes and kernel has shape {}".format(self.classes_.size, kernel.shape[0])
+                    "got {} classes and kernel has shape {}".format(
+                        self.classes_.size, kernel.shape[0]
+                    )
                 )
 
             out = kernel_time_graphical_lasso(
                 emp_cov,
                 alpha=self.alpha,
                 rho=self.rho,
                 kernel=kernel,
```

### Comparing `regain-0.3.3/regain/linear_model/group_lasso_overlap_.py` & `regain-0.3.8/regain/linear_model/group_lasso_overlap_.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import warnings
 
 import numpy as np
 import six
 from scipy import sparse
 from six.moves import range
 from sklearn.base import RegressorMixin
-from sklearn.linear_model.base import LinearClassifierMixin, LinearModel, _pre_fit
+from sklearn.linear_model._base import LinearClassifierMixin, LinearModel, _pre_fit # noqa
 from sklearn.preprocessing import LabelBinarizer
 from sklearn.utils import check_array, check_X_y, deprecated
 from sklearn.utils.extmath import safe_sparse_dot
 from sklearn.utils.validation import check_is_fitted
 
 from regain.prox import soft_thresholding
 from regain.utils import flatten
@@ -102,15 +102,15 @@
     A : array-like, 2-dimensional
         Input matrix.
     b : array-like, 1-dimensional
         Output vector.
     lamda : float, optional
         Regularisation parameter.
     groups : list
-        Groups of variables.
+        Groups of variables in the form list-of-lists.
     rho : float, optional
         Augmented Lagrangian parameter.
     alpha : float, optional
         Over-relaxation parameter (typically between 1.0 and 1.8).
     max_iter : int, optional
         Maximum number of iterations.
     tol : float, optional
@@ -198,18 +198,28 @@
         warm_start=False,
         positive=False,
         random_state=None,
         selection="cyclic",
         mode="admm",
         matlab_engine=None,
     ):
+        # TODO(Add documentation.)
+        """Group Lasso class.
+
+        Parameters
+        -----------
+        ...
+        groups: list
+            List of list of variables to group. For example, groups=[[1,2]].
+            Default None.
+        """
         self.alpha = alpha
         self.coef_ = None
         self.fit_intercept = fit_intercept
-        self.groups = groups
+        self.groups = groups or []
         self.rho = rho
         self.verbose = verbose
         self.normalize = normalize
         self.precompute = precompute
         self.max_iter = max_iter
         self.copy_X = copy_X
         self.tol = tol
@@ -509,15 +519,15 @@
     Atb = A.T.dot(b)
     inverse = np.linalg.inv(N * AtA + rho * np.eye(d))
     for k in range(max_iter):
         # % x-update (to be done in parallel)
         P_star_xk_bar = P_star_x_bar_function(x)
         for i, g in enumerate(groups):
             # x update; update each local x
-            x[i] = prox(x[i] + (z - P_star_xk_bar - y / rho)[g], lamda / rho)
+            x[i] = soft_thresholding(x[i] + (z - P_star_xk_bar - y / rho)[g], lamda / rho)
 
         P_star_xk1_bar = P_star_x_bar_function(x)
         z = inverse.dot(Atb + rho * P_star_xk1_bar + y)
 
         # y-update
         y += rho * (P_star_xk1_bar - z)
```

### Comparing `regain-0.3.3/regain/linear_model/_group_lasso_overlap_old_.py` & `regain-0.3.8/regain/linear_model/_group_lasso_overlap_old_.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,21 +128,22 @@
         for i in range(N):
             # % dual residual norm square
             s = s + np.linalg.norm(-rho * Ats[i].dot((zs[:, i] - zsold[:, i]))) ** 2
             # % dual residual epsilon
             q = q + np.linalg.norm(rho * Ats[i].dot(u)) ** 2
 
         # % diagnostics, reporting, termination checks
-        history = []
-        history.append(objective(A, b, lamda, x, z))
-        history.append(np.sqrt(N) * np.linalg.norm(z - Axbar))
-        history.append(np.sqrt(s))
-
-        history.append(np.sqrt(n) * ABSTOL + RELTOL * max(np.linalg.norm(Aixi, "fro"), np.linalg.norm(-zs, "fro")))
-        history.append(np.sqrt(n) * ABSTOL + RELTOL * np.sqrt(q))
+        history = [
+            objective(A, b, lamda, x, z),
+            np.sqrt(N) * np.linalg.norm(z - Axbar),
+            np.sqrt(s),
+            np.sqrt(n) * ABSTOL
+            + RELTOL * max(np.linalg.norm(Aixi, "fro"), np.linalg.norm(-zs, "fro")),
+            np.sqrt(n) * ABSTOL + RELTOL * np.sqrt(q),
+        ]
 
         hist.append(history)
         if history[1] < history[3] and history[2] < history[4]:
             break
 
     return x
```

### Comparing `regain-0.3.3/regain/linear_model/lasso_.py` & `regain-0.3.8/regain/linear_model/lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/linear_model/group_lasso_.py` & `regain-0.3.8/regain/linear_model/group_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/linear_model/__init__.py` & `regain-0.3.8/regain/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/validation.py` & `regain-0.3.8/regain/validation.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/prox.py` & `regain-0.3.8/regain/prox.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/plotting/graph.py` & `regain-0.3.8/regain/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/plotting/covariance.py` & `regain-0.3.8/regain/plotting/covariance.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/plotting/__init__.py` & `regain-0.3.8/regain/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/plotting/results.py` & `regain-0.3.8/regain/plotting/results.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,80 +55,118 @@
 
     for i, p in enumerate(preds):
         fpr, tpr, thresholds = roc_curve(true, p)
         tprs.append(interp(mean_fpr, fpr, tpr))
         tprs[-1][0] = 0.0
         roc_auc = auc(fpr, tpr)
         aucs.append(roc_auc)
-        ax.plot(fpr, tpr, lw=1, alpha=0.3, label="ROC fold %d (AUC = %0.2f)" % (i, roc_auc))
+        ax.plot(
+            fpr, tpr, lw=1, alpha=0.3, label="ROC fold %d (AUC = %0.2f)" % (i, roc_auc)
+        )
 
     mean_tpr = np.mean(tprs, axis=0)
     mean_tpr[-1] = 1.0
     mean_auc = auc(mean_fpr, mean_tpr)
     std_auc = np.std(aucs)
     ax.plot(
         mean_fpr,
         mean_tpr,
         color="b",
-        label=r"Mean ROC (AUC = %0.2f $\pm$ %0.2f)" % (mean_auc, std_auc),
+        label=rf"Mean ROC (AUC = {mean_auc:0.2f} $\pm$ {std_auc:0.2f})",
         lw=2,
         alpha=0.8,
     )
 
     std_tpr = np.std(tprs, axis=0)
     tprs_upper = np.minimum(mean_tpr + std_tpr, 1)
     tprs_lower = np.maximum(mean_tpr - std_tpr, 0)
-    ax.fill_between(mean_fpr, tprs_lower, tprs_upper, color="grey", alpha=0.2, label=r"$\pm$ 1 std. dev.")
+    ax.fill_between(
+        mean_fpr,
+        tprs_lower,
+        tprs_upper,
+        color="grey",
+        alpha=0.2,
+        label=r"$\pm$ 1 std. dev.",
+    )
 
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_xlabel("False Positive Rate")
     ax.set_ylabel("True Positive Rate")
     ax.legend(loc="lower right")
     plt.show()
 
 
-def plot_curve(true, predictions, mode="roc", ax=None, filename=None, fontsize=15, colors=None, multiple_true=False):
+def plot_curve(
+    true,
+    predictions,
+    mode="roc",
+    ax=None,
+    filename=None,
+    fontsize=15,
+    colors=None,
+    multiple_true=False,
+):
     """Plot a validation curve.
 
     Parameters
     ----------
     predictions : dict
         Keys is the algorithm, values list of predictions.
     mode : ('roc', 'precision_recall')
         Which curve to plot.
     """
     matplotlib.rcParams.update({"font.size": fontsize})
     if ax is None:
         fig, ax = plt.subplots(figsize=(15, 10))
-    ax.plot(([0, 1] if mode == "roc" else [1, 0]), [0, 1], linestyle="--", lw=2, color="k", label="Chance", alpha=0.8)
+    ax.plot(
+        ([0, 1] if mode == "roc" else [1, 0]),
+        [0, 1],
+        linestyle="--",
+        lw=2,
+        color="k",
+        label="Chance",
+        alpha=0.8,
+    )
     curve_func = roc_curve if mode == "roc" else precision_recall_curve
     for c, (key, preds) in enumerate(predictions.items()):
         if len(preds) == 1:
             if true.ndim != 2:
                 true = (~np.isclose(true, 0, rtol=1e-7)).astype(int).ravel()
                 preds_new = []
                 for p in preds:
                     preds_new.append(p.ravel())
                 preds = preds_new
             fpr, tpr, thresholds = curve_func(true, preds[0])
             kwargs = dict(lw=1, color=colors[c] if colors is not None else None)
             if mode == "roc":
                 roc_auc = auc(fpr, tpr)
-                ax.plot(fpr, tpr, label="%s %s (AUC = %0.2f)" % (mode, str(key), roc_auc), **kwargs)
+                ax.plot(
+                    fpr,
+                    tpr,
+                    label="%s %s (AUC = %0.2f)" % (mode, str(key), roc_auc),
+                    **kwargs,
+                )
             else:
                 roc_auc = auc(tpr, fpr)
-                ax.plot(tpr, fpr, label="%s %s (AUC = %0.2f)" % (mode, str(key), roc_auc), **kwargs)
+                ax.plot(
+                    tpr,
+                    fpr,
+                    label="%s %s (AUC = %0.2f)" % (mode, str(key), roc_auc),
+                    **kwargs,
+                )
         else:
             tprs = []
             aucs = []
             mean_fpr = np.linspace(0, 1, 100)
 
             if multiple_true:
-                true = [(~np.isclose(t, 0, rtol=1e-7)).astype(int).ravel() for t in true]
+                true = [
+                    (~np.isclose(t, 0, rtol=1e-7)).astype(int).ravel() for t in true
+                ]
             else:
                 true = (~np.isclose(true, 0, rtol=1e-7)).astype(int).ravel()
             preds = [p.ravel() for p in preds]
 
             for i, p in enumerate(preds):
                 if multiple_true:
                     t = true[i]
@@ -147,15 +185,16 @@
             mean_tpr[-1] = int(mode == "roc")
             mean_auc = auc(mean_fpr, mean_tpr)
             std_auc = np.std(aucs)
             ax.plot(
                 mean_fpr,
                 mean_tpr,
                 color=colors[c] if colors is not None else None,
-                label=r"Mean %s %s (AUC = %0.2f $\pm$ %0.2f)" % (mode, str(key), mean_auc, std_auc),
+                label=r"Mean %s %s (AUC = %0.2f $\pm$ %0.2f)"
+                % (mode, str(key), mean_auc, std_auc),
                 lw=2,
                 alpha=0.9,
             )
 
             std_tpr = np.std(tprs, axis=0)
             tprs_upper = np.minimum(mean_tpr + std_tpr, 1)
             tprs_lower = np.maximum(mean_tpr - std_tpr, 0)
@@ -173,18 +212,44 @@
     ax.grid()
     if filename is not None:
         plt.savefig(filename, dpi=300, transparent=True, bbox_inches="tight")
     plt.show()
 
 
 @deprecated
-def plot_roc_comparison(true, predictions, ax=None, filename=None, fontsize=15, colors=("red", "blue", "yellow")):
-    return plot_curve(true, predictions, mode="roc", ax=ax, filename=filename, fontsize=fontsize, colors=colors)
+def plot_roc_comparison(
+    true,
+    predictions,
+    ax=None,
+    filename=None,
+    fontsize=15,
+    colors=("red", "blue", "yellow"),
+):
+    return plot_curve(
+        true,
+        predictions,
+        mode="roc",
+        ax=ax,
+        filename=filename,
+        fontsize=fontsize,
+        colors=colors,
+    )
 
 
 @deprecated
 def plot_precision_recall_comparison(
-    true, predictions, ax=None, filename=None, fontsize=15, colors=("red", "blue", "yellow")
+    true,
+    predictions,
+    ax=None,
+    filename=None,
+    fontsize=15,
+    colors=("red", "blue", "yellow"),
 ):
     return plot_curve(
-        true, predictions, mode="precision_recall", ax=ax, filename=filename, fontsize=fontsize, colors=colors
+        true,
+        predictions,
+        mode="precision_recall",
+        ax=ax,
+        filename=filename,
+        fontsize=fontsize,
+        colors=colors,
     )
```

### Comparing `regain-0.3.3/regain/plotting/plotly.py` & `regain-0.3.8/regain/plotting/plotly.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/__init__.py` & `regain-0.3.8/regain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.3"
+__version__ = "0.3.8"
```

### Comparing `regain-0.3.3/regain/datasets/ising.py` & `regain-0.3.8/regain/datasets/ising.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/datasets/gaussian.py` & `regain-0.3.8/regain/datasets/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 
 import numpy as np
 from scipy import signal
 from scipy.spatial.distance import squareform
 from scipy.stats import norm
 from sklearn.utils import check_random_state
 
-from regain.utils import ensure_posdef
-from regain.utils import is_pos_def
-from regain.utils import is_pos_semidef
-from regain.utils import normalize_matrix
+from regain.utils import ensure_posdef, is_pos_def, is_pos_semidef, normalize_matrix
 
 
 def _compute_probabilities(locations, random_state, mask=None):
     p = len(locations)
     if mask is None:
         mask = np.zeros((p, p))
     probabilities = np.zeros((p, p))
@@ -56,17 +53,19 @@
     thresholds = random_state.uniform(low=0, high=1, size=(p, p))
     probabilities[np.where(thresholds > probabilities)] = 0
     return probabilities
 
 
 def _permute_locations(locations, random_state):
     new_locations = []
-    for l in locations:
+    for loc in locations:
         perm = random_state.uniform(low=-0.03, high=0.03, size=(1, 2))
-        new_locations.append(np.maximum(np.array(l) + np.array(perm), 0).flatten().tolist())
+        new_locations.append(
+            np.maximum(np.array(loc) + np.array(perm), 0).flatten().tolist()
+        )
     return new_locations
 
 
 def _theta_my(probs, p, random_state, value=0.245):
     theta = np.zeros((p, p))
     for i in range(p):
         ix = np.argsort(probs[i, :])[::-1]
@@ -135,15 +134,17 @@
         thetas_observed.append(theta_observed)
         covariances.append(sigma)
         sampless.append(random_state.multivariate_normal(np.zeros(p), sigma, size=n))
 
     return locations, thetas, thetas_observed, covariances, latent, sampless
 
 
-def data_Meinshausen_Yuan_sparse_latent(p=198, h=2, n=200, T=10, random_state=None, **kwargs):
+def data_Meinshausen_Yuan_sparse_latent(
+    p=198, h=2, n=200, T=10, random_state=None, **kwargs
+):
     random_state = check_random_state(random_state)
     nodes_locations = [list(random_state.uniform(size=2)) for i in range(p + h)]
     probs = _compute_probabilities(nodes_locations, random_state)
     theta = _theta_my(probs[:, :-h], p, random_state=random_state)
 
     latent = np.zeros((h, p + h))
     to_put = (p + h) * 0.5
@@ -249,15 +250,17 @@
 
 def make_ell(n_dim_obs=100, n_dim_lat=10):
     """Make ell matrix."""
     K_HO = np.zeros((n_dim_lat, n_dim_obs))
     for i in range(n_dim_lat):
         percentage = int(n_dim_obs * 0.99)
         indices = np.random.randint(0, high=n_dim_obs, size=percentage)
-        K_HO[i, indices] = np.random.rand(percentage) * (0.98 / (n_dim_lat + n_dim_obs) / 2)
+        K_HO[i, indices] = np.random.rand(percentage) * (
+            0.98 / (n_dim_lat + n_dim_obs) / 2
+        )
 
     K_HO /= np.sum(K_HO, axis=1)[:, None] / 2.0
     L = K_HO.T.dot(K_HO)
     # print("{}%".format(np.nonzero(L)[0].size / L.size))
     assert is_pos_semidef(L)
     assert np.linalg.matrix_rank(L) == n_dim_lat
     # from sklearn.datasets import make_low_rank_matrix
@@ -272,15 +275,18 @@
     L, K_HO = make_ell(n_dim_obs, n_dim_lat)
 
     if normalize:
         theta = np.zeros((n_dim_obs, n_dim_obs))
         for i in range(n_dim_obs):
             possible_idx = list(
                 set(range(n_dim_obs))
-                - (set(np.nonzero(theta[i, :])[0]) | set(np.where(np.count_nonzero(theta, axis=1) > degree)[0]))
+                - (
+                    set(np.nonzero(theta[i, :])[0])
+                    | set(np.where(np.count_nonzero(theta, axis=1) > degree)[0])
+                )
             )
             if not possible_idx:
                 continue
             n_choice = degree - (np.count_nonzero(theta[i, :]) - 1)
             if n_choice > 0:
                 indices = np.random.choice(possible_idx, n_choice)
             theta[i, indices] = theta[indices, i] = 1.0 / degree
@@ -288,15 +294,18 @@
         theta.flat[:: n_dim_obs + 1] = np.sum(theta, axis=1) + 0.002
 
     else:
         theta = np.eye(n_dim_obs)
         for i in range(n_dim_obs):
             possible_idx = list(
                 set(range(n_dim_obs))
-                - (set(np.nonzero(theta[i, :])[0]) | set(np.where(np.count_nonzero(theta, axis=1) > degree)[0]))
+                - (
+                    set(np.nonzero(theta[i, :])[0])
+                    | set(np.where(np.count_nonzero(theta, axis=1) > degree)[0])
+                )
             )
             if not possible_idx:
                 continue
             n_choice = degree - (np.count_nonzero(theta[i, :]) - 1)
             if n_choice > 0:
                 indices = np.random.choice(possible_idx, n_choice)
                 theta[i, indices] = theta[indices, i] = 0.5 / degree
@@ -305,15 +314,17 @@
         theta += np.diag(np.sum(theta, axis=1) + eps)
     if not is_pos_def(theta - L):
         theta += np.diag(eps + np.diag(L))
     assert is_pos_def(theta - L)
     return theta, theta - L, L, K_HO
 
 
-def _update_theta_l2(theta_old, n_dim_obs, degree, epsilon, keep_sparsity=False, indices=None):
+def _update_theta_l2(
+    theta_old, n_dim_obs, degree, epsilon, keep_sparsity=False, indices=None
+):
     addition = np.zeros_like(theta_old)
     for i in range(n_dim_obs):
         if keep_sparsity:
             ii = indices[i]
         else:
             ii = np.random.randint(0, n_dim_obs, size=degree)
         addition[i, ii] = np.random.randn(len(ii))
@@ -329,15 +340,17 @@
     theta = theta_init.copy()
     rows = np.zeros(no)
     cols = np.zeros(no)
     while np.any(rows == cols):
         rows = np.random.randint(0, n_dim_obs, no)
         cols = np.random.randint(0, n_dim_obs, no)
     for r, c in zip(rows, cols):
-        theta[r, c] = np.random.choice([0.12, 0, 0]) if theta[r, c] == 0 else 0.06  # np.random.rand(1) * .35
+        theta[r, c] = (
+            np.random.choice([0.12, 0, 0]) if theta[r, c] == 0 else 0.06
+        )  # np.random.rand(1) * .35
         theta[c, r] = theta[r, c]
     if not is_pos_def(theta):
         theta += np.diag(np.sum(theta, axis=1) + eps)
     return theta
 
 
 def _update_ell_l2(K_HO_old, epsilon, n_dim_obs):
@@ -362,29 +375,40 @@
     epsilon=1e-2,
     keep_sparsity=False,
     proportional=False,
 ):
     """Generate a list of T covariances and sparse precisions."""
     no = int(np.ceil(n_dim_obs / 20)) if proportional else 1
 
-    theta, theta_observed, L, K_HO = make_starting(n_dim_obs, n_dim_lat, degree, normalize=normalize_starting_matrices)
+    theta, theta_observed, L, K_HO = make_starting(
+        n_dim_obs, n_dim_lat, degree, normalize=normalize_starting_matrices
+    )
 
     thetas = [theta]
     thetas_obs = [theta_observed]
     ells = [L]
     K_HOs = [K_HO]
 
     idx = [np.nonzero(row)[0] for row in theta] if keep_sparsity else None
     for i in range(1, T):
         if update_theta == "l1":
             if keep_sparsity:
-                warnings.warn("keep_sparsity is specified but is not " "implemented with l1.")
+                warnings.warn(
+                    "keep_sparsity is specified but is not " "implemented with l1."
+                )
             theta = _update_theta_l1(thetas[-1], no, n_dim_obs)
         elif update_theta == "l2":
-            theta = _update_theta_l2(thetas[-1], n_dim_obs, degree, epsilon, keep_sparsity=keep_sparsity, indices=idx)
+            theta = _update_theta_l2(
+                thetas[-1],
+                n_dim_obs,
+                degree,
+                epsilon,
+                keep_sparsity=keep_sparsity,
+                indices=idx,
+            )
         else:
             raise ValueError(update_theta)
 
         if update_ell == "fixed" or n_dim_lat < 1:
             pass  # L is fixed or empty
         elif update_ell == "l1":
             K_HO = K_HOs[-1].copy()
@@ -419,15 +443,17 @@
 
 
 def make_fixed_sparsity(n_dim_obs=100, n_dim_lat=10, T=10, **kwargs):
     """Generate precisions with a fixed L matrix and sparsity."""
     degree = kwargs.get("degree", 2)
     epsilon = kwargs.get("epsilon", 1e-2)
     t = kwargs.get("changing_time", T / 2.0)
-    theta, theta_observed, L, K_HO = make_starting(n_dim_obs, n_dim_lat, degree, normalize=False)
+    theta, theta_observed, L, K_HO = make_starting(
+        n_dim_obs, n_dim_lat, degree, normalize=False
+    )
 
     theta = np.abs(theta)
     theta_observed = theta - L
     nonzeros = np.nonzero(theta - np.diag(theta))
 
     thetas = [theta]
     thetas_obs = [theta_observed]
@@ -437,26 +463,30 @@
         if t < T:
             theta[nonzeros] += np.random.randn(nonzeros[0].size) * 0.1
         else:
             theta[nonzeros] -= np.random.randn(nonzeros[0].size) * 0.1
         theta = np.abs(theta)
         theta = (theta + theta.T) / 2.0
         theta[theta < epsilon] = 0
-        theta.flat[:: n_dim_obs + 1] = np.sum(np.abs(theta), axis=1) + np.sum(np.abs(L), axis=1) + 0.1
+        theta.flat[:: n_dim_obs + 1] = (
+            np.sum(np.abs(theta), axis=1) + np.sum(np.abs(L), axis=1) + 0.1
+        )
         nonzeros = np.nonzero(theta - np.diag(theta))
 
         theta_observed = theta - L
         assert is_pos_def(theta_observed)
         thetas.append(theta)
         thetas_obs.append(theta_observed)
 
     return thetas, thetas_obs, np.array([L] * T)
 
 
-def make_sin(n_dim_obs, n_dim_lat, T, shape="smooth", closeness=1, normalize=False, **kwargs):
+def make_sin(
+    n_dim_obs, n_dim_lat, T, shape="smooth", closeness=1, normalize=False, **kwargs
+):
     """Generate list of sparse precision matrices that change periodically."""
     upper_idx = np.triu_indices(n_dim_obs, 1)
     n_interactions = len(upper_idx[0])
     x = np.tile(np.linspace(0, (T - 1.0) / closeness, T), (n_interactions, 1))
     phase = np.random.rand(n_interactions, 1)
     freq = np.random.rand(n_interactions, 1) - 0.50
     A = (np.random.rand(n_interactions, 1) + 1) / 2.0
@@ -465,15 +495,20 @@
         y = A * np.sin(2.0 * np.pi * freq * x + phase)
     else:
         y = A * signal.square(2 * np.pi * freq * x + phase, duty=0.5)
 
     # threshold
     y = np.maximum(y, 0)
 
-    Y = np.array([squareform(y[:, j]) + np.diag(np.sum(squareform(y[:, j]), axis=1)) for j in range(y.shape[1])])
+    Y = np.array(
+        [
+            squareform(y[:, j]) + np.diag(np.sum(squareform(y[:, j]), axis=1))
+            for j in range(y.shape[1])
+        ]
+    )
 
     if normalize:
         map(normalize_matrix, Y)  # in place
     # assert positive_definite(Y)
     ensure_posdef(Y)
 
     return Y, Y, np.zeros_like(Y)
@@ -503,15 +538,15 @@
     x = np.linspace(0, 2 * np.pi, T)
     for i in range(T):
         for r in range(n_dim_obs):
             for c in range(n_dim_obs):
                 if r == c:
                     continue
                 if clip[r, c]:
-                    thetas[i, r, c] = np.sin((x[i] + phase[r, c]) / T ** 2)
+                    thetas[i, r, c] = np.sin((x[i] + phase[r, c]) / T**2)
                 else:
                     thetas[i, r, c] = np.sin((x[i] + phase[r, c]))
         thetas[i][clip == 1] = np.clip(thetas[i][clip == 1], 0, 1)
         thetas[i][np.abs(thetas[i]) < eps] = 0
 
         assert is_pos_def(thetas[i])
         theta_observed = thetas[i] - L
@@ -579,15 +614,17 @@
         Ks.append(K)
         Ls.append(L)
         Kobs.append(K - L)
 
     return Ks, Kobs, Ls
 
 
-def make_ma_xue_zou(n_dim_obs=12, n_latent=3, T=1, epsilon=1e-3, sparsity=0.1, **kwargs):
+def make_ma_xue_zou(
+    n_dim_obs=12, n_latent=3, T=1, epsilon=1e-3, sparsity=0.1, **kwargs
+):
     """Generate the dataset as in Ma, Xue, Zou (2012)."""
     # p = n_dim_obs + n_latent  # int(n_dim_obs * 0.05)
     p = n_dim_obs + int(n_dim_obs * 0.05)
     po = n_dim_obs
     ph = p - n_dim_obs
     W = np.zeros((p, p))
     non_zeros = int(round(p * p * sparsity))
@@ -618,15 +655,17 @@
     # print(ph)
 
     N = 5 * po
     print("Note that, with this method, the n_samples should be %d" % N)
     return [K_O] * T, [K_O_tilde] * T, [L] * T
 
 
-def make_ma_xue_zou_rand_k(n_dim_obs=12, n_latent=3, T=1, epsilon=1e-3, sparsity=0.1, **kwargs):
+def make_ma_xue_zou_rand_k(
+    n_dim_obs=12, n_latent=3, T=1, epsilon=1e-3, sparsity=0.1, **kwargs
+):
     """Generate the dataset as in Ma, Xue, Zou (2012)."""
     # p = n_dim_obs + n_latent  # int(n_dim_obs * 0.05)
     p = n_dim_obs + int(n_dim_obs * 0.05)
     po = n_dim_obs
     nnzr = int(sparsity * (np.triu_indices(p, 1)[0].size))
 
     # Generate A, the original inverse covariance
```

### Comparing `regain-0.3.3/regain/datasets/poisson.py` & `regain-0.3.8/regain/datasets/poisson.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,22 @@
             G[r, c] = np.random.choice([0, G[r, c]])
             G[c, r] = G[r, c]
     assert np.all(G == G.T)
     return G
 
 
 def poisson_theta_generator(
-    n_dim_obs=10, T=10, mode="l1", random_graph="erdos-renyi", probability=0.2, degree=3, n_to_change=3, **kwargs
+    n_dim_obs=10,
+    T=10,
+    mode="l1",
+    random_graph="erdos-renyi",
+    probability=0.2,
+    degree=3,
+    n_to_change=3,
+    **kwargs
 ):
     """Generates adjacency matix for Ising graphical model.
 
     Parameters
     ----------
     n_dim_obs: int optional default 10
         Number of variables.
@@ -85,15 +92,17 @@
     import networkx as nx
 
     if random_graph.lower() == "erdos-renyi":
         graph = nx.random_graphs.fast_gnp_random_graph(n=n_dim_obs, p=probability)
     elif random_graph.lower() == "scale-free":
         graph = nx.random_graphs.barabasi_albert_graph(n=n_dim_obs, m=degree)
     elif random_graph.lower() == "small-world":
-        graph = nx.random_graphs.watts_strogatz_graph(n=n_dim_obs, k=degree, p=probability)
+        graph = nx.random_graphs.watts_strogatz_graph(
+            n=n_dim_obs, k=degree, p=probability
+        )
     else:
         graph = nx.random_graphs.gnm_random_graph(n=n_dim_obs, m=degree)
     graph = nx.adjacency_matrix(graph).todense()
     np.fill_diagonal(graph, 0)
     graphs = [graph]
     for t in range(1, T):
         if mode == "reshuffle":
@@ -185,11 +194,11 @@
         variances.reshape(n_dim_obs, 1)
 
         X = np.random.poisson(1, size=(n_samples, n_dim_obs))
 
         for iter_ in range(max_iter):
             for i in range(n_dim_obs):
                 selector = np.array([j for j in range(n_dim_obs) if j != i])
-                par = np.exp(variances[i] + X[:, selector].dot(theta[selector, j]))
+                par = np.exp(variances[i] + X[:, selector].dot(theta[selector, i]))
                 X[:, i] = np.array([np.random.poisson(p) for p in par])
 
     return X
```

### Comparing `regain-0.3.3/regain/datasets/base.py` & `regain-0.3.8/regain/datasets/base.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/datasets/__init__.py` & `regain-0.3.8/regain/plotting/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,8 +23,7 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from .base import make_dataset
```

### Comparing `regain-0.3.3/regain/datasets/kernels.py` & `regain-0.3.8/regain/datasets/kernels.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/datasets/multi_class.py` & `regain-0.3.8/regain/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/wrapper/paspal/glopridu.py` & `regain-0.3.8/regain/wrapper/paspal/glopridu.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.3/regain/wrapper/__init__.py` & `regain-0.3.8/regain/wrapper/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,54 +30,65 @@
 try:
     import matlab
     import matlab.engine
 except ImportError:
     # raise ImportError(
     #     "`matlab` package not found. "
     #     "Please note you will need Matlab >= 2016b to use it.")
-    pass
+    matlab = None
+
+try:
+    from oct2py import octave
+except:
+    octave = None
 
-import numpy as np
 import os
 
+import numpy as np
+
 matlab_engine = None  # matlab.engine.start_matlab()
 
 
 def check_matlab_engine(verbose=False):
     global matlab_engine
     if matlab_engine is None or not matlab_engine._check_matlab():
         if verbose:
             print("Starting matlab engine ...")
         # close_engine = True
         try:
             matlab_engine = matlab.engine.start_matlab()
         except NameError as e:
             if "name 'matlab' is not defined" in str(e):
-                raise ValueError("`matlab` package not found. " "Please note you will need Matlab >= 2016b to use it.")
+                raise ValueError(
+                    "`matlab` package not found. "
+                    "Please note you will need Matlab >= 2016b to use it."
+                )
     # else:
     #     close_engine = False
 
 
 def lvglasso(emp_cov, alpha, tau, rho=1, verbose=False, use_octave=True):
     """Wrapper for LVGLASSO in R.
 
     If emp_cov.ndim > 2, then emp_cov.shape[0] == emp_cov.shape[1].
     In the temporal case, this means that the time is the last dimension.
     """
-    lvglasso_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "matlab", "lvglasso")
+    lvglasso_path = os.path.join(
+        os.path.abspath(os.path.dirname(__file__)), "matlab", "lvglasso"
+    )
     if use_octave:
-        from oct2py import octave
-
         octave.addpath(lvglasso_path, nout=0)
         result = octave.LVGLASSO(emp_cov, alpha, tau, rho)
     else:
         global matlab_engine
         check_matlab_engine(verbose=verbose)
         matlab_engine.addpath(lvglasso_path, nargout=0)
-        result = matlab_engine.LVGLASSO(matlab.double(emp_cov.tolist()), float(alpha), float(tau), float(rho))
+        result = matlab_engine.LVGLASSO(
+            matlab.double(emp_cov.tolist()), float(alpha), float(tau), float(rho)
+        )
     return result
 
 
 def total_variation_condat(y, lamda, verbose=False):
     global matlab_engine
     check_matlab_engine(verbose=verbose)
 
@@ -115,23 +126,27 @@
     coef_
         Coefficient of the Lasso algorithm for each feature.
 
     """
     global matlab_engine
     check_matlab_engine(verbose=verbose)
 
-    glopridu_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "GLO_PRIMAL_DUAL_TOOLBOX")
+    glopridu_path = os.path.join(
+        os.path.abspath(os.path.dirname(__file__)), "GLO_PRIMAL_DUAL_TOOLBOX"
+    )
     matlab_engine.addpath(glopridu_path, nargout=0)
 
     if verbose:
         print("Start GLOPRIDU algorithm ...")
     coef_ = matlab_engine.glopridu_algorithm(
         matlab.double(X.tolist()),
         matlab.double(y[:, None].tolist()),
-        [matlab.int32((np.array(x) + 1).tolist()) for x in groups],  # +1 because of the change of indices
+        [
+            matlab.int32((np.array(x) + 1).tolist()) for x in groups
+        ],  # +1 because of the change of indices
         float(lamda),
     )
 
     # if close_engine:
     #     matlab_engine.quit()
     coef_ = np.asarray(coef_).ravel()
     return coef_, None, np.nan
```

### Comparing `regain-0.3.3/regain/scores.py` & `regain-0.3.8/regain/scores.py`

 * *Files identical despite different names*

