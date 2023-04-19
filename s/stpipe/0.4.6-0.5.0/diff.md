# Comparing `tmp/stpipe-0.4.6.tar.gz` & `tmp/stpipe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpipe-0.4.6.tar", last modified: Mon Mar 27 17:09:05 2023, max compression
+gzip compressed data, was "stpipe-0.5.0.tar", last modified: Wed Apr 19 13:21:11 2023, max compression
```

## Comparing `stpipe-0.4.6.tar` & `stpipe-0.5.0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.709471 stpipe-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-27 17:08:55.000000 stpipe-0.4.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.697471 stpipe-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.701471 stpipe-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-27 17:08:55.000000 stpipe-0.4.6/.github/workflows/cancel_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-27 17:08:55.000000 stpipe-0.4.6/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-27 17:08:55.000000 stpipe-0.4.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-27 17:08:55.000000 stpipe-0.4.6/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-27 17:08:55.000000 stpipe-0.4.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-27 17:08:55.000000 stpipe-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-27 17:08:55.000000 stpipe-0.4.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-03-27 17:08:55.000000 stpipe-0.4.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-27 17:08:55.000000 stpipe-0.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-27 17:08:55.000000 stpipe-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-27 17:08:55.000000 stpipe-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:08:55.000000 stpipe-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-27 17:09:05.705471 stpipe-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-27 17:08:55.000000 stpipe-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.701471 stpipe-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 17:08:55.000000 stpipe-0.4.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.701471 stpipe-0.4.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 17:08:55.000000 stpipe-0.4.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 17:08:55.000000 stpipe-0.4.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-27 17:08:55.000000 stpipe-0.4.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-27 17:08:55.000000 stpipe-0.4.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.701471 stpipe-0.4.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-03-27 17:08:55.000000 stpipe-0.4.6/scripts/strun
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 17:09:05.709471 stpipe-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-27 17:08:55.000000 stpipe-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.697471 stpipe-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.701471 stpipe-0.4.6/src/stpipe/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/cli/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/crds_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/extern/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/extern/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87652 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/extern/configobj/configobj.py
--rw-r--r--   0 runner    (1001) docker     (123)    46706 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/extern/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/format_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/resources/schemas/step_config-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/resources/schemas/step_config-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/resources/schemas/step_config_with_metadata-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    50998 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/subproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/tests/test_abstract_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-27 17:08:55.000000 stpipe-0.4.6/src/stpipe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/src/stpipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:09:05.000000 stpipe-0.4.6/src/stpipe.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:09:05.705471 stpipe-0.4.6/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/cli/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_format_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-03-27 17:08:55.000000 stpipe-0.4.6/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 17:08:55.000000 stpipe-0.4.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.874117 stpipe-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 13:21:00.000000 stpipe-0.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.862117 stpipe-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 13:21:00.000000 stpipe-0.5.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.862117 stpipe-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 13:21:00.000000 stpipe-0.5.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-19 13:21:00.000000 stpipe-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 13:21:00.000000 stpipe-0.5.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 13:21:00.000000 stpipe-0.5.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-19 13:21:00.000000 stpipe-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-19 13:21:00.000000 stpipe-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-19 13:21:00.000000 stpipe-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-19 13:21:00.000000 stpipe-0.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-19 13:21:00.000000 stpipe-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-19 13:21:00.000000 stpipe-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 13:21:00.000000 stpipe-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.000000 stpipe-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-19 13:21:11.874117 stpipe-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-19 13:21:00.000000 stpipe-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.866117 stpipe-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 13:21:00.000000 stpipe-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 13:21:00.000000 stpipe-0.5.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.866117 stpipe-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 13:21:00.000000 stpipe-0.5.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-19 13:21:00.000000 stpipe-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 13:21:00.000000 stpipe-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-19 13:21:00.000000 stpipe-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.866117 stpipe-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-19 13:21:00.000000 stpipe-0.5.0/scripts/strun
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:21:11.874117 stpipe-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-19 13:21:00.000000 stpipe-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.858117 stpipe-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.866117 stpipe-0.5.0/src/stpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/crds_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/extern/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/extern/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87613 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/extern/configobj/configobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46469 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/extern/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/format_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/resources/schemas/step_config-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/resources/schemas/step_config-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/resources/schemas/step_config_with_metadata-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    50842 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/subproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/tests/test_abstract_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-19 13:21:00.000000 stpipe-0.5.0/src/stpipe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.870117 stpipe-0.5.0/src/stpipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:21:11.000000 stpipe-0.5.0/src/stpipe.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.874117 stpipe-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:11.874117 stpipe-0.5.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/cli/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_format_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-04-19 13:21:00.000000 stpipe-0.5.0/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 13:21:00.000000 stpipe-0.5.0/tox.ini
```

### Comparing `stpipe-0.4.6/.github/workflows/ci.yml` & `stpipe-0.5.0/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,31 @@
       - '*'
   pull_request:
   schedule:
     # Weekly Monday 9AM build
     # * is a special character in YAML so you have to quote this string
     - cron: '0 9 * * 1'
 
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
-        - linux: check-security
         - linux: build-dist
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

### Comparing `stpipe-0.4.6/.github/workflows/publish-to-pypi.yml` & `stpipe-0.5.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/.gitignore` & `stpipe-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/.readthedocs.yaml` & `stpipe-0.5.0/.readthedocs.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 # .readthedocs.yaml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
+build:
+  os: "ubuntu-20.04"
+  tools:
+    python: "mambaforge-4.10"
+
+conda:
+  environment: docs/rtd_environment.yaml
+
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   builder: html
   configuration: docs/source/conf.py
   fail_on_warning: true
 
-# Optionally build your docs in additional formats such as PDF and ePub
-formats:
-  - htmlzip
-  - pdf
-
-# Optionally set the version of Python and requirements required to build your docs
+# Install regular dependencies.
+# Then, install special pinning for RTD.
 python:
-  version: 3.8
+  system_packages: false
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
+
+# Optionally build your docs in additional formats such as PDF and ePub
+formats:
+  - htmlzip
+  - pdf
```

### Comparing `stpipe-0.4.6/CHANGES.rst` & `stpipe-0.5.0/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+0.5.0 (2023-04-19)
+==================
+
+- Remove use of deprecated ``pytest-openfiles`` ``pytest`` plugin. This has been replaced by
+  catching ``ResourceWarning`` s. [#90]
+- Start using ``pre-commit`` to handle style checks. [#79]
+- Apply the ``isort`` and ``black`` code formatters and reduce the line length
+  maximum to 88 characters. [#80]
+- Add spell checking through the ``codespell`` tool. [#81]
+- Drop support for Python 3.8 [#93]
+- Remove ``stdatamodels`` dependency, as it is no longer used. [#91]
+- Add ``flynt`` string update checking tool. [#92]
+
 0.4.6 (2023-03-27)
 ==================
 
 - add ``importlib.metadata`` as a dependency and update loading of entry_points to drop
   usage of pkg_resources [#84]
 - update minimum python to 3.8 and ASDF version to 2.8 [#87]
 - replace legacy AsdfExtension with resource_mapping [#82]
```

### Comparing `stpipe-0.4.6/CODE_OF_CONDUCT.md` & `stpipe-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/CONTRIBUTING.md` & `stpipe-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/LICENSE` & `stpipe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/PKG-INFO` & `stpipe-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpipe
-Version: 0.4.6
+Version: 0.5.0
 Summary: Framework for calibration pipeline software
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -34,15 +34,15 @@
         
 Project-URL: repository, https://github.com/spacetelescope/stpipe
 Project-URL: tracker, https://github.com/spacetelescope/stpipe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # stpipe
```

### Comparing `stpipe-0.4.6/docs/Makefile` & `stpipe-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/docs/source/conf.py` & `stpipe-0.5.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import importlib
-import stsci_rtd_theme
 import sys
-import tomli
+
+import stsci_rtd_theme
+
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
+
 from datetime import datetime
 from pathlib import Path
 
 
 def setup(app):
     try:
         app.add_css_file("stsci.css")
@@ -18,21 +24,21 @@
 # Modules that automodapi will document need to be available
 # in the path:
 sys.path.insert(0, str(REPO_ROOT / "src" / "stpipe"))
 
 # Read the package's `pyproject.toml` so that we can use relevant
 # values here:
 with open(REPO_ROOT / "pyproject.toml", "rb") as configuration_file:
-    conf = tomli.load(configuration_file)
-setup_metadata = conf['project']
+    conf = tomllib.load(configuration_file)
+setup_metadata = conf["project"]
 
 project = setup_metadata["name"]
 primary_author = setup_metadata["authors"][0]
 author = f'{primary_author["name"]} <{primary_author["email"]}>'
-copyright = f'{datetime.now().year}, {author}'
+copyright = f"{datetime.now().year}, {author}"
 
 package = importlib.import_module(project)
 version = package.__version__.split("-", 1)[0]
 release = package.__version__
 
 extensions = [
     "sphinx_automodapi.automodapi",
@@ -41,15 +47,15 @@
 
 autosummary_generate = True
 numpydoc_show_class_members = False
 autoclass_content = "both"
 
 html_theme = "stsci_rtd_theme"
 html_theme_options = {
-    "collapse_navigation": True
+    "collapse_navigation": True,
 }
 html_theme_path = [stsci_rtd_theme.get_html_theme_path()]
 html_domain_indices = True
 html_sidebars = {"**": ["globaltoc.html", "relations.html", "searchbox.html"]}
 html_use_index = True
 
 # Enable nitpicky mode - which ensures that all references in the docs
```

### Comparing `stpipe-0.4.6/pyproject.toml` & `stpipe-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [project]
 name = 'stpipe'
 description = 'Framework for calibration pipeline software'
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
 ]
 dependencies = [
     'asdf>=2.13',
     'crds>=7.4.1.3',
     'astropy>=5.0.4',
-    'stdatamodels>=0.2.4',
     'importlib_metadata>=4.11.4',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 docs = [
     'numpydoc',
@@ -28,15 +27,14 @@
     'sphinx-rtd-theme',
     'stsci-rtd-theme',
     'tomli; python_version <"3.11"',
 ]
 test = [
     'pytest >=7.0.0',
     'pytest-doctestplus >=0.10.0',
-    'pytest-openfiles >=0.5.0',
 ]
 
 [project.urls]
 'repository' = 'https://github.com/spacetelescope/stpipe'
 'tracker' = 'https://github.com/spacetelescope/stpipe/issues'
 
 [project.entry-points]
@@ -63,32 +61,64 @@
 where = ['src']
 
 [tool.pytest.ini_options]
 minversion = 4.6
 doctest_plus = true
 doctest_rst = true
 text_file_format = 'rst'
-addopts = '--open-files'
+addopts = ''
 norecursedirs = [
     'src/stpipe/extern',
 ]
 testpaths = [
     'tests',
 ]
+filterwarnings = [
+    "error::ResourceWarning",
+]
 
 [tool.ruff]
 select = [
     'E402', # module level import not at top of file
     'E501', # line too long
     'E711', # comparison to None should be ‘if cond is None:’
     'E722', # do not use bare except, specify exception instead
     'F', # flakes
     'W', # whitespace / deprecation
 ]
-line-length = 130
+line-length = 88
 extend-exclude = [
     'docs',
     'src/stpipe/extern',
+    'scripts/strun',
 ]
 extend-ignore = [
     'W605', # invalid escape sequence
 ]
+
+[tool.isort]
+profile = "black"
+filter_files = true
+line_length = 88
+extend_skip_glob = ["src/stpipe/extern/*"]
+
+[tool.black]
+line-length = 88
+force-exclude = '''
+^/(
+  (
+      \.eggs
+    | \.git
+    | \.pytest_cache
+    | \.tox
+    | src/stpipe/extern
+  )/
+)
+'''
+
+[tool.flynt]
+exclude = ["src/stpipe/extern/*"]
+
+[tool.codespell]
+skip="*.pdf,*.fits,*.asdf,.tox,build,./tags,.git,docs/_build"
+# ignore-words-list="""
+# """
```

### Comparing `stpipe-0.4.6/scripts/strun` & `stpipe-0.5.0/scripts/strun`

 * *Files 19% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 
 import sys
 
 import stpipe
 from stpipe import Step
 from stpipe.exceptions import StpipeExitException
 
-
-if __name__ == '__main__':
-
-    if '--version' in sys.argv:
+if __name__ == "__main__":
+    if "--version" in sys.argv:
         sys.stdout.write(f"{stpipe.__version__}\n")
         sys.exit(0)
 
     try:
         step = Step.from_cmdline(sys.argv[1:])
     except StpipeExitException as e:
         sys.exit(e.exit_status)
     except Exception:
         import traceback
+
         traceback.print_exc()
         sys.exit(1)
```

### Comparing `stpipe-0.4.6/src/stpipe/cli/command.py` & `stpipe-0.5.0/src/stpipe/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class Command(abc.ABC):
     """
     Base class for stpipe CLI commands.  Every subclass should
     be added to the _COMMAND_CLASSES list in core.py.
     """
+
     @abc.abstractclassmethod
     def get_name(cls):
         """
         Get this command's name (the first argument to stpipe).
 
         Returns
         -------
```

### Comparing `stpipe-0.4.6/src/stpipe/cli/list.py` & `stpipe-0.5.0/src/stpipe/cli/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Implements the 'stpipe list' command, which lists available
 Step subclasses.
 """
-import sys
-
 import argparse
 import re
+import sys
 
-from .command import Command
 from .. import entry_points
+from .command import Command
 
 
 class ListCommand(Command):
     @classmethod
     def get_name(cls):
         return "list"
 
@@ -30,21 +29,36 @@
 
         parser = subparsers.add_parser(
             cls.get_name(),
             epilog=epilog,
             formatter_class=argparse.RawDescriptionHelpFormatter,
             description="list available classes",
             help="list available classes",
-    )
+        )
 
-        parser.add_argument("pattern", metavar="<pattern>", help="restrict classes to glob pattern (case-insensitive)", nargs="?")
+        parser.add_argument(
+            "pattern",
+            metavar="<pattern>",
+            help="restrict classes to glob pattern (case-insensitive)",
+            nargs="?",
+        )
 
         group = parser.add_mutually_exclusive_group()
-        group.add_argument("--pipelines-only", help="list only pipeline classes", action="store_true", default=False)
-        group.add_argument("--steps-only", help="list only step classes", action="store_true", default=False)
+        group.add_argument(
+            "--pipelines-only",
+            help="list only pipeline classes",
+            action="store_true",
+            default=False,
+        )
+        group.add_argument(
+            "--steps-only",
+            help="list only step classes",
+            action="store_true",
+            default=False,
+        )
 
     @classmethod
     def run(cls, args):
         steps = entry_points.get_steps()
 
         if args.steps_only:
             steps = [s for s in steps if not s.is_pipeline]
@@ -68,10 +82,12 @@
         return 0
 
 
 def _filter_pattern(pattern, steps):
     pattern = re.compile(re.escape(pattern.lower()).replace(r"\*", ".*"))
 
     return [
-        s for s in steps
-        if pattern.fullmatch(s.class_name.lower()) or (s.class_alias is not None and pattern.fullmatch(s.class_alias.lower()))
+        s
+        for s in steps
+        if pattern.fullmatch(s.class_name.lower())
+        or (s.class_alias is not None and pattern.fullmatch(s.class_alias.lower()))
     ]
```

### Comparing `stpipe-0.4.6/src/stpipe/cli/main.py` & `stpipe-0.5.0/src/stpipe/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Main function and argument parser for stpipe.
 """
 import argparse
 import sys
 import traceback
 
-from .list import ListCommand
 from ..exceptions import StpipeExitException
-
+from .list import ListCommand
 
 # New subclasses of Command must be imported
 # and appended to this list before they'll
 # become available in the CLI:
 _COMMAND_CLASSES = [
     ListCommand,
 ]
@@ -38,15 +37,17 @@
         _print_versions()
         return 0
 
     if args.command_name is None:
         parser.print_help()
         return 0
 
-    command_class = next(c for c in _COMMAND_CLASSES if c.get_name() == args.command_name)
+    command_class = next(
+        c for c in _COMMAND_CLASSES if c.get_name() == args.command_name
+    )
 
     return command_class.run(args)
 
 
 def main():
     """
     Main function for stpipe CLI.  Registered with the console_scripts
@@ -64,30 +65,39 @@
     except Exception:
         traceback.print_exc(file=sys.stderr)
         sys.exit(1)
 
 
 def _get_parser():
     parser = argparse.ArgumentParser("stpipe", description="stpipe CLI")
-    parser.add_argument("-v", "--version", help="print version information and exit", action="store_true")
+    parser.add_argument(
+        "-v",
+        "--version",
+        help="print version information and exit",
+        action="store_true",
+    )
 
     subparsers = parser.add_subparsers(dest="command_name", title="commands")
 
     for command_class in _COMMAND_CLASSES:
         command_class.add_subparser(subparsers)
 
     return parser
 
 
 def _print_versions():
     """
     Print stpipe version as well as versions of any packages
     that register an stpipe.steps entry point.
     """
-    from .. import entry_points
     import stpipe
 
-    packages = sorted({(s.package_name, s.package_version) for s in entry_points.get_steps()}, key=lambda tup: tup[0])
+    from .. import entry_points
+
+    packages = sorted(
+        {(s.package_name, s.package_version) for s in entry_points.get_steps()},
+        key=lambda tup: tup[0],
+    )
 
     print(f"stpipe: {stpipe.__version__}")
     for package_name, package_version in packages:
         print(f"{package_name}: {package_version}")
```

### Comparing `stpipe-0.4.6/src/stpipe/cmdline.py` & `stpipe-0.5.0/src/stpipe/cmdline.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,50 +2,57 @@
 Various utilities to handle running Steps from the commandline.
 """
 import io
 import os
 import os.path
 import textwrap
 
-from . import config_parser
-from . import log
-from . import utilities
-from .step import get_disable_crds_steppars, Step
+from . import config_parser, log, utilities
+from .step import Step, get_disable_crds_steppars
 
 built_in_configuration_parameters = [
-    'debug', 'logcfg', 'verbose'
-    ]
+    "debug",
+    "logcfg",
+    "verbose",
+]
+
 
 def _print_important_message(header, message, no_wrap=None):
-    print(u'-' * 70)
+    print("-" * 70)
     print(textwrap.fill(header))
-    print(textwrap.fill(
-        message, initial_indent='    ', subsequent_indent='    '))
+    print(
+        textwrap.fill(
+            message,
+            initial_indent="    ",
+            subsequent_indent="    ",
+        )
+    )
     if no_wrap:
         print(no_wrap)
-    print(u'-' * 70)
+    print("-" * 70)
 
 
 def _get_config_and_class(identifier):
     """
     Given a file path to a config file or Python module path, return a
     Step class and a configuration object.
     """
     if os.path.exists(identifier):
         config_file = identifier
         config = config_parser.load_config_file(config_file)
-        step_class, name = Step._parse_class_and_name(
-            config, config_file=config_file)
+        step_class, name = Step._parse_class_and_name(config, config_file=config_file)
     else:
         try:
-            step_class = utilities.import_class(utilities.resolve_step_class_alias(identifier), Step)
+            step_class = utilities.import_class(
+                utilities.resolve_step_class_alias(identifier), Step
+            )
         except (ImportError, AttributeError, TypeError):
             raise ValueError(
-                '{0!r} is not a path to a config file or a Python Step '
-                'class'.format(identifier))
+                f"{identifier!r} is not a path to a config file or a Python Step class"
+            )
         # Don't validate yet
         config = config_parser.config_from_dict({})
         name = None
         config_file = None
 
     return step_class, config, name, config_file
 
@@ -68,58 +75,70 @@
     import argparse
 
     # It doesn't translate the configspec types -- it instead
     # will accept any string.  However, the types of the arguments will
     # later be verified by configobj itself.
     parser = argparse.ArgumentParser(
         parents=[parent],
-        description=step_class.__doc__)
+        description=step_class.__doc__,
+    )
 
     def build_from_spec(subspec, parts=[]):
         for key, val in subspec.items():
             if isinstance(val, dict):
                 build_from_spec(val, parts + [key])
             else:
-                comment = subspec.inline_comments.get(key) or ''
-                comment = comment.lstrip('#').strip()
+                comment = subspec.inline_comments.get(key) or ""
+                comment = comment.lstrip("#").strip()
                 argument = "--" + ".".join(parts + [key])
                 if argument[2:] in built_in_configuration_parameters:
                     raise ValueError(
-                        "The Step's spec is trying to override a built-in "
-                        "parameter {0!r}".format(argument))
+                        "The Step's spec is trying to override a built-in parameter"
+                        f" {argument!r}"
+                    )
                 parser.add_argument(
                     "--" + ".".join(parts + [key]),
-                    type=str, help=comment, metavar='')
+                    type=str,
+                    help=comment,
+                    metavar="",
+                )
+
     build_from_spec(spec)
 
     parser.add_argument(
-        'args', nargs='*', help='arguments to pass to step')
+        "args",
+        nargs="*",
+        help="arguments to pass to step",
+    )
 
     return parser
 
 
 class FromCommandLine(str):
     """
     We need a way to distinguish between config values that come from
     a config file and those that come from the commandline.  For
     example, configfile paths must be resolved against the location of
     the config file.  Commandline paths must be resolved against the
     current working directory.  By setting all commandline overrides
     as instances of this class, we can later (in `config_parser.py`)
     use isinstance to see where the values came from.
     """
+
     pass
 
+
 def _override_config_from_args(config, args):
     """
     Overrides any configuration values in `config` with values from the
     parsed commandline arguments `args`.
     """
+
     def set_value(subconf, key, val):
-        root, sep, rest = key.partition('.')
+        root, sep, rest = key.partition(".")
         if rest:
             set_value(subconf.setdefault(root, {}), rest, val)
         else:
             val, comment = config._handle_value(val)
             if isinstance(val, str):
                 subconf[root] = FromCommandLine(val)
             else:
@@ -158,78 +177,93 @@
 
     positional: list of strings
         Positional parameters after arg parsing
 
     DOES NOT RUN THE STEP
     """
     import argparse
+
     parser1 = argparse.ArgumentParser(
         description="Run an stpipe Step or Pipeline",
-        add_help=False)
+        add_help=False,
+    )
     if cls is None:
         parser1.add_argument(
-            "cfg_file_or_class", type=str, nargs=1,
-            help="The configuration file or Python class to run")
+            "cfg_file_or_class",
+            type=str,
+            nargs=1,
+            help="The configuration file or Python class to run",
+        )
     else:
         parser1.add_argument(
-            "--config-file", type=str,
-            help="A configuration file to load parameters from")
+            "--config-file",
+            type=str,
+            help="A configuration file to load parameters from",
+        )
     parser1.add_argument(
-        "--logcfg", type=str,
-        help="The logging configuration file to load")
+        "--logcfg",
+        type=str,
+        help="The logging configuration file to load",
+    )
     parser1.add_argument(
-        "--verbose", "-v", action="store_true",
-        help="Turn on all logging messages")
+        "--verbose",
+        "-v",
+        action="store_true",
+        help="Turn on all logging messages",
+    )
     parser1.add_argument(
-        "--debug", action="store_true",
-        help="When an exception occurs, invoke the Python debugger, pdb")
+        "--debug",
+        action="store_true",
+        help="When an exception occurs, invoke the Python debugger, pdb",
+    )
     parser1.add_argument(
-        '--save-parameters', type=str,
-        help='Save step parameters to specified file.'
+        "--save-parameters",
+        type=str,
+        help="Save step parameters to specified file.",
     )
     parser1.add_argument(
-        '--disable-crds-steppars', action='store_true',
-        help='Disable retrieval of step parameter references files from CRDS'
+        "--disable-crds-steppars",
+        action="store_true",
+        help="Disable retrieval of step parameter references files from CRDS",
     )
     known, _ = parser1.parse_known_args(args)
 
     try:
         if cls is None:
-            step_class, config, name, config_file = \
-                _get_config_and_class(known.cfg_file_or_class[0])
+            step_class, config, name, config_file = _get_config_and_class(
+                known.cfg_file_or_class[0]
+            )
         else:
             config_file = known.config_file
             config = config_parser.load_config_file(config_file)
             step_class, name = Step._parse_class_and_name(
-                config, config_file=config_file)
+                config, config_file=config_file
+            )
             step_class = cls
 
         log_config = None
         if known.verbose:
             if known.logcfg is not None:
                 raise ValueError(
-                    "If --verbose is set, a logging configuration file may "
-                    "not be provided")
+                    "If --verbose is set, a logging configuration file may not be"
+                    " provided"
+                )
             log_config = io.BytesIO(log.MAX_CONFIGURATION)
         elif known.logcfg is not None:
             if not os.path.exists(known.logcfg):
-                raise IOError(
-                    "Logging config {0!r} not found".format(known.logcfg))
+                raise OSError(f"Logging config {known.logcfg!r} not found")
             log_config = known.logcfg
 
         if log_config is not None:
             try:
                 log.load_configuration(log_config)
             except Exception as e:
-                raise ValueError(
-                    "Error parsing logging config {0!r}:\n{1}".format(
-                        log_config, e))
+                raise ValueError(f"Error parsing logging config {log_config!r}:\n{e}")
     except Exception as e:
-        _print_important_message(
-            "ERROR PARSING CONFIGURATION:", str(e))
+        _print_important_message("ERROR PARSING CONFIGURATION:", str(e))
         parser1.print_help()
         raise
 
     debug_on_exception = known.debug
 
     # Determine whether CRDS should be queried for step parameters
     disable_crds_steppars = get_disable_crds_steppars(known.disable_crds_steppars)
@@ -254,55 +288,62 @@
     del args.debug
     del args.save_parameters
     del args.disable_crds_steppars
     positional = args.args
     del args.args
 
     # This updates config (a ConfigObj) with the values from the command line arguments
-    # Config is empty if class specified, otherwise contains values from config file specified
-    # on command line
+    # Config is empty if class specified, otherwise contains values from config file
+    # specified on command line
     _override_config_from_args(config, args)
 
     config = step_class.merge_config(config, config_file)
 
     if len(positional):
         input_file = positional[0]
         if args.input_dir:
-            input_file = args.input_dir + '/' + input_file
+            input_file = args.input_dir + "/" + input_file
 
         # Attempt to retrieve Step parameters from CRDS
         try:
-            parameter_cfg = step_class.get_config_from_reference(input_file, disable=disable_crds_steppars)
+            parameter_cfg = step_class.get_config_from_reference(
+                input_file, disable=disable_crds_steppars
+            )
         except (FileNotFoundError, OSError):
-            log.log.warning("Unable to open input file, cannot get parameters from CRDS")
+            log.log.warning(
+                "Unable to open input file, cannot get parameters from CRDS"
+            )
         else:
             if config:
                 config_parser.merge_config(parameter_cfg, config)
             config = parameter_cfg
     else:
         log.log.info("No input file specified, unable to retrieve parameters from CRDS")
 
     # This is where the step is instantiated
     try:
         step = step_class.from_config_section(
-            config, name=name, config_file=config_file)
+            config,
+            name=name,
+            config_file=config_file,
+        )
     except config_parser.ValidationError as e:
         # If the configobj validator failed, print usage information.
         _print_important_message("ERROR PARSING CONFIGURATION:", str(e))
         parser2.print_help()
         raise ValueError(str(e))
 
     # Define the primary input file.
     # Always have an output_file set on the outermost step
     if len(positional):
         step.set_primary_input(positional[0])
         step.save_results = True
 
-    log.log.info("Hostname: {0}".format(os.uname()[1]))
-    log.log.info("OS: {0}".format(os.uname()[0]))
+    log.log.info(f"Hostname: {os.uname()[1]}")
+    log.log.info(f"OS: {os.uname()[0]}")
 
     # Save the step configuration
     if known.save_parameters:
         step.export_config(known.save_parameters, include_metadata=True)
         log.log.info(f"Step/Pipeline parameters saved to '{known.save_parameters}'")
 
     return step, step_class, positional, debug_on_exception
@@ -327,31 +368,32 @@
         specifies a class, the return value will be as instance of
         that class.
 
         Any parameters found in the config file or on the commandline
         will be set as member variables on the returned `Step`
         instance.
     """
-    step, step_class, positional, debug_on_exception = \
-        just_the_step_from_cmdline(args, cls)
+    step, step_class, positional, debug_on_exception = just_the_step_from_cmdline(
+        args, cls
+    )
 
     try:
         profile_path = os.environ.pop("STPIPE_PROFILE", None)
         if profile_path:
             import cProfile
+
             cProfile.runctx("step.run(*positional)", globals(), locals(), profile_path)
         else:
             step.run(*positional)
     except Exception as e:
-        _print_important_message(
-            "ERROR RUNNING STEP {0!r}:".format(step_class.__name__), str(e)
-        )
+        _print_important_message(f"ERROR RUNNING STEP {step_class.__name__!r}:", str(e))
 
         if debug_on_exception:
             import pdb
+
             pdb.post_mortem()
         else:
             raise
 
     return step
```

### Comparing `stpipe-0.4.6/src/stpipe/config.py` & `stpipe-0.5.0/src/stpipe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Implementation of Step methods related to ASDF config files.  This module
 will eventually fully replace config_parser.py, but we'll need to maintain
 both until we replace configobj with traitlets.
 """
 from copy import deepcopy
 from datetime import datetime
 
-from .utilities import get_fully_qualified_class_name
-
 import asdf
 
+from .utilities import get_fully_qualified_class_name
 
 _CONFIG_SCHEMA_URI = "http://stsci.edu/schemas/stpipe/step_config-1.0.0"
 _LEGACY_CONFIG_SCHEMA_URI = "http://stsci.edu/schemas/stpipe/step_config-0.1.0"
 
 # The config schema validates that this substring is not present:
 _TEMPLATE_PLACEHOLDER = "<SPECIFY>"
 
@@ -43,14 +42,15 @@
     name : str
         Nickname
     parameters : dict
         Parameters indexed by parameter name.
     steps : list of StepConfig
         List of sub-step configs.
     """
+
     def __init__(self, class_name, name, parameters, steps):
         self._class_name = class_name
         self._name = name
         self._parameters = parameters
         self._steps = steps
 
     @property
@@ -70,18 +70,18 @@
         return self._steps
 
     def __eq__(self, other):
         if not isinstance(other, StepConfig):
             return False
 
         return (
-            self.class_name == other.class_name and
-            self.name == other.name and
-            self.parameters == other.parameters and
-            self.steps == other.steps
+            self.class_name == other.class_name
+            and self.name == other.name
+            and self.parameters == other.parameters
+            and self.steps == other.steps
         )
 
     def _to_tree(self):
         tree = {
             "class": self.class_name,
             "name": self.name,
             "parameters": self.parameters,
@@ -105,16 +105,21 @@
         -------
         asdf.AsdfFile
         """
         result = asdf.AsdfFile(self._to_tree())
 
         if include_metadata:
             meta = deepcopy(_META_TEMPLATE)
-            meta["date"] = meta["date"].replace(_TEMPLATE_PLACEHOLDER, datetime.utcnow().replace(microsecond=0).isoformat())
-            meta["description"] = meta["description"].replace(_TEMPLATE_PLACEHOLDER, self.class_name)
+            meta["date"] = meta["date"].replace(
+                _TEMPLATE_PLACEHOLDER,
+                datetime.utcnow().replace(microsecond=0).isoformat(),
+            )
+            meta["description"] = meta["description"].replace(
+                _TEMPLATE_PLACEHOLDER, self.class_name
+            )
             result["meta"] = meta
 
         _validate_asdf(result, _CONFIG_SCHEMA_URI)
 
         return result
 
     @classmethod
```

### Comparing `stpipe-0.4.6/src/stpipe/config_parser.py` & `stpipe-0.5.0/src/stpipe/config_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 """
 Our configuration files are ConfigObj/INI files.
 """
-from inspect import isclass
 import logging
 import os
 import os.path
 import textwrap
+from inspect import isclass
 
-from asdf import open as asdf_open
 from asdf import ValidationError as AsdfValidationError
-from stdatamodels import s3_utils
-
-from .extern.configobj.configobj import (
-    ConfigObj, Section, flatten_errors, get_extra_values)
-from .extern.configobj.validate import Validator, ValidateError, VdtTypeError
+from asdf import open as asdf_open
 
 from . import utilities
 from .config import StepConfig
 from .datamodel import AbstractDataModel
-
+from .extern.configobj.configobj import (
+    ConfigObj,
+    Section,
+    flatten_errors,
+    get_extra_values,
+)
+from .extern.configobj.validate import ValidateError, Validator, VdtTypeError
 
 # Configure logger
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class ValidationError(Exception):
     pass
 
 
 def _get_input_file_check(root_dir):
     from . import cmdline
 
-    root_dir = root_dir or ''
+    root_dir = root_dir or ""
 
     def _input_file_check(path):
         if not isinstance(path, cmdline.FromCommandLine):
             try:
                 path = str(path)
             except ValueError:
                 pass
 
             path = os.path.join(root_dir, path)
 
         path = os.path.abspath(path)
         if not os.path.exists(path):
-            raise ValidateError(
-                "Path {0!r} does not exist".format(path))
+            raise ValidateError(f"Path {path!r} does not exist")
 
         return path
 
     return _input_file_check
 
 
 def _get_output_file_check(root_dir):
     from . import cmdline
 
-    root_dir = root_dir or ''
+    root_dir = root_dir or ""
 
     def _output_file_check(path):
         if not isinstance(path, cmdline.FromCommandLine):
             try:
                 path = str(path)
             except ValueError:
                 pass
@@ -97,56 +97,40 @@
         raise VdtTypeError(value)
 
 
 def load_config_file(config_file):
     """
     Read the file `config_file` and return the parsed configuration.
     """
-    if s3_utils.is_s3_uri(config_file):
-        return _load_config_file_s3(config_file)
-    else:
-        return _load_config_file_filesystem(config_file)
-
-
-def _load_config_file_filesystem(config_file):
     if not os.path.isfile(config_file):
-        raise ValueError("Config file {0} not found.".format(config_file))
+        raise ValueError(f"Config file {config_file} not found.")
     try:
         with asdf_open(config_file) as asdf_file:
             return _config_obj_from_asdf(asdf_file)
     except (AsdfValidationError, ValueError):
-        logger.debug('Config file did not parse as ASDF. Trying as ConfigObj: %s', config_file)
+        logger.debug(
+            "Config file did not parse as ASDF. Trying as ConfigObj: %s", config_file
+        )
         return ConfigObj(config_file, raise_errors=True)
 
 
-def _load_config_file_s3(config_file):
-    if not s3_utils.object_exists(config_file):
-        raise ValueError("Config file {0} not found.".format(config_file))
-
-    content = s3_utils.get_object(config_file)
-    try:
-        with asdf_open(content) as asdf_file:
-            return _config_obj_from_asdf(asdf_file)
-    except (AsdfValidationError, ValueError):
-        logger.debug('Config file did not parse as ASDF. Trying as ConfigObj: %s', config_file)
-        content.seek(0)
-        return ConfigObj(content, raise_errors=True)
-
-
 def _config_obj_from_asdf(asdf_file):
     config = StepConfig.from_asdf(asdf_file)
     return _config_obj_from_step_config(config)
 
 
 def _config_obj_from_step_config(config):
     configobj = ConfigObj()
     merge_config(configobj, config.parameters)
     merge_config(configobj, {"class": config.class_name, "name": config.name})
     if len(config.steps) > 0:
-        merge_config(configobj, {"steps": { s.name: _config_obj_from_step_config(s) for s in config.steps }})
+        merge_config(
+            configobj,
+            {"steps": {s.name: _config_obj_from_step_config(s) for s in config.steps}},
+        )
     return configobj
 
 
 def get_merged_spec_file(cls, preserve_comments=False):
     """
     Creates a merged spec file for a Step class and all of its
     subclasses.
@@ -195,30 +179,34 @@
     spec_file: ConfigObj
         The resulting configuration object
     """
     # Don't use 'hasattr' here, because we don't want to inherit spec
     # from the base class.
     if not isclass(cls):
         cls = cls.__class__
-    if 'spec' in cls.__dict__:
+    if "spec" in cls.__dict__:
         spec = cls.spec.strip()
         spec_file = textwrap.dedent(spec)
-        spec_file = spec_file.split('\n')
+        spec_file = spec_file.split("\n")
         encoded = []
         for line in spec_file:
             if isinstance(line, str):
-                encoded.append(line.encode('utf8'))
+                encoded.append(line.encode("utf8"))
             else:
                 encoded.append(line)
         spec_file = encoded
     else:
         spec_file = utilities.find_spec_file(cls)
     if spec_file:
-        return ConfigObj(spec_file, _inspec=not preserve_comments,
-                         raise_errors=True, list_values=False)
+        return ConfigObj(
+            spec_file,
+            _inspec=not preserve_comments,
+            raise_errors=True,
+            list_values=False,
+        )
     return
 
 
 def merge_config(into, new):
     """
     Merges a configuration tree into another one.
 
@@ -243,15 +231,19 @@
         inline_comments = {}
         comments = {}
 
     for key, val in new.items():
         if isinstance(val, Section):
             if key not in into:
                 section = Section(
-                    into, into.depth + 1, into.main, name=key)
+                    into,
+                    into.depth + 1,
+                    into.main,
+                    name=key,
+                )
                 into[key] = section
             merge_config(into[key], val)
         elif key not in defaults:
             # The unrepr flag is configured to only allow dicts to be
             # treated as config sections.  This prevents other
             # Mappings (such as DataModel, used in reference overrides)
             # from being converted.
@@ -288,15 +280,17 @@
         validate(config, spec, root_dir=root_dir, allow_missing=allow_missing)
     else:
         config.walk(string_to_python_type)
 
     return config
 
 
-def validate(config, spec, section=None, validator=None, root_dir=None, allow_missing=False):
+def validate(
+    config, spec, section=None, validator=None, root_dir=None, allow_missing=False
+):
     """
     Parse config_file, in INI format, and do validation with the
     provided specfile.
 
     Parameters
     ----------
     config: ConfigObj
@@ -321,64 +315,62 @@
     """
     if spec is None:
         config.walk(string_to_python_type)
         return config
 
     if validator is None:
         validator = Validator()
-        validator.functions['input_file'] = _get_input_file_check(root_dir)
-        validator.functions['output_file'] = _get_output_file_check(root_dir)
-        validator.functions['is_datamodel'] = _is_datamodel
-        validator.functions['is_string_or_datamodel'] = _is_string_or_datamodel
+        validator.functions["input_file"] = _get_input_file_check(root_dir)
+        validator.functions["output_file"] = _get_output_file_check(root_dir)
+        validator.functions["is_datamodel"] = _is_datamodel
+        validator.functions["is_string_or_datamodel"] = _is_string_or_datamodel
 
     orig_configspec = config.main.configspec
     config.main.configspec = spec
 
     try:
         if config.main != config:
             section = config
         else:
             section = None
 
         errors = config.main.validate(
-            validator, preserve_errors=True,
-            section=section)
+            validator,
+            preserve_errors=True,
+            section=section,
+        )
 
         messages = []
         if errors is not True:
             for section_list, key, err in flatten_errors(config, errors):
                 if key is not None:
                     section_list.append(key)
                 else:
-                    section_list.append('[missing section]')
-                section_string = '/'.join(section_list)
+                    section_list.append("[missing section]")
+                section_string = "/".join(section_list)
                 if err == False:
                     if allow_missing:
                         config[key] = spec[key]
                         continue
                     else:
-                        err = 'missing'
+                        err = "missing"
 
-                messages.append(
-                    "Config parameter {0!r}: {1}".format(
-                        section_string, err))
+                messages.append(f"Config parameter {section_string!r}: {err}")
 
         extra_values = get_extra_values(config)
         if extra_values:
             sections, name = extra_values[0]
             if len(sections) == 0:
-                sections = 'root'
+                sections = "root"
             else:
-                sections = '/'.join(sections)
-            messages.append(
-                "Extra value {0!r} in {1}".format(
-                    name, sections))
+                sections = "/".join(sections)
+            messages.append(f"Extra value {name!r} in {sections}")
 
         if len(messages):
-            raise ValidationError('\n'.join(messages))
+            raise ValidationError("\n".join(messages))
     finally:
         config.main.configspec = orig_configspec
 
     return config
 
 
 def string_to_python_type(section, key):
@@ -395,17 +387,17 @@
     return
 
 
 def _parse(val):
     """
     Parse scalar strings into scalar python types.
     """
-    if val.lower() == 'true':
+    if val.lower() == "true":
         return True
-    elif val.lower() == 'false':
+    elif val.lower() == "false":
         return False
     try:
         return int(val)
     except ValueError:
         pass
     try:
         return float(val)
```

### Comparing `stpipe-0.4.6/src/stpipe/crds_client.py` & `stpipe-0.5.0/src/stpipe/crds_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 WARNING:  stpipe and crds have circular dependencies.  Do not use crds imports
 directly in modules other than this crds_client so that dependency order and
 general integration can be managed here.
 """
 import re
 
 import crds
-from crds.core import config, heavy_client, log
+from crds.core import config, crds_cache_locking, heavy_client, log
 from crds.core.exceptions import CrdsError
-from crds.core import crds_cache_locking
-from stdatamodels import s3_utils
-
 
 __all__ = [
     "check_reference_open",
     "CrdsError",
     "get_multiple_reference_paths",
     "get_override_name",
     "get_reference_file",
@@ -31,15 +28,15 @@
 def get_multiple_reference_paths(parameters, reference_file_types, observatory):
     """Aligns stpipe requirements with CRDS library top level interfaces.
 
     Parameters
     ----------
     parameters : dict
         Parameters used by CRDS to compute best references.  Can
-        be obtained from `~stdatamodels.DataModel.get_crds_parameters`.
+        be obtained from `DataModel.get_crds_parameters`.
 
     reference_file_types : list of str
         List of reference file types.
 
     observatory : str
         CRDS observatory code.
 
@@ -54,40 +51,41 @@
     log.set_log_time(True)
     refpaths = _get_refpaths(parameters, tuple(reference_file_types), observatory)
     return refpaths
 
 
 def _get_refpaths(data_dict, reference_file_types, observatory):
     """Tailor the CRDS core library getreferences() call to the stpipe code by
-    adding locking and truncating expected exceptions.   Also simplify 'NOT FOUND n/a' to
-    'N/A'.  Re-interpret empty reference_file_types as "no types" instead of core
+    adding locking and truncating expected exceptions.   Also simplify 'NOT FOUND n/a'
+    to 'N/A'.  Re-interpret empty reference_file_types as "no types" instead of core
     library default of "all types."
     """
-    if not reference_file_types:   # [] interpreted as *all types*.
+    if not reference_file_types:  # [] interpreted as *all types*.
         return {}
     with crds_cache_locking.get_cache_lock():
         bestrefs = crds.getreferences(
-            data_dict, reftypes=reference_file_types, observatory=observatory)
-    refpaths = {filetype: filepath if "N/A" not in filepath.upper() else "N/A"
-                for (filetype, filepath) in bestrefs.items()}
+            data_dict,
+            reftypes=reference_file_types,
+            observatory=observatory,
+        )
+    refpaths = {
+        filetype: filepath if "N/A" not in filepath.upper() else "N/A"
+        for (filetype, filepath) in bestrefs.items()
+    }
     return refpaths
 
 
 def check_reference_open(refpath):
     """Verify that `refpath` exists and is readable for the current user.
 
     Ignore reference path values of "N/A" or "" for checking.
     """
     if refpath != "N/A" and refpath.strip() != "":
-        if s3_utils.is_s3_uri(refpath):
-            if not s3_utils.object_exists(refpath):
-                raise RuntimeError("S3 object does not exist: " + refpath)
-        else:
-            with open(refpath, "rb"):
-                pass
+        with open(refpath, "rb"):
+            pass
     return refpath
 
 
 def get_reference_file(parameters, reference_file_type, observatory):
     """
     Gets a reference file from CRDS as a readable file-like object.
     The actual file may be optionally overridden.
@@ -109,16 +107,17 @@
     -------
     reference_filepath : string
         The path of the reference in the CRDS file cache.
 
 
     See also get_multiple_reference_paths().
     """
-    return get_multiple_reference_paths(
-        parameters, [reference_file_type], observatory)[reference_file_type]
+    return get_multiple_reference_paths(parameters, [reference_file_type], observatory)[
+        reference_file_type
+    ]
 
 
 def get_override_name(reference_file_type):
     """
     Returns the name of the override configuration parameter for the
     given reference file type.
 
@@ -129,19 +128,20 @@
 
     Returns
     -------
     config_parameter_name : string
         The configuration parameter name to use to override the given
         reference file type.
     """
-    if not re.match('^[_A-Za-z][_A-Za-z0-9]*$', reference_file_type):
+    if not re.match("^[_A-Za-z][_A-Za-z0-9]*$", reference_file_type):
         raise ValueError(
-            "{0!r} is not a valid reference file type name. "
-            "It must be an identifier".format(reference_file_type))
-    return "override_{0}".format(reference_file_type)
+            f"{reference_file_type!r} is not a valid reference file type name. It must"
+            " be an identifier"
+        )
+    return f"override_{reference_file_type}"
 
 
 def get_svn_version():
     """Return the CRDS s/w version used for determining best references."""
     return crds.__version__
 
 
@@ -167,15 +167,17 @@
     environment variable.  See https://jwst-crds.stsci.edu guide and top level
     page for more info on configuring CRDS.
 
     The default CRDS_PATH value is /grp/crds/cache, currently on the Central Store.
     """
     if not reference_uri.startswith("crds://"):
         raise CrdsError(
-            "CRDS reference URI's should start with 'crds://' but got", repr(reference_uri))
+            "CRDS reference URI's should start with 'crds://' but got",
+            repr(reference_uri),
+        )
     basename = config.pop_crds_uri(reference_uri)
     return crds.locate_file(basename, observatory)
 
 
 def get_context_used(observatory):
     """Return the context (.pmap) used for determining best references.
```

### Comparing `stpipe-0.4.6/src/stpipe/datamodel.py` & `stpipe-0.5.0/src/stpipe/datamodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-
 import abc
 
+
 class AbstractDataModel(abc.ABC):
     """
     This Abstract Base Class is intended to cover multiple implementations of
     data models so that each will be considered an appropriate subclass of this
     class without requiring that they inherit this class.
 
     Any datamodel class instance that desires to be considered an instance of
@@ -14,31 +14,32 @@
     this is still being considered), such instances must have a meta.filename
     attribute.
     """
 
     @classmethod
     def __subclasshook__(cls, C):
         """
-        Psuedo subclass check based on these attributes and methods
+        Pseudo subclass check based on these attributes and methods
         """
         if cls is AbstractDataModel:
             mro = C.__mro__
-            if (any([hasattr(CC, "crds_observatory") for CC in mro]) and
-                any([hasattr(CC, "get_crds_parameters") for CC in mro]) and
-                any([hasattr(CC, "save") for CC in mro])):
+            if (
+                any([hasattr(CC, "crds_observatory") for CC in mro])
+                and any([hasattr(CC, "get_crds_parameters") for CC in mro])
+                and any([hasattr(CC, "save") for CC in mro])
+            ):
                 return True
         return False
 
     @property
     @abc.abstractmethod
     def crds_observatory(self):
         """This should return a string identifying the observatory as CRDS expects it"""
         pass
 
-
     @abc.abstractmethod
     def get_crds_parameters(self):
         """
         This should return a dictionary of key/value pairs corresponding to the
         parkey values CRDS is using to match reference files. Typically it returns
         all metadata simple values.
         """
```

### Comparing `stpipe-0.4.6/src/stpipe/entry_points.py` & `stpipe-0.5.0/src/stpipe/entry_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from collections import namedtuple
 import warnings
+from collections import namedtuple
 
 from importlib_metadata import entry_points
 
-
 STEPS_GROUP = "stpipe.steps"
 
 
-StepInfo = namedtuple("StepInfo", ["class_name", "class_alias", "is_pipeline", "package_name", "package_version"])
+StepInfo = namedtuple(
+    "StepInfo",
+    ["class_name", "class_alias", "is_pipeline", "package_name", "package_version"],
+)
 
 
 def get_steps():
     """
     Get the list of steps registered with stpipe's entry point group.  Each entry
     point is expected to return a list of tuples, where the first tuple element
     is a fully-qualified Step subclass name, the second element is an optional
@@ -33,14 +35,14 @@
             elements = entry_point.load()()
 
             for element in elements:
                 package_steps.append(StepInfo(*element, package_name, package_version))
         except Exception as e:
             warnings.warn(
                 f"{STEPS_GROUP} plugin from package {package_name}=={package_version} "
-                f"failed to load:\n\n"
+                "failed to load:\n\n"
                 f"{e.__class__.__name__}: {e}"
             )
 
         steps.extend(package_steps)
 
     return steps
```

### Comparing `stpipe-0.4.6/src/stpipe/extern/configobj/configobj.py` & `stpipe-0.5.0/src/stpipe/extern/configobj/configobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     return p.getChildren()[1].getChildren()[0].getChildren()[1]
 
 
 class UnknownType(Exception):
     pass
 
 
-class Builder(object):
+class Builder:
 
     def build(self, o):
         if m is None:
             raise UnknownType(o.__class__.__name__)
         return m(o)
 
     def build_List(self, o):
@@ -241,15 +241,15 @@
     """
     The keyword or section specified already exists.
     """
 
 
 class ConfigspecError(ConfigObjError):
     """
-    An error occured whilst parsing a configspec.
+    An error occurred whilst parsing a configspec.
     """
 
 
 class InterpolationError(ConfigObjError):
     """Base class for the two interpolation errors."""
 
 
@@ -277,15 +277,15 @@
 
 
 class UnreprError(ConfigObjError):
     """An error parsing in unrepr mode."""
 
 
 
-class InterpolationEngine(object):
+class InterpolationEngine:
     """
     A helper class to help perform string interpolation.
 
     This class is an abstract base class; its descendants perform
     the actual work.
     """
 
@@ -722,15 +722,15 @@
     def iteritems(self):
         """D.iteritems() -> an iterator over the (key, value) items of D"""
         return iter(list(self.items()))
 
 
     def iterkeys(self):
         """D.iterkeys() -> an iterator over the keys of D"""
-        return iter((self.scalars + self.sections))
+        return iter(self.scalars + self.sections)
 
     __iter__ = iterkeys
 
 
     def itervalues(self):
         """D.itervalues() -> an iterator over the values of D"""
         return iter(list(self.values()))
@@ -739,15 +739,15 @@
     def __repr__(self):
         """x.__repr__() <==> repr(x)"""
         def _getval(key):
             try:
                 return self[key]
             except MissingInterpolationOption:
                 return dict.__getitem__(self, key)
-        return '{%s}' % ', '.join([('%s: %s' % (repr(key), repr(_getval(key))))
+        return '{%s}' % ', '.join([(f'{repr(key)}: {repr(_getval(key))}')
             for key in (self.scalars + self.sections)])
 
     __str__ = __repr__
     __str__.__doc__ = "x.__str__() <==> str(x)"
 
 
     # Extra methods - not in a normal dictionary
@@ -840,19 +840,19 @@
     def walk(self, function, raise_errors=True,
             call_on_sections=False, **keywargs):
         """
         Walk every member and call a function on the keyword and value.
 
         Return a dictionary of the return values
 
-        If the function raises an exception, raise the errror
+        If the function raises an exception, raise the error
         unless ``raise_errors=False``, in which case set the return value to
         ``False``.
 
-        Any unrecognised keyword arguments you pass to walk, will be pased on
+        Any unrecognised keyword arguments you pass to walk, will be passed on
         to the function you pass in.
 
         Note: if ``call_on_sections`` is ``True`` then - on encountering a
         subsection, *first* the function is called for the *whole* subsection,
         and then recurses into it's members. This means your function must be
         able to handle strings, dictionaries and lists. This allows you
         to change the key of subsections as well as for ordinary members. The
@@ -1231,15 +1231,15 @@
         if isinstance(infile, str):
             self.filename = infile
             if os.path.isfile(infile):
                 with open(infile, 'rb') as h:
                     content = h.readlines() or []
             elif self.file_error:
                 # raise an error if the file doesn't exist
-                raise IOError('Config file not found: "%s".' % self.filename)
+                raise OSError('Config file not found: "%s".' % self.filename)
             else:
                 # file doesn't already exist
                 if self.create_empty:
                     # this is a good test that the filename specified
                     # isn't impossible - like on a non-existent device
                     with open(infile, 'w') as h:
                         h.write('')
@@ -1357,16 +1357,16 @@
 
     def __repr__(self):
         def _getval(key):
             try:
                 return self[key]
             except MissingInterpolationOption:
                 return dict.__getitem__(self, key)
-        return ('%s({%s})' % (self.__class__.__name__,
-                ', '.join([('%s: %s' % (repr(key), repr(_getval(key))))
+        return ('{}({{{}}})'.format(self.__class__.__name__,
+                ', '.join([(f'{repr(key)}: {repr(_getval(key))}')
                 for key in (self.scalars + self.sections)])))
 
 
     def _handle_bom(self, infile):
         """
         Handle any BOM, and decode if necessary.
 
@@ -1522,15 +1522,15 @@
     # TODO: this may need to be modified
     def _str(self, value):
         """
         Used by ``stringify`` within validate, to turn non-string values
         into strings.
         """
         if not isinstance(value, str):
-            # intentially 'str' because it's just whatever the "normal"
+            # intentionally 'str' because it's just whatever the "normal"
             # string type is for the python version we're dealing with
             return str(value)
         else:
             return value
 
 
     def _parse(self, infile):
@@ -1616,15 +1616,15 @@
                 continue
             #
             # it's not a section marker,
             # so it should be a valid ``key = value`` line
             mat = self._keyword.match(line)
             if mat is None:
                 self._handle_error(
-                    'Invalid line ({0!r}) (matched as neither section nor keyword)'.format(line),
+                    f'Invalid line ({line!r}) (matched as neither section nor keyword)',
                     ParseError, infile, cur_index)
             else:
                 # is a keyword value
                 # value will include any inline comment
                 (indent, key, value) = mat.groups()
                 if indent and (self.indent_type is None):
                     self.indent_type = indent
@@ -1720,19 +1720,19 @@
 
 
     def _handle_error(self, text, ErrorClass, infile, cur_index):
         """
         Handle an error according to the error settings.
 
         Either raise the error or store it.
-        The error will have occured at ``cur_index``
+        The error will have occurred at ``cur_index``
         """
         line = infile[cur_index]
         cur_index += 1
-        message = '{0} at line {1}.'.format(text, cur_index)
+        message = f'{text} at line {cur_index}.'
         error = ErrorClass(message, cur_index, line)
         if self.raise_errors:
             # raise the error - parsing stops here
             raise error
         # store the error
         # reraise when parsing has finished
         self._errors.append(error)
@@ -1777,15 +1777,15 @@
                 return ','
             elif len(value) == 1:
                 return self._quote(value[0], multiline=False) + ','
             return ', '.join([self._quote(val, multiline=False)
                 for val in value])
         if not isinstance(value, str):
             if self.stringify:
-                # intentially 'str' because it's just whatever the "normal"
+                # intentionally 'str' because it's just whatever the "normal"
                 # string type is for the python version we're dealing with
                 value = str(value)
             else:
                 raise TypeError('Value "%s" is not a string.' % value)
 
         if not value:
             return '""'
@@ -1933,16 +1933,16 @@
                                        raise_errors=True,
                                        file_error=True,
                                        _inspec=True)
             except ConfigObjError as e:
                 # FIXME: Should these errors have a reference
                 #        to the already parsed ConfigObj ?
                 raise ConfigspecError('Parsing configspec failed: %s' % e)
-            except IOError as e:
-                raise IOError('Reading configspec failed: %s' % e)
+            except OSError as e:
+                raise OSError('Reading configspec failed: %s' % e)
 
         self.configspec = configspec
 
 
 
     def _set_configspec(self, section, copy):
         """
@@ -1975,24 +1975,24 @@
     def _write_line(self, indent_string, entry, this_entry, comment):
         """Write an individual line, for the write method"""
         # NOTE: the calls to self._quote here handles non-StringType values.
         if not self.unrepr:
             val = self._decode_element(self._quote(this_entry))
         else:
             val = repr(this_entry)
-        return '%s%s%s%s%s' % (indent_string,
+        return '{}{}{}{}{}'.format(indent_string,
                                self._decode_element(self._quote(entry, multiline=False)),
                                self._a_to_u(' = '),
                                val,
                                self._decode_element(comment))
 
 
     def _write_marker(self, indent_string, depth, entry, comment):
         """Write a section marker line"""
-        return '%s%s%s%s%s' % (indent_string,
+        return '{}{}{}{}{}'.format(indent_string,
                                self._a_to_u('[' * depth),
                                self._quote(self._decode_element(entry), multiline=False),
                                self._a_to_u(']' * depth),
                                self._decode_element(comment))
 
 
     def _handle_comment(self, comment):
@@ -2361,15 +2361,15 @@
 
         self.clear()
         self._initialise(current_options)
         self._load(filename, configspec)
 
 
 
-class SimpleVal(object):
+class SimpleVal:
     """
     A simple validator.
     Can be used to check that all members expected are present.
 
     To use it, provide a configspec with all your members in (the value given
     will be ignored). Pass an instance of ``SimpleVal`` to the ``validate``
     method of your ``ConfigObj``. ``validate`` will return ``True`` if all
```

### Comparing `stpipe-0.4.6/src/stpipe/extern/configobj/validate.py` & `stpipe-0.5.0/src/stpipe/extern/configobj/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,33 +159,27 @@
     'is_mixed_list',
     'is_option',
     '__docformat__',
 )
 
 import re
 import sys
-from pprint import pprint
-
-from stdatamodels import DataModel
 
 #TODO - #21 - six is part of the repo now, but we didn't switch over to it here
 # this could be replaced if six is used for compatibility, or there are no
 # more assertions about items being a string
-if sys.version_info < (3,):
-    string_type = basestring
-else:
-    string_type = str
-    # so tests that care about unicode on 2.x can specify unicode, and the same
-    # tests when run on 3.x won't complain about a undefined name "unicode"
-    # since all strings are unicode on 3.x we just want to pass it through
-    # unchanged
-    unicode = lambda x: x
-    # in python 3, all ints are equivalent to python 2 longs, and they'll
-    # never show "L" in the repr
-    long = int
+string_type = str
+# so tests that care about unicode on 2.x can specify unicode, and the same
+# tests when run on 3.x won't complain about a undefined name "unicode"
+# since all strings are unicode on 3.x we just want to pass it through
+# unchanged
+unicode = lambda x: x
+# in python 3, all ints are equivalent to python 2 longs, and they'll
+# never show "L" in the repr
+long = int
 
 _list_arg = re.compile(r'''
     (?:
         ([a-zA-Z_][a-zA-Z0-9_]*)\s*=\s*list\(
             (
                 (?:
                     \s*
@@ -293,15 +287,15 @@
 
     # import here to avoid it when ip_addr values are not used
     import socket, struct
 
     try:
         return struct.unpack('!L',
             socket.inet_aton(ip.strip()))[0]
-    except socket.error:
+    except OSError:
         raise ValueError('Not a good dotted-quad IP: %s' % ip)
     return
 
 
 def numToDottedQuad(num):
     """
     Convert int or long int to dotted quad string
@@ -346,15 +340,15 @@
 
     # no need to intercept here, 4294967295L is fine
     if num > long(4294967295) or num < 0:
         raise ValueError('Not a good numeric IP: %s' % num)
     try:
         return socket.inet_ntoa(
             struct.pack('!L', long(num)))
-    except (socket.error, struct.error, OverflowError):
+    except (OSError, struct.error, OverflowError):
         raise ValueError('Not a good numeric IP: %s' % num)
 
 
 class ValidateError(Exception):
     """
     This error indicates that the check failed.
     It can be the base class for more specific errors.
@@ -377,104 +371,104 @@
 
     def __init__(self, value):
         """
         >>> raise VdtUnknownCheckError('yoda')
         Traceback (most recent call last):
         VdtUnknownCheckError: the check "yoda" is unknown.
         """
-        ValidateError.__init__(self, 'the check "%s" is unknown.' % (value,))
+        ValidateError.__init__(self, f'the check "{value}" is unknown.')
 
 
 class VdtParamError(SyntaxError):
     """An incorrect parameter was passed"""
 
     def __init__(self, name, value):
         """
         >>> raise VdtParamError('yoda', 'jedi')
         Traceback (most recent call last):
         VdtParamError: passed an incorrect value "jedi" for parameter "yoda".
         """
-        SyntaxError.__init__(self, 'passed an incorrect value "%s" for parameter "%s".' % (value, name))
+        SyntaxError.__init__(self, f'passed an incorrect value "{value}" for parameter "{name}".')
 
 
 class VdtTypeError(ValidateError):
     """The value supplied was of the wrong type"""
 
     def __init__(self, value):
         """
         >>> raise VdtTypeError('jedi')
         Traceback (most recent call last):
         VdtTypeError: the value "jedi" is of the wrong type.
         """
-        ValidateError.__init__(self, 'the value "%s" is of the wrong type.' % (value,))
+        ValidateError.__init__(self, f'the value "{value}" is of the wrong type.')
 
 
 class VdtValueError(ValidateError):
     """The value supplied was of the correct type, but was not an allowed value."""
 
     def __init__(self, value):
         """
         >>> raise VdtValueError('jedi')
         Traceback (most recent call last):
         VdtValueError: the value "jedi" is unacceptable.
         """
-        ValidateError.__init__(self, 'the value "%s" is unacceptable.' % (value,))
+        ValidateError.__init__(self, f'the value "{value}" is unacceptable.')
 
 
 class VdtValueTooSmallError(VdtValueError):
     """The value supplied was of the correct type, but was too small."""
 
     def __init__(self, value):
         """
         >>> raise VdtValueTooSmallError('0')
         Traceback (most recent call last):
         VdtValueTooSmallError: the value "0" is too small.
         """
-        ValidateError.__init__(self, 'the value "%s" is too small.' % (value,))
+        ValidateError.__init__(self, f'the value "{value}" is too small.')
 
 
 class VdtValueTooBigError(VdtValueError):
     """The value supplied was of the correct type, but was too big."""
 
     def __init__(self, value):
         """
         >>> raise VdtValueTooBigError('1')
         Traceback (most recent call last):
         VdtValueTooBigError: the value "1" is too big.
         """
-        ValidateError.__init__(self, 'the value "%s" is too big.' % (value,))
+        ValidateError.__init__(self, f'the value "{value}" is too big.')
 
 
 class VdtValueTooShortError(VdtValueError):
     """The value supplied was of the correct type, but was too short."""
 
     def __init__(self, value):
         """
         >>> raise VdtValueTooShortError('jed')
         Traceback (most recent call last):
         VdtValueTooShortError: the value "jed" is too short.
         """
         ValidateError.__init__(
             self,
-            'the value "%s" is too short.' % (value,))
+            f'the value "{value}" is too short.')
 
 
 class VdtValueTooLongError(VdtValueError):
     """The value supplied was of the correct type, but was too long."""
 
     def __init__(self, value):
         """
         >>> raise VdtValueTooLongError('jedie')
         Traceback (most recent call last):
         VdtValueTooLongError: the value "jedie" is too long.
         """
-        ValidateError.__init__(self, 'the value "%s" is too long.' % (value,))
+        ValidateError.__init__(self, f'the value "{value}" is too long.')
 
 
-class Validator(object):
+class Validator:
     """
     Validator is an object that allows you to register a set of 'checks'.
     These checks take input and test that it conforms to the check.
 
     This can also involve converting the value from a string into
     the correct datatype.
 
@@ -640,15 +634,15 @@
             fun_name, fun_args, fun_kwargs, default = self._cache[check]
             # We call list and dict below to work with *copies* of the data
             # rather than the original (which are mutable of course)
             fun_args = list(fun_args)
             fun_kwargs = dict(fun_kwargs)
         else:
             fun_name, fun_args, fun_kwargs, default = self._parse_check(check)
-            fun_kwargs = dict([(str(key), value) for (key, value) in list(fun_kwargs.items())])
+            fun_kwargs = {str(key): value for (key, value) in list(fun_kwargs.items())}
             self._cache[check] = fun_name, list(fun_args), dict(fun_kwargs), default
         return fun_name, fun_args, fun_kwargs, default
 
 
     def _check_value(self, value, fun_name, fun_args, fun_kwargs):
         try:
             fun = self.functions[fun_name]
@@ -941,15 +935,15 @@
     """
     if isinstance(value, string_type):
         try:
             return bool_dict[value.lower()]
         except KeyError:
             raise VdtTypeError(value)
     # we do an equality test rather than an identity test
-    # this ensures Python 2.2 compatibilty
+    # this ensures Python 2.2 compatibility
     # and allows 0 and 1 to represent True and False
     if value == False:
         return False
     elif value == True:
         return True
     else:
         raise VdtTypeError(value)
@@ -1228,15 +1222,15 @@
 def force_list(value, min=None, max=None):
     """
     Check that a value is a list, coercing strings into
     a list with one member. Useful where users forget the
     trailing comma that turns a single value into a list.
 
     You can optionally specify the minimum and maximum number of members.
-    A minumum of greater than one will fail if the user only supplies a
+    A minimum of greater than one will fail if the user only supplies a
     string.
 
     >>> vtor.check('force_list', ())
     []
     >>> vtor.check('force_list', [])
     []
     >>> vtor.check('force_list', 'hello')
@@ -1465,8 +1459,8 @@
     globs.update({
         'vtor': Validator(),
     })
 
     failures, tests = doctest.testmod(
         m, globs=globs,
         optionflags=doctest.IGNORE_EXCEPTION_DETAIL | doctest.ELLIPSIS)
-    assert not failures, '{} failures out of {} tests'.format(failures, tests)
+    assert not failures, f'{failures} failures out of {tests} tests'
```

### Comparing `stpipe-0.4.6/src/stpipe/format_template.py` & `stpipe-0.5.0/src/stpipe/format_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """FormatTemplate
 
 Format template string allowing partial formatting.
 """
 from collections import defaultdict
 from string import Formatter
 
-__all__ = ['FormatTemplate']
+__all__ = ["FormatTemplate"]
 
 
 # Define conversion based on format type
 CONVERSION = {
-    '%': float,
-    'b': int,
-    'c': int,
-    'd': int,
-    'e': float,
-    'E': float,
-    'f': float,
-    'F': float,
-    'g': float,
-    'G': float,
-    'n': int,
-    'o': int,
-    's': str,
-    'x': int,
-    'X': int,
+    "%": float,
+    "b": int,
+    "c": int,
+    "d": int,
+    "e": float,
+    "E": float,
+    "f": float,
+    "F": float,
+    "g": float,
+    "G": float,
+    "n": int,
+    "o": int,
+    "s": str,
+    "x": int,
+    "X": int,
 }
 
 
 class FormatTemplate(Formatter):
     """Format a template
 
     Parameters
     ----------
     template : str
         A Python format string
 
     separator : string
-        Separater to use for values which have no
+        Separator to use for values which have no
         matching replacement strings
 
     key_formats : dict or None
         A dict of key-specific formatting where the value will
         be pre-formatted before being passed to the final format
         string. Each format will be tried until success.
 
@@ -99,34 +99,35 @@
 
     Setup preformatting
     >>> key_formats = {'value': ['pre_{:s}_format']}
     >>> fmt_preformat = FormatTemplate(key_formats=key_formats)
     >>> fmt_preformat(template, name='fred', value='great')
     'name="fred" value="pre_great_format"'
     """
-    def __init__(self, separator='_', key_formats=None, remove_unused=False):
+
+    def __init__(self, separator="_", key_formats=None, remove_unused=False):
         """Inialize class
 
         Parameters
         ----------
         separator : str
             For key/value pairs given that do not have a
-            replacement field, the values are appened to
+            replacement field, the values are appended to
             the string using this separator.
 
         key_formats : {key: format(, ...)}
             dict of formats to pre-format the related values
             before insertion into the template.
         """
-        super(FormatTemplate, self).__init__()
+        super().__init__()
         self.separator = separator
         self.remove_unused = remove_unused
         self._used_keys = []
 
-        self.key_formats = defaultdict(lambda: ['{:s}'])
+        self.key_formats = defaultdict(lambda: ["{:s}"])
         if key_formats:
             self.key_formats.update(key_formats)
 
     def format(self, format_string, **kwargs):
         """Perform the formatting
 
         Parameters
@@ -145,38 +146,37 @@
         self._used_keys = []
 
         # Preformat the values
         formatted_kwargs = {}
         for key, value in kwargs.items():
             if value is not None:
                 for key_format in self.key_formats[key]:
-
                     # Get the formatting type character. Indices are:
                     #  0: The first replacement field. There should only be one.
                     #  2: Get the format spec.
                     #  -1: Get the last character representing the type.
                     format_type = list(self.parse(key_format))[0][2][-1]
 
                     try:
                         value = key_format.format(CONVERSION[format_type](value))
                     except ValueError:
                         pass
                     else:
                         break
                 else:
                     raise RuntimeError(
-                        'No suitable formatting for {key}: {value} found. Given formatting options:'
-                        '\n\t{formats}'.format(
-                            key=key, value=value, formats=self.key_formats[key]
+                        "No suitable formatting for {key}: {value} found. Given"
+                        " formatting options:\n\t{formats}".format(
+                            key=key,
+                            value=value,
+                            formats=self.key_formats[key],
                         )
                     )
             formatted_kwargs[key] = value
-        result = super(FormatTemplate, self).format(
-            format_string, **formatted_kwargs
-        )
+        result = super().format(format_string, **formatted_kwargs)
 
         # Get any unused arguments and simply do the appending
         unused_keys = set(formatted_kwargs).difference(self._used_keys)
         unused_values = [
             formatted_kwargs[unused]
             for unused in unused_keys
             if formatted_kwargs[unused] is not None
@@ -207,16 +207,16 @@
         Returns
         -------
         obj
             The value from the kwargs.
             If not found, the string '{key}' is returned.
         """
         if self.remove_unused:
-            default = ''
+            default = ""
         else:
-            default = '{' + key + '}'
+            default = "{" + key + "}"
         value = kwargs.get(key, default)
         self._used_keys.append(key)
         if value is None:
-            value = ''
+            value = ""
 
         return value
```

### Comparing `stpipe-0.4.6/src/stpipe/hooks.py` & `stpipe-0.5.0/src/stpipe/hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """
 Pre- and post-hooks
 """
 import types
 
-from .step import Step
 from . import utilities
+from .step import Step
+
 
 def hook_from_string(step, type, num, command):
-    name = '{0}_hook{1:d}'.format(type, num)
+    name = f"{type}_hook{num:d}"
 
     step_class = None
     try:
-        step_class = utilities.import_class(
-            command, Step, step.config_file)
+        step_class = utilities.import_class(command, Step, step.config_file)
     except Exception:
         pass
 
     if step_class is not None:
-        return step_class(
-            name, parent=step, config_file=step.config_file)
+        return step_class(name, parent=step, config_file=step.config_file)
 
     step_func = None
     try:
         step_func = utilities.import_class(
-            command, types.FunctionType, step.config_file)
+            command, types.FunctionType, step.config_file
+        )
     except Exception:
         pass
 
     if step_func is not None:
         from . import function_wrapper
+
         return function_wrapper.FunctionWrapper(
-            step_func, parent=step, config_file=step.config_file)
+            step_func, parent=step, config_file=step.config_file
+        )
 
     from .subproc import SystemCall
 
     return SystemCall(name, parent=step, command=command)
 
 
 def get_hook_objects(step, type, hooks):
-    return [hook_from_string(step, type, i, hook)
-            for i, hook in enumerate(hooks)]
+    return [hook_from_string(step, type, i, hook) for i, hook in enumerate(hooks)]
```

### Comparing `stpipe-0.4.6/src/stpipe/log.py` & `stpipe-0.5.0/src/stpipe/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Logging setup etc.
 """
-from contextlib import contextmanager
 import fnmatch
 import io
 import logging
 import os
 import sys
 import threading
-
-from .extern.configobj.configobj import ConfigObj
-from .extern.configobj import validate
+from contextlib import contextmanager
 
 from . import config_parser
+from .extern.configobj import validate
+from .extern.configobj.configobj import ConfigObj
 
-STPIPE_ROOT_LOGGER = 'stpipe'
-DEFAULT_FORMAT = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+STPIPE_ROOT_LOGGER = "stpipe"
+DEFAULT_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
 DEFAULT_CONFIGURATION = b"""
 [*]
 handler = stderr
 level = INFO
 """
 
 MAX_CONFIGURATION = b"""
@@ -28,106 +27,116 @@
 level = DEBUG
 """
 
 
 ###########################################################################
 # LOGS AS EXCEPTIONS
 
+
 class LoggedException(Exception):
     """
     This is an exception used when a log record is converted into an
     exception.
 
     Use its `record` member to get the original `logging.LogRecord`.
     """
+
     def __init__(self, record):
         self.record = record
         Exception.__init__(self, record.getMessage())
 
 
 class BreakHandler(logging.Handler):
     """
     A handler that turns logs of a certain severity or higher into
     exceptions.
     """
+
     _from_config = True
 
     def emit(self, record):
         raise LoggedException(record)
 
 
 #########################################################################
 # LOGGING CONFIGURATION
 
 # A dictionary mapping patterns to
 log_config = {}
 
 
-class LogConfig():
+class LogConfig:
     """
     Stores a single logging configuration.
 
     Parameters
     ----------
     name : str
         The `fnmatch` pattern used to match the logging class
 
     handler, level, break_level, format : str
         See LogConfig.spec for a description of these values.
     """
-    def __init__(self, name, handler=None, level=logging.NOTSET,
-                 break_level=logging.NOTSET, format=None):
-        if name in ('', '.', 'root'):
-            name = '*'
+
+    def __init__(
+        self,
+        name,
+        handler=None,
+        level=logging.NOTSET,
+        break_level=logging.NOTSET,
+        format=None,
+    ):
+        if name in ("", ".", "root"):
+            name = "*"
         self.name = name
         self.handler = handler
         if not isinstance(self.handler, list):
-            if self.handler.strip() == '':
+            if self.handler.strip() == "":
                 self.handler = []
             else:
-                self.handler = [x.strip() for x in self.handler.split(',')]
+                self.handler = [x.strip() for x in self.handler.split(",")]
         self.level = level
         self.break_level = break_level
         if format is None:
             format = DEFAULT_FORMAT
         self.format = format
 
     def match(self, log_name):
         """
         Returns `True` if `log_name` matches the pattern of this
         configuration.
         """
         if log_name.startswith(STPIPE_ROOT_LOGGER):
-            log_name = log_name[len(STPIPE_ROOT_LOGGER) + 1:]
+            log_name = log_name[len(STPIPE_ROOT_LOGGER) + 1 :]
             if fnmatch.fnmatchcase(log_name, self.name):
                 return True
         return False
 
     def get_handler(self, handler_str):
         """
         Given a handler string, returns a `logging.Handler` object.
         """
         if handler_str.startswith("file:"):
-            return logging.FileHandler(handler_str[5:], 'w', 'utf-8', True)
+            return logging.FileHandler(handler_str[5:], "w", "utf-8", True)
         elif handler_str.startswith("append:"):
-            return logging.FileHandler(handler_str[7:], 'a', 'utf-8', True)
-        elif handler_str == 'stdout':
+            return logging.FileHandler(handler_str[7:], "a", "utf-8", True)
+        elif handler_str == "stdout":
             return logging.StreamHandler(sys.stdout)
-        elif handler_str == 'stderr':
+        elif handler_str == "stderr":
             return logging.StreamHandler(sys.stderr)
         else:
-            raise ValueError("Can't parse handler {0!r}".format(handler_str))
+            raise ValueError(f"Can't parse handler {handler_str!r}")
 
     def apply(self, log):
         """
         Applies the configuration to the given `logging.Logger`
         object.
         """
         for handler in log.handlers[:]:
-            if hasattr(handler, '_from_config'):
+            if hasattr(handler, "_from_config"):
                 log.handlers.remove(handler)
 
         # Set a handler
         for handler_str in self.handler:
             handler = self.get_handler(handler_str)
             handler._from_config = True
             handler.setLevel(self.level)
@@ -138,16 +147,17 @@
 
         # Set the break level
         if self.break_level != logging.NOTSET:
             log.addHandler(BreakHandler(self.break_level))
 
         formatter = logging.Formatter(self.format)
         for handler in log.handlers:
-            if (isinstance(handler, logging.Handler) and
-                hasattr(handler, '_from_config')):
+            if isinstance(handler, logging.Handler) and hasattr(
+                handler, "_from_config"
+            ):
                 handler.setFormatter(formatter)
 
     def match_and_apply(self, log):
         """
         If the given `logging.Logger` object matches the pattern of
         this configuration, it applies the configuration to it.
         """
@@ -160,29 +170,30 @@
     Loads a logging configuration file.  The format of this file is
     defined in LogConfig.spec.
 
     Parameters
     ----------
     config_file : str or readable file-like object
     """
+
     def _level_check(value):
         try:
             value = int(value)
         except ValueError:
             pass
         try:
             value = logging._checkLevel(value)
         except ValueError:
             raise validate.VdtTypeError(value)
         return value
 
     spec = config_parser.load_spec_file(LogConfig)
     config = ConfigObj(config_file, raise_errors=True, interpolation=False)
     val = validate.Validator()
-    val.functions['level'] = _level_check
+    val.functions["level"] = _level_check
     config_parser.validate(config, spec, validator=val)
 
     log_config.clear()
 
     for key, val in config.items():
         log_config[key] = LogConfig(key, **val)
 
@@ -195,19 +206,15 @@
 def getLogger(name=None):
     log = logging.getLogger(name)
 
     return log
 
 
 def _find_logging_config_file():
-    files = [
-        "stpipe-log.cfg",
-        "~/.stpipe-log.cfg",
-        "/etc/stpipe-log.cfg"
-        ]
+    files = ["stpipe-log.cfg", "~/.stpipe-log.cfg", "/etc/stpipe-log.cfg"]
 
     for file in files:
         file = os.path.expanduser(file)
         if os.path.exists(file):
             return os.path.abspath(file)
 
     buffer = io.BytesIO(DEFAULT_CONFIGURATION)
@@ -218,47 +225,48 @@
 # LOGGING DELEGATION
 
 
 class DelegationHandler(logging.Handler):
     """
     A handler that delegates messages along to the currently active
     `Step` logger.  It only delegates messages that come from outside
-    of the `stpipe` heirarchy, in order to prevent infinite recursion.
+    of the `stpipe` hierarchy, in order to prevent infinite recursion.
 
     Since we could be multi-threaded and each thread may be running a
     different thread, we need to manage a dictionary mapping the
     current thread to the Step's logger on that thread.
     """
+
     def __init__(self, *args, **kwargs):
         self._logs = {}
         logging.Handler.__init__(self, *args, **kwargs)
 
     def emit(self, record):
         log = self.log
-        if (log is not None and
-            not record.name.startswith(STPIPE_ROOT_LOGGER)):
+        if log is not None and not record.name.startswith(STPIPE_ROOT_LOGGER):
             record.name = log.name
             log.handle(record)
 
     @property
     def log(self):
         return self._logs.get(threading.current_thread(), None)
 
     @log.setter
     def log(self, log):
-        assert (log is None or
-                (isinstance(log, logging.Logger) and
-                 log.name.startswith(STPIPE_ROOT_LOGGER)))
+        assert log is None or (
+            isinstance(log, logging.Logger) and log.name.startswith(STPIPE_ROOT_LOGGER)
+        )
         self._logs[threading.current_thread()] = log
 
 
 class RecordingHandler(logging.Handler):
     """
     A handler that simply accumulates LogRecord instances.
     """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._log_records = []
 
     @property
     def log_records(self):
         return self._log_records
```

### Comparing `stpipe-0.4.6/src/stpipe/pipeline.py` & `stpipe-0.5.0/src/stpipe/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Pipeline
 """
 from collections.abc import Sequence
 from os.path import dirname, join
-from .extern.configobj.configobj import Section, ConfigObj
-
-from . import config_parser
-from . import crds_client
-from . import log
-from .step import get_disable_crds_steppars, Step
 
+from . import config_parser, crds_client, log
+from .extern.configobj.configobj import ConfigObj, Section
+from .step import Step, get_disable_crds_steppars
 
 # For classmethods, the logger to use is the
 # delegator, since the pipeline has not yet been instantiated.
 logger = log.delegator.log
 
+
 class Pipeline(Step):
     """
     A Pipeline is a way of combining a number of steps together.
     """
 
     # Configuration
     spec = """
@@ -34,40 +32,54 @@
         Step.__init__(self, *args, **kwargs)
 
         # Configure all of the steps
         for key, val in self.step_defs.items():
             cfg = self.steps.get(key)
             if cfg is not None:
                 new_step = val.from_config_section(
-                    cfg, parent=self, name=key,
-                    config_file=self.config_file)
+                    cfg,
+                    parent=self,
+                    name=key,
+                    config_file=self.config_file,
+                )
             else:
                 new_step = val(
-                    key, parent=self, config_file=self.config_file,
-                    **kwargs.get(key, {}))
+                    key,
+                    parent=self,
+                    config_file=self.config_file,
+                    **kwargs.get(key, {}),
+                )
 
             setattr(self, key, new_step)
 
     @property
     def reference_file_types(self):
         """Collect the list of all reftypes for child Steps that are not skipped.
         Overridden reftypes are included but handled normally later by the
         Pipeline version of the get_ref_override() method defined below.
         """
-        return [reftype for step in self._unskipped_steps
-                for reftype in step.reference_file_types]
+        return [
+            reftype
+            for step in self._unskipped_steps
+            for reftype in step.reference_file_types
+        ]
 
     @property
     def _unskipped_steps(self):
         """Return a list of the unskipped Step objects launched by `self`.
 
         Steps are also excluded if `Step.prefetch_references` is False.
         """
-        return [getattr(self, name) for name in self.step_defs
-                if (not getattr(self, name).skip and getattr(self, name).prefetch_references)]
+        return [
+            getattr(self, name)
+            for name in self.step_defs
+            if (
+                not getattr(self, name).skip and getattr(self, name).prefetch_references
+            )
+        ]
 
     def get_ref_override(self, reference_file_type):
         """Return any override for `reference_file_type` for any of the steps in
         Pipeline `self`.  OVERRIDES Step.
 
         Returns
         -------
@@ -78,53 +90,53 @@
             override = step.get_ref_override(reference_file_type)
             if override is not None:
                 return override
         return None
 
     @classmethod
     def merge_config(cls, config, config_file):
-        steps = config.get('steps', {})
+        steps = config.get("steps", {})
 
         # Configure all of the steps
         for key in cls.step_defs:
             cfg = steps.get(key)
             if cfg is not None:
                 # If a config_file is specified, load those values and
                 # then override them with our values.
-                if cfg.get('config_file'):
+                if cfg.get("config_file"):
                     cfg2 = config_parser.load_config_file(
-                        join(dirname(config_file or ''), cfg.get('config_file')))
-                    del cfg['config_file']
+                        join(dirname(config_file or ""), cfg.get("config_file"))
+                    )
+                    del cfg["config_file"]
                     config_parser.merge_config(cfg2, cfg)
                     steps[key] = cfg2
         return config
 
     @classmethod
     def load_spec_file(cls, preserve_comments=False):
         spec = config_parser.get_merged_spec_file(
-            cls, preserve_comments=preserve_comments)
+            cls, preserve_comments=preserve_comments
+        )
 
-        spec['steps'] = Section(spec, spec.depth + 1, spec.main, name="steps")
-        steps = spec['steps']
+        spec["steps"] = Section(spec, spec.depth + 1, spec.main, name="steps")
+        steps = spec["steps"]
         for key, val in cls.step_defs.items():
             if not issubclass(val, Step):
-                raise TypeError(
-                    "Entry {0!r} in step_defs is not a Step subclass"
-                    .format(key))
+                raise TypeError(f"Entry {key!r} in step_defs is not a Step subclass")
             stepspec = val.load_spec_file(preserve_comments=preserve_comments)
             steps[key] = Section(steps, steps.depth + 1, steps.main, name=key)
 
             config_parser.merge_config(steps[key], stepspec)
 
             # Also add a key that can be used to specify an external
             # config_file
-            step = spec['steps'][key]
-            step['config_file'] = 'string(default=None)'
-            step['name'] = "string(default='')"
-            step['class'] = "string(default='')"
+            step = spec["steps"][key]
+            step["config_file"] = "string(default=None)"
+            step["name"] = "string(default='')"
+            step["class"] = "string(default='')"
 
         return spec
 
     @classmethod
     def get_config_from_reference(cls, dataset, disable=None, crds_observatory=None):
         """Retrieve step parameters from reference database
 
@@ -149,54 +161,59 @@
         -------
         step_parameters : configobj
             The parameters as retrieved from CRDS. If there is an issue, log as such
             and return an empty config obj.
         """
         reftype = cls.get_config_reftype()
         refcfg = ConfigObj()
-        refcfg['steps'] = Section(refcfg, refcfg.depth + 1, refcfg.main, name="steps")
+        refcfg["steps"] = Section(refcfg, refcfg.depth + 1, refcfg.main, name="steps")
 
         # Check if retrieval should be attempted.
         if disable is None:
             disable = get_disable_crds_steppars()
         if disable:
-            logger.debug(f'{reftype.upper()}: CRDS parameter reference retrieval disabled.')
+            logger.debug(
+                f"{reftype.upper()}: CRDS parameter reference retrieval disabled."
+            )
             return refcfg
 
-
-        logger.debug('Retrieving all substep parameters from CRDS')
+        logger.debug("Retrieving all substep parameters from CRDS")
         #
         # Iterate over the steps in the pipeline
         with cls._datamodels_open(dataset, asn_n_members=1) as model:
             if isinstance(model, Sequence):
                 crds_parameters = model._models[0].get_crds_parameters()
                 crds_observatory = model.crds_observatory
             else:
                 crds_parameters = model.get_crds_parameters()
                 crds_observatory = model.crds_observatory
 
         for cal_step in cls.step_defs.keys():
             cal_step_class = cls.step_defs[cal_step]
-            refcfg['steps'][cal_step] = cal_step_class.get_config_from_reference(crds_parameters,
-                                                                                 crds_observatory=crds_observatory)
+            refcfg["steps"][cal_step] = cal_step_class.get_config_from_reference(
+                crds_parameters,
+                crds_observatory=crds_observatory,
+            )
         #
         # Now merge any config parameters from the step cfg file
-        logger.debug(f'Retrieving pipeline {reftype.upper()} parameters from CRDS')
+        logger.debug(f"Retrieving pipeline {reftype.upper()} parameters from CRDS")
         try:
-            ref_file = crds_client.get_reference_file(crds_parameters,
-                                                      reftype,
-                                                      crds_observatory)
+            ref_file = crds_client.get_reference_file(
+                crds_parameters,
+                reftype,
+                crds_observatory,
+            )
         except (AttributeError, crds_client.CrdsError):
-            logger.debug(f'{reftype.upper()}: No parameters found')
+            logger.debug(f"{reftype.upper()}: No parameters found")
         else:
-            if ref_file != 'N/A':
-                logger.info(f'{reftype.upper()} parameters found: {ref_file}')
+            if ref_file != "N/A":
+                logger.info(f"{reftype.upper()} parameters found: {ref_file}")
                 refcfg = cls.merge_pipeline_config(refcfg, ref_file)
             else:
-                logger.debug(f'No {reftype.upper()} reference files found.')
+                logger.debug(f"No {reftype.upper()} reference files found.")
 
         return refcfg
 
     @classmethod
     def merge_pipeline_config(cls, refcfg, ref_file):
         """
         Merge the config parameters from a pipeline config reference file into the
@@ -239,21 +256,20 @@
         input_file:  filename, model container, or model
 
         Returns
         -------
         None
         """
         try:
-            with self.open_model(input_file, asn_n_members=1,
-                                asn_exptypes=["science"]) as model:
+            with self.open_model(
+                input_file, asn_n_members=1, asn_exptypes=["science"]
+            ) as model:
                 self._precache_references_opened(model)
-        except (ValueError, TypeError, IOError):
-            self.log.info(
-                'First argument {0} does not appear to be a '
-                'model'.format(input_file))
+        except (ValueError, TypeError, OSError):
+            self.log.info(f"First argument {input_file} does not appear to be a model")
 
     def _precache_references_opened(self, model_or_container):
         """Pre-fetches references for `model_or_container`.
 
         Handles recursive pre-fetches for any models inside a container,
         or just a single model.
 
@@ -282,25 +298,31 @@
             Only a `DataModel` instance is allowed.
             Cannot be a filename, Sequence, etc.
         """
         ovr_refs = {
             reftype: self.get_ref_override(reftype)
             for reftype in self.reference_file_types
             if self.get_ref_override(reftype) is not None
-            }
+        }
 
         fetch_types = sorted(set(self.reference_file_types) - set(ovr_refs.keys()))
 
-        self.log.info("Prefetching reference files for dataset: " + repr(model.meta.filename) +
-                      " reftypes = " + repr(fetch_types))
-        crds_refs = crds_client.get_multiple_reference_paths(model.get_crds_parameters(), fetch_types, model.crds_observatory)
+        self.log.info(
+            "Prefetching reference files for dataset: "
+            + repr(model.meta.filename)
+            + " reftypes = "
+            + repr(fetch_types)
+        )
+        crds_refs = crds_client.get_multiple_reference_paths(
+            model.get_crds_parameters(), fetch_types, model.crds_observatory
+        )
 
         ref_path_map = dict(list(crds_refs.items()) + list(ovr_refs.items()))
 
-        for (reftype, refpath) in sorted(ref_path_map.items()):
+        for reftype, refpath in sorted(ref_path_map.items()):
             how = "Override" if reftype in ovr_refs else "Prefetch"
             self.log.info(f"{how} for {reftype.upper()} reference file is '{refpath}'.")
             crds_client.check_reference_open(refpath)
 
     def get_pars(self, full_spec=True):
         """Retrieve the configuration parameters of a pipeline
 
@@ -316,11 +338,13 @@
 
         Returns
         -------
         pars : dict
             Keys are the parameters and values are the values.
         """
         pars = super().get_pars(full_spec=full_spec)
-        pars['steps'] = {}
+        pars["steps"] = {}
         for step_name, step_class in self.step_defs.items():
-            pars['steps'][step_name] = getattr(self, step_name).get_pars(full_spec=full_spec)
+            pars["steps"][step_name] = getattr(self, step_name).get_pars(
+                full_spec=full_spec
+            )
         return pars
```

### Comparing `stpipe-0.4.6/src/stpipe/resources/schemas/step_config-0.1.0.yaml` & `stpipe-0.5.0/src/stpipe/resources/schemas/step_config-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/src/stpipe/resources/schemas/step_config-1.0.0.yaml` & `stpipe-0.5.0/src/stpipe/resources/schemas/step_config-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/src/stpipe/resources/schemas/step_config_with_metadata-1.0.0.yaml` & `stpipe-0.5.0/src/stpipe/resources/schemas/step_config_with_metadata-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/src/stpipe/step.py` & `stpipe-0.5.0/src/stpipe/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 """
 Step
 """
+import gc
+import os
+import sys
 from collections.abc import Sequence
 from contextlib import contextmanager
 from functools import partial
-import gc
-import os
 from os.path import (
     abspath,
     basename,
     dirname,
     expanduser,
     expandvars,
     isfile,
     join,
     split,
     splitext,
 )
-import sys
 
 try:
     from astropy.io import fits
+
     DISCOURAGED_TYPES = (fits.HDUList,)
 except ImportError:
     DISCOURAGED_TYPES = None
 
-from . import config
-from . import config_parser
-from . import crds_client
-from . import log
-from . import utilities
+from . import config, config_parser, crds_client, log, utilities
 from .datamodel import AbstractDataModel
 from .format_template import FormatTemplate
 
 
 class Step:
     """
     Step
     """
+
     spec = """
     pre_hooks          = string_list(default=list())
     post_hooks         = string_list(default=list())
     output_file        = output_file(default=None)   # File to save output to.
     output_dir         = string(default=None)        # Directory path for output files
     output_ext         = string()                    # Default type of output
     output_use_model   = boolean(default=False)      # When saving use `DataModel.meta.filename`
     output_use_index   = boolean(default=True)       # Append index.
     save_results       = boolean(default=False)      # Force save results
     skip               = boolean(default=False)      # Skip this step
     suffix             = string(default=None)        # Default suffix for output files
     search_output_file = boolean(default=True)       # Use outputfile define in parent step
     input_dir          = string(default=None)        # Input directory
-    """
+    """  # noqa: E501
     # Nickname used to refer to this class in lieu of the fully-qualified class
     # name.  Must be globally unique!
     class_alias = None
 
     # String defining the format of the output name, which defines how
     # **components are inserted into the output file name. If None, use the
     # default formatting, which is to append Step.suffix to the name. If False,
@@ -90,22 +88,23 @@
     @classmethod
     def merge_config(cls, config, config_file):
         return config
 
     @classmethod
     def load_spec_file(cls, preserve_comments=False):
         spec = config_parser.get_merged_spec_file(
-            cls, preserve_comments=preserve_comments)
+            cls, preserve_comments=preserve_comments
+        )
         # Add arguments for all of the expected reference files
         for reference_file_type in cls.reference_file_types:
             override_name = crds_client.get_override_name(reference_file_type)
-            spec[override_name] = 'is_string_or_datamodel(default=None)'
-            spec.inline_comments[override_name] = (
-                '# Override the {0} reference file'.format(
-                    reference_file_type))
+            spec[override_name] = "is_string_or_datamodel(default=None)"
+            spec.inline_comments[
+                override_name
+            ] = f"# Override the {reference_file_type} reference file"
         return spec
 
     @classmethod
     def print_configspec(cls):
         specfile = cls.load_spec_file(preserve_comments=True)
         specfile.write(sys.stdout.buffer)
 
@@ -142,22 +141,30 @@
 
             Any parameters found in the config file will be set
             as member variables on the returned `Step` instance.
         """
         config = config_parser.load_config_file(config_file)
 
         # If a file object was passed in, pass the file name along
-        if hasattr(config_file, 'name'):
+        if hasattr(config_file, "name"):
             config_file = config_file.name
 
         step_class, name = cls._parse_class_and_name(
-            config, parent, name, config_file)
+            config,
+            parent,
+            name,
+            config_file,
+        )
 
         return step_class.from_config_section(
-            config, parent=parent, name=name, config_file=config_file)
+            config,
+            parent=parent,
+            name=name,
+            config_file=config_file,
+        )
 
     @staticmethod
     def from_cmdline(args):
         """
         Create a step from a configuration file.
 
         Parameters
@@ -176,43 +183,50 @@
         """
         from . import cmdline
 
         return cmdline.step_from_cmdline(args)
 
     @classmethod
     def _parse_class_and_name(cls, config, parent=None, name=None, config_file=None):
-        if 'class' in config:
-            step_class = utilities.import_class(utilities.resolve_step_class_alias(config['class']),
-                                                config_file=config_file)
+        if "class" in config:
+            step_class = utilities.import_class(
+                utilities.resolve_step_class_alias(config["class"]),
+                config_file=config_file,
+            )
             if not issubclass(step_class, cls):
                 raise TypeError(
-                    "Configuration file does not match the "
-                    "expected step class.  Expected {0}, "
-                    "got {1}".format(cls, step_class))
+                    "Configuration file does not match the expected step class. "
+                    f" Expected {cls}, got {step_class}"
+                )
         else:
             step_class = cls
 
         if not name:
-            name = config.get('name')
+            name = config.get("name")
             if not name:
                 if isinstance(config_file, str):
                     name = splitext(basename(config_file))[0]
                 else:
                     name = step_class.__name__
 
-        if 'name' in config:
-            del config['name']
-        if 'class' in config:
-            del config['class']
+        if "name" in config:
+            del config["name"]
+        if "class" in config:
+            del config["class"]
 
         return step_class, name
 
     @classmethod
-    def from_config_section(cls, config, parent=None, name=None,
-                            config_file=None):
+    def from_config_section(
+        cls,
+        config,
+        parent=None,
+        name=None,
+        config_file=None,
+    ):
         """
         Create a step from a configuration file fragment.
 
         Parameters
         ----------
         config : configobj.Section instance
             The config file fragment containing parameters for this
@@ -234,35 +248,34 @@
         Returns
         -------
         step : instance of cls
             Any parameters found in the config file fragment will be
             set as member variables on the returned `Step` instance.
         """
         if not name:
-            if config.get('name'):
-                name = config['name']
+            if config.get("name"):
+                name = config["name"]
             else:
                 name = cls.__name__
 
-        if 'name' in config:
-            del config['name']
-        if 'class' in config:
-            del config['class']
-        if 'config_file' in config:
-            del config['config_file']
+        if "name" in config:
+            del config["name"]
+        if "class" in config:
+            del config["class"]
+        if "config_file" in config:
+            del config["config_file"]
 
         spec = cls.load_spec_file()
         config = cls.merge_config(config, config_file)
-        config_parser.validate(
-            config, spec, root_dir=dirname(config_file or ''))
+        config_parser.validate(config, spec, root_dir=dirname(config_file or ""))
 
-        if 'config_file' in config:
-            del config['config_file']
-        if 'name' in config:
-            del config['name']
+        if "config_file" in config:
+            del config["config_file"]
+        if "name" in config:
+            del config["name"]
 
         # cmdline.FromCommandLine instances should not be passed to
         # steps. Instead, convert them back to strings.
         from . import cmdline
 
         kwargs = {}
         for k in config:
@@ -272,20 +285,27 @@
                 kwargs[k] = config[k]
 
         step = cls(
             name=name,
             parent=parent,
             config_file=config_file,
             _validate_kwds=False,
-            **kwargs)
+            **kwargs,
+        )
 
         return step
 
-    def __init__(self, name=None, parent=None, config_file=None,
-                 _validate_kwds=True, **kws):
+    def __init__(
+        self,
+        name=None,
+        parent=None,
+        config_file=None,
+        _validate_kwds=True,
+        **kws,
+    ):
         """
         Create a `Step` instance.
 
         Parameters
         ----------
         name : str, optional
             The name of the Step instance.  Used in logging messages
@@ -311,68 +331,66 @@
         self._log_records = []
         self._input_filename = None
         self._input_dir = None
         self._keywords = kws
         if _validate_kwds:
             spec = self.load_spec_file()
             kws = config_parser.config_from_dict(
-                kws, spec, root_dir=dirname(config_file or ''))
+                kws,
+                spec,
+                root_dir=dirname(config_file or ""),
+            )
 
         if name is None:
             name = self.__class__.__name__
         self.name = name
         if parent is None:
-            self.qualified_name = '.'.join([
-                log.STPIPE_ROOT_LOGGER, self.name])
+            self.qualified_name = ".".join([log.STPIPE_ROOT_LOGGER, self.name])
         else:
-            self.qualified_name = '.'.join([
-                parent.qualified_name, self.name])
+            self.qualified_name = ".".join([parent.qualified_name, self.name])
         self.parent = parent
 
         # Set the parameters as member variables
-        for (key, val) in kws.items():
+        for key, val in kws.items():
             setattr(self, key, val)
 
         # Create a new logger for this step
         self.log = log.getLogger(self.qualified_name)
 
         self.log.setLevel(log.logging.DEBUG)
 
         # Log the fact that we have been init-ed.
-        self.log.info('{0} instance created.'.format(self.__class__.__name__))
+        self.log.info(f"{self.__class__.__name__} instance created.")
 
         # Store the config file path so config filenames can be resolved
         # against it.
         self.config_file = config_file
 
         # Setup the hooks
         if len(self.pre_hooks) or len(self.post_hooks):
             from . import hooks
-            self._pre_hooks = hooks.get_hook_objects(
-                self, 'pre', self.pre_hooks
-            )
-            self._post_hooks = hooks.get_hook_objects(
-                self, 'post', self.post_hooks
-            )
+
+            self._pre_hooks = hooks.get_hook_objects(self, "pre", self.pre_hooks)
+            self._post_hooks = hooks.get_hook_objects(self, "post", self.post_hooks)
         else:
             self._pre_hooks = []
             self._post_hooks = []
 
     def _check_args(self, args, discouraged_types, msg):
         if discouraged_types is None:
             return
 
         if type(args) not in (list, tuple):
             args = [args]
 
         for i, arg in enumerate(args):
             if isinstance(arg, discouraged_types):
                 self.log.error(
-                    "{0} {1} object.  Use an instance of AbstractDataModel instead.".format(
-                        msg, i))
+                    f"{msg} {i} object.  Use an instance of AbstractDataModel instead."
+                )
 
     @property
     def log_records(self):
         """
         Retrieve logs from the most recent run of this step.
 
         Returns
@@ -394,21 +412,17 @@
 
             # Make generic log messages go to this step's logger
             orig_log = log.delegator.log
             log.delegator.log = self.log
 
             step_result = None
 
-            self.log.info(
-                'Step {0} running with args {1}.'.format(
-                    self.name, args))
+            self.log.info(f"Step {self.name} running with args {args}.")
 
-            self.log.info(
-                f'Step {self.name} parameters are: {self.get_pars()}'
-            )
+            self.log.info(f"Step {self.name} parameters are: {self.get_pars()}")
 
             if len(args):
                 self.set_primary_input(args[0])
 
             try:
                 # Default output file configuration
                 if self.output_file is not None:
@@ -428,39 +442,47 @@
 
                 # Warn if passing in objects that should be
                 # discouraged.
                 self._check_args(args, DISCOURAGED_TYPES, "Passed")
 
                 # Run the Step-specific code.
                 if self.skip:
-                    self.log.info('Step skipped.')
+                    self.log.info("Step skipped.")
                     if isinstance(args[0], AbstractDataModel):
                         if self.class_alias is not None:
                             if isinstance(args[0], Sequence):
                                 for model in args[0]:
                                     try:
-                                        model[f"meta.cal_step.{self.class_alias}"] = 'SKIPPED'
+                                        model[
+                                            f"meta.cal_step.{self.class_alias}"
+                                        ] = "SKIPPED"
                                     except AttributeError as e:
-                                        self.log.info(f"Could not record skip into DataModel header: {e}")
+                                        self.log.info(
+                                            "Could not record skip into DataModel"
+                                            f" header: {e}"
+                                        )
                             elif isinstance(args[0], AbstractDataModel):
                                 try:
-                                    args[0][f"meta.cal_step.{self.class_alias}"] = 'SKIPPED'
+                                    args[0][
+                                        f"meta.cal_step.{self.class_alias}"
+                                    ] = "SKIPPED"
                                 except AttributeError as e:
-                                    self.log.info(f"Could not record skip into DataModel header: {e}")
+                                    self.log.info(
+                                        "Could not record skip into DataModel"
+                                        f" header: {e}"
+                                    )
                     step_result = args[0]
                 else:
                     if self.prefetch_references:
                         self.prefetch(*args)
                     try:
                         step_result = self.process(*args)
                     except TypeError as e:
                         if "process() takes exactly" in str(e):
-                            raise TypeError(
-                                "Incorrect number of arguments to step"
-                            )
+                            raise TypeError("Incorrect number of arguments to step")
                         raise
 
                 # Warn if returning a discouraged object
                 self._check_args(step_result, DISCOURAGED_TYPES, "Returned")
 
                 # Run the post hooks
                 for post_hook in self._post_hooks:
@@ -480,46 +502,44 @@
                 for result in results:
                     self.finalize_result(result, self._reference_files_used)
 
                 self._reference_files_used = []
 
                 # Save the output file if one was specified
                 if not self.skip and self.save_results:
-
                     # Setup the save list.
                     if not isinstance(step_result, (list, tuple)):
                         results_to_save = [step_result]
                     else:
                         results_to_save = step_result
 
                     for idx, result in enumerate(results_to_save):
                         if len(results_to_save) <= 1:
                             idx = None
                         if isinstance(result, AbstractDataModel):
                             self.save_model(result, idx=idx, format=self.name_format)
-                        elif hasattr(result, 'save'):
+                        elif hasattr(result, "save"):
                             try:
-                                output_path = self.make_output_path(idx=idx, name_format=self.name_format)
+                                output_path = self.make_output_path(
+                                    idx=idx, name_format=self.name_format
+                                )
                             except AttributeError:
                                 self.log.warning(
-                                    '`save_results` has been requested,'
-                                    ' but cannot determine filename.'
+                                    "`save_results` has been requested, but cannot"
+                                    " determine filename."
                                 )
                                 self.log.warning(
-                                    'Specify an output file with `--output_file`'
-                                    ' or set `--save_results=false`'
+                                    "Specify an output file with `--output_file` or set"
+                                    " `--save_results=false`"
                                 )
                             else:
-                                self.log.info(
-                                    'Saving file {0}'.format(output_path)
-                                )
+                                self.log.info(f"Saving file {output_path}")
                                 result.save(output_path, overwrite=True)
 
-                self.log.info(
-                    'Step {0} done'.format(self.name))
+                self.log.info(f"Step {self.name} done")
             finally:
                 log.delegator.log = orig_log
 
         return step_result
 
     __call__ = run
 
@@ -557,35 +577,35 @@
         str
             Separator that delimited the original suffix.
         """
         return name, "_"
 
     def prefetch(self, *args):
         """Prefetch reference files,  nominally called when
-        self.prefetch_references is True.  Can be called explictly
+        self.prefetch_references is True.  Can be called explicitly
         when self.prefetch_refences is False.
         """
         # prefetch truly occurs at the Pipeline (or subclass) level.
         if len(args) and len(self.reference_file_types) and not self.skip:
             self._precache_references(args[0])
 
     def process(self, *args):
         """
         This is where real work happens. Every Step subclass has to
         override this method. The default behaviour is to raise a
         NotImplementedError exception.
         """
-        raise NotImplementedError('Steps have to override process().')
+        raise NotImplementedError("Steps have to override process().")
 
     def resolve_file_name(self, file_name):
         """
         Resolve a file name expressed relative to this Step's
         configuration file.
         """
-        return join(dirname(self.config_file or ''), file_name)
+        return join(dirname(self.config_file or ""), file_name)
 
     @classmethod
     def call(cls, *args, **kwargs):
         """
         Creates and runs a new instance of the class.
 
         Gets a config file from CRDS if one is available
@@ -610,58 +630,54 @@
         class.
         """
         filename = None
         if len(args) > 0:
             filename = args[0]
         config, config_file = cls.build_config(filename, **kwargs)
 
-        if 'class' in config:
-            del config['class']
+        if "class" in config:
+            del config["class"]
 
-        if 'logcfg' in config:
+        if "logcfg" in config:
             try:
-                log.load_configuration(config['logcfg'])
+                log.load_configuration(config["logcfg"])
             except Exception as e:
                 raise RuntimeError(
                     f"Error parsing logging config {config['logcfg']}"
                 ) from e
-            del config['logcfg']
+            del config["logcfg"]
 
-        name = config.get('name', None)
-        instance = cls.from_config_section(config,
-            name=name, config_file=config_file)
+        name = config.get("name", None)
+        instance = cls.from_config_section(config, name=name, config_file=config_file)
 
         return instance.run(*args)
 
     @property
     def input_dir(self):
-        return self.search_attr('_input_dir', '')
+        return self.search_attr("_input_dir", "")
 
     @input_dir.setter
     def input_dir(self, input_dir):
         self._input_dir = input_dir
 
     def default_output_file(self, input_file=None):
         """Create a default filename based on the input name"""
         output_file = input_file
         if output_file is None or not isinstance(output_file, str):
-                output_file = self.search_attr('_input_filename')
+            output_file = self.search_attr("_input_filename")
         if output_file is None:
-            output_file = 'step_{}{}'.format(
-                self.name,
-                self.output_ext
-            )
+            output_file = f"step_{self.name}{self.output_ext}"
         return output_file
 
     def default_suffix(self):
         """Return a default suffix based on the step"""
         return self.name.lower()
 
     def search_attr(self, attribute, default=None, parent_first=False):
-        """Return first non-None attribute in step heirarchy
+        """Return first non-None attribute in step hierarchy
 
         Parameters
         ----------
         attribute : str
             The attribute to retrieve
 
         default : obj
@@ -673,17 +689,15 @@
         Returns
         -------
         value : obj
             Attribute value or `default` if not found
         """
         if parent_first:
             try:
-                value = self.parent.search_attr(
-                    attribute, parent_first=parent_first
-                )
+                value = self.parent.search_attr(attribute, parent_first=parent_first)
             except AttributeError:
                 value = None
             if value is None:
                 value = getattr(self, attribute, default)
             return value
         else:
             value = getattr(self, attribute, None)
@@ -714,15 +728,15 @@
         override_filepath or None.
         """
         override_name = crds_client.get_override_name(reference_file_type)
         path = getattr(self, override_name, None)
         if isinstance(path, AbstractDataModel):
             return path
         else:
-            return abspath(path) if path and path != 'N/A' else path
+            return abspath(path) if path and path != "N/A" else path
 
     def get_reference_file(self, input_file, reference_file_type):
         """
         Get a reference file from CRDS.
 
         If the configuration file or commandline parameters override the
         reference file, it will be automatically used when calling this
@@ -743,41 +757,40 @@
         -------
         reference_file : path of reference file,  a string
         """
         override = self.get_ref_override(reference_file_type)
         if override is not None:
             if isinstance(override, AbstractDataModel):
                 self._reference_files_used.append(
-                    (reference_file_type, override.override_handle))
+                    (reference_file_type, override.override_handle)
+                )
                 return override
             elif override.strip() != "":
                 self._reference_files_used.append(
-                    (reference_file_type, basename(override)))
+                    (reference_file_type, basename(override))
+                )
                 reference_name = override
             else:
                 return ""
         else:
             with self.open_model(input_file) as model:
                 reference_name = crds_client.get_reference_file(
                     model.get_crds_parameters(),
                     reference_file_type,
                     model.crds_observatory,
                 )
             if reference_name != "N/A":
                 hdr_name = "crds://" + basename(reference_name)
             else:
                 hdr_name = "N/A"
-            self._reference_files_used.append(
-                (reference_file_type, hdr_name))
+            self._reference_files_used.append((reference_file_type, hdr_name))
         return crds_client.check_reference_open(reference_name)
 
     @classmethod
-    def get_config_from_reference(cls, dataset,
-                                  disable=None,
-                                  crds_observatory=None):
+    def get_config_from_reference(cls, dataset, disable=None, crds_observatory=None):
         """Retrieve step parameters from reference database
 
         Parameters
         ----------
         cls : stpipe.Step
             Either a class or instance of a class derived
             from `Step`.
@@ -814,48 +827,52 @@
             try:
                 model = cls._datamodels_open(dataset)
                 if isinstance(model, Sequence):
                     # Pull out first model in ModelContainer
                     model = model[0]
                 crds_parameters = model.get_crds_parameters()
                 crds_observatory = model.crds_observatory
-            except (IOError, TypeError, ValueError):
-                logger.warning('Input dataset is not an instance of AbstractDataModel.')
+            except (OSError, TypeError, ValueError):
+                logger.warning("Input dataset is not an instance of AbstractDataModel.")
                 disable = True
 
         # Check if retrieval should be attempted.
         if disable is None:
             disable = get_disable_crds_steppars()
         if disable:
-            logger.info(f'{reftype.upper()}: CRDS parameter reference retrieval disabled.')
+            logger.info(
+                f"{reftype.upper()}: CRDS parameter reference retrieval disabled."
+            )
             return config_parser.ConfigObj()
 
         # Retrieve step parameters from CRDS
-        logger.debug(f'Retrieving step {reftype.upper()} parameters from CRDS')
+        logger.debug(f"Retrieving step {reftype.upper()} parameters from CRDS")
         try:
-            ref_file = crds_client.get_reference_file(crds_parameters,
-                                                      reftype,
-                                                      crds_observatory)
+            ref_file = crds_client.get_reference_file(
+                crds_parameters,
+                reftype,
+                crds_observatory,
+            )
         except (AttributeError, crds_client.CrdsError):
-            logger.debug(f'{reftype.upper()}: No parameters found')
+            logger.debug(f"{reftype.upper()}: No parameters found")
             return config_parser.ConfigObj()
-        if ref_file != 'N/A':
-            logger.info(f'{reftype.upper()} parameters found: {ref_file}')
+        if ref_file != "N/A":
+            logger.info(f"{reftype.upper()} parameters found: {ref_file}")
             ref = config_parser.load_config_file(ref_file)
 
             ref_pars = {
-                par: value
-                for par, value in ref.items()
-                if par not in ['class', 'name']
+                par: value for par, value in ref.items() if par not in ["class", "name"]
             }
-            logger.debug(f'{reftype.upper()} parameters retrieved from CRDS: {ref_pars}')
+            logger.debug(
+                f"{reftype.upper()} parameters retrieved from CRDS: {ref_pars}"
+            )
 
             return ref
         else:
-            logger.debug(f'No {reftype.upper()} reference files found.')
+            logger.debug(f"No {reftype.upper()} reference files found.")
             return config_parser.ConfigObj()
 
     @classmethod
     def reference_uri_to_cache_path(cls, reference_uri, observatory):
         """Convert an abstract CRDS reference URI to an absolute file path in the CRDS
         cache.  Reference URI's are typically output to dataset headers to record the
         reference files used.
@@ -881,38 +898,37 @@
 
         exclusive : bool
             If True, only set if an input name is not already used
             by a parent Step. Otherwise, always set.
         """
         self._set_input_dir(obj, exclusive=exclusive)
 
-        err_message = (
-            'Cannot set master input file name from object'
-            ' {}'.format(obj)
-        )
-        parent_input_filename = self.search_attr('_input_filename')
+        err_message = f"Cannot set master input file name from object {obj}"
+        parent_input_filename = self.search_attr("_input_filename")
         if not exclusive or parent_input_filename is None:
             if isinstance(obj, str):
                 self._input_filename = obj
             elif isinstance(obj, AbstractDataModel):
                 try:
                     self._input_filename = obj.meta.filename
                 except AttributeError:
                     self.log.debug(err_message)
             else:
                 self.log.debug(err_message)
 
-    def save_model(self,
-                   model,
-                   suffix=None,
-                   idx=None,
-                   output_file=None,
-                   force=False,
-                   format=None,
-                   **components):
+    def save_model(
+        self,
+        model,
+        suffix=None,
+        idx=None,
+        output_file=None,
+        force=False,
+        format=None,
+        **components,
+    ):
         """
         Saves the given model using the step/pipeline's naming scheme
 
         Parameters
         ----------
         model : a instance of AbstractDataModel
             The model to save.
@@ -942,74 +958,69 @@
             Other components to add to the file name.
 
         Returns
         -------
         output_paths : [str[, ...]]
             List of output file paths the model(s) were saved in.
         """
-        if output_file is None or output_file == '':
+        if output_file is None or output_file == "":
             output_file = self.output_file
 
         # Check if saving is even specified.
-        if not force and \
-           not self.save_results and \
-           not output_file:
+        if not force and not self.save_results and not output_file:
             return
 
         if isinstance(model, Sequence):
             save_model_func = partial(
                 self.save_model,
                 suffix=suffix,
                 force=force,
                 format=format,
-                **components
+                **components,
             )
             output_path = model.save(
                 path=output_file,
-                save_model_func=save_model_func)
+                save_model_func=save_model_func,
+            )
         else:
-
             # Search for an output file name.
-            if (
-                    self.output_use_model or
-                    (output_file is None and not self.search_output_file)
+            if self.output_use_model or (
+                output_file is None and not self.search_output_file
             ):
                 output_file = model.meta.filename
                 idx = None
             output_path = model.save(
                 self.make_output_path(
                     basepath=output_file,
                     suffix=suffix,
                     idx=idx,
                     name_format=format,
-                    **components
+                    **components,
                 )
             )
-            self.log.info('Saved model in {}'.format(output_path))
+            self.log.info(f"Saved model in {output_path}")
 
         return output_path
 
     @property
     def make_output_path(self):
         """Return function that creates the output path"""
-        make_output_path = self.search_attr(
-            '_make_output_path'
-        )
+        make_output_path = self.search_attr("_make_output_path")
         return partial(make_output_path, self)
 
     @staticmethod
     def _make_output_path(
-            step,
-            basepath=None,
-            ext=None,
-            suffix=None,
-            name_format=None,
-            component_format='',
-            separator='_',
-            **components
+        step,
+        basepath=None,
+        ext=None,
+        suffix=None,
+        name_format=None,
+        component_format="",
+        separator="_",
+        **components,
     ):
         """Create the output path
 
         Parameters
         ----------
         step : Step
             The `Step` in question.
@@ -1050,69 +1061,69 @@
         -----
         The values found in the `components` dict are placed in the string
         where the "{components}" replacement field is specified. If there are
         more than one component, the components are separated by the `separator`
         string.
         """
         if basepath is None and step.search_output_file:
-            basepath = step.search_attr('output_file')
+            basepath = step.search_attr("output_file")
         if basepath is None:
             basepath = step.default_output_file()
 
         basename, basepath_ext = splitext(split(basepath)[1])
         if ext is None:
             ext = step.output_ext
         if ext is None and len(basepath_ext):
             ext = basepath_ext
-        if ext.startswith('.'):
+        if ext.startswith("."):
             ext = ext[1:]
 
         # Suffix check. An explicit check on `False` is necessary
         # because `None` is also allowed.
         suffix = _get_suffix(suffix, step=step)
         if suffix is not False:
-            default_name_format = '{basename}{components}{suffix_sep}{suffix}.{ext}'
+            default_name_format = "{basename}{components}{suffix_sep}{suffix}.{ext}"
             suffix_sep = None
             if suffix is not None:
                 basename, suffix_sep = step.remove_suffix(basename)
             if suffix_sep is None:
                 suffix_sep = separator
         else:
-            default_name_format = '{basename}{components}.{ext}'
+            default_name_format = "{basename}{components}.{ext}"
             suffix = None
             suffix_sep = None
 
         # Setup formatting
         if name_format is None:
             name_format = default_name_format
         elif not name_format:
-            name_format = basename + '.{ext}'
-            basename = ''
-            suffix_sep = ''
-            separator = ''
+            name_format = basename + ".{ext}"
+            basename = ""
+            suffix_sep = ""
+            separator = ""
         formatter = FormatTemplate(
             separator=separator,
-            remove_unused=True
+            remove_unused=True,
         )
 
         if len(components):
             component_str = formatter(component_format, **components)
         else:
-            component_str = ''
+            component_str = ""
 
         basename = formatter(
             name_format,
             basename=basename,
             suffix=suffix,
             suffix_sep=suffix_sep,
             ext=ext,
-            components=component_str
+            components=component_str,
         )
 
-        output_dir = step.search_attr('output_dir', default='')
+        output_dir = step.search_attr("output_dir", default="")
         output_dir = expandvars(expanduser(output_dir))
         full_output_path = join(output_dir, basename)
 
         return full_output_path
 
     def closeout(self, to_close=None, to_del=None):
         """Close out step processing
@@ -1134,21 +1145,18 @@
         if to_close is None:
             to_close = []
         if to_del is None:
             to_del = []
         to_del += to_close
         for item in to_close:
             try:
-                if hasattr(item, 'close'):
+                if hasattr(item, "close"):
                     item.close()
             except Exception as exception:
-                self.log.debug(
-                    'Could not close "{}"'
-                    'Reason:\n{}'.format(item, exception)
-                )
+                self.log.debug(f'Could not close "{item}"Reason:\n{exception}')
         for item in to_del:
             try:
                 del item
             except NameError as error:
                 self.log.debug("An error has occurred: %s", error)
         gc.collect()
 
@@ -1207,15 +1215,14 @@
         if isinstance(file_path, str):
             original_path, file_name = split(file_path)
             if not len(original_path):
                 full_path = join(self.input_dir, file_name)
 
         return full_path
 
-
     def _set_input_dir(self, input, exclusive=True):
         """Set the input directory
 
         If sufficient information is at hand, set a value
         for the attribute `input_dir`.
 
         Parameters
@@ -1224,15 +1231,15 @@
             Input to determine path from.
 
         exclusive : bool
             If True, only set if an input directory is not already
             defined by a parent Step. Otherwise, always set.
 
         """
-        if not exclusive or self.search_attr('_input_dir') is None:
+        if not exclusive or self.search_attr("_input_dir") is None:
             try:
                 if isfile(input):
                     self.input_dir = split(input)[0]
             except Exception:
                 # Not a file-checkable object. Ignore.
                 pass
 
@@ -1284,15 +1291,17 @@
         filename : str or pathlib.PurePath
             Path to config file.
 
         include_metadata : bool, optional
             Set to True to include metadata that is required
             for submission to CRDS.
         """
-        with config.export_config(self).to_asdf(include_metadata=include_metadata) as af:
+        with config.export_config(self).to_asdf(
+            include_metadata=include_metadata
+        ) as af:
             af.write_to(filename)
 
     def update_pars(self, parameters):
         """Update step parameters
 
         Only existing parameters are updated. Otherwise, new keys
         found in `parameters` are ignored.
@@ -1309,21 +1318,23 @@
         special in that it is a dict whose keys are the steps assigned
         directly as parameters to the current step. This is standard
         practice for `Pipeline`-based steps.
         """
         existing = self.get_pars().keys()
         for parameter, value in parameters.items():
             if parameter in existing:
-                if parameter != 'steps':
+                if parameter != "steps":
                     setattr(self, parameter, value)
                 else:
                     for step_name, step_parameters in value.items():
                         getattr(self, step_name).update_pars(step_parameters)
             else:
-                self.log.debug(f'Parameter {parameter} is not valid for step {self}. Ignoring.')
+                self.log.debug(
+                    f"Parameter {parameter} is not valid for step {self}. Ignoring."
+                )
 
     @classmethod
     def build_config(cls, input, **kwargs):
         """Build the ConfigObj to initialize a Step
 
         A Step config is built in the following order:
 
@@ -1348,61 +1359,62 @@
         log_cls = log.getLogger(logger_name)
         if input:
             config = cls.get_config_from_reference(input)
         else:
             log_cls.info("No filename given, cannot retrieve config from CRDS")
             config = config_parser.ConfigObj()
 
-        if 'config_file' in kwargs:
-            config_file = kwargs['config_file']
-            del kwargs['config_file']
+        if "config_file" in kwargs:
+            config_file = kwargs["config_file"]
+            del kwargs["config_file"]
             config_from_file = config_parser.load_config_file(config_file)
             config_parser.merge_config(config, config_from_file)
             config_dir = os.path.dirname(config_file)
         else:
             config_file = None
-            config_dir = ''
+            config_dir = ""
 
         config_kwargs = config_parser.ConfigObj()
 
         # load and merge configuration files for each step they are provided:
         steps = {}
-        if 'steps' in kwargs:
-            for step, pars in kwargs['steps'].items():
-                if 'config_file' in pars:
-                    step_config_file = os.path.join(config_dir, pars['config_file'])
+        if "steps" in kwargs:
+            for step, pars in kwargs["steps"].items():
+                if "config_file" in pars:
+                    step_config_file = os.path.join(config_dir, pars["config_file"])
                     cfgd = config_parser.load_config_file(step_config_file)
-                    if 'name' in cfgd:
-                        if cfgd['name'] != step:
+                    if "name" in cfgd:
+                        if cfgd["name"] != step:
                             raise ValueError(
                                 "Step name from configuration file "
                                 f"'{step_config_file}' does not match step "
                                 "name in the 'steps' argument."
                             )
-                        del cfgd['name']
-                    cfgd.pop('class', None)
+                        del cfgd["name"]
+                    cfgd.pop("class", None)
                     cfgd.update(pars)
                     steps[step] = cfgd
                 else:
                     steps[step] = pars
 
-            kwargs = {k : v for k, v in kwargs.items() if k != 'steps'}
+            kwargs = {k: v for k, v in kwargs.items() if k != "steps"}
             if steps:
-                kwargs['steps'] = steps
+                kwargs["steps"] = steps
 
         config_parser.merge_config(config_kwargs, kwargs)
         config_parser.merge_config(config, config_kwargs)
 
         return config, config_file
 
 
 # #########
 # Utilities
 # #########
 
+
 def _get_suffix(suffix, step=None, default_suffix=None):
     """Retrieve either specified or pipeline-supplied suffix
 
     Parameters
     ----------
     suffix : str or None
         Suffix to use if specified.
@@ -1416,15 +1428,15 @@
 
     Returns
     -------
     suffix : str or None
         Suffix to use
     """
     if suffix is None and step is not None:
-        suffix = step.search_attr('suffix')
+        suffix = step.search_attr("suffix")
     if suffix is None:
         suffix = default_suffix
     if suffix is None and step is not None:
         suffix = step.name.lower()
     return suffix
 
 
@@ -1440,23 +1452,23 @@
         Flag to use. If None, the environmental is used.
 
     Returns
     -------
     flag: bool
         True to disable CRDS STEPPARS retrieval.
     """
-    truths =  ('true', 'True', 't', 'yes', 'y')
+    truths = ("true", "True", "t", "yes", "y")
     if default:
         if isinstance(default, bool):
             return default
         elif isinstance(default, str):
             return default in truths
-        raise ValueError(f'default must be string or boolean: {default}')
+        raise ValueError(f"default must be string or boolean: {default}")
 
-    flag = os.environ.get('STPIPE_DISABLE_CRDS_STEPPARS', '')
+    flag = os.environ.get("STPIPE_DISABLE_CRDS_STEPPARS", "")
     return flag in truths
 
 
 @contextmanager
 def preserve_step_pars(step):
     """Context manager to preserve step parameters
```

### Comparing `stpipe-0.4.6/src/stpipe/subproc.py` & `stpipe-0.5.0/src/stpipe/subproc.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .step import Step
 
 
 class SystemCall(Step):
     """
     Execute a system call in the shell.
     """
+
     spec = """
     # SystemCall is a step to run external processes as Steps.
 
     # The command can pass along arguments that were passed to the step.
     # To refer to positional arguments, use {0}, {1}, {2}, etc.
     # To refer to keyword arguments, use {keyword}.
     command = string() # The command to execute
@@ -21,57 +22,57 @@
     log_stdout = boolean(default=True) # Do we want to log STDOUT?
 
     log_stderr = boolean(default=True) # Do we want to log STDERR?
 
     exitcode_as_exception = boolean(default=True) # Should a non-zero exit code be converted into an exception?
 
     failure_as_exception = boolean(default=True) # If subprocess fails to run at all, should that be an exception?
-    """
+    """  # noqa: E501
 
     def process(self, *args):
         from .. import datamodels
 
         newargs = []
         for i, arg in enumerate(args):
             if isinstance(arg, datamodels.DataModel):
-                filename = "{0}.{1:04d}.{2}".format(
-                    self.qualified_name, i, arg.get_fileext())
+                filename = f"{self.qualified_name}.{i:04d}.{arg.getfileext()}"
                 arg.save(filename)
                 newargs.append(filename)
             else:
                 newargs.append(arg)
 
         cmd_str = self.command.format(*newargs)
 
         env = dict(os.environ)
         for item in self.env:
-            var, sep, val = item.partition('=')
+            var, sep, val = item.partition("=")
             env[var] = val or None
 
         # Start the process and wait for it to finish.
-        self.log.info('Spawning {0!r}'.format(cmd_str))
+        self.log.info(f"Spawning {cmd_str!r}")
         try:
-            p = subprocess.Popen(args=[cmd_str],
-                                 stdin=None,
-                                 stdout=subprocess.PIPE,
-                                 stderr=subprocess.PIPE,
-                                 shell=True,
-                                 env=env)
+            p = subprocess.Popen(
+                args=[cmd_str],
+                stdin=None,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                shell=True,
+                env=env,
+            )
             err = p.wait()
         except Exception as e:
-            msg = ('Failed with an exception: \n{0}'.format(e))
+            msg = f"Failed with an exception: \n{e}"
             self.log.info(msg)
 
             if self.failure_as_exception:
                 raise
         else:
-            self.log.info('Done with errorcode {0}'.format(err))
+            self.log.info(f"Done with errorcode {err}")
 
             # Log STDOUT/ERR if we are asked to do so.
             if self.log_stdout:
-                self.log.info('STDOUT: {0}'.format(p.stdout.read()))
+                self.log.info(f"STDOUT: {p.stdout.read()}")
             if self.log_stderr:
-                self.log.info('STDERR: {0}'.format(p.stderr.read()))
+                self.log.info(f"STDERR: {p.stderr.read()}")
 
             if self.exitcode_as_exception and err != 0:
-                raise IOError('{0!r} returned error code {1}'.format(
-                    cmd_str, err))
+                raise OSError(f"{cmd_str!r} returned error code {err}")
```

### Comparing `stpipe-0.4.6/src/stpipe/tests/test_abstract_datamodel.py` & `stpipe-0.5.0/src/stpipe/tests/test_abstract_datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 """
 Test that the AbstractDataModel interface works properly
 """
 
 import pytest
+
 from ..step import AbstractDataModel
 
+
 def test_roman_datamodel():
     roman_datamodels = pytest.importorskip("roman_datamodels.datamodels")
     import roman_datamodels.tests.util as rutil
+
     roman_image_tree = rutil.mk_level2_image()
     image_model = roman_datamodels.ImageModel(roman_image_tree)
     assert isinstance(image_model, AbstractDataModel)
 
+
 def test_jwst_datamodel():
     jwst_datamodel = pytest.importorskip("jwst.datamodels")
     image_model = jwst_datamodel.ImageModel()
     assert isinstance(image_model, AbstractDataModel)
 
+
 class GoodDataModel:
     def __init__(self):
         pass
+
     def crds_observatory(self):
         pass
+
     def get_crds_parameters(self):
         pass
+
     def save(self):
         pass
+
+
 class BadDataModel:
     def __init__(self):
         pass
+
     def crds_observatory(self):
         pass
+
     def get_crds_parameters(self):
         pass
 
 
 def test_good_datamodel():
     gdm = GoodDataModel()
     assert isinstance(gdm, AbstractDataModel)
 
+
 def test_bad_datamodel():
     gdm = BadDataModel()
     assert not isinstance(gdm, AbstractDataModel)
```

### Comparing `stpipe-0.4.6/src/stpipe/utilities.py` & `stpipe-0.5.0/src/stpipe/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,38 @@
     #      subclass of `subclassof`, which HAS to be a Python class.
 
     if config_file is not None:
         sys.path.insert(0, os.path.dirname(config_file))
 
     try:
         full_name = full_name.strip()
-        package_name, sep, class_name = full_name.rpartition('.')
+        package_name, sep, class_name = full_name.rpartition(".")
         if not package_name:
-            raise ImportError("{0} is not a Python class".format(full_name))
+            raise ImportError(f"{full_name} is not a Python class")
         imported = __import__(
-            package_name, globals(), locals(), [class_name, ], level=0)
+            package_name,
+            globals(),
+            locals(),
+            [
+                class_name,
+            ],
+            level=0,
+        )
 
         step_class = getattr(imported, class_name)
 
         if not isinstance(step_class, type):
             raise TypeError(
-                'Object {0} from package {1} is not a class'.format(
-                    class_name, package_name))
+                f"Object {class_name} from package {package_name} is not a class"
+            )
         elif not issubclass(step_class, subclassof):
             raise TypeError(
-                'Class {0} from package {1} is not a subclass of {2}'.format(
-                    class_name, package_name, subclassof.__name__))
+                f"Class {class_name} from package {package_name} is not a subclass of"
+                f" {subclassof.__name__}"
+            )
     finally:
         if config_file is not None:
             del sys.path[0]
 
     return step_class
 
 
@@ -89,15 +97,15 @@
     except TypeError:
         return None
     step_source_file = os.path.abspath(step_source_file)
 
     # Since `step_class` could be defined in a file called whatever,
     # we need the source file basedir and the class name.
     dir = os.path.dirname(step_source_file)
-    return os.path.join(dir, step_class.__name__ + '.spec')
+    return os.path.join(dir, step_class.__name__ + ".spec")
 
 
 def find_spec_file(step_class):
     """
     Return the full path of the given Step subclass `step_class`, if
     it exists or None if it does not.
     """
@@ -122,8 +130,8 @@
         For other input, the fully-qualified name of the input's class.
     """
     cls = cls_or_obj if inspect.isclass(cls_or_obj) else cls_or_obj.__class__
     module = cls.__module__
     if module is None or module == str.__class__.__module__:
         return cls.__name__  # Avoid reporting __builtin__
     else:
-        return module + '.' + cls.__name__
+        return module + "." + cls.__name__
```

### Comparing `stpipe-0.4.6/src/stpipe.egg-info/PKG-INFO` & `stpipe-0.5.0/src/stpipe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpipe
-Version: 0.4.6
+Version: 0.5.0
 Summary: Framework for calibration pipeline software
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -34,15 +34,15 @@
         
 Project-URL: repository, https://github.com/spacetelescope/stpipe
 Project-URL: tracker, https://github.com/spacetelescope/stpipe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # stpipe
```

### Comparing `stpipe-0.4.6/src/stpipe.egg-info/SOURCES.txt` & `stpipe-0.5.0/src/stpipe.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 .flake8
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tox.ini
-.github/workflows/cancel_workflows.yml
+.github/CODEOWNERS
 .github/workflows/changelog.yml
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
+docs/rtd_environment.yaml
 docs/source/api.rst
 docs/source/conf.py
 docs/source/index.rst
 scripts/strun
 src/stpipe/__init__.py
 src/stpipe/__main__.py
 src/stpipe/_version.py
```

### Comparing `stpipe-0.4.6/tests/test_config_parser.py` & `stpipe-0.5.0/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `stpipe-0.4.6/tests/test_format_template.py` & `stpipe-0.5.0/tests/test_format_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,105 +3,93 @@
 
 import pytest
 
 from stpipe.format_template import FormatTemplate
 
 
 @pytest.mark.parametrize(
-    'key_formats, template, expected, fields, errors',
+    "key_formats, template, expected, fields, errors",
     [
         # No replacement at all.
         (
             None,
             'name="{name}" value="{value}"',
             'name="{name}" value="{value}"',
             {},
-            None
+            None,
         ),
-
         # Basic replacement
         (
             None,
             'name="{name}" value="{value}"',
             'name="fred" value="great"',
-            {'name': 'fred', 'value': 'great'},
-            None
+            {"name": "fred", "value": "great"},
+            None,
         ),
-
         # But wait, too many values given:
         (
             None,
             'name="{name}" value="{value}"',
             'name="fred" value="great"_more',
-            {'name': 'fred', 'value': 'great', 'extra': 'more'},
-            None
+            {"name": "fred", "value": "great", "extra": "more"},
+            None,
         ),
-
         # And with too many and not enough:
         (
             None,
             'name="{name}" value="{value}"',
             'name="{name}" value="great"_more',
-            {'value': 'great', 'extra': 'more'},
-            None
+            {"value": "great", "extra": "more"},
+            None,
         ),
-
         # Nothing should be added if value is None
         (
             None,
             'name="{name}" value="{value}"',
             'name="{name}" value=""',
-            {'value': None},
-            None
+            {"value": None},
+            None,
         ),
-
         # Multiple key formats, using none.
         (
             {
-                'field': ['s{:05d}', 's{:s}'],
+                "field": ["s{:05d}", "s{:s}"],
             },
-            'astring',
-            'astring',
+            "astring",
+            "astring",
             {},
-            None
+            None,
         ),
-
         # Multiple key formats, using first.
         (
             {
-                'field': ['s{:05d}', 's{:s}'],
+                "field": ["s{:05d}", "s{:s}"],
             },
-            'astring',
-            'astring_s00001',
-            {'field': 1},
-            None
+            "astring",
+            "astring_s00001",
+            {"field": 1},
+            None,
         ),
-
         # Multiple key formats, using second.
         (
-            {
-                'field': ['s{:05d}', 's{:s}']
-            },
-            'astring',
-            'astring_smysource',
-            {'field': "mysource"},
-            None
+            {"field": ["s{:05d}", "s{:s}"]},
+            "astring",
+            "astring_smysource",
+            {"field": "mysource"},
+            None,
         ),
-
         # No matching formats is an error.
         (
-            {
-                'field': ['s{:05d}']
-            },
-            'astring',
-            'astring_error',
-            {'field': '5.5'},
-            (RuntimeError,)
+            {"field": ["s{:05d}"]},
+            "astring",
+            "astring_error",
+            {"field": "5.5"},
+            (RuntimeError,),
         ),
-    ]
+    ],
 )
 def test_basics(key_formats, template, expected, fields, errors):
     """Test all basic formatting options"""
 
     format_product = FormatTemplate(key_formats=key_formats)
     statement = partial(format_product, template, **fields)
 
@@ -115,21 +103,21 @@
 
 def test_separators():
     """Test changing separators"""
     template = 'name="{name}" value="{value}"'
     fmt = FormatTemplate()
 
     # With a different separator:
-    fmt.separator = '---'
-    result = fmt(template, name='fred', value='great', extra='more')
+    fmt.separator = "---"
+    result = fmt(template, name="fred", value="great", extra="more")
     assert result == 'name="fred" value="great"---more'
 
     # Initializing with a different separator:
-    fmt_newsep = FormatTemplate(separator='_now-with_')
-    result = fmt_newsep(template, name='fred', value='great', extra='more')
+    fmt_newsep = FormatTemplate(separator="_now-with_")
+    result = fmt_newsep(template, name="fred", value="great", extra="more")
     assert result == 'name="fred" value="great"_now-with_more'
 
 
 def test_allow_unknown():
     """Keep None values in string"""
     template = 'name="{name}" value="{value}"'
     fmt = FormatTemplate(remove_unused=False)
```

### Comparing `stpipe-0.4.6/tests/test_logger.py` & `stpipe-0.5.0/tests/test_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 def clean_up_logging():
     yield
     logging.shutdown()
     stpipe_log.load_configuration(io.BytesIO(stpipe_log.DEFAULT_CONFIGURATION))
 
 
 def test_configuration(tmpdir):
-    logfilename = tmpdir.join('output.log')
+    logfilename = tmpdir.join("output.log")
 
-    configuration = """
+    configuration = f"""
 [.]
-handler = file:{0}
+handler = file:{logfilename}
 break_level = ERROR
 level = WARNING
 format = '%(message)s'
-""".format(logfilename)
+"""
 
     fd = io.StringIO()
     fd.write(configuration)
     fd.seek(0)
     stpipe_log.load_configuration(fd)
     fd.close()
 
@@ -36,33 +36,37 @@
     log.warning("Shown")
 
     with pytest.raises(stpipe_log.LoggedException):
         log.critical("Breaking")
 
     logging.shutdown()
 
-    with open(logfilename, 'r') as fd:
+    with open(logfilename) as fd:
         lines = [x.strip() for x in fd.readlines()]
 
-    assert lines == ['Shown', 'Breaking']
+    assert lines == ["Shown", "Breaking"]
 
 
 def test_record_logs():
     stpipe_logger = stpipe_log.getLogger(stpipe_log.STPIPE_ROOT_LOGGER)
     root_logger = stpipe_log.getLogger()
 
-    assert not any(isinstance(h, stpipe_log.RecordingHandler) for h in root_logger.handlers)
+    assert not any(
+        isinstance(h, stpipe_log.RecordingHandler) for h in root_logger.handlers
+    )
 
     with stpipe_log.record_logs(level=logging.ERROR) as log_records:
         stpipe_logger.warning("Warning from stpipe")
         stpipe_logger.error("Error from stpipe")
         root_logger.warning("Warning from root")
         root_logger.error("Error from root")
 
-    assert not any(isinstance(h, stpipe_log.RecordingHandler) for h in root_logger.handlers)
+    assert not any(
+        isinstance(h, stpipe_log.RecordingHandler) for h in root_logger.handlers
+    )
 
     stpipe_logger.error("Additional error from stpipe")
     root_logger.error("Additional error from root")
 
     assert len(log_records) == 2
     assert log_records[0].message == "Error from stpipe"
     assert log_records[1].message == "Error from root"
```

### Comparing `stpipe-0.4.6/tox.ini` & `stpipe-0.5.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # see a list of example environments that can be run, along with a description,
 # run:
 #
 #     tox -l -v
 #
 
 [testenv:check-style]
-description = check code style, e.g. with ruff
 skip_install = true
+description = Run all style and file checks with pre-commit
 deps =
-    ruff
+    pre-commit
 commands =
-    ruff . {posargs}
+    pre-commit install-hooks
+    pre-commit run {posargs:--color always --all-files --show-diff-on-failure}
 
 [testenv:check-security]
 description = run bandit to check security compliance
 skip_install = true
 deps =
     bandit>=1.7
 commands =
@@ -50,15 +51,15 @@
     oldestdeps: minimum_dependencies
 pass_env =
     CRDS_*
     CI
 set_env =
     jwst: CRDS_SERVER_URL=https://jwst-crds.stsci.edu
     romancal: CRDS_SERVER_URL=https://roman-crds.stsci.edu
-package = 
+package =
     !cov: wheel
     cov: editable
 allowlist_externals =
     echo
 commands_pre =
     oldestdeps: minimum_dependencies stpipe --filename requirements-min.txt
     oldestdeps: pip install -r requirements-min.txt
```

