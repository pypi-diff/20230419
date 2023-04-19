# Comparing `tmp/stcal-1.3.5.tar.gz` & `tmp/stcal-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.3.5.tar", last modified: Thu Mar 30 20:12:23 2023, max compression
+gzip compressed data, was "stcal-1.3.6.tar", last modified: Wed Apr 19 18:19:23 2023, max compression
```

## Comparing `stcal-1.3.5.tar` & `stcal-1.3.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.827346 stcal-1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.747346 stcal-1.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.751346 stcal-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/cancel_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-30 20:12:12.000000 stcal-1.3.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-30 20:12:12.000000 stcal-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-30 20:12:12.000000 stcal-1.3.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-03-30 20:12:12.000000 stcal-1.3.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-30 20:12:12.000000 stcal-1.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-30 20:12:12.000000 stcal-1.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-30 20:12:12.000000 stcal-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-30 20:12:23.827346 stcal-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 20:12:12.000000 stcal-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-30 20:12:12.000000 stcal-1.3.5/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.751346 stcal-1.3.5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-03-30 20:12:12.000000 stcal-1.3.5/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.751346 stcal-1.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.751346 stcal-1.3.5/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.751346 stcal-1.3.5/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.755346 stcal-1.3.5/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-30 20:12:12.000000 stcal-1.3.5/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-30 20:12:12.000000 stcal-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:12:23.827346 stcal-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.743347 stcal-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.755346 stcal-1.3.5/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.759346 stcal-1.3.5/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.759346 stcal-1.3.5/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.759346 stcal-1.3.5/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.763346 stcal-1.3.5/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   127072 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10024 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.763346 stcal-1.3.5/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-30 20:12:12.000000 stcal-1.3.5/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.755346 stcal-1.3.5/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 20:12:23.000000 stcal-1.3.5/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:12:22.000000 stcal-1.3.5/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.795346 stcal-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:12:23.827346 stcal-1.3.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48432 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-03-30 20:12:12.000000 stcal-1.3.5/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-30 20:12:12.000000 stcal-1.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.778066 stcal-1.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-19 18:19:13.000000 stcal-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 18:19:13.000000 stcal-1.3.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-19 18:19:13.000000 stcal-1.3.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-19 18:19:13.000000 stcal-1.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-19 18:19:13.000000 stcal-1.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 18:19:13.000000 stcal-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-19 18:19:23.778066 stcal-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-19 18:19:13.000000 stcal-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-19 18:19:13.000000 stcal-1.3.6/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-19 18:19:13.000000 stcal-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:19:23.778066 stcal-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127072 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:22.000000 stcal-1.3.6/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.746065 stcal-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/current_gdqfits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.778066 stcal-1.3.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48432 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-19 18:19:13.000000 stcal-1.3.6/tox.ini
```

### Comparing `stcal-1.3.5/.github/labeler.yml` & `stcal-1.3.6/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/.github/pull_request_template.md` & `stcal-1.3.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/.github/workflows/ci.yml` & `stcal-1.3.6/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,32 @@
   pull_request:
     branches:
       - main
   schedule:
     # Weekly Monday 9AM build
     - cron: "0 9 * * 1"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   check:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
         - linux: check-style
         - linux: check-security
         - linux: check-build
   test:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
         - linux: test-oldestdeps-cov-xdist
-          python-version: 3.8
-        - linux: test-xdist
-          python-version: '3.8'
+          python-version: 3.9
         - linux: test-xdist
           python-version: '3.9'
         - linux: test-xdist
           python-version: '3.10'
         - linux: test-xdist
           python-version: '3.11'
         - macos: test-xdist
```

### Comparing `stcal-1.3.5/.github/workflows/publish-to-pypi.yml` & `stcal-1.3.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/.gitignore` & `stcal-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/.readthedocs.yaml` & `stcal-1.3.6/.readthedocs.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,23 @@
   fail_on_warning: true
 
 # Optionally build your docs in additional formats such as PDF and ePub
 formats:
   - htmlzip
   - pdf
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: mambaforge-4.10
+
+conda:
+  environment: docs/rtd_environment.yaml
+
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.8
+  system_packages: false
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
```

### Comparing `stcal-1.3.5/CHANGES.rst` & `stcal-1.3.6/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+1.4.0 (unreleased)
+==================
+
+Bug Fixes
+---------
+
+-
+
+Changes to API
+--------------
+
+- drop support for Python 3.8 [#162]
+
+Other
+-----
+
+-
+
+1.3.6 (2023-04-19)
+==================
+
+Bug Fixes
+---------
+
+ramp_fitting
+~~~~~~~~~~~~
+
+- The ``meta`` tag was missing when checking for ``drop_frame1``.  It has been
+  added to the check. [#161]
+
+
+Changes to API
+--------------
+
+- 
+
+Other
+-----
+
+- Remove use of deprecated ``pytest-openfiles`` ``pytest`` plugin. This has been replaced by
+  catching ``ResourceWarning``s. [#159]
+
+
 1.3.5 (2023-03-30)
 ==================
 
 Bug Fixes
 ---------
 
 jump
```

### Comparing `stcal-1.3.5/CODE_OF_CONDUCT.md` & `stcal-1.3.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/CONTRIBUTING.md` & `stcal-1.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/LICENSE` & `stcal-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/benchmarks/dark_current.py` & `stcal-1.3.6/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/benchmarks/linearity.py` & `stcal-1.3.6/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/benchmarks/ramp_fitting.py` & `stcal-1.3.6/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/benchmarks/saturation.py` & `stcal-1.3.6/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/docs/Makefile` & `stcal-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/docs/conf.py` & `stcal-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/docs/stcal/jump/description.rst` & `stcal-1.3.6/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/docs/stcal/ramp_fitting/description.rst` & `stcal-1.3.6/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/pyproject.toml` & `stcal-1.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = 'stcal'
 description = 'STScI tools and algorithms used in calibration pipelines'
 readme = 'README.md'
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 license = { file = 'LICENSE' }
 authors = [{ name = 'STScI', email = 'help@stsci.edu' }]
 classifiers = [
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Astronomy',
     'License :: OSI Approved :: BSD License',
     'Programming Language :: Python :: 3',
@@ -30,15 +30,14 @@
     'tomli; python_version <"3.11"',
 ]
 test = [
     'psutil',
     'pytest >=4.6.0',
     'pytest-cov',
     'pytest-doctestplus',
-    'pytest-openfiles >=0.5.0',
 ]
 
 [project.urls]
 'repository' = 'https://github.com/spacetelescope/stcal'
 'tracker' = 'https://github.com/spacetelescope/stcal/issues'
 
 [build-system]
@@ -59,23 +58,26 @@
 where = ['src']
 
 [tool.pytest.ini_options]
 minversion = 4.6
 doctest_plus = true
 doctest_rst = true
 text_file_format = 'rst'
-addopts = '--open-files'
+addopts = ''
 norecursedirs = [
     'benchmarks',
     '.asv',
     '.eggs',
     '.tox',
     'build',
     'venv',
 ]
+filterwarnings = [
+    "error::ResourceWarning",
+]
 
 [tool.ruff]
 line-length = 110
 select = ['F', 'W', 'E', 'C']
 ignore = [
     'C901', # variable is too complex
 ]
```

### Comparing `stcal-1.3.5/src/stcal/dark_current/dark_class.py` & `stcal-1.3.6/src/stcal/dark_current/dark_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/dark_current/dark_sub.py` & `stcal-1.3.6/src/stcal/dark_current/dark_sub.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/dqflags.py` & `stcal-1.3.6/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/jump/jump.py` & `stcal-1.3.6/src/stcal/jump/jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/jump/twopoint_difference.py` & `stcal-1.3.6/src/stcal/jump/twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/linearity/linearity.py` & `stcal-1.3.6/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.3.6/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.3.6/src/stcal/ramp_fitting/ols_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                              model.groupdq, model.pixeldq)
     else:
         ramp_data.set_arrays(model.data, model.err,
                              model.groupdq, model.pixeldq)
 
     # Attribute may not be supported by all pipelines.  Default is NoneType.
     if hasattr(model, 'drop_frames1'):
-        drop_frames1 = model.exposure.drop_frames1
+        drop_frames1 = model.meta.exposure.drop_frames1
     else:
         drop_frames1 = None
     ramp_data.set_meta(
         name=model.meta.instrument.name,
         frame_time=model.meta.exposure.frame_time,
         group_time=model.meta.exposure.group_time,
         groupgap=model.meta.exposure.groupgap,
```

### Comparing `stcal-1.3.5/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/ramp_fitting/utils.py` & `stcal-1.3.6/src/stcal/ramp_fitting/utils.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal/saturation/saturation.py` & `stcal-1.3.6/src/stcal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/src/stcal.egg-info/SOURCES.txt` & `stcal-1.3.6/src/stcal.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 README.md
 asv.conf.json
 pyproject.toml
 tox.ini
 .github/CODEOWNERS
 .github/labeler.yml
 .github/pull_request_template.md
-.github/workflows/cancel_workflows.yml
 .github/workflows/changelog.yml
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/label_pull_request.yml
 .github/workflows/publish-to-pypi.yml
 benchmarks/__init__.py
 benchmarks/dark_current.py
@@ -24,14 +23,15 @@
 benchmarks/linearity.py
 benchmarks/ramp_fitting.py
 benchmarks/saturation.py
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
+docs/rtd_environment.yaml
 docs/stcal/package_index.rst
 docs/stcal/jump/description.rst
 docs/stcal/jump/index.rst
 docs/stcal/ramp_fitting/description.rst
 docs/stcal/ramp_fitting/index.rst
 src/stcal/__init__.py
 src/stcal/_version.py
```

### Comparing `stcal-1.3.5/tests/current_gdqfits` & `stcal-1.3.6/tests/current_gdqfits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/data/input_gdq_flarge.fits` & `stcal-1.3.6/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.3.6/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/data/snowball1.fits` & `stcal-1.3.6/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_dark_current.py` & `stcal-1.3.6/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_dq.py` & `stcal-1.3.6/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_jump.py` & `stcal-1.3.6/tests/test_jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_linearity.py` & `stcal-1.3.6/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_ramp_fitting.py` & `stcal-1.3.6/tests/test_ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.3.6/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_saturation.py` & `stcal-1.3.6/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tests/test_twopoint_difference.py` & `stcal-1.3.6/tests/test_twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.5/tox.ini` & `stcal-1.3.6/tox.ini`

 * *Files identical despite different names*

