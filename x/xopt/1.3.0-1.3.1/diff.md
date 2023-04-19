# Comparing `tmp/xopt-1.3.0.tar.gz` & `tmp/xopt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-0o0z5bgh/xopt-1.3.0.tar", last modified: Wed Apr 19 16:45:56 2023, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-roqjaqyi/xopt-1.3.1.tar", last modified: Wed Apr 19 17:57:55 2023, max compression
```

## Comparing `xopt-1.3.0.tar` & `xopt-1.3.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 16:45:47.000000 xopt-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:47.000000 xopt-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 16:45:56.000000 xopt-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-19 16:45:47.000000 xopt-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:47.000000 xopt-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 16:45:56.000000 xopt-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 16:45:47.000000 xopt-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_bayesian_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_generator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/generators/test_rcds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-19 16:45:47.000000 xopt-1.3.0/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-04-19 16:45:47.000000 xopt-1.3.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/prior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/transformed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/bayesian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/rcds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/rcds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/rcds/rcds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/ackley_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/sphere_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-19 16:45:47.000000 xopt-1.3.0/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 16:45:56.000000 xopt-1.3.0/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 16:45:55.000000 xopt-1.3.0/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 17:57:46.000000 xopt-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:46.000000 xopt-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 17:57:55.000000 xopt-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-19 17:57:46.000000 xopt-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:46.000000 xopt-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 17:57:55.000000 xopt-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 17:57:46.000000 xopt-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_generator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-04-19 17:57:46.000000 xopt-1.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/transformed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/top_level.txt
```

### Comparing `xopt-1.3.0/LICENSE` & `xopt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/PKG-INFO` & `xopt-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.3.0/README.md` & `xopt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/setup.py` & `xopt-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-1.3.1/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-1.3.1/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_bayesian_options.py` & `xopt-1.3.1/tests/generators/bayesian/test_bayesian_options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_custom_model.py` & `xopt-1.3.1/tests/generators/bayesian/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_expected_improvement.py` & `xopt-1.3.1/tests/generators/bayesian/test_expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_high_level.py` & `xopt-1.3.1/tests/generators/bayesian/test_high_level.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_mggpo.py` & `xopt-1.3.1/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_mobo.py` & `xopt-1.3.1/tests/generators/bayesian/test_mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_multi_fidelity.py` & `xopt-1.3.1/tests/generators/bayesian/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-1.3.1/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_turbo.py` & `xopt-1.3.1/tests/generators/bayesian/test_turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-1.3.1/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/bayesian/test_utils.py` & `xopt-1.3.1/tests/generators/bayesian/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/test_extremum_seeking.py` & `xopt-1.3.1/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/generators/test_rcds.py` & `xopt-1.3.1/tests/generators/test_rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/test_evaluator.py` & `xopt-1.3.1/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/test_io.py` & `xopt-1.3.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/test_pydantic.py` & `xopt-1.3.1/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/test_vocs.py` & `xopt-1.3.1/tests/test_vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/tests/test_xopt.py` & `xopt-1.3.1/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/versioneer.py` & `xopt-1.3.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/base.py` & `xopt-1.3.1/xopt/base.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/evaluator.py` & `xopt-1.3.1/xopt/evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generator.py` & `xopt-1.3.1/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/__init__.py` & `xopt-1.3.1/xopt/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/__init__.py` & `xopt-1.3.1/xopt/generators/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/base_model.py` & `xopt-1.3.1/xopt/generators/bayesian/base_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-1.3.1/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/bayesian_generator.py` & `xopt-1.3.1/xopt/generators/bayesian/bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py` & `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py` & `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/expected_improvement.py` & `xopt-1.3.1/xopt/generators/bayesian/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/mggpo.py` & `xopt-1.3.1/xopt/generators/bayesian/mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/mobo.py` & `xopt-1.3.1/xopt/generators/bayesian/mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/models/prior_mean.py` & `xopt-1.3.1/xopt/generators/bayesian/models/prior_mean.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/models/standard.py` & `xopt-1.3.1/xopt/generators/bayesian/models/standard.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/models/time_dependent.py` & `xopt-1.3.1/xopt/generators/bayesian/models/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/models/transformed_model.py` & `xopt-1.3.1/xopt/generators/bayesian/models/transformed_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/models/utils.py` & `xopt-1.3.1/xopt/generators/bayesian/models/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/multi_fidelity.py` & `xopt-1.3.1/xopt/generators/bayesian/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/objectives.py` & `xopt-1.3.1/xopt/generators/bayesian/objectives.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/options.py` & `xopt-1.3.1/xopt/generators/bayesian/options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/time_dependent.py` & `xopt-1.3.1/xopt/generators/bayesian/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/turbo.py` & `xopt-1.3.1/xopt/generators/bayesian/turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-1.3.1/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/bayesian/utils.py` & `xopt-1.3.1/xopt/generators/bayesian/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/es/extremumseeking.py` & `xopt-1.3.1/xopt/generators/es/extremumseeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/ga/cnsga.py` & `xopt-1.3.1/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/ga/deap_creator.py` & `xopt-1.3.1/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-1.3.1/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/ga/fitness_with_constraints.py` & `xopt-1.3.1/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/random.py` & `xopt-1.3.1/xopt/generators/random.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/rcds/rcds.py` & `xopt-1.3.1/xopt/generators/rcds/rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/generators/scipy/neldermead.py` & `xopt-1.3.1/xopt/generators/scipy/neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/log.py` & `xopt-1.3.1/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/mpi/run.py` & `xopt-1.3.1/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/pydantic.py` & `xopt-1.3.1/xopt/pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/resources/test_functions/modified_tnk.py` & `xopt-1.3.1/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/resources/test_functions/rosenbrock.py` & `xopt-1.3.1/xopt/resources/test_functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/resources/test_functions/tnk.py` & `xopt-1.3.1/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/resources/testing.py` & `xopt-1.3.1/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt/utils.py` & `xopt-1.3.1/xopt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import sys
 import time
 import traceback
 
 import pandas as pd
 import torch
 import yaml
-from matplotlib import pyplot as plt
 
 from .pydantic import get_descriptions_defaults
 from .vocs import VOCS
 
 
 def add_constraint_information(data: pd.DataFrame, vocs: VOCS) -> pd.DataFrame:
     """
@@ -169,21 +168,28 @@
     dfs = []
     for file in files:
         df = pd.read_csv(file, index_col="xopt_index")
         dfs.append(df)
     return pd.concat(dfs)
 
 
-def visualize_model(generator, data):
+def visualize_model(generator, data, axes=None):
     test_x = torch.linspace(*torch.tensor(generator.vocs.bounds.flatten()), 100)
     generator.add_data(data)
     model = generator.train_model()
 
-    fig, ax = plt.subplots(2, 1, sharex="all")
-    fig.set_size_inches(6, 6)
+    if axes is None:
+        # Lazy import
+        from matplotlib import pyplot as plt
+
+        fig, ax = plt.subplots(2, 1, sharex="all")
+        fig.set_size_inches(6, 6)
+    else:
+        ax = axes
+
     with torch.no_grad():
         post = model.posterior(test_x.reshape(-1, 1, 1).double())
 
         for i in range(len(generator.vocs.output_names)):
             mean = post.mean
             l, u = post.mvn.confidence_region()
```

### Comparing `xopt-1.3.0/xopt/vocs.py` & `xopt-1.3.1/xopt/vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.0/xopt.egg-info/PKG-INFO` & `xopt-1.3.1/xopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.3.0/xopt.egg-info/SOURCES.txt` & `xopt-1.3.1/xopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

