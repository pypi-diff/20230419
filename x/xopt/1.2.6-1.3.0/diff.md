# Comparing `tmp/xopt-1.2.6.tar.gz` & `tmp/xopt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-9r0zhkhc/xopt-1.2.6.tar", last modified: Sun Mar 12 01:46:21 2023, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-0o0z5bgh/xopt-1.3.0.tar", last modified: Wed Apr 19 16:45:56 2023, max compression
```

## Comparing `xopt-1.2.6.tar` & `xopt-1.3.0.tar`

### file list

```diff
@@ -1,102 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-12 01:46:10.000000 xopt-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-12 01:46:10.000000 xopt-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-12 01:46:21.000000 xopt-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-03-12 01:46:10.000000 xopt-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-12 01:46:11.000000 xopt-1.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-12 01:46:21.000000 xopt-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-12 01:46:11.000000 xopt-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_bayesian_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_custom_botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/test_generator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-12 01:46:11.000000 xopt-1.2.6/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-03-12 01:46:11.000000 xopt-1.2.6/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/constraint_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/bayesian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-03-12 01:46:11.000000 xopt-1.2.6/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-12 01:46:21.000000 xopt-1.2.6/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 16:45:47.000000 xopt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:47.000000 xopt-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 16:45:56.000000 xopt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-19 16:45:47.000000 xopt-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:47.000000 xopt-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 16:45:56.000000 xopt-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 16:45:47.000000 xopt-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_generator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-04-19 16:45:47.000000 xopt-1.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/transformed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/top_level.txt
```

### Comparing `xopt-1.2.6/LICENSE` & `xopt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/PKG-INFO` & `xopt-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.2.6
+Version: 1.3.0
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.2.6/README.md` & `xopt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/setup.py` & `xopt-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-1.3.0/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-1.3.0/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,39 @@
         # test evaluating the model
         test_pts = torch.tensor(
             pd.DataFrame(TEST_VOCS_BASE.random_inputs(5, False, False)).to_numpy()
         )
         with torch.no_grad():
             model(test_pts)
 
+        # test with maximize and minimize
+        test_vocs = deepcopy(TEST_VOCS_BASE)
+        test_vocs.objectives["y1"] = "MINIMIZE"
+        test_data = deepcopy(TEST_VOCS_DATA)
+        gen = BayesianGenerator(test_vocs)
+        model = gen.train_model(test_data)
+        assert torch.allclose(
+            model.models[0].outcome_transform(torch.tensor(test_data["y1"].to_numpy()))[
+                0
+            ],
+            model.train_targets[0],
+        )
+
+        test_vocs = deepcopy(TEST_VOCS_BASE)
+        test_vocs.objectives["y1"] = "MAXIMIZE"
+        test_data = deepcopy(TEST_VOCS_DATA)
+        gen = BayesianGenerator(test_vocs)
+        model = gen.train_model(test_data)
+        assert torch.allclose(
+            model.models[0].outcome_transform(torch.tensor(test_data["y1"].to_numpy()))[
+                0
+            ],
+            model.train_targets[0],
+        )
+
         # try with input data that contains Nans due to xopt raising an error
         # currently we drop all rows containing Nans
         test_data = deepcopy(TEST_VOCS_DATA)
         test_data["y1"].iloc[5] = np.NaN
         model = gen.train_model(test_data)
         assert len(model.models[0].train_inputs[0]) == len(test_data) - 1
 
@@ -96,52 +121,38 @@
                 outcome_transform(
                     torch.from_numpy(X.data["y1"].to_numpy()).unsqueeze(-1)
                 )[0]
             ),
         )
 
         # constraint transform - bilog
-        C = torch.from_numpy(X.data["c1"].to_numpy())
-        assert torch.allclose(
-            model.train_targets[1], torch.sign(-C) * torch.log(1 + torch.abs(-C))
-        )
-
-    @patch.multiple(BayesianGenerator, __abstractmethods__=set())
-    def test_get_training_data(self):
-        gen = BayesianGenerator(TEST_VOCS_BASE)
-        inputs, outputs = gen.get_training_data(TEST_VOCS_DATA)
-        inames = list(TEST_VOCS_BASE.variables.keys())
-        onames = list(TEST_VOCS_BASE.objectives.keys()) + list(
-            TEST_VOCS_BASE.constraints.keys()
-        )
-
-        true_inputs = torch.from_numpy(TEST_VOCS_DATA[inames].to_numpy())
-        true_outputs = torch.from_numpy(TEST_VOCS_DATA[onames].to_numpy())
-        assert torch.allclose(inputs, true_inputs)
-        assert torch.allclose(outputs, true_outputs)
+        # C = torch.from_numpy(X.data["c1"].to_numpy())
+        # assert torch.allclose(
+        #    model.train_targets[1], torch.sign(-C) * torch.log(1 + torch.abs(-C))
+        # )
 
     # TODO: test passing UCB options to bayesian exploration
 
     @patch.multiple(BayesianGenerator, __abstractmethods__=set())
     def test_get_bounds(self):
         gen = BayesianGenerator(TEST_VOCS_BASE)
-        bounds = gen._get_bounds()
+        bounds = gen._get_optimization_bounds()
         assert torch.allclose(bounds, torch.tensor(TEST_VOCS_BASE.bounds))
 
         # test with max_travel_distances specified but no data
         defaults = BayesianGenerator.default_options()
         defaults.optim.max_travel_distances = [0.1, 0.2]
         gen = BayesianGenerator(TEST_VOCS_BASE, defaults)
         with pytest.raises(ValueError):
-            gen._get_bounds()
+            gen._get_optimization_bounds()
 
         # test with max_travel_distances specified and data
         gen = BayesianGenerator(TEST_VOCS_BASE, defaults)
         gen.add_data(pd.DataFrame({"x1": [0.5], "x2": [5.0], "y1": [0.5], "c1": [0.5]}))
-        bounds = gen._get_bounds()
+        bounds = gen._get_optimization_bounds()
         assert torch.allclose(bounds, torch.tensor([[0.4, 3.0], [0.6, 7.0]]).to(bounds))
 
         # test with max_travel_distances specified and data
         high_d_vocs = deepcopy(TEST_VOCS_BASE)
         high_d_vocs.variables["x3"] = [0, 1]
 
         defaults = BayesianGenerator.default_options()
@@ -149,15 +160,15 @@
 
         gen = BayesianGenerator(high_d_vocs, defaults)
         gen.add_data(
             pd.DataFrame(
                 {"x1": [0.5], "x2": [5.0], "x3": [0.5], "y1": [0.5], "c1": [0.5]}
             )
         )
-        bounds = gen._get_bounds()
+        bounds = gen._get_optimization_bounds()
         assert torch.allclose(
             bounds, torch.tensor([[0.4, 3.0, 0.4], [0.6, 7.0, 0.6]]).to(bounds)
         )
 
         # test with bad max_distances
         defaults = BayesianGenerator.default_options()
         defaults.optim.max_travel_distances = [0.1, 0.2]
@@ -165,8 +176,8 @@
         gen = BayesianGenerator(high_d_vocs, defaults)
         gen.add_data(
             pd.DataFrame(
                 {"x1": [0.5], "x2": [5.0], "x3": [0.5], "y1": [0.5], "c1": [0.5]}
             )
         )
         with pytest.raises(ValueError):
-            gen._get_bounds()
+            gen._get_optimization_bounds()
```

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_expected_improvement.py` & `xopt-1.3.0/tests/generators/bayesian/test_expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_high_level.py` & `xopt-1.3.0/tests/generators/bayesian/test_high_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         x = torch.linspace(*bounds.T[0], n)
         y = torch.linspace(*bounds.T[1], n)
         xx, yy = torch.meshgrid(x, y)
         pts = torch.hstack([ele.reshape(-1, 1) for ele in (xx, yy)]).double()
 
         with torch.no_grad():
             acq_val = acq(pts.unsqueeze(1))
-            assert torch.allclose(acq_val.max(), torch.tensor(9.36).double(), atol=0.1)
+            assert torch.allclose(
+                acq_val.max(), torch.tensor(9.9955).double(), atol=0.1
+            )
 
     def test_constrained_mobo(self):
         YAML = """
         xopt: {}
         generator:
             name: mobo
             n_initial: 5
```

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_mggpo.py` & `xopt-1.3.0/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_mobo.py` & `xopt-1.3.0/tests/generators/bayesian/test_mobo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from copy import deepcopy
 
 import numpy as np
+import pandas as pd
 import pytest
+
 from xopt.base import Xopt
 from xopt.evaluator import Evaluator
 from xopt.generators.bayesian.mobo import MOBOGenerator
 from xopt.resources.test_functions.tnk import evaluate_TNK, tnk_vocs
 from xopt.resources.testing import TEST_VOCS_BASE
 
 
@@ -31,15 +33,14 @@
 
         for ele in [bad_options, bad_options2]:
             with pytest.raises(ValueError):
                 MOBOGenerator(tnk_vocs, ele)
 
         base_options = deepcopy(MOBOGenerator.default_options())
         base_options.acq.reference_point = {"y1": 1.5, "y2": 1.5}
-        base_options.optim.raw_samples = 5
         base_options.acq.monte_carlo_samples = 20
 
         proximal_biasing = deepcopy(base_options)
         proximal_biasing.acq.reference_point = {"y1": 1.5, "y2": 1.5}
         proximal_biasing.optim.num_restarts = 1  # required
         proximal_biasing.acq.proximal_lengthscales = [1.0, 1.0]
 
@@ -49,7 +50,35 @@
         proximal_biasing2.acq.proximal_lengthscales = np.array([1.0, 1.0])
 
         for ele in [base_options, proximal_biasing, proximal_biasing2]:
             generator = MOBOGenerator(tnk_vocs, ele)
             X = Xopt(generator=generator, evaluator=evaluator, vocs=tnk_vocs)
             X.step()
             X.step()
+
+    def test_hypervolume_calculation(self):
+        vocs = deepcopy(TEST_VOCS_BASE)
+        vocs.objectives.update({"y2": "MINIMIZE"})
+        vocs.constraints = {}
+
+        data = pd.DataFrame(
+            {
+                "x1": np.random.rand(2),
+                "x2": np.random.rand(2),
+                "y1": np.array((1.0, 0.0)),
+                "y2": np.array((0.0, 2.0)),
+            }
+        )
+
+        options = MOBOGenerator.default_options()
+        options.acq.reference_point = {"y1": 10.0, "y2": 1.0}
+
+        generator = MOBOGenerator(vocs, options)
+        generator.add_data(data)
+
+        assert generator.calculate_hypervolume() == 9.0
+
+        vocs.objectives["y1"] = "MAXIMIZE"
+        generator = MOBOGenerator(vocs, options)
+        generator.add_data(data)
+
+        assert generator.calculate_hypervolume() == 0.0
```

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-1.3.0/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-1.3.0/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         gen.data = TEST_VOCS_DATA
 
         candidate = gen.generate(1)
         assert len(candidate) == 1
 
         # candidate = gen.generate(2)
         # assert len(candidate) == 2
+
     def test_cuda(self):
         gen = UpperConfidenceBoundGenerator(
             TEST_VOCS_BASE,
         )
 
         if torch.cuda.is_available():
             gen.options.use_cuda = True
```

### Comparing `xopt-1.2.6/tests/generators/bayesian/test_utils.py` & `xopt-1.3.0/tests/generators/bayesian/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from copy import deepcopy
 
 import torch
 
-from xopt.generators.bayesian.objectives import (
-    create_mobo_objective,
-)
+from xopt.generators.bayesian.objectives import create_mobo_objective
 from xopt.resources.testing import TEST_VOCS_BASE
 
 
 class TestUtils:
     def test_mobo_objective(self):
         test_vocs_copy = deepcopy(TEST_VOCS_BASE)
         test_vocs_copy.objectives["y2"] = "MAXIMIZE"
@@ -18,9 +16,9 @@
         test_samples = torch.randn(3, 4, 5, 3).double()
         output = obj(test_samples)
         assert output.shape == torch.Size([3, 4, 5, 2])
 
         # test to make sure values are correct - minimize axis should be negated
         test_samples = torch.rand(5, 4, 3)
         output = obj(test_samples)
-        assert torch.allclose(output[..., 1], -test_samples[..., 1])
+        assert torch.allclose(output[..., 1], test_samples[..., 1])
         assert torch.allclose(output[..., 0], -test_samples[..., 0])
```

### Comparing `xopt-1.2.6/tests/generators/test_extremum_seeking.py` & `xopt-1.3.0/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/test_evaluator.py` & `xopt-1.3.0/tests/test_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 import numpy as np
 import pandas as pd
 
 from xopt import Evaluator
+from xopt.vocs import VOCS
 
 
 class TestEvaluator:
     @staticmethod
     def f(x, a=True):
         if a:
             return {"f": x["x1"] ** 2 + x["x2"] ** 2}
@@ -99,7 +100,18 @@
             "max_workers": 1,
         }
 
         for Executor in [ThreadPoolExecutor, ProcessPoolExecutor]:
             test_dict["executor"] = Executor()
             ev = Evaluator(**test_dict)
             ev.json()
+
+    def test_multithreading(self):
+        MAX_WORKERS = 10
+
+        vocs = VOCS(variables={"x": [0, 1], "y": [0, 1]}, objectives={"f1": "MINIMIZE"})
+        in10 = vocs.random_inputs(10)
+
+        # Create Executor insance
+        executor = ProcessPoolExecutor(max_workers=MAX_WORKERS)
+        ev = Evaluator(function=self.f, executor=executor, max_workers=MAX_WORKERS)
+        ev.evaluate_data(in10)
```

### Comparing `xopt-1.2.6/tests/test_io.py` & `xopt-1.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/test_pydantic.py` & `xopt-1.3.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/test_vocs.py` & `xopt-1.3.0/tests/test_vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/tests/test_xopt.py` & `xopt-1.3.0/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/versioneer.py` & `xopt-1.3.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/base.py` & `xopt-1.3.0/xopt/base.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/evaluator.py` & `xopt-1.3.0/xopt/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,17 +214,21 @@
     if "xopt_non_dict_result" in outputs:
         result = outputs["xopt_non_dict_result"]
         raise XoptError(
             "Xopt evaluator returned a non-dict result, type is: "
             f"{type(result)}, result is: {result}"
         )
     else:
-        raise XoptError(
-            "Xopt evaluator caught an exception: " f"{outputs['xopt_error_str']}"
-        )
+        error_string = "Xopt evaluator caught exception(s):\n\n"
+        for i in range(len(outputs["xopt_error_str"])):
+            error_string += f"Evaluation index {i}:\n"
+            error_string += outputs["xopt_error_str"].iloc[i]
+            error_string += "\n"
+
+        raise XoptError(error_string)
 
 
 class DummyExecutor(Executor):
     """
     Dummy executor.
 
     From: https://stackoverflow.com/questions/10434593/dummyexecutor-for-pythons-futures
```

### Comparing `xopt-1.2.6/xopt/generator.py` & `xopt-1.3.0/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/__init__.py` & `xopt-1.3.0/xopt/generators/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import warnings
 
 from xopt.errors import XoptError
+from xopt.generators.bayesian.mggpo import MGGPOGenerator
 from xopt.generators.es.extremumseeking import ExtremumSeekingGenerator
 from xopt.generators.random import RandomGenerator
+from xopt.generators.rcds.rcds import RCDSGenerator
 
 # add generators here to be registered
 registered_generators = [
     RandomGenerator,
     ExtremumSeekingGenerator,
+    MGGPOGenerator,
+    RCDSGenerator,
 ]
 
 # generators needing deap
 try:
     from xopt.generators.ga import CNSGAGenerator
 
     registered_generators += [CNSGAGenerator]
@@ -24,25 +28,27 @@
     from xopt.generators.bayesian.bayesian_exploration import (
         BayesianExplorationGenerator,
     )
     from xopt.generators.bayesian.expected_improvement import (
         ExpectedImprovementGenerator,
     )
     from xopt.generators.bayesian.mobo import MOBOGenerator
+    from xopt.generators.bayesian.multi_fidelity import MultiFidelityGenerator
     from xopt.generators.bayesian.upper_confidence_bound import (
         TDUpperConfidenceBoundGenerator,
         UpperConfidenceBoundGenerator,
     )
 
     registered_generators += [
         UpperConfidenceBoundGenerator,
         MOBOGenerator,
         BayesianExplorationGenerator,
         TDUpperConfidenceBoundGenerator,
         ExpectedImprovementGenerator,
+        MultiFidelityGenerator,
     ]
 
 except ModuleNotFoundError:
     warnings.warn("WARNING: `botorch` not found, Bayesian generators are not available")
 
 # generators requiring deap AND botorch
 try:
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-1.3.0/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/bayesian/bayesian_generator.py` & `xopt-1.3.0/xopt/generators/bayesian/bayesian_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,136 @@
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from typing import Dict, List
 
 import pandas as pd
 import torch
+from botorch.acquisition import qUpperConfidenceBound
 from botorch.models import ModelListGP
 from botorch.optim import optimize_acqf
-from botorch.optim.initializers import sample_truncated_normal_perturbations
 from botorch.sampling import SobolQMCNormalSampler
 from botorch.sampling.get_sampler import get_sampler
 from gpytorch import Module
 
 from xopt.generator import Generator
+from xopt.generators.bayesian.custom_botorch.constrained_acqusition import (
+    ConstrainedMCAcquisitionFunction,
+)
 from xopt.generators.bayesian.custom_botorch.proximal import ProximalAcquisitionFunction
-from xopt.generators.bayesian.objectives import create_mc_objective, \
-    create_constraint_callables
+from xopt.generators.bayesian.models.utils import get_model_constructor
+from xopt.generators.bayesian.objectives import (
+    create_constraint_callables,
+    create_mc_objective,
+)
 from xopt.generators.bayesian.options import BayesianOptions
+from xopt.generators.bayesian.turbo import get_trust_region, TurboState, update_state
+from xopt.generators.bayesian.utils import rectilinear_domain_union
 from xopt.vocs import VOCS
 
 logger = logging.getLogger()
 
 
 class BayesianGenerator(Generator, ABC):
-    def __init__(self, vocs: VOCS, options: BayesianOptions = None):
+    def __init__(
+        self,
+        vocs: VOCS,
+        options: BayesianOptions = None,
+        supports_batch_generation=False,
+    ):
         options = options or BayesianOptions()
         if not isinstance(options, BayesianOptions):
             raise ValueError("options must be of type BayesianOptions")
 
         super().__init__(vocs, options)
 
         self._model = None
         self._acquisition = None
+        self._trust_region = None
+        self.supports_batch_generation = supports_batch_generation
         self.sampler = SobolQMCNormalSampler(self.options.acq.monte_carlo_samples)
+        self.model_constructor = get_model_constructor(options.model)(
+            self.vocs, options.model
+        )
+
+        # set up turbo if requested
+        if self.options.optim.use_turbo:
+            self.turbo_state = TurboState(self.vocs.n_variables, 1)
+            self.first_call = True
 
     @staticmethod
     def default_options() -> BayesianOptions:
         return BayesianOptions()
 
     def add_data(self, new_data: pd.DataFrame):
         self.data = pd.concat([self.data, new_data], axis=0)
 
     def generate(self, n_candidates: int) -> List[Dict]:
-        if n_candidates > 1:
+        if n_candidates > 1 and not self.supports_batch_generation:
             raise NotImplementedError(
-                "Bayesian algorithms don't currently support parallel candidate "
+                "This Bayesian algorithm does not currently support parallel candidate "
                 "generation"
             )
 
         # if no data exists use random generator to generate candidates
         if self.data.empty:
             return self.vocs.random_inputs(self.options.n_initial)
 
         else:
-            bounds = self._get_bounds()
-
             # update internal model with internal data
-            self.train_model(self.data)
+            model = self.train_model(self.data)
 
-            # get initial points for optimization (if specified)
-            batch_initial_points, raw_samples = self._get_initial_batch_points(bounds)
+            # calculate optimization bounds
+            bounds = self._get_optimization_bounds()
 
-            acq_funct = self.get_acquisition(self._model)
+            # get acquisition function
+            acq_funct = self.get_acquisition(model)
 
-            # get candidates in real domain
-            candidates, out = optimize_acqf(
-                acq_function=acq_funct,
-                bounds=bounds,
-                q=n_candidates,
-                raw_samples=raw_samples,
-                batch_initial_conditions=batch_initial_points,
-                num_restarts=self.options.optim.num_restarts,
-            )
-            logger.debug("Best candidate from optimize", candidates, out)
-            return self.vocs.convert_numpy_to_inputs(candidates.detach().cpu().numpy())
+            # get candidates
+            candidates = self.optimize_acqf(acq_funct, bounds, n_candidates)
+
+            # post process candidates
+            result = self._process_candidates(candidates)
+            return result
 
     def train_model(self, data: pd.DataFrame = None, update_internal=True) -> Module:
         """
         Returns a ModelListGP containing independent models for the objectives and
         constraints
 
         """
         if data is None:
             data = self.data
+        if data.empty:
+            raise ValueError("no data available to build model")
 
-        # drop nans
-        valid_data = data[
-            pd.unique(self.vocs.variable_names + self.vocs.output_names)
-        ].dropna()
-
-        kwargs = self.options.model.kwargs.dict()
-
-        _model = self.options.model.function(
-            valid_data, self.vocs, self._tkwargs, **kwargs
-        )
+        _model = self.model_constructor.build_model(data, self._tkwargs)
 
         # validate returned model
         self._validate_model(_model)
 
         if update_internal:
             self._model = _model
         return _model
 
+    def get_input_data(self, data):
+        return torch.tensor(
+            self.vocs.variable_data(data, "").to_numpy(), **self._tkwargs
+        )
+
     def get_acquisition(self, model):
         """
         Returns a function that can be used to evaluate the acquisition function
         """
-        # re-create sampler/objective from options
 
         # need a sampler for botorch > 0.8
+        # get input data
+        input_data = self.get_input_data(self.data)
         self.sampler = get_sampler(
-            model.posterior(self.get_input_data(self.data)),
+            model.posterior(input_data),
             sample_shape=torch.Size([self.options.acq.monte_carlo_samples]),
         )
 
         # get base acquisition function
         acq = self._get_acquisition(model)
 
         # add proximal biasing if requested
@@ -124,57 +140,69 @@
                 torch.tensor(self.options.acq.proximal_lengthscales, **self._tkwargs),
                 transformed_weighting=self.options.acq.use_transformed_proximal_weights,
                 beta=10.0,
             )
 
         return acq
 
-    def get_training_data(self, data: pd.DataFrame):
-        return self.get_input_data(data), self.get_outcome_data(data)
+    def optimize_acqf(self, acq_funct, bounds, n_candidates):
+        # get candidates in real domain
+        candidates, out = optimize_acqf(
+            acq_function=acq_funct,
+            bounds=bounds,
+            q=n_candidates,
+            raw_samples=self.options.optim.raw_samples,
+            num_restarts=self.options.optim.num_restarts,
+        )
+        return candidates
 
-    def get_input_data(self, data: pd.DataFrame):
-        return torch.tensor(data[self.vocs.variable_names].to_numpy(), **self._tkwargs)
+    def get_optimum(self):
+        """select the best point(s) (for multi-objective generators, given by the
+        model using the Posterior mean"""
+        c_posterior_mean = ConstrainedMCAcquisitionFunction(
+            self.model,
+            qUpperConfidenceBound(
+                model=self.model, beta=0.0, objective=self._get_objective()
+            ),
+            self._get_constraint_callables(),
+        )
 
-    def get_outcome_data(self, data: pd.DataFrame):
-        return torch.tensor(data[self.vocs.output_names].to_numpy(), **self._tkwargs)
+        result, out = optimize_acqf(
+            acq_function=c_posterior_mean,
+            bounds=self._get_bounds(),
+            q=1,
+            raw_samples=self.options.optim.raw_samples * 5,
+            num_restarts=self.options.optim.num_restarts * 5,
+        )
 
-    def _get_initial_batch_points(self, bounds):
-        if self.options.optim.use_nearby_initial_points:
-            # generate starting points for optimization (note in real domain)
-            inputs = self.get_input_data(self.data)
-            batch_initial_points = sample_truncated_normal_perturbations(
-                inputs[-1].unsqueeze(0),
-                n_discrete_points=self.options.optim.raw_samples,
-                sigma=0.5,
-                bounds=bounds,
-            ).unsqueeze(-2)
-            raw_samples = None
-        else:
-            batch_initial_points = None
-            raw_samples = self.options.optim.raw_samples
+        return self._process_candidates(result)
 
-        return batch_initial_points, raw_samples
+    def _process_candidates(self, candidates):
+        logger.debug("Best candidate from optimize", candidates)
+        return self.vocs.convert_numpy_to_inputs(candidates.detach().cpu().numpy())
 
     @abstractmethod
     def _get_acquisition(self, model):
         pass
 
     def _get_objective(self):
-        """ return default objective (scalar objective) determined by vocs """
+        """return default objective (scalar objective) determined by vocs"""
         return create_mc_objective(self.vocs, self._tkwargs)
 
     def _get_constraint_callables(self):
-        """ return default objective (scalar objective) determined by vocs """
+        """return default objective (scalar objective) determined by vocs"""
         constraint_callables = create_constraint_callables(self.vocs)
         if len(constraint_callables) == 0:
             constraint_callables = None
         return constraint_callables
 
     @property
     def model(self):
+        if self._model is None:
+            self.train_model(self.data)
         return self._model
 
     @property
     def _tkwargs(self):
         # set device and data type for generator
         device = "cpu"
         if self.options.use_cuda:
@@ -185,50 +213,99 @@
                     "Cuda requested in generator options but not found on "
                     "machine! Using CPU instead"
                 )
 
         return {"dtype": torch.double, "device": device}
 
     def _get_bounds(self):
-        bounds = torch.tensor(self.vocs.bounds, **self._tkwargs)
+        """convert bounds from vocs to torch tensors"""
+        return torch.tensor(self.vocs.bounds, **self._tkwargs)
+
+    def _get_optimization_bounds(self):
+        """
+        gets optimization bounds based on the union of several domains
+        - if use_turbo is True include trust region
+        - if max_travel_distances is not None limit max travel distance
+
+        """
+        bounds = self._get_bounds()
+
+        # if using turbo, update turbo state and set bounds according to turbo state
+        if self.options.optim.use_turbo:
+            bounds = self.get_trust_region(bounds)
+
         # if specified modify bounds to limit maximum travel distances
         if self.options.optim.max_travel_distances is not None:
-            if len(self.options.optim.max_travel_distances) != bounds.shape[-1]:
-                raise ValueError(
-                    f"length of max_travel_distances must match the number of "
-                    f"variables {bounds.shape[-1]}"
-                )
+            bounds = self.get_max_travel_distances_region(bounds)
 
-            # get last point
-            if self.data.empty:
-                raise ValueError(
-                    "No data exists to specify max_travel_distances "
-                    "from, add data first to use during BO"
+        return bounds
+
+    def get_trust_region(self, bounds):
+        """get trust region based on turbo_state and last observation"""
+        if self.options.optim.use_turbo:
+            objective_data = self.vocs.objective_data(self.data, "")
+
+            # if this is the first time we are updating the state use the best f
+            # instead of the last f
+            if self.first_call:
+                y_last = torch.tensor(objective_data.min().to_numpy(), **self._tkwargs)
+                self.first_call = False
+            else:
+                y_last = torch.tensor(
+                    objective_data.iloc[-1].to_numpy(), **self._tkwargs
                 )
-            last_point = torch.tensor(
-                self.data[self.vocs.variable_names].iloc[-1].to_numpy(), **self._tkwargs
-            )
+            self.turbo_state = update_state(self.turbo_state, y_last)
 
-            # bound lengths for normalization
-            lengths = bounds[1, :] - bounds[0, :]
+            # calculate trust region and apply to base bounds
+            trust_region = get_trust_region(
+                self.vocs,
+                self.model,
+                bounds,
+                self.data,
+                self.turbo_state,
+                self._tkwargs,
+            )
 
-            # get maximum travel distances
-            max_travel_distances = (
-                torch.tensor(self.options.optim.max_travel_distances, **self._tkwargs)
-                * lengths
+            return rectilinear_domain_union(bounds, trust_region)
+        else:
+            raise RuntimeError(
+                "cannot get trust region when `use_turbo` option is False"
             )
-            bounds[0, :] = torch.max(
-                bounds[0, :],
-                last_point - max_travel_distances,
+
+    def get_max_travel_distances_region(self, bounds):
+        """get region based on max travel distances and last observation"""
+        if len(self.options.optim.max_travel_distances) != bounds.shape[-1]:
+            raise ValueError(
+                f"length of max_travel_distances must match the number of "
+                f"variables {bounds.shape[-1]}"
             )
-            bounds[1, :] = torch.min(
-                bounds[1, :],
-                last_point + max_travel_distances,
+
+        # get last point
+        if self.data.empty:
+            raise ValueError(
+                "No data exists to specify max_travel_distances "
+                "from, add data first to use during BO"
             )
-        return bounds
+        last_point = torch.tensor(
+            self.data[self.vocs.variable_names].iloc[-1].to_numpy(), **self._tkwargs
+        )
+
+        # bound lengths for normalization
+        lengths = bounds[1, :] - bounds[0, :]
+
+        # get maximum travel distances
+        max_travel_distances = (
+            torch.tensor(self.options.optim.max_travel_distances, **self._tkwargs)
+            * lengths
+        )
+        max_travel_bounds = torch.stack(
+            (last_point - max_travel_distances, last_point + max_travel_distances)
+        )
+
+        return rectilinear_domain_union(bounds, max_travel_bounds)
 
     def _check_options(self, options: BayesianOptions):
         if options.acq.proximal_lengthscales is not None:
             n_lengthscales = len(options.acq.proximal_lengthscales)
 
             if n_lengthscales != self.vocs.n_variables:
                 raise ValueError(
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py` & `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         self,
         model: Model,
         base_acqusition: MCAcquisitionFunction,
         constraints: List[Callable],
         posterior_transform: Optional[PosteriorTransform] = None,
         X_pending: Optional[Tensor] = None,
     ) -> None:
-
         # make it consistent with botorch constrained EHVI
         if constraints is None:
             constraints = []
 
         super().__init__(
             model=model,
             sampler=base_acqusition.sampler,
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/bayesian/expected_improvement.py` & `xopt-1.3.0/xopt/generators/bayesian/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/bayesian/mggpo.py` & `xopt-1.3.0/xopt/generators/bayesian/mggpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from typing import Dict, List
 
 import pandas as pd
 import torch
 from botorch.acquisition.multi_objective import qNoisyExpectedHypervolumeImprovement
 from pydantic import Field
 
-from xopt.generators.bayesian.objectives import (
-    create_mobo_objective,
-)
+from xopt.generators.bayesian.objectives import create_mobo_objective
 from xopt.generators.ga.cnsga import CNSGAGenerator, CNSGAOptions
 from xopt.vocs import VOCS
+from ...errors import XoptError
 from .bayesian_generator import BayesianGenerator
 from .options import AcqOptions, BayesianOptions
-from ...errors import XoptError
 
 
 class MGGPOAcqOptions(AcqOptions):
     reference_point: Dict[str, float] = Field(
         None, description="dict of reference points for multi-objective optimization"
     )
     population_size: int = Field(64, description="population size for ga")
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/mobo.py` & `xopt-1.3.0/xopt/generators/bayesian/mobo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Dict
 
 import torch
 from botorch.acquisition.multi_objective import qNoisyExpectedHypervolumeImprovement
+from botorch.utils.multi_objective.box_decompositions import DominatedPartitioning
 from pydantic import Field
 
-from xopt.generators.bayesian.objectives import (
-    create_mobo_objective,
-)
+from xopt.generators.bayesian.objectives import create_mobo_objective
 from xopt.vocs import VOCS
-from .bayesian_generator import BayesianGenerator
-from .options import AcqOptions, BayesianOptions
 from ...errors import XoptError
 from ...utils import format_option_descriptions
+from .bayesian_generator import BayesianGenerator
+from .options import AcqOptions, BayesianOptions
+from .utils import set_botorch_weights
 
 
 class MOBOAcqOptions(AcqOptions):
     reference_point: Dict[str, float] = Field(
         None, description="dict of reference points for multi-objective optimization"
     )
 
@@ -30,18 +30,18 @@
         """Implements Multi-Objective Bayesian Optimization using the Expected
             Hypervolume Improvement acquisition function"""
         + f"{format_option_descriptions(MOBOOptions())}"
     )
 
     def __init__(self, vocs: VOCS, options: MOBOOptions = None):
         options = options or MOBOOptions()
-        if not type(options) is MOBOOptions:
+        if not isinstance(options, MOBOOptions):
             raise ValueError("options must be a MOBOOptions object")
 
-        super().__init__(vocs, options)
+        super().__init__(vocs, options, supports_batch_generation=True)
 
     @staticmethod
     def default_options() -> MOBOOptions:
         return MOBOOptions()
 
     @property
     def reference_point(self):
@@ -68,20 +68,42 @@
     def _get_objective(self):
         return create_mobo_objective(self.vocs, self._tkwargs)
 
     def _get_acquisition(self, model):
         inputs = self.get_input_data(self.data)
 
         # fix problem with qNEHVI interpretation with constraints
-
         acq = qNoisyExpectedHypervolumeImprovement(
             model,
             X_baseline=inputs,
             constraints=self._get_constraint_callables(),
             ref_point=self.reference_point,
             sampler=self.sampler,
             objective=self._get_objective(),
             cache_root=False,
             prune_baseline=True,
         )
 
         return acq
+
+    def calculate_hypervolume(self):
+        """compute hypervolume given data"""
+        objective_data = torch.tensor(
+            self.vocs.objective_data(self.data, return_raw=True).to_numpy()
+        )
+
+        # hypervolume must only take into account feasible data points
+        if self.vocs.n_constraints > 0:
+            objective_data = objective_data[
+                self.vocs.feasibility_data(self.data)["feasible"].to_list()
+            ]
+
+        n_objectives = self.vocs.n_objectives
+        weights = torch.zeros(n_objectives)
+        weights = set_botorch_weights(weights, self.vocs)
+        objective_data = objective_data * weights
+
+        # compute hypervolume
+        bd = DominatedPartitioning(ref_point=self.reference_point, Y=objective_data)
+        volume = bd.compute_hypervolume().item()
+
+        return volume
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/models/standard.py` & `xopt-1.3.0/xopt/generators/bayesian/models/standard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,127 @@
 import pandas as pd
 import torch
-from botorch import fit_gpytorch_mll
-from botorch.models import ModelListGP, SingleTaskGP
-from botorch.models.transforms import Bilog, Normalize, Standardize
-from gpytorch import ExactMarginalLogLikelihood
-from gpytorch.kernels import MaternKernel, ScaleKernel
+from botorch.models import ModelListGP
+from botorch.models.transforms import Normalize, Standardize
+from gpytorch import Module
 from gpytorch.likelihoods import GaussianLikelihood
 from gpytorch.priors import GammaPrior
 
+from xopt.generators.bayesian.base_model import ModelConstructor
+from xopt.generators.bayesian.models.prior_mean import CustomMean
 from xopt.vocs import VOCS
 
 
-def create_standard_model(
-    data: pd.DataFrame,
-    vocs: VOCS,
-    tkwargs: dict,
-    use_conservative_prior_lengthscale: bool = False,
-    use_conservative_prior_mean: bool = False,
-    use_low_noise_prior: bool = False,
-):
-    input_data, objective_data, constraint_data = vocs.extract_data(data)
-
-    input_transform = Normalize(
-        vocs.n_variables, bounds=torch.tensor(vocs.bounds, **tkwargs)
-    )
-
-    objective_models = create_objective_models(
-        input_data, objective_data, input_transform, tkwargs, use_low_noise_prior
-    )
-    constraint_models = create_constraint_models(
-        input_data,
-        constraint_data,
-        input_transform,
-        tkwargs,
-        use_low_noise_prior,
-        use_conservative_prior_lengthscale,
-        use_conservative_prior_mean,
-    )
-
-    return ModelListGP(*objective_models, *constraint_models)
-
-
-def create_objective_models(
-    input_data, objective_data, input_transform, tkwargs, use_low_noise_prior=False
-):
-    # validate data
-    if len(input_data) == 0:
-        raise ValueError("input_data is empty/all Nans, cannot create model")
-
-    train_X = torch.tensor(input_data.to_numpy(), **tkwargs)
-
-    models = []
-
-    # create models for objectives
-    for name in objective_data.keys():
-        train_Y = torch.tensor(objective_data[name].to_numpy(), **tkwargs).unsqueeze(-1)
-
-        likelihood = None
-        if use_low_noise_prior:
-            likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.0, 10.0))
-
-        models.append(
-            SingleTaskGP(
-                train_X,
-                train_Y,
-                input_transform=input_transform,
-                outcome_transform=Standardize(1),
-                likelihood=likelihood,
-            )
-        )
-        mll = ExactMarginalLogLikelihood(models[-1].likelihood, models[-1])
-        fit_gpytorch_mll(mll)
-
-    return models
-
-
-def create_constraint_models(
-    input_data,
-    constraint_data,
-    input_transform,
-    tkwargs,
-    use_low_noise_prior=False,
-    use_conservative_prior_lengthscale: bool = False,
-    use_conservative_prior_mean: bool = False,
-):
-    # validate data
-    if len(input_data) == 0:
-        raise ValueError("input_data is empty/all Nans, cannot create model")
-
-    train_X = torch.tensor(input_data.to_numpy(), **tkwargs)
-    models = []
-
-    # do constraint models
-    for name in constraint_data.keys():
-        train_Y = torch.tensor(constraint_data[name].to_numpy(), **tkwargs).unsqueeze(
-            -1
+class StandardModelConstructor(ModelConstructor):
+    def __init__(self, vocs: VOCS, options):
+        super().__init__(vocs, options)
+        # get input transform
+        self.input_transform = Normalize(
+            self.vocs.n_variables, bounds=torch.tensor(self.vocs.bounds)
         )
 
-        outcome_transform = Bilog()
-
-        # use conservative priors if requested
-        covar_module = None
-        if use_conservative_prior_lengthscale:
-            covar_module = ScaleKernel(
-                MaternKernel(
-                    nu=1.5,
-                    ard_num_dims=train_X.shape[-1],
-                    lengthscale_prior=GammaPrior(10.0, 100.0),
-                ),
-                outputscale_prior=GammaPrior(5.0, 1.0),
-            )
-
-        likelihood = None
-        if use_low_noise_prior:
-            likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.0, 10.0))
-
-        models.append(
-            SingleTaskGP(
-                train_X,
-                train_Y,
-                input_transform=input_transform,
-                outcome_transform=outcome_transform,
-                covar_module=covar_module,
-                likelihood=likelihood,
+        # get likelihood
+        self.likelihood = None
+        if self.options.use_low_noise_prior:
+            self.likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.0, 10.0))
+
+        self.input_data = None
+        self.objective_data = None
+        self.constraint_data = None
+        self.train_X = None
+        self.tkwargs = {"dtype": torch.double, "device": "cpu"}
+
+    def collect_data(self, data: pd.DataFrame):
+        # drop nans
+        valid_data = data[
+            pd.unique(self.vocs.variable_names + self.vocs.output_names)
+        ].dropna()
+
+        # get data
+        (
+            self.input_data,
+            self.objective_data,
+            self.constraint_data,
+        ) = self.vocs.extract_data(valid_data, return_raw=True)
+
+        self.train_X = torch.tensor(self.input_data.to_numpy(), **self.tkwargs)
+        self.input_transform.to(**self.tkwargs)
+        if self.likelihood is not None:
+            self.likelihood.to(**self.tkwargs)
+
+    def build_model(self, data: pd.DataFrame, tkwargs: dict = None) -> ModelListGP:
+        """construct independent model for each objective and constraint"""
+        # overwrite tkwargs if specified
+        self.tkwargs = tkwargs or self.tkwargs
+
+        # collect data from dataframe
+        self.collect_data(data)
+
+        # build model
+        return self.build_standard_model()
+
+    def build_standard_model(self, **model_kwargs):
+        models = []
+        for name in self.vocs.output_names:
+            outcome_transform = Standardize(1)
+            covar_module = self._get_module(self.options.covar_modules, name)
+            mean_module = self._get_module(self.options.mean_modules, name)
+
+            # objective specifics
+            if name in self.vocs.objective_names:
+                # if we are doing minimization add a negative sign to the prior model
+                # if self.vocs.objectives[name] == "MINIMIZE" and mean_module is not
+                # None:
+                #    mean_module = _NegativeModule(mean_module)
+
+                train_Y = torch.tensor(
+                    self.objective_data[name].to_numpy(), **self.tkwargs
+                ).unsqueeze(-1)
+
+            # constraint specific
+            elif name in self.vocs.constraint_names:
+                train_Y = torch.tensor(
+                    self.constraint_data[name].to_numpy(), **self.tkwargs
+                ).unsqueeze(-1)
+
+            else:
+                raise RuntimeError(
+                    "if you are recieving this message there is "
+                    "something wrong with vocs"
+                )
+
+            if mean_module is not None:
+                mean_module = CustomMean(
+                    mean_module, self.input_transform, outcome_transform
+                )
+
+            models.append(
+                self.build_single_task_gp(
+                    self.train_X,
+                    train_Y,
+                    input_transform=self.input_transform,
+                    outcome_transform=outcome_transform,
+                    covar_module=covar_module,
+                    mean_module=mean_module,
+                    likelihood=self.likelihood,
+                )
             )
-        )
 
-        if use_conservative_prior_mean:
-            models[-1].mean_module.constant.data = torch.tensor(1.0, **tkwargs)
-            models[-1].mean_module.constant.requires_grad = False
+        return ModelListGP(*models)
 
-        mll = ExactMarginalLogLikelihood(models[-1].likelihood, models[-1])
-        fit_gpytorch_mll(mll)
+    @staticmethod
+    def _get_module(base, name):
+        if isinstance(base, Module):
+            return base
+        elif isinstance(base, dict):
+            return base.get(name)
+        else:
+            return None
+
+
+class _NegativeModule(Module):
+    def __init__(self, base):
+        super().__init__()
+        self.base = base
 
-    # create model list
-    return models
+    def forward(self, X):
+        return -self.base(X)
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/objectives.py` & `xopt-1.3.0/xopt/generators/bayesian/objectives.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from functools import partial
 
 import torch
 from botorch.acquisition import GenericMCObjective
 from botorch.acquisition.multi_objective import WeightedMCMultiOutputObjective
 
+from xopt.generators.bayesian.custom_botorch.constrained_acqusition import (
+    FeasibilityObjective,
+)
+from xopt.generators.bayesian.utils import set_botorch_weights
+
+
+def feasibility(X, model, sampler, vocs, posterior_transform=None):
+    constraints = create_constraint_callables(vocs)
+    posterior = model.posterior(X=X, posterior_transform=posterior_transform)
+    samples = sampler(posterior)
+    objective = FeasibilityObjective(constraints)
+    return torch.mean(objective(samples, X), dim=0)
+
 
 def constraint_function(Z, vocs, index, quantile_cutoff=0.0):
     """
     create constraint function
     - if a distribution of samples has a quantile level, given by `quantile_cutoff`,
     that is infeasiable penalize the entire set of samples to make all infeasible
     """
@@ -44,31 +57,30 @@
 
 
 def create_mc_objective(vocs, tkwargs):
     """
     create the objective object
 
     """
-    weights = torch.zeros(vocs.n_outputs, **tkwargs)
-    for idx, ele in enumerate(vocs.objective_names):
-        weights[idx] = -1.0
+    n_outputs = vocs.n_outputs
+    weights = torch.zeros(n_outputs).to(**tkwargs)
+
+    weights = set_botorch_weights(weights, vocs)
 
     def obj_callable(Z):
         return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
 
     return GenericMCObjective(obj_callable)
 
 
 def create_mobo_objective(vocs, tkwargs):
     """
     botorch assumes maximization so we need to negate any objectives that have
     minimize keyword and zero out anything that is a constraint
     """
-    n_objectives = len(vocs.objectives)
+    n_objectives = vocs.n_objectives
     weights = torch.zeros(n_objectives).to(**tkwargs)
-
-    for idx, ele in enumerate(vocs.objectives):
-        weights[idx] = -1.0
+    weights = set_botorch_weights(weights, vocs)
 
     return WeightedMCMultiOutputObjective(
-        weights, outcomes=list(range(n_objectives)), num_outcomes=n_objectives
+        weights, outcomes=list(range(vocs.n_objectives)), num_outcomes=vocs.n_objectives
     )
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/options.py` & `xopt-1.3.0/xopt/generators/bayesian/options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from typing import Callable, List
+from pathlib import Path
+from typing import Dict, List, Type, Union
 
-from pydantic import BaseModel, create_model, Field, root_validator
+import torch
+from pydantic import Field, FilePath, validator
 
 from xopt.generator import GeneratorOptions
-from xopt.generators.bayesian.models.standard import create_standard_model
-from xopt.pydantic import get_descriptions_defaults, JSON_ENCODERS, XoptBaseModel
-from xopt.utils import get_function, get_function_defaults
+from xopt.generators.bayesian.base_model import ModelConstructor
+from xopt.pydantic import (
+    get_descriptions_defaults,
+    JSON_ENCODERS,
+    orjson_dumps,
+    XoptBaseModel,
+)
 
 
 class AcqOptions(XoptBaseModel):
     """Options for defining the acquisition function in BO"""
 
     # monte carlo options
     monte_carlo_samples = Field(128, description="number of monte carlo samples to use")
@@ -22,58 +28,76 @@
     )
 
 
 class OptimOptions(XoptBaseModel):
     """Options for optimizing the acquisition function in BO"""
 
     num_restarts: int = Field(
-        5, description="number of restarts during acquistion " "function optimization"
+        20, description="number of restarts during acquistion function optimization"
     )
     raw_samples: int = Field(
         20, description="number of raw samples used to seed optimization"
     )
     sequential: bool = Field(
         True,
         description="flag to use sequential optimization for q-batch point "
         "selection",
     )
-    use_nearby_initial_points: bool = Field(
-        False, description="flag to use local samples to start acqf optimization"
-    )
     max_travel_distances: List[float] = Field(
         None,
         description="limits for travel distance between points in normalized space",
     )
+    use_turbo: bool = Field(
+        False,
+        description="flag to use Trust region Bayesian Optimization (TuRBO) "
+        "for local optimization",
+    )
 
 
 class ModelOptions(XoptBaseModel):
     """Options for defining the GP model in BO"""
 
-    function: Callable
-    kwargs: BaseModel
+    name: str = Field("standard", description="name of model constructor")
+    custom_constructor: Type[ModelConstructor] = Field(
+        None,
+        description="custom model constructor definition, overrides specified name",
+    )
+
+    use_low_noise_prior: bool = Field(
+        True, description="specify if model should assume a low noise environment"
+    )
+
+    covar_modules: Union[
+        torch.nn.Module, FilePath, Dict[str, torch.nn.Module], Dict[str, FilePath]
+    ] = Field({}, description="covariance modules for GP models")
+
+    mean_modules: Union[
+        torch.nn.Module, FilePath, Dict[str, torch.nn.Module], Dict[str, FilePath]
+    ] = Field({}, description="prior mean modules for GP models")
 
     class Config:
-        arbitrary_types_allowed = True
-        json_encoders = JSON_ENCODERS
         extra = "forbid"
-        allow_mutation = False
+        arbitrary_types_allowed = True
+        json_encoders = {}
+        json_dumps = orjson_dumps
 
-    @root_validator(pre=True)
-    def validate_all(cls, values):
-        if "function" in values.keys():
-            f = get_function(values["function"])
+    @validator("covar_modules", "mean_modules")
+    def validate_torch_modules(cls, v):
+        if isinstance(v, Path):
+            return torch.load(v)
+        elif isinstance(v, dict):
+            new_v = {}
+            for name, item in v.items():
+                if isinstance(item, Path):
+                    new_v[name] = torch.load(item)
+                else:
+                    new_v[name] = v[name]
+            return new_v
         else:
-            f = create_standard_model
-
-        kwargs = values.get("kwargs", {})
-        kwargs = {**get_function_defaults(f), **kwargs}
-        values["function"] = f
-        values["kwargs"] = create_model("kwargs", **kwargs)()
-
-        return values
+            return v
 
 
 class BayesianOptions(GeneratorOptions):
     optim: OptimOptions = OptimOptions()
     acq: AcqOptions = AcqOptions()
     model: ModelOptions = ModelOptions()
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/time_dependent.py` & `xopt-1.3.0/xopt/generators/es/extremumseeking.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,141 @@
-import time
-import warnings
-from abc import ABC
-from typing import Callable, Dict, List
+import logging
 
+import numpy as np
 import pandas as pd
-import torch
-from botorch.acquisition import FixedFeatureAcquisitionFunction
-from gpytorch import Module
-from pydantic import BaseModel, create_model, Field, root_validator
+from pydantic import validator
 
-from xopt.errors import XoptError
-from xopt.generators.bayesian import BayesianGenerator
-from xopt.generators.bayesian.models.time_dependent import create_time_dependent_model
-from xopt.generators.bayesian.options import AcqOptions, BayesianOptions, ModelOptions
-from xopt.utils import get_function, get_function_defaults
-from xopt.vocs import VOCS
+from xopt.generator import Generator, GeneratorOptions
 
+logger = logging.getLogger(__name__)
 
-class TDAcqOptions(AcqOptions):
-    added_time: float = Field(
-        0.0,
-        description="time added to current time to get target predcition time",
-    )
 
+class ExtremumSeekingOptions(GeneratorOptions):
+    k: float = 2.0
+    oscillation_size: float = 0.1
+    decay_rate: float = 1.0
 
-class TDModelOptions(ModelOptions):
-    """Options for defining the GP model in BO"""
+    @validator("oscillation_size", "decay_rate", pre=True)
+    def must_positive(cls, v):
+        if v <= 0:
+            raise ValueError("must larger than 0")
+        return v
 
-    function: Callable
-    kwargs: BaseModel
+    class Config:
+        validate_assignment = True
 
-    @root_validator(pre=True)
-    def validate_all(cls, values):
-        if "function" in values.keys():
-            f = get_function(values["function"])
-        else:
-            f = create_time_dependent_model
 
-        kwargs = values.get("kwargs", {})
-        kwargs = {**get_function_defaults(f), **kwargs}
-        # remove add time
-        kwargs.pop("added_time")
+class ExtremumSeekingGenerator(Generator):
+    """
+    Extremum seeking algorithm.
 
-        values["function"] = f
-        values["kwargs"] = create_model("kwargs", **kwargs)()
+    Reference:
+    Extremum Seeking-Based Control System for Particle Accelerator
+    Beam Loss Minimization
+    A. Scheinker, E. -C. Huang and C. Taylor
+    doi: 10.1109/TCST.2021.3136133
 
-        return values
+    This algorithm must be stepped serially.
+    """
 
+    alias = "extremum_seeking"
 
-class TDOptions(BayesianOptions):
-    acq = TDAcqOptions()
-    model = TDModelOptions()
+    @staticmethod
+    def default_options() -> ExtremumSeekingOptions:
+        return ExtremumSeekingOptions()
 
+    def __init__(self, vocs, options: ExtremumSeekingOptions = None):
+        options = options or ExtremumSeekingOptions()
+        if not isinstance(options, ExtremumSeekingOptions):
+            raise ValueError("options must be a ExtremumSeekingOptions object")
 
-class TimeDependentBayesianGenerator(BayesianGenerator, ABC):
-    def __init__(self, vocs: VOCS, options: TDOptions = None):
-        options = options or TDOptions()
-        if not isinstance(options, TDOptions):
-            raise ValueError("options must be a TDOptions object")
+        if vocs.n_objectives != 1:
+            raise ValueError("vocs must have one objective for optimization")
 
         super().__init__(vocs, options)
-        self.target_prediction_time = None
-
-    @staticmethod
-    def default_options() -> TDOptions:
-        return TDOptions()
+        self.nES = len(vocs.variables)
+        self.wES = np.linspace(1.0, 1.75, int(np.ceil(self.nES / 2)))
+        self.dtES = 2 * np.pi / (10 * np.max(self.wES))
+        self.aES = np.zeros(self.nES)
+        for n in np.arange(self.nES):
+            jw = int(np.floor(n / 2))
+            self.aES[n] = self.wES[jw] * (options.oscillation_size) ** 2
+        bound_low, bound_up = vocs.bounds
+        self.p_ave = (bound_up + bound_low) / 2
+        self.p_diff = bound_up - bound_low
+        self.amplitude = 1
+
+        # Evaluation counter, note that the first point counts as zero in ES
+        self.i = -1
+        # Track the last variables and objectives
+        self.last_input = None  # 1d numpy array
+        self.last_outcome = None  # float
+
+    def add_data(self, new_data: pd.DataFrame):
+        assert (
+            len(new_data) == 1
+        ), f"length of new_data must be 1, found: {len(new_data)}"
+
+        self.data = new_data.iloc[-1:]
+        self.last_input = self.data[self.vocs.variable_names].to_numpy()[0]
+
+        res = self.vocs.objective_data(new_data).to_numpy()
+        assert res.shape == (1, 1)
+        self.last_outcome = res[0, 0]
+
+        self.i += 1
+
+    # Function that normalizes paramters
+    def p_normalize(self, p):
+        p_norm = 2.0 * (p - self.p_ave) / self.p_diff
+        return p_norm
+
+    # Function that un-normalizes parameters
+    def p_un_normalize(self, p):
+        p_un_norm = p * self.p_diff / 2.0 + self.p_ave
+        return p_un_norm
+
+    def generate(self, n_candidates) -> pd.DataFrame:
+        if n_candidates != 1:
+            raise NotImplementedError(
+                "extremum seeking can only produce one candidate at a time"
+            )
 
-    def get_input_data(self, data: pd.DataFrame):
-        return torch.tensor(
-            data[self.vocs.variable_names + ["time"]].to_numpy(), **self._tkwargs
-        )
-
-    def generate(self, n_candidates: int) -> List[Dict]:
-        self.target_prediction_time = time.time() + self.options.acq.added_time
-        output = super().generate(n_candidates)
-
-        if time.time() > self.target_prediction_time:
-            warnings.warn(
-                "target prediction time is in the past! Increase "
-                "added time for accurate results",
-                RuntimeWarning,
+        # Initial data point
+        if self.data.empty:
+            return pd.DataFrame(
+                dict(zip(self.vocs.variable_names, self.p_ave.reshape(-1, 1)))
             )
-        while time.time() < self.target_prediction_time:
-            time.sleep(0.001)
 
-        return output
+        p_n = self.p_normalize(self.last_input)
 
-    def train_model(self, data: pd.DataFrame = None, update_internal=True) -> Module:
-        """
-        Returns a ModelListGP containing independent models for the objectives and
-        constraints
-
-        """
-        if data is None:
-            data = self.data
-
-        # drop nans
-        valid_data = data[
-            self.vocs.variable_names + self.vocs.output_names + ["time"]
-        ].dropna()
-
-        kwargs = self.options.model.kwargs.dict()
-
-        _model = self.options.model.function(
-            valid_data,
-            self.vocs,
-            self._tkwargs,
-            added_time=self.options.acq.added_time,
-            **kwargs
-        )
-
-        if update_internal:
-            self._model = _model
-        return _model
-
-    def get_acquisition(self, model):
-        acq = super().get_acquisition(model)
-
-        # identify which column has the `time` attribute
-        column = [-1]
-        value = torch.tensor(self.target_prediction_time, **self._tkwargs).unsqueeze(0)
-        fixed_acq = FixedFeatureAcquisitionFunction(
-            acq, self.vocs.n_variables + 1, column, value
-        )
-
-        return fixed_acq
-
-    def _get_initial_batch_points(self, bounds):
-        if self.options.optim.use_nearby_initial_points:
-            raise XoptError(
-                "nearby initial points not implemented for "
-                "time dependent optimization"
-            )
-        else:
-            batch_initial_points = None
-            raw_samples = self.options.optim.raw_samples
-        return batch_initial_points, raw_samples
+        # ES step for each parameter
+        p_next_n = np.zeros(self.nES)
+
+        # Loop through each parameter
+        for j in np.arange(self.nES):
+            # Use the same frequency for each two parameters
+            # Alternating Sine and Cosine
+            jw = int(np.floor(j / 2))
+            if not j % 2:
+                p_next_n[j] = p_n[j] + self.amplitude * self.dtES * np.cos(
+                    self.dtES * self.i * self.wES[jw]
+                    + self.options.k * self.last_outcome
+                ) * np.sqrt(self.aES[j] * self.wES[jw])
+            else:
+                p_next_n[j] = p_n[j] + self.amplitude * self.dtES * np.sin(
+                    self.dtES * self.i * self.wES[jw]
+                    + self.options.k * self.last_outcome
+                ) * np.sqrt(self.aES[j] * self.wES[jw])
+
+            # For each new ES value, check that we stay within min/max constraints
+            if p_next_n[j] < -1.0:
+                p_next_n[j] = -1.0
+            if p_next_n[j] > 1.0:
+                p_next_n[j] = 1.0
+
+        p_next = self.p_un_normalize(p_next_n)
+
+        self.amplitude *= self.options.decay_rate  # decay the osc amplitude
+
+        # Return the next value
+        return pd.DataFrame(dict(zip(self.vocs.variable_names, p_next.reshape(-1, 1))))
```

### Comparing `xopt-1.2.6/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-1.3.0/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 
 from xopt.generators.bayesian.bayesian_generator import BayesianGenerator
 from xopt.generators.bayesian.custom_botorch.constrained_acqusition import (
     ConstrainedMCAcquisitionFunction,
 )
 from xopt.generators.bayesian.options import AcqOptions, BayesianOptions
 from xopt.generators.bayesian.time_dependent import (
-    TDAcqOptions,
-    TDModelOptions,
-    TimeDependentBayesianGenerator, TDOptions,
+    TimeDependentAcqOptions,
+    TimeDependentBayesianGenerator,
+    TimeDependentModelOptions,
+    TimeDependentOptions,
 )
 from xopt.utils import format_option_descriptions
 from xopt.vocs import VOCS
 
 
 class UpperConfidenceBoundOptions(AcqOptions):
     beta: float = Field(2.0, description="Beta parameter for UCB optimization")
 
 
-class TDUpperConfidenceBoundOptions(TDAcqOptions):
+class TDUpperConfidenceBoundOptions(TimeDependentAcqOptions):
     beta: float = Field(2.0, description="Beta parameter for UCB optimization")
 
 
 class UCBOptions(BayesianOptions):
     acq = UpperConfidenceBoundOptions()
 
 
-class TDUCBOptions(UCBOptions, TDOptions):
+class TDUCBOptions(UCBOptions, TimeDependentOptions):
     acq = TDUpperConfidenceBoundOptions()
-    model = TDModelOptions()
+    model = TimeDependentModelOptions()
 
 
 class UpperConfidenceBoundGenerator(BayesianGenerator):
     alias = "upper_confidence_bound"
     __doc__ = (
         """Implements Bayeisan Optimization using the Upper Confidence Bound
     acquisition function"""
@@ -58,15 +59,15 @@
 
         if vocs.n_objectives != 1:
             raise ValueError("vocs must have one objective for optimization")
 
         super().__init__(vocs, options)
 
     @staticmethod
-    def default_options() -> UCBOptions:
+    def default_options() -> BayesianOptions:
         return UCBOptions()
 
     def _get_acquisition(self, model):
         qUCB = qUpperConfidenceBound(
             model,
             sampler=self.sampler,
             objective=self._get_objective(),
```

### Comparing `xopt-1.2.6/xopt/generators/ga/cnsga.py` & `xopt-1.3.0/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/ga/deap_creator.py` & `xopt-1.3.0/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-1.3.0/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/ga/fitness_with_constraints.py` & `xopt-1.3.0/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/random.py` & `xopt-1.3.0/xopt/generators/random.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/generators/scipy/neldermead.py` & `xopt-1.3.0/xopt/generators/scipy/neldermead.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     @property
     def initial_point(self):
         return self.options.initial_point
 
     @initial_point.setter
     def initial_point(self, value):
         if value is None:
-            value = self.vocs.random_inputs(
-                include_constants=False, include_linked_variables=False
-            )
+            value = self.vocs.random_inputs()
         self.options.initial_point = value
 
     def add_data(self, new_data: pd.DataFrame):
         assert (
             len(new_data) == 1
         ), f"length of new_data must be 1, found: {len(new_data)}"
         res = self.vocs.objective_data(new_data).to_numpy()
@@ -114,15 +112,20 @@
             )
 
         try:
             self.x, self.state = next(
                 self._algorithm
             )  # raw x point and any state to be passed back
             self._lock = True
-            self.inputs = [dict(zip(self.vocs.variable_names, self.x))]
+
+            inputs = dict(zip(self.vocs.variable_names, self.x))
+            if self.vocs.constants is not None:
+                inputs.update(self.vocs.constants)
+            self.inputs = [inputs]
+
         except StopIteration:
             self._is_done = True
 
         return self.inputs
 
 
 class NelderMeadOptions(GeneratorOptions):
```

### Comparing `xopt-1.2.6/xopt/log.py` & `xopt-1.3.0/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/mpi/run.py` & `xopt-1.3.0/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/pydantic.py` & `xopt-1.3.0/xopt/pydantic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,79 @@
 import copy
 import inspect
+import json
 import logging
 from concurrent.futures import Future
 from importlib import import_module
 from types import FunctionType, MethodType
 from typing import Any, Callable, Generic, Iterable, List, Optional, TypeVar
 
 import numpy as np
+import orjson
+import torch.nn
 from pydantic import BaseModel, create_model, Extra, Field, root_validator, validator
 from pydantic.generics import GenericModel
 
 ObjType = TypeVar("ObjType")
 logger = logging.getLogger(__name__)
 
 JSON_ENCODERS = {
     # function/method type distinguished for class members
     # and not recognized as callables
     FunctionType: lambda x: f"{x.__module__}.{x.__qualname__}",
     MethodType: lambda x: f"{x.__module__}.{x.__qualname__}",
-    Callable: lambda x: f"{x.__module__}.{type(x).__qualname__}",
+    Callable: lambda x: f"{x.__module__}.{x.__qualname__}",
     type: lambda x: f"{x.__module__}.{x.__name__}",
     # for encoding instances of the ObjType}
-    ObjType: lambda x: f"{x.__module__}.{x.__class__.__qualname__}",
+    # ObjType: lambda x: f"{x.__module__}.{x.__class__.__qualname__}",
     np.ndarray: lambda x: x.tolist(),
     np.int64: lambda x: int(x),
     np.float64: lambda x: float(x),
+    # torch.nn.Module: lambda x: process_torch_module(x),
+    # torch.Tensor: lambda x: x.detach().cpu().numpy().tolist(),
 }
 
 
+def recursive_serialize(v, base_key=""):
+    for key, value in v.items():
+        if isinstance(value, dict):
+            v[key] = recursive_serialize(value, key)
+        elif isinstance(value, torch.nn.Module):
+            v[key] = process_torch_module(module=value, name="_".join((base_key, key)))
+        else:
+            for _type, func in JSON_ENCODERS.items():
+                if isinstance(value, _type):
+                    v[key] = func(value)
+
+        # check to make sure object has been serialized,
+        # if not use a generic serializer
+        try:
+            json.dumps(v[key])
+        except (TypeError, OverflowError):
+            v[key] = f"{v[key].__module__}.{v[key].__class__.__qualname__}"
+
+    return v
+
+
+# define custom json_dumps using orjson
+def orjson_dumps(v, *, default):
+    v = recursive_serialize(v)
+    # orjson.dumps returns bytes, to match standard json.dumps we need to decode
+    return orjson.dumps(v, default=default).decode()
+
+
+def process_torch_module(module, name):
+    """save module to file based on module name and return file path to json"""
+    # module_name = "".join(random.choices(string.ascii_uppercase + string.digits,
+    #                                     k=7)) + ".pt"
+    module_name = f"{name}.pt"
+    torch.save(module, module_name)
+    return module_name
+
+
 def get_descriptions_defaults(model: BaseModel):
     """get a dict containing the descriptions of fields inside nested pydantic models"""
 
     description_dict = {}
     for name, val in model.__fields__.items():
         try:
             if issubclass(val.type_, BaseModel):
@@ -48,24 +90,24 @@
 
     return description_dict
 
 
 class XoptBaseModel(BaseModel):
     class Config:
         extra = "forbid"
-        json_encoders = JSON_ENCODERS
+        json_dumps = orjson_dumps
 
 
 class CallableModel(BaseModel):
     callable: Callable
     signature: BaseModel
 
     class Config:
         arbitrary_types_allowed = True
-        json_encoders = JSON_ENCODERS
+        json_dumps = orjson_dumps
         extra = Extra.forbid
 
     @root_validator(pre=True)
     def validate_all(cls, values):
         callable = values.pop("callable")
 
         if not isinstance(
@@ -126,15 +168,15 @@
         return self.callable(*fn_args, **fn_kwargs)
 
 
 class ObjLoader(
     GenericModel,
     Generic[ObjType],
     arbitrary_types_allowed=True,
-    json_encoders=JSON_ENCODERS,
+    json_dumps=orjson_dumps,
 ):
     object: Optional[ObjType]
     loader: CallableModel = None
     object_type: Optional[type]
 
     @root_validator(pre=True)
     def validate_all(cls, values):
@@ -166,19 +208,20 @@
 
                     # opt for obj type
                     values["loader"].pop("callable")
 
                 # re-init drop callable from loader vals to use new instance
                 loader = CallableModel(callable=obj_type, **values["loader"])
 
-        # update the class json encoders. Will only execute on initial type construction
-        if obj_type not in cls.__config__.json_encoders:
-            cls.__config__.json_encoders[obj_type] = cls.__config__.json_encoders.pop(
-                ObjType
-            )
+        # update the class json encoders. Will only execute on initial type
+        # construction
+        # if obj_type not in cls.__config__.json_encoders:
+        #    cls.__config__.json_encoders[obj_type] = cls.__config__.json_encoders.pop(
+        #        ObjType
+        #    )
         return {"object_type": obj_type, "loader": loader}
 
     def load(self, store: bool = False):
         # store object reference on loader
         if store:
             self.object = self.loader.call()
             return self.object
@@ -189,15 +232,15 @@
 
 
 # COMMON BASE FOR EXECUTORS
 class BaseExecutor(
     GenericModel,
     Generic[ObjType],
     arbitrary_types_allowed=True,
-    json_encoders=JSON_ENCODERS,
+    json_dumps=orjson_dumps,
     copy_on_model_validation="none",
     # Needed to avoid: https://github.com/samuelcolvin/pydantic/discussions/4099
 ):
     # executor_type must comply with https://peps.python.org/pep-3148/ standard
     loader: Optional[ObjLoader[ObjType]]  # loader of executor type
 
     # This is a utility field not included in reps. The typing lib has opened
@@ -284,18 +327,18 @@
             if "executor" in loader_values:
                 loader_values.pop("executor")
 
             loader = ObjLoader[executor_type](**loader_values)
 
         # update encoders
         # update the class json encoders. Will only execute on initial type construction
-        if executor_type not in cls.__config__.json_encoders:
-            cls.__config__.json_encoders[
-                executor_type
-            ] = cls.__config__.json_encoders.pop(ObjType)
+        # if executor_type not in cls.__config__.json_encoders:
+        #    cls.__config__.json_encoders[
+        #        executor_type
+        #    ] = cls.__config__.json_encoders.pop(ObjType)
 
         return {
             "executor_type": executor_type,
             "submit_callable": submit_callable,
             "shutdown_callable": shutdown_callable,
             "map_callable": map_callable,
             "loader": loader,
@@ -308,15 +351,15 @@
 
 
 # NormalExecutor with no context handling on submission and executor persistence
 class NormalExecutor(
     BaseExecutor[ObjType],
     Generic[ObjType],
     arbitrary_types_allowed=True,
-    json_encoders=JSON_ENCODERS,
+    json_dumps=orjson_dumps,
 ):
     @validator("executor", always=True)
     def validate_executor(cls, v, values):
         if v is None:
             v = values["loader"].load()
 
         # if not None, validate against executor type
```

### Comparing `xopt-1.2.6/xopt/resources/test_functions/modified_tnk.py` & `xopt-1.3.0/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/resources/test_functions/rosenbrock.py` & `xopt-1.3.0/xopt/resources/test_functions/rosenbrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     n = len(x)
 
     return sum(
         (100 * (x[i + 1] - x[i] ** 2) ** 2 + (1 - x[i]) ** 2 for i in range(n - 1))
     )
 
 
-def evaluate_rosenbrock(inputs: Dict, label="y") -> Dict[str, float]:
+def evaluate_rosenbrock(inputs: Dict, label="y", dummy=1) -> Dict[str, float]:
     """
     Evaluate the Rosenbrock function with labeled inputs and outputs.
 
     Parameters
     ----------
     inputs: Dict[str, float]
         labeled vector of inputs. The labels can be arbitrary.
```

### Comparing `xopt-1.2.6/xopt/resources/test_functions/tnk.py` & `xopt-1.3.0/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/resources/testing.py` & `xopt-1.3.0/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-1.2.6/xopt/utils.py` & `xopt-1.3.0/xopt/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import importlib
 import inspect
 import sys
 import time
 import traceback
 
 import pandas as pd
+import torch
 import yaml
+from matplotlib import pyplot as plt
 
 from .pydantic import get_descriptions_defaults
 from .vocs import VOCS
 
 
 def add_constraint_information(data: pd.DataFrame, vocs: VOCS) -> pd.DataFrame:
     """
@@ -165,7 +167,45 @@
         DataFrame with xopt_index as the index column
     """
     dfs = []
     for file in files:
         df = pd.read_csv(file, index_col="xopt_index")
         dfs.append(df)
     return pd.concat(dfs)
+
+
+def visualize_model(generator, data):
+    test_x = torch.linspace(*torch.tensor(generator.vocs.bounds.flatten()), 100)
+    generator.add_data(data)
+    model = generator.train_model()
+
+    fig, ax = plt.subplots(2, 1, sharex="all")
+    fig.set_size_inches(6, 6)
+    with torch.no_grad():
+        post = model.posterior(test_x.reshape(-1, 1, 1).double())
+
+        for i in range(len(generator.vocs.output_names)):
+            mean = post.mean
+            l, u = post.mvn.confidence_region()
+
+            ax[0].plot(
+                test_x,
+                mean[..., i],
+                f"C{i}",
+                label=f"{generator.vocs.output_names[i]} model",
+            )
+            ax[0].fill_between(
+                test_x, l[..., i].flatten(), u[..., i].flatten(), alpha=0.5
+            )
+            generator.data.plot(
+                x=generator.vocs.variable_names[0],
+                y=generator.vocs.output_names[i],
+                ax=ax[0],
+                style=f"oC{i}",
+            )
+
+        ax[0].legend()
+
+        acq = generator.get_acquisition(model)(test_x.reshape(-1, 1, 1).double())
+
+        ax[1].plot(test_x, acq, label="Acquisition Function")
+        ax[1].legend()
```

### Comparing `xopt-1.2.6/xopt/vocs.py` & `xopt-1.3.0/xopt/vocs.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,27 +223,28 @@
         """
         return form_variable_data(self.variables, data, prefix=prefix)
 
     def objective_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "objective_",
+        return_raw=False,
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing objective data transformed according to
         `vocs.objectives` such that we always assume minimization.
 
         Args:
             data: data to be processed.
             prefix: prefix added to column names.
 
         Returns:
             result: processed Dataframe
         """
-        return form_objective_data(self.objectives, data, prefix)
+        return form_objective_data(self.objectives, data, prefix, return_raw)
 
     def constraint_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "constraint_",
     ) -> pd.DataFrame:
         """
@@ -290,29 +291,31 @@
             None
 
         Raises:
             ValueError: if input data does not satisfy requirements.
         """
         validate_input_data(self, input_points)
 
-    def extract_data(self, data: pd.DataFrame):
+    def extract_data(self, data: pd.DataFrame, return_raw=False):
         """
         split dataframe into seperate dataframes for variables, objectives and
-        constraints based on vocs
+        constraints based on vocs - objective data is transformed based on
+        `vocs.objectives` properties
 
         Args:
             data: dataframe to be split
+            return_raw: if True, return untransformed objective data
 
         Returns:
             variable_data: dataframe containing variable data
             objective_data: dataframe containing objective data
             constraint_data: dataframe containing constraint data
         """
         variable_data = self.variable_data(data, "")
-        objective_data = self.objective_data(data, "")
+        objective_data = self.objective_data(data, "", return_raw)
         constraint_data = self.constraint_data(data, "")
         return variable_data, objective_data, constraint_data
 
 
 # --------------------------------
 # dataframe utilities
 
@@ -330,19 +333,22 @@
     vdata = pd.DataFrame()
     for k in sorted(list(variables)):
         vdata[prefix + k] = data[k]
 
     return vdata
 
 
-def form_objective_data(objectives: Dict, data, prefix="objective_"):
+def form_objective_data(
+    objectives: Dict, data, prefix="objective_", return_raw: bool = False
+):
     """
     Use objective dict and data (dataframe) to generate objective data (dataframe)
 
-    Weights are applied to convert all objectives into mimimization form.
+    Weights are applied to convert all objectives into mimimization form unless
+    `return_raw` is True
 
     Returns a dataframe with the objective data intented to be minimized.
 
     Missing or nan values will be filled with: np.inf
 
     """
     if not objectives:
@@ -358,15 +364,15 @@
             odata[prefix + k] = np.inf
             continue
 
         operator = objectives[k].upper()
         if operator not in OBJECTIVE_WEIGHT:
             raise ValueError(f"Unknown objective operator: {operator}")
 
-        weight = OBJECTIVE_WEIGHT[operator]
+        weight = 1.0 if return_raw else OBJECTIVE_WEIGHT[operator]
         odata[prefix + k] = (weight * data[k]).fillna(np.inf)  # Protect against nans
 
     return odata
 
 
 def form_constraint_data(constraints: Dict, data: pd.DataFrame, prefix="constraint_"):
     """
```

### Comparing `xopt-1.2.6/xopt.egg-info/PKG-INFO` & `xopt-1.3.0/xopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.2.6
+Version: 1.3.0
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.2.6/xopt.egg-info/SOURCES.txt` & `xopt-1.3.0/xopt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 tests/test_utils.py
 tests/test_vocs.py
 tests/test_xopt.py
 tests/generators/__init__.py
 tests/generators/test_extremum_seeking.py
 tests/generators/test_generator_options.py
 tests/generators/test_random.py
+tests/generators/test_rcds.py
 tests/generators/bayesian/__init__.py
 tests/generators/bayesian/test_bayesian_exploration.py
 tests/generators/bayesian/test_bayesian_generator.py
 tests/generators/bayesian/test_bayesian_options.py
-tests/generators/bayesian/test_custom_botorch.py
+tests/generators/bayesian/test_custom_model.py
 tests/generators/bayesian/test_expected_improvement.py
 tests/generators/bayesian/test_high_level.py
 tests/generators/bayesian/test_mggpo.py
 tests/generators/bayesian/test_mobo.py
+tests/generators/bayesian/test_multi_fidelity.py
 tests/generators/bayesian/test_time_dependent_bo.py
+tests/generators/bayesian/test_turbo.py
 tests/generators/bayesian/test_upper_confidence_bound.py
 tests/generators/bayesian/test_utils.py
 xopt/__init__.py
 xopt/_version.py
 xopt/base.py
 xopt/errors.py
 xopt/evaluator.py
@@ -42,44 +45,53 @@
 xopt.egg-info/SOURCES.txt
 xopt.egg-info/dependency_links.txt
 xopt.egg-info/requires.txt
 xopt.egg-info/top_level.txt
 xopt/generators/__init__.py
 xopt/generators/random.py
 xopt/generators/bayesian/__init__.py
+xopt/generators/bayesian/base_model.py
 xopt/generators/bayesian/bayesian_exploration.py
 xopt/generators/bayesian/bayesian_generator.py
 xopt/generators/bayesian/expected_improvement.py
 xopt/generators/bayesian/mggpo.py
 xopt/generators/bayesian/mobo.py
+xopt/generators/bayesian/multi_fidelity.py
 xopt/generators/bayesian/objectives.py
 xopt/generators/bayesian/options.py
 xopt/generators/bayesian/time_dependent.py
+xopt/generators/bayesian/turbo.py
 xopt/generators/bayesian/upper_confidence_bound.py
 xopt/generators/bayesian/utils.py
 xopt/generators/bayesian/custom_botorch/__init__.py
 xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
-xopt/generators/bayesian/custom_botorch/constraint_transform.py
 xopt/generators/bayesian/custom_botorch/identity.py
+xopt/generators/bayesian/custom_botorch/multi_fidelity.py
 xopt/generators/bayesian/custom_botorch/proximal.py
 xopt/generators/bayesian/models/__init__.py
+xopt/generators/bayesian/models/prior_mean.py
 xopt/generators/bayesian/models/standard.py
 xopt/generators/bayesian/models/time_dependent.py
+xopt/generators/bayesian/models/transformed_model.py
 xopt/generators/bayesian/models/utils.py
 xopt/generators/es/__init__.py
 xopt/generators/es/extremumseeking.py
 xopt/generators/ga/__init__.py
 xopt/generators/ga/cnsga.py
 xopt/generators/ga/deap_creator.py
 xopt/generators/ga/deap_fitness_with_constraints.py
 xopt/generators/ga/fitness_with_constraints.py
+xopt/generators/rcds/__init__.py
+xopt/generators/rcds/rcds.py
 xopt/generators/scipy/__init__.py
 xopt/generators/scipy/neldermead.py
 xopt/mpi/__init__.py
 xopt/mpi/run.py
 xopt/resources/__init__.py
 xopt/resources/testing.py
 xopt/resources/test_functions/__init__.py
+xopt/resources/test_functions/ackley_20.py
 xopt/resources/test_functions/modified_tnk.py
 xopt/resources/test_functions/rosenbrock.py
 xopt/resources/test_functions/sinusoid_1d.py
+xopt/resources/test_functions/sphere_20.py
 xopt/resources/test_functions/tnk.py
```

