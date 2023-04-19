# Comparing `tmp/ffpuppet-0.9.2.tar.gz` & `tmp/ffpuppet-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffpuppet-0.9.2.tar", last modified: Fri Sep 30 00:06:21 2022, max compression
+gzip compressed data, was "ffpuppet-0.9.3.tar", last modified: Wed Apr 19 19:59:55 2023, max compression
```

## Comparing `ffpuppet-0.9.2.tar` & `ffpuppet-0.9.3.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.858960 ffpuppet-0.9.2/
--rw-r--r--   0 worker    (1000) worker    (1000)       55 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.codecov.yml
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.850959 ffpuppet-0.9.2/.github/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.854960 ffpuppet-0.9.2/.github/scripts/
--rwxr-xr-x   0 worker    (1000) worker    (1000)     1820 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.github/scripts/start-worker.sh
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.854960 ffpuppet-0.9.2/.github/workflows/
--rw-r--r--   0 worker    (1000) worker    (1000)      404 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.github/workflows/taskcluster-pr.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      402 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.github/workflows/taskcluster-push.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      414 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.github/workflows/taskcluster-release.yml
--rw-r--r--   0 worker    (1000) worker    (1000)     1073 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     1733 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     3119 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    16725 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/LICENSE
--rw-r--r--   0 worker    (1000) worker    (1000)       52 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/MANIFEST.in
--rw-r--r--   0 worker    (1000) worker    (1000)     6731 2022-09-30 00:06:21.858960 ffpuppet-0.9.2/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     6006 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/README.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.858960 ffpuppet-0.9.2/ffpuppet/
--rw-r--r--   0 worker    (1000) worker    (1000)      581 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      258 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/__main__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     6520 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/bootstrapper.py
--rw-r--r--   0 worker    (1000) worker    (1000)     5811 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/checks.py
--rw-r--r--   0 worker    (1000) worker    (1000)      359 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/cmds.gdb
--rw-r--r--   0 worker    (1000) worker    (1000)    35923 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/core.py
--rw-r--r--   0 worker    (1000) worker    (1000)      827 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/exceptions.py
--rw-r--r--   0 worker    (1000) worker    (1000)    20274 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/helpers.py
--rw-r--r--   0 worker    (1000) worker    (1000)    10100 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/main.py
--rw-r--r--   0 worker    (1000) worker    (1000)     7429 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/minidump_parser.py
--rw-r--r--   0 worker    (1000) worker    (1000)    10513 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/puppet_logger.py
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/py.typed
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.858960 ffpuppet-0.9.2/ffpuppet/resources/
--rwxr-xr-x   0 worker    (1000) worker    (1000)     4061 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/resources/testff.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3860 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/sanitizer_util.py
--rw-r--r--   0 worker    (1000) worker    (1000)     6986 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_bootstrapper.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2888 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_checks.py
--rw-r--r--   0 worker    (1000) worker    (1000)    37554 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_ffpuppet.py
--rw-r--r--   0 worker    (1000) worker    (1000)    15916 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_helpers.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4820 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_main.py
--rw-r--r--   0 worker    (1000) worker    (1000)     6892 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_minidump_parser.py
--rw-r--r--   0 worker    (1000) worker    (1000)    10468 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_puppet_logger.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3013 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/ffpuppet/test_sanitizer_util.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-09-30 00:06:21.858960 ffpuppet-0.9.2/ffpuppet.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     6731 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     1062 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       48 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)      111 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        9 2022-09-30 00:06:21.000000 ffpuppet-0.9.2/ffpuppet.egg-info/top_level.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     1034 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)     1029 2022-09-30 00:06:21.862960 ffpuppet-0.9.2/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/setup.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1285 2022-09-30 00:06:11.000000 ffpuppet-0.9.2/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/
+-rw-r--r--   0 worker    (1000) worker    (1000)       55 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.codecov.yml
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.727330 ffpuppet-0.9.3/.github/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.731330 ffpuppet-0.9.3/.github/scripts/
+-rwxr-xr-x   0 worker    (1000) worker    (1000)     1820 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.github/scripts/start-worker.sh
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.731330 ffpuppet-0.9.3/.github/workflows/
+-rw-r--r--   0 worker    (1000) worker    (1000)      404 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.github/workflows/taskcluster-pr.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      402 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.github/workflows/taskcluster-push.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      414 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.github/workflows/taskcluster-release.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1073 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     1854 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3017 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    16725 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/LICENSE
+-rw-r--r--   0 worker    (1000) worker    (1000)       60 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/MANIFEST.in
+-rw-r--r--   0 worker    (1000) worker    (1000)     6731 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     6006 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)     1062 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1051 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.727330 ffpuppet-0.9.3/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/src/ffpuppet/
+-rw-r--r--   0 worker    (1000) worker    (1000)      654 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      258 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/__main__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     6811 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/bootstrapper.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     5803 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/checks.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      359 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/cmds.gdb
+-rw-r--r--   0 worker    (1000) worker    (1000)    36611 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/core.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      942 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/exceptions.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    16184 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/helpers.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2913 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/job_object.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     6837 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/lsof.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    11111 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/main.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     8541 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/minidump_parser.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9167 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/profile.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10501 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/puppet_logger.py
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/py.typed
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/src/ffpuppet/resources/
+-rwxr-xr-x   0 worker    (1000) worker    (1000)     4061 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/resources/testff.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3856 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/sanitizer_util.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     7826 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_bootstrapper.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2888 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_checks.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    39446 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_ffpuppet.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10624 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_helpers.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1345 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_job_object.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     5430 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_main.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     7215 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_minidump_parser.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9286 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_profile.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10468 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_puppet_logger.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3001 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/src/ffpuppet/test_sanitizer_util.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-19 19:59:55.739331 ffpuppet-0.9.3/src/ffpuppet.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6731 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     1311 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       48 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)      111 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        9 2023-04-19 19:59:55.000000 ffpuppet-0.9.3/src/ffpuppet.egg-info/top_level.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     1279 2023-04-19 19:59:46.000000 ffpuppet-0.9.3/tox.ini
```

### Comparing `ffpuppet-0.9.2/.github/scripts/start-worker.sh` & `ffpuppet-0.9.3/.github/scripts/start-worker.sh`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/.gitignore` & `ffpuppet-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/.pre-commit-config.yaml` & `ffpuppet-0.9.3/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 repos:
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/yesqa
-    rev: v1.3.0
+    rev: v1.4.0
     hooks:
       - id: yesqa
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
-        args: ['--py36-plus']
+        args: ['--py38-plus']
   - repo: https://github.com/ambv/black
-    rev: 22.6.0
+    rev: 22.12.0
     hooks:
       - id: black
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
+      - id: check-added-large-files
       - id: check-ast
+      - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-symlinks
-      - id: debug-statements
-      - id: trailing-whitespace
+      - id: check-json
+      - id: check-toml
       - id: check-yaml
+      - id: debug-statements
+      - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ['--django']
-      - id: check-json
       - id: requirements-txt-fixer
+      - id: trailing-whitespace
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.2
     hooks:
       - id: codespell
         exclude_types: [json]
   - repo: https://github.com/marco-c/taskcluster_yml_validator
-    rev: v0.0.7
+    rev: v0.0.9
     hooks:
       - id: taskcluster_yml
   - repo: https://github.com/MozillaSecurity/orion
-    rev: v0.0.4
+    rev: v0.0.6
     hooks:
       - id: orion_ci
   - repo: meta
     hooks:
       - id: check-useless-excludes
   - repo: local
     hooks:
```

### Comparing `ffpuppet-0.9.2/.taskcluster.yml` & `ffpuppet-0.9.3/.taskcluster.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,44 +16,40 @@
           key: token
       script:
         - bash
         - '-xec'
         - tox; tox -e codecov
       jobs:
         include:
-          - name: tests python 3.6
-            version: "3.6"
-            env:
-              TOXENV: py36,lint
-          - name: tests python 3.7
-            version: "3.7"
-            env:
-              TOXENV: py37,lint
           - name: tests python 3.8
             version: "3.8"
             env:
               TOXENV: py38,lint
-          - name: test python 3.8 (windows)
-            version: "3.8"
-            platform: windows
-            env:
-              TOXENV: py38
           - name: tests python 3.9
             version: "3.9"
             env:
               TOXENV: py39,lint
-          - name: test python 3.9 (macos)
-            version: "3.9"
-            platform: macos
-            env:
-              TOXENV: py39
           - name: tests python 3.10
             version: "3.10"
             env:
               TOXENV: py310,lint
+          - name: test python 3.10 (macos)
+            version: "3.10"
+            platform: macos
+            env:
+              TOXENV: py310
+          - name: test python 3.10 (windows)
+            version: "3.10"
+            platform: windows
+            env:
+              TOXENV: py310
+          - name: tests python 3.11
+            version: "3.11"
+            env:
+              TOXENV: py311,lint
           - name: PyPI upload
             version: "3.8"
             env:
               TOXENV: pypi
             script:
               - tox
             when:
```

### Comparing `ffpuppet-0.9.2/CODE_OF_CONDUCT.md` & `ffpuppet-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/LICENSE` & `ffpuppet-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/PKG-INFO` & `ffpuppet-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ffpuppet
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python module that aids in the automation of Firefox at the process level
 Home-page: https://github.com/MozillaSecurity/ffpuppet
 Author: Tyson Smith
 Author-email: twsmith@mozilla.com
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: automation firefox fuzz fuzzing security test testing
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 FFPuppet
 ========
```

### Comparing `ffpuppet-0.9.2/README.md` & `ffpuppet-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/ffpuppet/__init__.py` & `ffpuppet-0.9.3/src/ffpuppet/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """FFPuppet module"""
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from .core import Debugger, FFPuppet, Reason
-from .exceptions import BrowserTerminatedError, BrowserTimeoutError, LaunchError
+from .exceptions import (
+    BrowserExecutionError,
+    BrowserTerminatedError,
+    BrowserTimeoutError,
+    LaunchError,
+)
 from .sanitizer_util import SanitizerOptions
 
 __all__ = (
     "Debugger",
     "FFPuppet",
     "Reason",
+    "BrowserExecutionError",
     "BrowserTimeoutError",
     "BrowserTerminatedError",
     "LaunchError",
     "SanitizerOptions",
 )
 __author__ = "Tyson Smith"
```

### Comparing `ffpuppet-0.9.2/ffpuppet/bootstrapper.py` & `ffpuppet-0.9.3/src/ffpuppet/bootstrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """ffpuppet bootstrapper module"""
 import socket
-from errno import EADDRINUSE
 from logging import getLogger
-from platform import system
-from random import randint
-from time import time
+from time import sleep, time
 from typing import Any, Callable, Optional
 
 from .exceptions import BrowserTerminatedError, BrowserTimeoutError, LaunchError
 
 LOG = getLogger(__name__)
 
 __author__ = "Tyson Smith"
 __all__ = ("Bootstrapper",)
 
 
 class Bootstrapper:  # pylint: disable=missing-docstring
-    BUF_SIZE = 4096  # receive buffer size
-    POLL_WAIT: float = 1  # duration of initial blocking socket operations
-    PORT_MAX = 0xFFFF  # bootstrap range
-    PORT_MIN = 0x2000  # bootstrap range
-    PORT_RETRIES = 100  # number of attempts to find an available port
+    # see: searchfox.org/mozilla-central/source/netwerk/base/nsIOService.cpp
+    # include ports above 1024
+    BLOCKED_PORTS = (
+        1719,
+        1720,
+        1723,
+        2049,
+        3659,
+        4045,
+        5060,
+        5061,
+        6000,
+        6566,
+        6665,
+        6666,
+        6667,
+        6668,
+        6669,
+        6697,
+        10080,
+    )
+    # receive buffer size
+    BUF_SIZE = 4096
+    # duration of initial blocking socket operations
+    POLL_WAIT: float = 1
+    # number of attempts to find an available port
+    PORT_ATTEMPTS = 50
 
     __slots__ = ("_socket",)
 
-    def __init__(self) -> None:
-        self._socket: Optional[socket.socket] = socket.socket(
-            socket.AF_INET, socket.SOCK_STREAM
-        )
-        if system().startswith("Windows"):
-            self._socket.setsockopt(
-                socket.SOL_SOCKET,
-                socket.SO_EXCLUSIVEADDRUSE,  # pylint: disable=no-member
-                1,
-            )
-        self._socket.settimeout(self.POLL_WAIT)
-        for _ in range(self.PORT_RETRIES):
+    def __init__(self, attempts: int = PORT_ATTEMPTS, port: int = 0) -> None:
+        assert attempts > 0
+        assert port >= 0
+        for _ in range(attempts):
+            self._socket: Optional[socket.socket] = socket.socket()
+            self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self._socket.settimeout(self.POLL_WAIT)
             try:
-                self._socket.bind(("127.0.0.1", randint(self.PORT_MIN, self.PORT_MAX)))
+                self._socket.bind(("127.0.0.1", port))
                 self._socket.listen(5)
-            except OSError as soc_e:
-                if soc_e.errno in (EADDRINUSE, 10013):
-                    # Address already in use
-                    continue
-                raise  # pragma: no cover
+            except (OSError, PermissionError) as exc:
+                LOG.debug("%s: %s", type(exc).__name__, exc)
+                self._socket.close()
+                sleep(0.1)
+                continue
+            # avoid blocked ports
+            if port == 0 and self._socket.getsockname()[1] in self.BLOCKED_PORTS:
+                LOG.debug("bound to blocked port, retrying...")
+                self._socket.close()
+                continue
             break
         else:
-            self._socket.close()
             raise LaunchError("Could not find available port")
 
     def __enter__(self) -> "Bootstrapper":
         return self
 
     def __exit__(self, *exc: Any) -> None:
         self.close()
@@ -179,12 +197,12 @@
             else:
                 resp_timeout = False
             if not cb_continue():
                 raise BrowserTerminatedError("Failure during browser startup")
             if resp_timeout:
                 raise BrowserTimeoutError("Timeout sending response")
             LOG.debug("bootstrap complete (%0.2fs)", time() - start_time)
-        except OSError as soc_e:  # pragma: no cover
-            raise LaunchError(f"Error attempting to launch browser: {soc_e}") from soc_e
+        except OSError as exc:  # pragma: no cover
+            raise LaunchError(f"Error attempting to launch browser: {exc}") from exc
         finally:
             if conn is not None:
                 conn.close()
```

### Comparing `ffpuppet-0.9.2/ffpuppet/checks.py` & `ffpuppet-0.9.3/src/ffpuppet/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def __init__(
         self, log_files: Iterable[str], search_tokens: Iterable[Pattern[str]]
     ) -> None:
         assert log_files, "log_files is empty"
         assert search_tokens, "search_tokens is empty"
         super().__init__()
-        self.logs: List[_LogContentsCheckState] = list()
+        self.logs: List[_LogContentsCheckState] = []
         for log_file in log_files:
             self.logs.append(_LogContentsCheckState(log_file))
         self.tokens = search_tokens
 
     def check(self) -> bool:
         """Collect log contents for tokens.
 
@@ -168,15 +168,15 @@
         Args:
             None
 
         Returns:
             True if the total usage is greater than or equal to
             self.limit otherwise False.
         """
-        proc_info = list()
+        proc_info = []
         total_usage = 0
         for proc in get_processes(self.pid):
             try:
                 cur_rss = proc.memory_info().rss
                 total_usage += cur_rss
                 proc_info.append((proc.pid, cur_rss))
             except (AccessDenied, NoSuchProcess):  # pragma: no cover
```

### Comparing `ffpuppet-0.9.2/ffpuppet/core.py` & `ffpuppet-0.9.3/src/ffpuppet/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,48 +10,44 @@
 from os.path import join as pathjoin
 from os.path import realpath
 from pathlib import Path
 from platform import system
 from re import IGNORECASE
 from re import compile as re_compile
 from re import match as re_match
-from shutil import rmtree
 from subprocess import Popen, check_output
 from sys import executable
 from typing import Any, Dict, Iterator, List, Optional, Pattern, Set, Tuple, Union
 from urllib.request import pathname2url
 
 try:
     # pylint: disable=ungrouped-imports
     from subprocess import CREATE_NEW_PROCESS_GROUP  # type: ignore[attr-defined]
 except ImportError:
     pass
 
-from psutil import AccessDenied, NoSuchProcess, Process, process_iter, wait_procs
+from psutil import AccessDenied, NoSuchProcess, Process, wait_procs
 
 try:
     from xvfbwrapper import Xvfb
 except ImportError:
     pass
 
 from .bootstrapper import Bootstrapper
 from .checks import CheckLogContents, CheckLogSize, CheckMemoryUsage
-from .exceptions import InvalidPrefs, LaunchError, TerminateError
-from .helpers import (
-    append_prefs,
-    create_profile,
-    files_in_use,
-    get_processes,
-    onerror,
-    prepare_environment,
-    wait_on_files,
-)
+from .exceptions import BrowserExecutionError, InvalidPrefs, LaunchError, TerminateError
+from .helpers import files_in_use, get_processes, prepare_environment, wait_on_files
 from .minidump_parser import process_minidumps
+from .profile import Profile
 from .puppet_logger import PuppetLogger
 
+if system() == "Windows":
+    # config_job_object is only available on Windows
+    from .job_object import config_job_object
+
 LOG = getLogger(__name__)
 
 __author__ = "Tyson Smith"
 __all__ = ("Debugger", "FFPuppet", "Reason")
 
 
 @unique
@@ -117,27 +113,25 @@
         use_profile: Optional[str] = None,
         use_xvfb: bool = False,
         working_path: Optional[str] = None,
     ):
         # tokens used to notify log scanner to kill the browser process
         self._abort_tokens: Set[Pattern[str]] = set()
         self._bin_path: Optional[str] = None
-        self._checks: List[
-            Union[CheckLogContents, CheckLogSize, CheckMemoryUsage]
-        ] = list()
+        self._checks: List[Union[CheckLogContents, CheckLogSize, CheckMemoryUsage]] = []
         self._dbg = debugger
         self._dbg_sanity_check(self._dbg)
         self._headless = headless
         self._launches = 0  # number of successful browser launches
         self._logs = PuppetLogger(base_path=working_path)
         self._proc: Optional["Popen[bytes]"] = None
         self._profile_template = use_profile  # profile that is used as a template
         self._xvfb = None
         self._working_path = working_path
-        self.profile: Optional[str] = None  # path to profile
+        self.profile: Optional[Profile] = None
         self.reason: Optional[Reason] = Reason.CLOSED
 
         if use_xvfb:
             self._headless = "xvfb"
 
         if self._headless == "xvfb":
             try:
@@ -231,15 +225,16 @@
         if self._dbg == Debugger.VALGRIND:
             for entry in log_path.glob(f"{self._logs.PREFIX_VALGRIND}*"):
                 if entry.stat().st_size:
                     yield entry.resolve()
         # scan for minidump files
         if not skip_md:
             assert self.profile is not None
-            for entry in (Path(self.profile) / "minidumps").glob("*.dmp"):
+            assert self.profile.path is not None
+            for entry in (self.profile.path / "minidumps").glob("*.dmp"):
                 yield entry.resolve()
 
     @classmethod
     def _dbg_sanity_check(cls, dbg: Debugger) -> None:
         """Check requested debugger is supported and available.
 
         Args:
@@ -351,22 +346,22 @@
             additional_args: Additional arguments to pass to the browser.
 
         Returns:
             List of arguments that make up the launch command.
         """
         # if a python script is passed use 'sys.executable' as the binary
         # this is used by the test framework
-        cmd = list()
+        cmd = []
         if bin_path.lower().endswith(".py"):
             cmd.append(executable)
         cmd += [bin_path, "-no-remote"]
         if self._headless == "default":
             cmd.append("-headless")
         if self.profile is not None:
-            cmd += ["-profile", self.profile]
+            cmd += ["-profile", str(self.profile)]
 
         if additional_args:
             cmd.extend(additional_args)
 
         if self._dbg == Debugger.VALGRIND:
             assert self._logs.working_path is not None
             valgrind_log_prefix = pathjoin(
@@ -374,26 +369,28 @@
             )
             valgrind_cmd = [
                 "valgrind",
                 "-q",
                 "--error-exitcode=99",
                 "--exit-on-first-error=yes",
                 "--expensive-definedness-checks=yes",
-                "--fair-sched=try",
+                "--fair-sched=yes",
                 "--gen-suppressions=all",
                 "--leak-check=no",
                 f"--log-file={valgrind_log_prefix}.%p",
-                "--read-inline-info=no",
+                "--num-transtab-sectors=48",
+                "--read-inline-info=yes",
                 "--show-mismatched-frees=no",
                 "--show-possibly-lost=no",
                 "--smc-check=all-non-file",
                 "--trace-children=yes",
                 "--trace-children-skip=python*,*/lsb_release",
-                "--track-origins=yes",
+                "--track-origins=no",
                 "--vex-iropt-register-updates=allregs-at-mem-access",
+                "--vgdb=no",
             ]
 
             sup_file = getenv("VALGRIND_SUP_PATH")
             if sup_file:
                 if not isfile(sup_file):
                     raise OSError(f"Missing Valgrind suppressions {sup_file!r}")
                 LOG.debug("using Valgrind suppressions: %r", sup_file)
@@ -519,27 +516,25 @@
         if self.reason is not None:
             # make sure browser logs are closed
             self._logs.close()
             return
 
         assert self._proc is not None
         pid = self.get_pid()
-        procs = get_processes(pid) if pid is not None else list()
+        procs = list(get_processes(pid)) if pid is not None else []
         LOG.debug("browser pid: %r, %d process(es)", pid, len(procs))
         # If the parent process closes while other processes are still open
-        # get_processes() will return an empty list, perform a secondary scan if needed
+        # procs will be empty, perform a secondary scan if needed
         if not procs and self._logs.get_fp("stderr"):
             stderr_fp = self._logs.get_fp("stderr")
             assert stderr_fp is not None
             # create a list of processes that are using the stderr file
             # this *should* only include the browser and the current Python process
             procs = []
-            for _, other_pid, _ in files_in_use(
-                [Path(stderr_fp.name)], process_iter(["pid", "name", "open_files"])
-            ):
+            for _, other_pid, _ in files_in_use([Path(stderr_fp.name)]):
                 # don't include the current Python process in the results
                 if other_pid != getpid():
                     try:
                         procs.append(Process(other_pid))
                     except (AccessDenied, NoSuchProcess):  # pragma: no cover
                         pass
             LOG.debug("secondary scan found %d browser process(es)", len(procs))
@@ -619,17 +614,18 @@
                         check.dump_log(
                             dst_fp=self._logs.add_log(f"ffp_worker_{check.name}")
                         )
                 # collect logs (excluding minidumps)
                 for log_path in self._crashreports(skip_md=True, skip_benign=False):
                     self._logs.add_log(log_path.name, log_path.open("rb"))
                 assert self.profile is not None
+                assert self.profile.path is not None
                 assert self._bin_path is not None
                 # check for minidumps and process them if possible
-                md_path = Path(self.profile) / "minidumps"
+                md_path = self.profile.path / "minidumps"
                 if any(md_path.glob("*.dmp")):
                     # check for local build symbols
                     sym_path = Path(self._bin_path) / ".." / "crashreporter-symbols"
                     if not sym_path.is_dir():
                         # use packaged symbols
                         sym_path = Path(self._bin_path) / "symbols"
                     process_minidumps(
@@ -644,25 +640,18 @@
                         stderr_fp.write(f"[ffpuppet] Exit code: {exit_code}\n".encode())
                     stderr_fp.write(f"[ffpuppet] Reason code: {r_code.name}\n".encode())
 
         # reset remaining to closed state
         try:
             self._proc = None
             self._logs.close()
-            self._checks = list()
-            # remove temporary profile directory if necessary
-            try:
-                assert self.profile is not None
-                rmtree(self.profile, onerror=onerror)
-            except OSError:  # pragma: no cover
-                LOG.error("Failed to remove profile %r", self.profile)
-                if not force_close:
-                    raise
-            finally:
-                self.profile = None
+            self._checks = []
+            assert self.profile
+            self.profile.remove(ignore_errors=force_close)
+            self.profile = None
         finally:
             LOG.debug("reason code: %s", r_code.name)
             self.reason = r_code
 
     def cpu_usage(self) -> Iterator[Tuple[int, float]]:
         """Collect percentage of CPU usage per process.
 
@@ -740,14 +729,15 @@
         env_mod: Optional[Dict[str, Optional[str]]] = None,
         launch_timeout: int = 300,
         location: Optional[str] = None,
         log_limit: int = 0,
         memory_limit: int = 0,
         prefs_js: Optional[str] = None,
         extension: Optional[str] = None,
+        cert_files: Optional[List[str]] = None,
     ) -> None:
         """Launch a new browser process.
 
         Args:
             bin_path: Path to the Firefox binary.
             env_mod: Environment modifier. Add, remove and update entries
                      in the prepared environment. Add and update by
@@ -781,28 +771,41 @@
             if isfile(location):
                 location = "///".join(
                     ["file:", pathname2url(realpath(location)).lstrip("/")]
                 )
             elif re_match(r"http(s)?://", location, IGNORECASE) is None:
                 raise OSError(f"Cannot find {location!r}")
 
-        # create and modify a profile
-        self.profile = create_profile(
+        # clean up existing log files
+        self._logs.reset()
+        assert self._logs.working_path is not None
+        sanitizer_logs = pathjoin(self._logs.working_path, self._logs.PREFIX_SAN)
+
+        # process environment
+        env_mod = env_mod or {}
+        if self._dbg in (Debugger.PERNOSCO, Debugger.RR):
+            env_mod["_RR_TRACE_DIR"] = self._logs.add_path(self._logs.PATH_RR)
+        elif self._dbg == Debugger.VALGRIND:
+            # https://developer.gimp.org/api/2.0/glib/glib-running.html#G_DEBUG
+            env_mod["G_DEBUG"] = "gc-friendly"
+            env_mod["MOZ_CRASHREPORTER_DISABLE"] = "1"
+        if self._headless == "xvfb":
+            env_mod["MOZ_ENABLE_WAYLAND"] = "0"
+
+        # create a profile
+        self.profile = Profile(
+            browser_bin=bin_path,
+            cert_files=cert_files,
             extension=extension,
-            prefs_js=prefs_js,
+            prefs_file=prefs_js,
             template=self._profile_template,
             working_path=self._working_path,
         )
-        LOG.debug("using profile %r", self.profile)
+        LOG.debug("using profile '%s'", self.profile)
 
-        launch_timeout = max(launch_timeout, self.LAUNCH_TIMEOUT_MIN)
-        LOG.debug("launch timeout: %d", launch_timeout)
-        # clean up existing log files
-        self._logs.reset()
-        self.reason = None
         # performing the bootstrap helps guarantee that the browser
         # will be loaded and ready to accept input when launch() returns
         bootstrapper = Bootstrapper()
         try:
             # added `network.proxy.failover_direct` and `network.proxy.allow_bypass`
             # to workaround default prefs.js packaged with Grizzly test cases.
             # This can be removed in the future but for now it unblocks
@@ -811,83 +814,87 @@
                 "capability.policy.localfilelinks.checkloaduri.enabled": "'allAccess'",
                 "capability.policy.localfilelinks.sites": f"'{bootstrapper.location}'",
                 "capability.policy.policynames": "'localfilelinks'",
                 "network.proxy.allow_bypass": "false",
                 "network.proxy.failover_direct": "false",
                 "privacy.partition.network_state": "false",
             }
-            append_prefs(self.profile, prefs)
+            self.profile.add_prefs(prefs)
 
             launch_args = [bootstrapper.location]
             is_windows = system().startswith("Windows")
             if is_windows:
                 # disable launcher process
                 launch_args.append("-no-deelevate")
                 launch_args.append("-wait-for-browser")
             cmd = self.build_launch_cmd(bin_path, additional_args=launch_args)
 
-            if self._dbg in (Debugger.PERNOSCO, Debugger.RR):
-                if env_mod is None:
-                    env_mod = dict()
-                env_mod["_RR_TRACE_DIR"] = self._logs.add_path(self._logs.PATH_RR)
-            elif self._dbg == Debugger.VALGRIND:
-                if env_mod is None:
-                    env_mod = dict()
-                # https://developer.gimp.org/api/2.0/glib/glib-running.html#G_DEBUG
-                env_mod["G_DEBUG"] = "gc-friendly"
-                env_mod["MOZ_CRASHREPORTER_DISABLE"] = "1"
-
-            if self._headless == "xvfb":
-                if env_mod is None:
-                    env_mod = dict()
-                env_mod["MOZ_ENABLE_WAYLAND"] = "0"
-
             # open logs
             self._logs.add_log("stdout")
             stderr = self._logs.add_log("stderr")
             stderr.write(f"[ffpuppet] Launch command: {' '.join(cmd)}\n\n".encode())
             stderr.flush()
-            assert self._logs.working_path is not None
-            sanitizer_logs = pathjoin(self._logs.working_path, self._logs.PREFIX_SAN)
             # launch the browser
+            launch_timeout = max(launch_timeout, self.LAUNCH_TIMEOUT_MIN)
+            LOG.debug("launch timeout: %d", launch_timeout)
             LOG.debug("launch command: %r", " ".join(cmd))
+            self.reason = None
             # pylint: disable=consider-using-with
             self._proc = Popen(
                 cmd,
                 bufsize=0,  # unbuffered (for log scanners)
                 creationflags=CREATE_NEW_PROCESS_GROUP if is_windows else 0,
                 env=prepare_environment(
                     self._bin_path, sanitizer_logs, env_mod=env_mod
                 ),
                 shell=False,
                 stderr=stderr,
                 stdout=self._logs.get_fp("stdout"),
             )
             LOG.debug("launched process %r", self.get_pid())
+            if memory_limit and is_windows:
+                LOG.debug("configuring job object")
+                # pylint: disable=no-member,protected-access
+                config_job_object(
+                    self._proc._handle,  # type: ignore[attr-defined]
+                    memory_limit,
+                )
             bootstrapper.wait(self.is_healthy, timeout=launch_timeout, url=location)
+        except FileNotFoundError as exc:
+            if Path(exc.filename).exists():
+                # this is known to happen when attempting to launch 32-bit binaries
+                # on a 64-bit environment without proper libraries installed
+                raise BrowserExecutionError("Cannot execute binary") from None
+            raise
         finally:
+            if self._proc is None:
+                # only clean up here if a launch was not attempted or Popen failed
+                LOG.debug("process not launched")
+                self.profile.remove()
+                self.profile = None
+                self.reason = Reason.CLOSED
             bootstrapper.close()
-            if prefs_js is not None and isfile(
-                pathjoin(self.profile, "Invalidprefs.js")
-            ):
-                raise InvalidPrefs(f"{prefs_js!r} is invalid")
+
+        if prefs_js and self.profile.invalid_prefs:
+            raise InvalidPrefs(f"{prefs_js!r} is invalid")
 
         logs_fp_stderr = self._logs.get_fp("stderr")
         assert logs_fp_stderr is not None
         logs_fp_stdout = self._logs.get_fp("stdout")
         assert logs_fp_stdout is not None
         if log_limit:
             self._checks.append(
                 CheckLogSize(
                     log_limit,
                     logs_fp_stderr.name,
                     logs_fp_stdout.name,
                 )
             )
-        if memory_limit:
+        if memory_limit and not is_windows:
+            # memory limit is enforced with config_job_object on Windows
             curr_pid = self.get_pid()
             assert curr_pid is not None
             self._checks.append(CheckMemoryUsage(curr_pid, memory_limit))
         if self._abort_tokens:
             self._checks.append(
                 CheckLogContents(
                     [
@@ -959,11 +966,11 @@
                              None (wait indefinitely).
 
         Returns:
             True if processes exit before timeout expires otherwise False.
         """
         assert timeout is None or timeout >= 0
         pid = self.get_pid()
-        if pid is None or not wait_procs(get_processes(pid), timeout=timeout)[1]:
+        if pid is None or not wait_procs(list(get_processes(pid)), timeout=timeout)[1]:
             return True
         LOG.debug("wait(timeout=%0.2f) timed out", timeout)
         return False
```

### Comparing `ffpuppet-0.9.2/ffpuppet/exceptions.py` & `ffpuppet-0.9.3/src/ffpuppet/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 class LaunchError(Exception):
     """
     Raised when the browser process does not appear to be in a functional state
     during launch.
     """
 
 
+class BrowserExecutionError(LaunchError):
+    """
+    Raised when the browser binary cannot be executed.
+    """
+
+
 class BrowserTerminatedError(LaunchError):
     """
     Raised when the browser process goes away during launch.
     """
 
 
 class BrowserTimeoutError(LaunchError):
```

### Comparing `ffpuppet-0.9.2/ffpuppet/helpers.py` & `ffpuppet-0.9.3/src/ffpuppet/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,45 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """ffpuppet helper utilities"""
 
-from json import load as json_load
 from logging import getLogger
-from os import W_OK, access, chmod, environ, mkdir, remove
-from os.path import abspath, basename, isdir, isfile
+from os import W_OK, access, chmod, environ
+from os.path import isfile
 from os.path import join as pathjoin
 from pathlib import Path
 from platform import system
-from shutil import copyfile, copytree, rmtree
 from stat import S_IWUSR
-from tempfile import mkdtemp
+from subprocess import STDOUT, CalledProcessError, check_output
 from time import sleep, time
-from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Union
-from xml.etree import ElementTree
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple
 
 from psutil import AccessDenied, NoSuchProcess, Process, process_iter
 
 from .sanitizer_util import SanitizerOptions
 
+if system() == "Windows":
+    from .lsof import pids_by_file
+
 LOG = getLogger(__name__)
 
 __author__ = "Tyson Smith"
 __all__ = (
-    "check_prefs",
-    "create_profile",
+    "certutil_available",
+    "certutil_find",
     "files_in_use",
     "get_processes",
     "onerror",
     "prepare_environment",
     "wait_on_files",
     "warn_open",
 )
 
 
-def append_prefs(profile_path: str, prefs: Dict[str, str]) -> None:
-    """Write or append preferences from prefs to prefs.js file in profile_path.
-
-    Args:
-        profile_path: Directory containing prefs.js file to write to.
-        prefs: preferences to add.
-
-    Returns:
-        None
-    """
-    assert isinstance(prefs, dict)
-    with open(pathjoin(profile_path, "prefs.js"), "a") as prefs_fp:
-        # make sure there is a newline before appending to prefs.js
-        prefs_fp.write("\n")
-        for name, value in prefs.items():
-            prefs_fp.write(f"user_pref('{name}', {value});\n")
-
-
-def check_prefs(prof_prefs: str, input_prefs: str) -> bool:
-    """Check that the given prefs.js file in use by the browser contains all
-    the requested preferences.
-    NOTE: There will be false positives if input_prefs does not adhere to the
-    formatting that is used in prefs.js file generated by the browser.
-
-    Args:
-        prof_prefs: Path to profile prefs.js file.
-        input_prefs: Path to prefs.js file that contains prefs that
-                           should be merged into the prefs.js file generated by
-                           the browser.
-
-    Returns:
-        True if all expected preferences are found otherwise False.
-    """
-    with open(prof_prefs) as p_fp, open(input_prefs) as i_fp:
-        p_prefs = {pref.split(",")[0] for pref in p_fp if pref.startswith("user_pref(")}
-        i_prefs = {pref.split(",")[0] for pref in i_fp if pref.startswith("user_pref(")}
-    missing_prefs = i_prefs - p_prefs
-    for missing in missing_prefs:
-        LOG.debug("pref not set %r", missing)
-    return not missing_prefs
-
-
 def _configure_sanitizers(
     orig_env: Dict[str, str], target_dir: str, log_path: str
 ) -> Dict[str, str]:
     """Copy environment and update default values in *SAN_OPTIONS entries.
     These values are only updated if they are not provided, with the exception of
     'log_path'. 'log_path' is used by FFPuppet to detect results.
 
@@ -107,18 +65,18 @@
         ("symbolize", "true"),
     ]
     # set llvm-symbolizer path
     # *SAN_OPTIONS=external_symbolizer_path takes priority if it is defined in env
     llvm_sym = env.get("ASAN_SYMBOLIZER_PATH")
     if not llvm_sym:
         # use packaged llvm-symbolizer
-        if system().startswith("Windows"):
-            llvm_sym = pathjoin(target_dir, "llvm-symbolizer.exe")
-        else:
-            llvm_sym = pathjoin(target_dir, "llvm-symbolizer")
+        llvm_sym = pathjoin(
+            target_dir,
+            "llvm-symbolizer.exe" if system() == "Windows" else "llvm-symbolizer",
+        )
     if isfile(llvm_sym):
         # add *SAN_OPTIONS=external_symbolizer_path
         common_flags.append(("external_symbolizer_path", f"'{llvm_sym}'"))
     else:
         # assume system llvm-symbolizer will be used
         LOG.debug("llvm-symbolizer not found (%s)", llvm_sym)
 
@@ -132,27 +90,27 @@
     # asan_config.add("alloc_dealloc_mismatch", "false")
     asan_config.add("check_initialization_order", "true")
     # https://bugzil.la/1057551
     # asan_config.add("detect_stack_use_after_return", "true")
     # asan_config.add("detect_stack_use_after_scope", "true")
     asan_config.add("detect_invalid_pointer_pairs", "1")
     asan_config.add("detect_leaks", "false")
+    # hard_rss_limit_mb requires background thread so only works on Linux for now...
+    # see https://github.com/llvm/llvm-project/blob/main/compiler-rt/lib/
+    # sanitizer_common/sanitizer_common_libcdep.cpp#L116
+    asan_config.add("hard_rss_limit_mb", "12288")
     # log_path is required for FFPuppet logging to function properly
     if "log_path" in asan_config:
         LOG.warning(
             "ASAN_OPTIONS=log_path is used internally and cannot be set externally"
         )
     asan_config.add("log_path", f"'{log_path}'", overwrite=True)
-    # WARNING: setting max_allocation_size_mb too low can result in missing crashes
-    asan_config.add("max_allocation_size_mb", "12288")
+    # This is an experimental feature added in Bug 1792757
+    asan_config.add("rss_limit_heap_profile", "true")
     asan_config.add("sleep_before_dying", "0")
-    # soft_rss_limit_mb requires background thread so only works on Linux for now...
-    # see https://github.com/llvm/llvm-project/blob/main/compiler-rt/lib/
-    # sanitizer_common/sanitizer_common_libcdep.cpp#L116
-    asan_config.add("soft_rss_limit_mb", "12288")
     asan_config.add("strict_init_order", "true")
     # temporarily revert to default (false) until https://bugzil.la/1767068 is fixed
     # asan_config.add("strict_string_checks", "true")
     env["ASAN_OPTIONS"] = str(asan_config)
 
     # setup Leak Sanitizer options ONLY if not set manually in environment
     # https://github.com/google/sanitizers/wiki/AddressSanitizerLeakSanitizer
@@ -164,25 +122,25 @@
     lsan_config.add("report_objects", "1")
     env["LSAN_OPTIONS"] = str(lsan_config)
 
     # setup Thread Sanitizer options ONLY if not set manually in environment
     tsan_config = SanitizerOptions(env.get("TSAN_OPTIONS"))
     assert tsan_config.check_path("suppressions"), "missing suppressions file"
     tsan_config.add("halt_on_error", "1")
+    # hard_rss_limit_mb requires background thread so only works on Linux for now...
+    # see https://github.com/llvm/llvm-project/blob/main/compiler-rt/lib/
+    # sanitizer_common/sanitizer_common_libcdep.cpp#L116
+    tsan_config.add("hard_rss_limit_mb", "12288")
     if "log_path" in tsan_config:
         LOG.warning(
             "TSAN_OPTIONS=log_path is used internally and cannot be set externally"
         )
     tsan_config.add("log_path", f"'{log_path}'", overwrite=True)
-    # WARNING: setting max_allocation_size_mb too low can result in missing crashes
-    tsan_config.add("max_allocation_size_mb", "12288")
-    # soft_rss_limit_mb requires background thread so only works on Linux for now...
-    # see https://github.com/llvm/llvm-project/blob/main/compiler-rt/lib/
-    # sanitizer_common/sanitizer_common_libcdep.cpp#L116
-    tsan_config.add("soft_rss_limit_mb", "12288")
+    # This is an experimental feature added in Bug 1792757
+    tsan_config.add("rss_limit_heap_profile", "true")
     env["TSAN_OPTIONS"] = str(tsan_config)
 
     # setup Undefined Behavior Sanitizer options ONLY if not set manually in environment
     ubsan_config = SanitizerOptions(env.get("UBSAN_OPTIONS"))
     assert ubsan_config.check_path("suppressions"), "missing suppressions file"
     for flag in common_flags:
         ubsan_config.add(*flag)
@@ -194,158 +152,116 @@
     ubsan_config.add("print_stacktrace", "1")
     ubsan_config.add("report_error_type", "1")
     env["UBSAN_OPTIONS"] = str(ubsan_config)
 
     return env
 
 
-def create_profile(
-    extension: Optional[Union[List[str], str]] = None,
-    prefs_js: Optional[str] = None,
-    template: Optional[str] = None,
-    working_path: Optional[str] = None,
-) -> str:
-    """Create a profile to be used with Firefox.
+def certutil_available(certutil: str) -> bool:
+    """Check if NSS certutil is available.
 
     Args:
-        extension: Path to an extension to be installed.
-        prefs_js: Path to the prefs.js file to install in the profile.
-        template: Path to an existing profile directory to use.
-        working_path: Used as base directory for temporary files.
+        certutil: certutil location.
 
     Returns:
-        Path to directory to be used as a profile.
+        True if certutil is available for use otherwise False.
     """
-    profile = mkdtemp(dir=working_path, prefix="ffprofile_")
     try:
-        if template is not None:
-            LOG.debug("using profile template: %r", template)
-            rmtree(profile)
-            copytree(template, profile)
-            invalid_prefs = pathjoin(profile, "Invalidprefs.js")
-            # if Invalidprefs.js was copied from the template profile remove it
-            if isfile(invalid_prefs):
-                remove(invalid_prefs)
-        if prefs_js is not None:
-            LOG.debug("using prefs.js: %r", prefs_js)
-            copyfile(prefs_js, pathjoin(profile, "prefs.js"))
-            # times.json only needs to be created when using a custom prefs.js
-            times_json = pathjoin(profile, "times.json")
-            if not isfile(times_json):
-                with open(times_json, "w") as times_fp:
-                    times_fp.write(f'{{"created":{int(time()) * 1000}}}')
-    except OSError:
-        rmtree(profile)
-        raise
+        check_output([certutil], stderr=STDOUT, timeout=10)
+    except CalledProcessError as exc:
+        # there are multiple "certutil" tools and one is installed on Windows by default
+        # check the help output to make sure we have the correct tool
+        if (
+            exc.output
+            and b"Utility to manipulate NSS certificate databases" in exc.output
+        ):
+            return True
+    except OSError as exc:
+        LOG.debug(str(exc))
+    LOG.debug("%r is not suitable for use", certutil)
+    return False
 
-    # extension support
-    try:
-        if extension is None:
-            extensions = []
-        elif isinstance(extension, (list, tuple)):
-            extensions = extension
-        else:
-            extensions = [extension]
-        if extensions and not isdir(pathjoin(profile, "extensions")):
-            mkdir(pathjoin(profile, "extensions"))
-        for ext in extensions:
-            if isfile(ext) and ext.endswith(".xpi"):
-                copyfile(ext, pathjoin(profile, "extensions", basename(ext)))
-            elif isdir(ext):
-                # read manifest to see what the folder should be named
-                ext_name = None
-                if isfile(pathjoin(ext, "manifest.json")):
-                    try:
-                        with open(pathjoin(ext, "manifest.json")) as manifest:
-                            manifest_loaded_json = json_load(manifest)
-                        ext_name = manifest_loaded_json["applications"]["gecko"]["id"]
-                    except (OSError, KeyError, ValueError) as exc:
-                        LOG.debug("Failed to parse manifest.json: %s", exc)
-                elif isfile(pathjoin(ext, "install.rdf")):
-                    try:
-                        xmlns = {
-                            "x": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
-                            "em": "http://www.mozilla.org/2004/em-rdf#",
-                        }
-                        tree = ElementTree.parse(pathjoin(ext, "install.rdf"))
-                        assert tree.getroot().tag == f"{{{xmlns['x']}}}RDF"
-                        ids = tree.findall("./x:Description/em:id", namespaces=xmlns)
-                        assert len(ids) == 1
-                        ext_name = ids[0].text
-                    except (AssertionError, OSError, ElementTree.ParseError) as exc:
-                        LOG.debug("Failed to parse install.rdf: %s", exc)
-                if ext_name is None:
-                    raise RuntimeError(
-                        f"Failed to find extension id in manifest: {ext!r}"
-                    )
-                copytree(abspath(ext), pathjoin(profile, "extensions", ext_name))
-            else:
-                raise RuntimeError(f"Unknown extension: {ext!r}")
-    except Exception:
-        # cleanup on failure
-        rmtree(profile, True)
-        raise
-    return profile
-
-
-def files_in_use(
-    files: Iterable[Path], procs: Iterable[Process]
-) -> Iterator[Tuple[Path, int, str]]:
-    """Check if any of the given files are open by any of the given processes.
+
+def certutil_find(browser_bin: Optional[str] = None) -> str:
+    """Look for NSS certutil in known location or fallback to built-in tool.
+
+    Args:
+        browser_bin: Location of browser binary.
+
+    Returns:
+        Path to certutil tool to use.
+    """
+    if browser_bin:
+        path = Path(browser_bin).parent / "bin" / "certutil"
+        if path.is_file():
+            return str(path)
+    return "certutil"
+
+
+def files_in_use(files: Iterable[Path]) -> Iterator[Tuple[Path, int, str]]:
+    """Check if any of the given files are open.
+    WARNING: This can be slow on Windows.
 
     Args:
         files: Files to check.
-        procs: Processes to scan for open files.
 
     Yields:
         Path of file, process ID and process name.
     """
-    assert isinstance(files, (set, tuple, list))
+    # only check existing file
+    files = tuple(x for x in files if x.exists())
     if files:
-        for proc in procs:
-            try:
-                # WARNING: Process.open_files() has issues on Windows!
-                # https://psutil.readthedocs.io/en/latest/#psutil.Process.open_files
-                for open_file in (Path(x.path) for x in proc.open_files()):
+        # WARNING: Process.open_files() has issues on Windows!
+        # https://psutil.readthedocs.io/en/latest/#psutil.Process.open_files
+        # use an alternative implementation instead
+        if system() == "Windows":
+            for open_file, pids in pids_by_file().items():
+                for check_file in files:
+                    try:
+                        if check_file.samefile(open_file):
+                            for pid in pids:
+                                yield open_file, pid, Process(pid).name
+                    except OSError:  # pragma: no cover
+                        # samefile() can raise if either file cannot be accessed
+                        # this is triggered on Windows if a file is missing
+                        pass
+        else:
+            for proc in process_iter(["pid", "name", "open_files"]):
+                if not proc.info["open_files"]:
+                    continue
+                for open_file in (Path(x.path) for x in proc.info["open_files"]):
                     for check_file in files:
                         try:
                             if check_file.samefile(open_file):
-                                yield open_file, proc.pid, proc.name()
-                        except OSError:
+                                yield open_file, proc.info["pid"], proc.info["name"]
+                        except OSError:  # pragma: no cover
                             # samefile() can raise if either file cannot be accessed
-                            # this is triggered on Windows if a file is missing
                             pass
-            except (AccessDenied, NoSuchProcess):  # pragma: no cover
-                pass
 
 
-def get_processes(pid: int, recursive: bool = True) -> List[Process]:
+def get_processes(pid: int, recursive: bool = True) -> Iterator[Process]:
     """From a given PID create a psutil.Process object and lookup all of its
     children.
 
     Args:
         pid: PID of the process to lookup.
         recursive: Include the children (and so on) of the Process
                           that was created.
 
-    Returns:
-        A list of psutil.Process objects. The first object will always
-        be the Process that corresponds to PID.
+    Yields:
+        psutil.Process objects. The first object will always be the Process that
+        corresponds to pid.
     """
     try:
-        procs = [Process(pid)]
+        proc = Process(pid)
+        yield proc
+        if recursive and proc:
+            yield from proc.children(recursive=True)
     except (AccessDenied, NoSuchProcess):
-        return list()
-    if not recursive:
-        return procs
-    try:
-        procs += procs[0].children(recursive=True)
-    except (AccessDenied, NoSuchProcess):  # pragma: no cover
         pass
-    return procs
 
 
 def onerror(
     func: Callable[[str], Any], path: str, _exc_info: Any
 ) -> None:  # pragma: no cover
     """
     Error handler for `shutil.rmtree`.
@@ -384,15 +300,15 @@
         env_mod (dict): Environment modifier. Add, remove and update entries
                         in the prepared environment. Add and update by setting
                         value (str) and remove by setting entry value to None.
 
     Returns:
         Environment to use when launching browser.
     """
-    base: Dict[str, Optional[str]] = dict()
+    base: Dict[str, Optional[str]] = {}
     env: Dict[str, str] = dict(environ)
 
     # https://developer.gimp.org/api/2.0/glib/glib-running.html#G_SLICE
     base["G_SLICE"] = "always-malloc"
     base["MOZ_AUTOMATION"] = "1"
     base["MOZ_CC_RUN_DURING_SHUTDOWN"] = "1"
     # https://firefox-source-docs.mozilla.org/toolkit/crashreporter/crashreporter/ ...
@@ -448,15 +364,17 @@
 
     if env.get("MOZ_CRASHREPORTER_DISABLE") == "1":
         env.pop("MOZ_CRASHREPORTER", None)
         env.pop("MOZ_CRASHREPORTER_NO_DELETE_DUMP", None)
         env.pop("MOZ_CRASHREPORTER_NO_REPORT", None)
         env.pop("MOZ_CRASHREPORTER_SHUTDOWN", None)
 
-    return _configure_sanitizers(env, target_dir, sanitizer_log)
+    env = _configure_sanitizers(env, target_dir, sanitizer_log)
+    # filter environment to avoid leaking sensitive information
+    return {k: v for k, v in env.items() if "_SECRET" not in k}
 
 
 def wait_on_files(
     wait_files: Iterable[Path],
     poll_rate: float = 1.0,
     timeout: float = 60,
 ) -> bool:
@@ -472,17 +390,15 @@
     """
     assert poll_rate >= 0
     assert timeout >= 0
     all_closed = False
     poll_rate = min(poll_rate, timeout)
     deadline = time() + timeout
     while True:
-        open_iter = files_in_use(
-            wait_files, process_iter(["pid", "name", "open_files"])
-        )
+        open_iter = files_in_use(wait_files)
         if deadline <= time():
             LOG.debug("wait_on_files() timeout (%ds)", timeout)
             for entry in open_iter:
                 LOG.debug("%r open by %r (%d)", str(entry[0]), entry[2], entry[1])
             break
         if not any(open_iter):
             all_closed = True
@@ -498,11 +414,9 @@
 
     Args:
         path: Path to scan for initial files.
 
     Returns:
         None
     """
-    for entry in files_in_use(
-        list(Path(path).iterdir()), process_iter(["pid", "name", "open_files"])
-    ):
+    for entry in files_in_use(Path(path).iterdir()):
         LOG.warning("%r open by %r (%d)", str(entry[0]), entry[2], entry[1])
```

### Comparing `ffpuppet-0.9.2/ffpuppet/main.py` & `ffpuppet-0.9.3/src/ffpuppet/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """ffpuppet main.py"""
 
 from argparse import ArgumentParser, Namespace
+from importlib.metadata import PackageNotFoundError, version
 from logging import DEBUG, ERROR, INFO, WARNING, basicConfig, getLogger
 from os import scandir
 from os.path import abspath, exists, isdir, isfile
-from os.path import join as pathjoin
 from platform import system
 from shutil import rmtree
 from tempfile import mkdtemp
 from time import sleep, strftime
 from typing import List, Optional
 
 from .core import Debugger, FFPuppet, Reason
-from .helpers import check_prefs
+from .exceptions import BrowserExecutionError
+from .helpers import certutil_available, certutil_find
+from .profile import Profile
 
 LOG = getLogger(__name__)
 
 __author__ = "Tyson Smith"
+try:
+    __version__ = version("ffpuppet")
+except PackageNotFoundError:  # pragma: no cover
+    # package is not installed
+    __version__ = "unknown"
 
 
 def dump_to_console(log_dir: str, log_quota: int = 0x8000) -> str:
     """Read and merge log files and format for output on the console.
 
     Args:
         log_dir: Directory to scan for logs.
@@ -45,15 +52,15 @@
                 found = log
                 break
         # move to the end of the print list
         if found and logs[-1] != found:
             logs.remove(found)
             logs.append(found)
     # merge logs
-    lines = list()
+    lines = []
     for log in logs:
         fsize = log.stat().st_size
         lines.append("\n===\n")
         lines.append(f"=== Dumping {log.name!r} ({fsize / 1024.0:0.2f}KB)")
         with open(log.path, "rb") as log_fp:
             # tail log if needed
             log_fp.seek(max(fsize - log_quota, 0))
@@ -89,17 +96,29 @@
     )
     parser.add_argument(
         "--log-level",
         choices=sorted(log_level_map),
         default="INFO",
         help="Configure console logging (default: %(default)s)",
     )
+    parser.add_argument(
+        "--version",
+        "-V",
+        action="version",
+        version=__version__,
+        help="Show version number",
+    )
 
     cfg_group = parser.add_argument_group("Browser Configuration")
     cfg_group.add_argument(
+        "--certs",
+        nargs="+",
+        help="Install trusted certificates.",
+    )
+    cfg_group.add_argument(
         "-e",
         "--extension",
         action="append",
         help="Install extensions. Specify the path to the xpi or the directory "
         "containing the unpacked extension.",
     )
     headless_choices = ["default"]
@@ -135,15 +154,15 @@
         cfg_group.set_defaults(xvfb=False)
 
     report_group = parser.add_argument_group("Issue Detection & Reporting")
     report_group.add_argument(
         "-a",
         "--abort-token",
         action="append",
-        default=list(),
+        default=[],
         help="Scan the browser logs for the given value and close browser if detected. "
         "For example '-a ###!!! ASSERTION:' would be used to detect soft assertions.",
     )
     report_group.add_argument(
         "--launch-timeout",
         type=int,
         default=300,
@@ -220,15 +239,21 @@
     parser.set_defaults(debugger=Debugger.NONE)
 
     args = parser.parse_args(argv)
 
     # sanity checks
     if not isfile(args.binary):
         parser.error(f"Invalid browser binary {args.binary!r}")
-    if args.extension is not None:
+    if args.certs:
+        if not certutil_available(certutil_find(args.binary)):
+            parser.error("'--certs' requires NSS certutil")
+        for cert in args.certs:
+            if not isfile(cert):
+                parser.error(f"Invalid certificate file {cert!r}")
+    if args.extension:
         for ext in args.extension:
             if not exists(ext):
                 parser.error(f"Extension {ext!r} does not exist")
     if not isdir(args.logs):
         parser.error(f"Log output directory is invalid {args.logs!r}")
     args.log_level = log_level_map[args.log_level]
     if args.log_limit < 0:
@@ -272,21 +297,25 @@
             args.binary,
             location=args.url,
             launch_timeout=args.launch_timeout,
             log_limit=args.log_limit,
             memory_limit=args.memory,
             prefs_js=args.prefs,
             extension=args.extension,
+            cert_files=args.certs,
         )
         if args.prefs and isfile(args.prefs):
             assert ffp.profile is not None
-            check_prefs(pathjoin(ffp.profile, "prefs.js"), args.prefs)
+            assert ffp.profile.path is not None
+            Profile.check_prefs(str(ffp.profile.path / "prefs.js"), args.prefs)
         LOG.info("Running Firefox (pid: %d)...", ffp.get_pid())
         while ffp.is_healthy():
             sleep(args.poll_interval)
+    except BrowserExecutionError:
+        LOG.error("Cannot execute binary. Perhaps required libraries are missing?")
     except KeyboardInterrupt:
         user_exit = True
         LOG.info("Ctrl+C detected.")
     finally:
         LOG.info("Shutting down...")
         ffp.close()
         if ffp.reason is not None:
```

### Comparing `ffpuppet-0.9.2/ffpuppet/minidump_parser.py` & `ffpuppet-0.9.3/src/ffpuppet/minidump_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from shutil import copy2, rmtree
 from subprocess import DEVNULL, CalledProcessError, TimeoutExpired, call, run
 from tempfile import NamedTemporaryFile, mkdtemp
 from typing import IO, Any, Callable, Dict, List, Optional
 
 LOG = getLogger(__name__)
 
+MDSW_AVAILABLE = False
+
 __author__ = "Tyson Smith"
 __all__ = ("process_minidumps",)
 
 
 class MinidumpStackwalkFailure(Exception):
     """
     Raised when the minidump-stackwalk fails.
@@ -51,15 +53,15 @@
 
         Returns:
             None
         """
         assert limit > 0
         # generate register information lines
         frames = md_data["crashing_thread"]["frames"]
-        reg_lines: List[str] = list()
+        reg_lines: List[str] = []
         for reg, value in frames[0]["registers"].items():
             # display three registers per line
             sep = "\t" if (len(reg_lines) + 1) % 3 else "\n"
             reg_lines.append(f"{reg:>3} = {value}{sep}")
         out_fp.write("".join(reg_lines).strip().encode())
         out_fp.write(b"\n")
 
@@ -125,48 +127,61 @@
         Args:
             src: Minidump file.
             dst: Location to save JSON file.
 
         Returns:
             A file containing JSON output.
         """
-        cmd = [self.MDSW_BIN, "--json"]
+        cmd = [self.MDSW_BIN, "--no-color", "--json"]
         if self._symbols_path:
             cmd.extend(["--symbols-path", str(self._symbols_path)])
         else:
             cmd.extend(["--symbols-url", "https://symbols.mozilla.org/"])
         cmd.append(str(src))
-        with NamedTemporaryFile(delete=False, dir=dst, prefix="mdsw_out_") as out_fp:
+        with NamedTemporaryFile(
+            dir=dst, prefix="mdsw_err_", suffix=".txt"
+        ) as err_fp, NamedTemporaryFile(
+            delete=False, dir=dst, prefix="mdsw_out_", suffix=".json"
+        ) as out_fp:
             LOG.debug("running %r", " ".join(cmd))
             try:
-                run(cmd, check=True, stderr=out_fp, stdout=out_fp, timeout=60)
+                run(cmd, check=True, stderr=err_fp, stdout=out_fp, timeout=60)
             except CalledProcessError as exc:
-                raise MinidumpStackwalkFailure(
-                    f"{self.MDSW_BIN!r} returned {exc.returncode!r} processing {src!s}"
-                ) from None
+                LOG.error("Failed to process: %s (%r)", src, exc.returncode)
+                # keep stderr file
+                err_fp.delete = False
+                err_fp.seek(0)
+                # use last line of stderr which should be the error message
+                err_msg: List[bytes] = err_fp.read().strip().splitlines() or [
+                    b"minidump-stackwalk failed"
+                ]
+                raise MinidumpStackwalkFailure(err_msg[-1]) from None
             except TimeoutExpired:
-                raise MinidumpStackwalkFailure(
-                    f"{self.MDSW_BIN!r} hung processing {src!s}"
-                ) from None
+                LOG.error("Failed to process: %s", src)
+                raise MinidumpStackwalkFailure("minidump-stackwalk hung") from None
             return Path(out_fp.name)
 
     @classmethod
-    def mdsw_available(cls) -> bool:
-        """Check if MDSW binary is available.
+    def mdsw_available(cls, force_check: bool = False) -> bool:
+        """Check if minidump-stackwalk binary is available.
 
         Args:
-            None
+            force_check: Always perform a check.
 
         Returns:
             True if binary is available otherwise False.
         """
-        try:
-            call([cls.MDSW_BIN], stdout=DEVNULL, stderr=DEVNULL)
-        except OSError:
-            return False
+        global MDSW_AVAILABLE  # pylint: disable=global-statement
+        if not MDSW_AVAILABLE or force_check:
+            try:
+                call([cls.MDSW_BIN], stdout=DEVNULL, stderr=DEVNULL)
+            except OSError:
+                LOG.debug("minidump-stackwalk not available (%s)", cls.MDSW_BIN)
+                return False
+            MDSW_AVAILABLE = True
         return True
 
 
 def process_minidumps(
     path: Path,
     symbols_path: Path,
     cb_create_log: Callable[..., Any],
@@ -196,15 +211,21 @@
         LOG.warning("Local packaged symbols not found: %r", str(symbols_path))
         local_symbols = False
 
     # create working path
     working_path = mkdtemp(prefix="minidump_", dir=working_path)
 
     md_parser = MinidumpParser(symbols_path=symbols_path if local_symbols else None)
-    for count, file in enumerate(path.glob("*.dmp")):
+    # order by last modified date hopefully the oldest log is the cause of the issue
+    dmp_files = sorted(path.glob("*.dmp"), key=lambda x: x.stat().st_mtime)
+    for count, file in enumerate(dmp_files):
+        # filter out zero byte files and warn
+        if file.stat().st_size == 0:
+            LOG.warning("Ignored zero byte minidump: %s", file)
+            continue
         try:
             # parse minidump with minidump-stackwalk
             md_json = md_parser.to_json(file, Path(working_path))
             # load json data from file to dict
             with md_json.open("rb") as json_fp:
                 md_data = load(json_fp)
             md_json.unlink()
```

### Comparing `ffpuppet-0.9.2/ffpuppet/puppet_logger.py` & `ffpuppet-0.9.3/src/ffpuppet/puppet_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     PREFIX_SAN = f"ffp_asan_{getpid()}.log"
     PREFIX_VALGRIND = f"valgrind.{getpid()}"
 
     __slots__ = ("_base", "_logs", "_rr_packed", "closed", "watching", "working_path")
 
     def __init__(self, base_path: Optional[str] = None) -> None:
         self._base = base_path
-        self._logs: Dict[str, IO[bytes]] = dict()
+        self._logs: Dict[str, IO[bytes]] = {}
         self._rr_packed = False
         self.closed = True
-        self.watching: Dict[str, int] = dict()
+        self.watching: Dict[str, int] = {}
         self.working_path: Optional[str] = None
         self.reset()
 
     def __enter__(self) -> "PuppetLogger":
         return self
 
     def __exit__(self, *exc: Any) -> None:
@@ -277,15 +277,15 @@
         assert self.closed, "save_logs() cannot be called before calling close()"
         assert self.working_path is not None
 
         # copy log to location specified by dest
         makedirs(dest, exist_ok=True)
         dest = abspath(dest)
 
-        meta_map = dict()
+        meta_map = {}
         for log_id, log_fp in self._logs.items():
             out_name = f"log_{log_id}.txt"
             if meta:
                 file_stat = stat(log_fp.name)
                 meta_map[out_name] = {
                     field: getattr(file_stat, field)
                     for field in dir(stat_result)
```

### Comparing `ffpuppet-0.9.2/ffpuppet/resources/testff.py` & `ffpuppet-0.9.3/src/ffpuppet/resources/testff.py`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/ffpuppet/sanitizer_util.py` & `ffpuppet-0.9.3/src/ffpuppet/sanitizer_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class SanitizerOptions:  # pylint: disable=missing-docstring
     re_delim = re_compile(r":(?![\\|/])")
 
     __slots__ = ("_options",)
 
     def __init__(self, options: Optional[str] = None) -> None:
-        self._options: Dict[str, str] = dict()
+        self._options: Dict[str, str] = {}
         if options is not None:
             self.load_options(options)
 
     def __contains__(self, item: str) -> bool:
         return item in self._options
 
     def __iter__(self) -> Iterator[Tuple[str, str]]:
```

### Comparing `ffpuppet-0.9.2/ffpuppet/test_bootstrapper.py` & `ffpuppet-0.9.3/src/ffpuppet/test_bootstrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # type: ignore
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 """ffpuppet bootstrapper tests"""
 # pylint: disable=protected-access
 
-from socket import AF_INET, SOCK_STREAM, error, socket, timeout
+from itertools import repeat
+from socket import socket, timeout
 from threading import Thread
 
 from pytest import mark, raises
 
 from .bootstrapper import Bootstrapper
 from .exceptions import BrowserTerminatedError, BrowserTimeoutError, LaunchError
 
@@ -17,21 +18,22 @@
 def test_bootstrapper_01():
     """test simple Bootstrapper()"""
     with Bootstrapper() as bts:
         assert bts._socket is not None
         assert bts.location.startswith("http://127.0.0.1:")
         assert int(bts.location.split(":")[-1]) > 1024
         assert bts.port > 1024
+        assert bts.port not in Bootstrapper.BLOCKED_PORTS
         bts.close()
         assert bts._socket is None
 
 
 def test_bootstrapper_02(mocker):
     """test Bootstrapper.wait() failure waiting for initial connection"""
-    fake_sock = mocker.Mock(spec_set=socket)
+    fake_sock = mocker.MagicMock(spec_set=socket)
     fake_sock.accept.side_effect = timeout
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
     with Bootstrapper() as bts:
         # test failure
         with raises(
             BrowserTerminatedError, match="Failure waiting for browser connection"
         ):
@@ -46,15 +48,15 @@
             bts.wait(lambda: True, timeout=0.1)
         # should call accept() at least 2x for positive and negative timeout check
         assert fake_sock.accept.call_count > 1
 
 
 def test_bootstrapper_03(mocker):
     """test Bootstrapper.wait() failure waiting for request"""
-    fake_sock = mocker.Mock(spec_set=socket)
+    fake_sock = mocker.MagicMock(spec_set=socket)
     fake_conn = mocker.Mock(spec_set=socket)
     fake_conn.recv.side_effect = timeout
     fake_sock.accept.return_value = (fake_conn, None)
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
     with Bootstrapper() as bts:
         # test failure
         with raises(BrowserTerminatedError, match="Failure waiting for request"):
@@ -69,15 +71,15 @@
         # should call recv() at least 2x for positive and negative timeout check
         assert fake_conn.recv.call_count > 1
         assert fake_conn.close.call_count == 1
 
 
 def test_bootstrapper_04(mocker):
     """test Bootstrapper.wait() failure sending response"""
-    fake_sock = mocker.Mock(spec_set=socket)
+    fake_sock = mocker.MagicMock(spec_set=socket)
     fake_conn = mocker.Mock(spec_set=socket)
     fake_conn.recv.return_value = "A"
     fake_conn.sendall.side_effect = timeout
     fake_sock.accept.return_value = (fake_conn, None)
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
     with Bootstrapper() as bts:
         # test timeout
@@ -93,15 +95,15 @@
         assert fake_conn.recv.call_count == 1
         assert fake_conn.sendall.call_count == 1
         assert fake_conn.close.call_count == 1
 
 
 def test_bootstrapper_05(mocker):
     """test Bootstrapper.wait() target crashed"""
-    fake_sock = mocker.Mock(spec_set=socket)
+    fake_sock = mocker.MagicMock(spec_set=socket)
     fake_conn = mocker.Mock(spec_set=socket)
     fake_conn.recv.return_value = "foo"
     fake_sock.accept.return_value = (fake_conn, None)
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
     with Bootstrapper() as bts:
         with raises(BrowserTerminatedError, match="Failure during browser startup"):
             bts.wait(lambda: False)
@@ -123,15 +125,15 @@
         (None, (timeout, timeout, "foo"), 1),
         # slow failed startup with retry
         (None, (timeout, "", "foo"), 2),
     ],
 )
 def test_bootstrapper_06(mocker, redirect, recv, closed):
     """test Bootstrapper.wait()"""
-    fake_sock = mocker.Mock(spec_set=socket)
+    fake_sock = mocker.MagicMock(spec_set=socket)
     fake_conn = mocker.Mock(spec_set=socket)
     fake_conn.recv.side_effect = recv
     fake_sock.accept.return_value = (fake_conn, None)
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
     with Bootstrapper() as bts:
         bts.wait(lambda: True, url=redirect)
     assert fake_conn.close.call_count == closed
@@ -139,15 +141,15 @@
     assert fake_conn.sendall.call_count == 1
 
 
 def test_bootstrapper_07():
     """test Bootstrapper.wait() with a fake browser"""
 
     def _fake_browser(port, payload_size=5120):
-        conn = socket(AF_INET, SOCK_STREAM)
+        conn = socket()
         # 50 x 0.1 = 5 seconds
         conn.settimeout(0.1)
         # open connection
         for attempt in reversed(range(50)):
             try:
                 conn.connect(("127.0.0.1", port))
                 break
@@ -168,16 +170,40 @@
         try:
             browser_thread.start()
             bts.wait(lambda: True, timeout=10)
         finally:
             browser_thread.join()
 
 
-def test_bootstrapper_08(mocker):
-    """test Bootstrapper() hit PORT_RETRIES"""
-    fake_sock = mocker.Mock(spec_set=socket)
-    fake_sock.bind.side_effect = error(10013, "TEST")
+@mark.parametrize(
+    "bind, attempts, raised",
+    [
+        # failed to bind (OSError)
+        ((OSError(0, "foo1"),), 1, LaunchError),
+        # failed to bind (PermissionError) - multiple attempts
+        (repeat(PermissionError(10013, "foo2"), 4), 4, LaunchError),
+    ],
+)
+def test_bootstrapper_08(mocker, bind, attempts, raised):
+    """test Bootstrapper() - failures"""
+    mocker.patch("ffpuppet.bootstrapper.sleep", autospec=True)
+    fake_sock = mocker.MagicMock(spec_set=socket)
+    fake_sock.bind.side_effect = bind
     mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
-    with raises(LaunchError, match="Could not find available port"):
-        with Bootstrapper():
+    with raises(raised):
+        with Bootstrapper(attempts=attempts):
             pass
-    assert fake_sock.bind.call_count == Bootstrapper.PORT_RETRIES
+    assert fake_sock.bind.call_count == attempts
+    assert fake_sock.close.call_count == attempts
+
+
+def test_bootstrapper_09(mocker):
+    """test Bootstrapper() - blocked ports"""
+    fake_sock = mocker.MagicMock(spec_set=socket)
+    fake_sock.getsockname.side_effect = (
+        (None, Bootstrapper.BLOCKED_PORTS[0]),
+        (None, 12345),
+    )
+    mocker.patch("ffpuppet.bootstrapper.socket.socket", return_value=fake_sock)
+    with Bootstrapper(attempts=2):
+        pass
+    assert fake_sock.close.call_count == 2
```

### Comparing `ffpuppet-0.9.2/ffpuppet/test_checks.py` & `ffpuppet-0.9.3/src/ffpuppet/test_checks.py`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/ffpuppet/test_ffpuppet.py` & `ffpuppet-0.9.3/src/ffpuppet/test_ffpuppet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 """ffpuppet tests"""
 
 import os
 from errno import EADDRINUSE
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import Path
 from platform import system
-from shutil import rmtree
 from stat import S_IREAD, S_IWRITE
 from subprocess import Popen
 from threading import Thread
 from time import sleep
 
 from psutil import Process
 from pytest import mark, raises
 
 from .bootstrapper import Bootstrapper
 from .core import Debugger, FFPuppet, Reason
 from .exceptions import (
+    BrowserExecutionError,
     BrowserTerminatedError,
     BrowserTimeoutError,
     LaunchError,
     TerminateError,
 )
+from .profile import Profile
 
 Bootstrapper.POLL_WAIT = 0.2
 TESTFF_BIN = str((Path(__file__).parent / "resources" / "testff.py").resolve())
 
 
 class ReqHandler(BaseHTTPRequestHandler):
     def do_GET(self):
@@ -104,38 +105,40 @@
         assert ffp.reason == Reason.CLOSED
         assert ffp._proc is None
         assert not ffp.is_running()
         assert not ffp.is_healthy()
         assert ffp.wait(timeout=10)
 
 
-def test_ffpuppet_02(mocker):
+@mark.parametrize(
+    "exc_type",
+    [
+        # startup crash
+        BrowserTerminatedError,
+        # startup hang
+        BrowserTimeoutError,
+    ],
+)
+def test_ffpuppet_02(mocker, exc_type):
     """test launch failures"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
     mocker.patch("ffpuppet.core.Popen", autospec=True)
     fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
-    bts = mocker.Mock(spec_set=Bootstrapper, location="")
-    fake_bts.return_value = bts
-    # startup crash
-    with FFPuppet() as ffp:
-        bts.wait.side_effect = BrowserTerminatedError("test")
-        with raises(BrowserTerminatedError, match="test"):
-            ffp.launch(TESTFF_BIN)
-        assert not ffp.is_running()
-        assert ffp.launches == 0
-    # startup hang
+    fake_bts.return_value.location = ""
+    fake_bts.return_value.wait.side_effect = exc_type("test")
     with FFPuppet() as ffp:
-        bts.wait.side_effect = BrowserTimeoutError("test")
-        with raises(BrowserTimeoutError, match="test"):
+        with raises(exc_type, match="test"):
             ffp.launch(TESTFF_BIN)
         assert not ffp.is_healthy()
         assert ffp.launches == 0
 
 
-def test_ffpuppet_03(tmp_path):
+def test_ffpuppet_03(mocker, tmp_path):
     """test logging"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
     with FFPuppet() as ffp:
         ffp.close()
         ffp.save_logs(str(tmp_path / "no_logs"))
         prefs = tmp_path / "prefs.js"
         prefs.write_bytes(b"//fftest_exit_code_0\n")
         with HTTPTestServer() as srv:
             ffp.launch(TESTFF_BIN, location=srv.get_addr(), prefs_js=str(prefs))
@@ -241,14 +244,15 @@
                 if os.path.isfile(rnd_log):
                     os.remove(rnd_log)
         ffp.clean_up()
         # verify clean_up() removed the logs
         assert ffp.clone_log("stdout", target_file=str(logs)) is None
 
 
+@mark.skipif(system() == "Windows", reason="Unsupported on Windows")
 def test_ffpuppet_08(tmp_path):
     """test hitting memory limit"""
     with FFPuppet() as ffp:
         prefs = tmp_path / "prefs.js"
         prefs.write_bytes(b"//fftest_memory\n")
         with HTTPTestServer() as srv:
             # launch with 1MB memory limit
@@ -334,14 +338,15 @@
                 ffp.launch(TESTFF_BIN, location=srv.get_addr())
             with raises(AssertionError):
                 ffp.close()
 
 
 def test_ffpuppet_13(mocker):
     """test launching under Xvfb"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
     mocker.patch("ffpuppet.core.Popen", autospec=True)
     fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
     fake_bts.return_value.location = "http://test:123"
     fake_system = mocker.patch("ffpuppet.core.system", autospec=True)
     is_linux = system() == "Linux"
     fake_xvfb = mocker.patch(
         "ffpuppet.core.Xvfb", autospec=is_linux, create=not is_linux
@@ -363,16 +368,17 @@
     # not installed
     fake_xvfb.side_effect = NameError
     with raises(OSError, match="Please install xvfbwrapper"):
         FFPuppet(headless="xvfb")
     assert fake_xvfb.start.call_count == 0
 
 
-def test_ffpuppet_14(tmp_path):
+def test_ffpuppet_14(mocker, tmp_path):
     """test passing a file and a non existing file to launch() via location"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
     with FFPuppet() as ffp:
         with raises(OSError, match="Cannot find"):
             ffp.launch(TESTFF_BIN, location="missing.file")
         ffp.close()
         prefs = tmp_path / "prefs.js"
         prefs.write_bytes(b"//fftest_exit_code_0\n")
         test_file = tmp_path / "test_file"
@@ -399,15 +405,15 @@
 
 def test_ffpuppet_15(mocker, tmp_path):
     """test launching with gdb"""
     mocker.patch("ffpuppet.core.check_output", autospec=True)
     mocker.patch(
         "ffpuppet.core.get_processes",
         autospec=True,
-        return_value=[mocker.Mock(spec=Process)],
+        return_value=(mocker.Mock(spec=Process),),
     )
     mocker.patch("ffpuppet.core.system", autospec=True, return_value="Linux")
     fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
     fake_bts.return_value.location = "http://test:123"
     fake_proc = mocker.patch("ffpuppet.core.Popen", autospec=True)
     fake_proc.return_value.pid = 0xFFFF
     fake_proc.return_value.poll.return_value = None
@@ -437,15 +443,15 @@
     """test launching with Valgrind"""
     mocker.patch(
         "ffpuppet.core.check_output", autospec=True, return_value=b"valgrind-99.0"
     )
     mocker.patch(
         "ffpuppet.core.get_processes",
         autospec=True,
-        return_value=[mocker.Mock(spec=Process)],
+        return_value=(mocker.Mock(spec=Process),),
     )
     mocker.patch("ffpuppet.core.system", autospec=True, return_value="Linux")
     fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
     fake_bts.return_value.location = "http://test:123"
     fake_proc = mocker.patch("ffpuppet.core.Popen", autospec=True)
     fake_proc.return_value.pid = 0xFFFF
     fake_proc.return_value.poll.return_value = None
@@ -488,15 +494,15 @@
         ffp.clean_up()
         # verify clean_up() removed the logs
         assert ffp.log_length("stderr") is None
 
 
 def test_ffpuppet_20():
     """test running multiple instances in parallel"""
-    ffps = list()
+    ffps = []
     try:
         with HTTPTestServer() as srv:
             # use test pool size of 10
             for _ in range(10):
                 ffps.append(FFPuppet())
                 # NOTE: launching truly in parallel can DoS the test webserver
                 ffps[-1].launch(TESTFF_BIN, location=srv.get_addr())
@@ -531,17 +537,19 @@
         assert sum(x.stat().st_size for x in logfiles) > limit
         assert (
             b"LOG_SIZE_LIMIT_EXCEEDED"
             in (logs / "log_ffp_worker_log_size.txt").read_bytes()
         )
 
 
-def test_ffpuppet_22(tmp_path):
+def test_ffpuppet_22(mocker, tmp_path):
     """test collecting and cleaning up ASan logs"""
-    test_logs = list()
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
+    mocker.patch("ffpuppet.core.wait_on_files", autospec=True)
+    test_logs = []
     with FFPuppet() as ffp:
         ffp.launch(TESTFF_BIN)
         assert ffp._logs.working_path is not None
         asan_prefix = os.path.join(ffp._logs.working_path, ffp._logs.PREFIX_SAN)
         for i in range(4):
             test_logs.append(".".join([asan_prefix, str(i)]))
         # ignore benign ASan warning
@@ -594,31 +602,33 @@
                     "==123==WARNING: Symbolizer buffer too small",
                 )
     assert not any(os.path.isfile(f) for f in test_logs)
 
 
 def test_ffpuppet_23(mocker, tmp_path):
     """test multiple minidumps"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
+    mocker.patch("ffpuppet.core.wait_on_files", autospec=True)
 
     # pylint: disable=unused-argument
     def _fake_process_minidumps(dmps, _, add_log, working_path=None):
         for num, _ in enumerate(x for x in os.listdir(dmps) if x.endswith(".dmp")):
             lfp = add_log(f"minidump_{num + 1:02}")
             lfp.write(b"test")
 
     mocker.patch("ffpuppet.core.process_minidumps", side_effect=_fake_process_minidumps)
     profile = tmp_path / "profile"
     profile.mkdir()
     (profile / "minidumps").mkdir()
     with FFPuppet(use_profile=str(profile)) as ffp:
         ffp.launch(TESTFF_BIN)
-        ffp._bin_path = ffp.profile
+        ffp._bin_path = str(ffp.profile.path)
         assert ffp._bin_path is not None
         # create "test.dmp" files
-        md_path = Path(ffp._bin_path) / "minidumps"
+        md_path = ffp.profile.path / "minidumps"
         (md_path / "test1.dmp").write_text("1a\n1b")
         (md_path / "test2.dmp").write_text("2a\n2b")
         (md_path / "test3.dmp").write_text("3a\n3b")
         assert not ffp.is_healthy()
         # close fake browser process before calling close to avoid hang
         Process(ffp.get_pid()).terminate()
         ffp.close()
@@ -631,15 +641,15 @@
 
 def test_ffpuppet_24(mocker, tmp_path):
     """test launching with rr"""
     mocker.patch("ffpuppet.core.check_output", autospec=True)
     mocker.patch(
         "ffpuppet.core.get_processes",
         autospec=True,
-        return_value=[mocker.Mock(spec=Process)],
+        return_value=(mocker.Mock(spec=Process),),
     )
     mocker.patch("ffpuppet.core.system", autospec=True, return_value="Linux")
     fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
     fake_bts.return_value.location = "http://test:123"
     fake_proc = mocker.patch("ffpuppet.core.Popen", autospec=True)
     fake_proc.return_value.pid = 0xFFFF
     fake_proc.return_value.poll.return_value = None
@@ -659,69 +669,66 @@
 def test_ffpuppet_25(tmp_path):
     """test rmtree error handler"""
     # normal profile creation
     # - just create a puppet, write a readonly file in its profile, then call close()
     with FFPuppet() as ffp:
         ffp.launch(TESTFF_BIN)
         assert ffp.profile is not None
-        ro_file = Path(ffp.profile) / "read-only-test.txt"
+        ro_file = ffp.profile.path / "read-only-test.txt"
         ro_file.touch()
         ro_file.chmod(S_IREAD)
         ffp.close()
-        assert not os.path.isfile(ro_file)
+        assert not ro_file.is_file()
         ffp.clean_up()
     # use template profile that contains a readonly file
     profile = tmp_path / "profile"
     profile.mkdir()
     ro_file = profile / "read-only.txt"
     ro_file.touch()
     ro_file.chmod(S_IREAD)
     with FFPuppet(use_profile=str(profile)) as ffp:
         ffp.launch(TESTFF_BIN)
         assert ffp.profile is not None
-        prof_path = ffp.profile
-        assert os.path.isdir(prof_path)
+        prof_path = ffp.profile.path
+        assert prof_path.is_dir()
         ffp.close()
-        assert not os.path.isdir(prof_path)
+        assert not prof_path.is_dir()
 
 
 def test_ffpuppet_26(tmp_path):
     """test using a readonly prefs.js and extension"""
     prefs = tmp_path / "prefs.js"
     prefs.touch()
     prefs.chmod(S_IREAD)
     ext = tmp_path / "ext.xpi"
     ext.touch()
     ext.chmod(S_IREAD)
     with FFPuppet() as ffp:
         ffp.launch(TESTFF_BIN, extension=str(ext), prefs_js=str(prefs))
-        prof_path = ffp.profile
+        prof_path = ffp.profile.path
         ffp.close()
         assert prof_path is not None
-        assert not os.path.isdir(prof_path)
+        assert not prof_path.is_dir()
 
 
 def test_ffpuppet_27(mocker, tmp_path):
     """test _crashreports()"""
     mocker.patch(
         "ffpuppet.core.check_output", autospec=True, return_value=b"valgrind-99.0"
     )
 
     class StubbedLaunch(FFPuppet):
         # pylint: disable=arguments-differ
         def launch(self):
-            profile = tmp_path / "profile"
-            profile.mkdir()
-            (profile / "minidumps").mkdir()
-            self.profile = str(profile)
+            self.profile = Profile(working_path=tmp_path)
+            (self.profile.path / "minidumps").mkdir()
 
         def close(self, force_close=False):
             assert self.profile is not None
-            if os.path.isdir(self.profile):
-                rmtree(self.profile)
+            self.profile.remove()
             self.profile = None
 
     is_linux = system() == "Linux"
     # only check Valgrind logs on Linux
     debugger = Debugger.VALGRIND if is_linux else Debugger.NONE
     with StubbedLaunch(debugger=debugger) as ffp:
         assert ffp._dbg == debugger
@@ -745,17 +752,17 @@
         vg1_log.write_text("test\n")
         # valid Valgrind log - without error
         (Path(ffp._logs.working_path) / (f"{ffp._logs.PREFIX_VALGRIND}.2")).touch()
         # nothing interesting
         (Path(ffp._logs.working_path) / "junk.log").write_text("test\n")
         # valid minidump
         assert ffp.profile is not None
-        (Path(ffp.profile) / "minidumps" / "test.dmp").write_text("test\n")
+        (ffp.profile.path / "minidumps" / "test.dmp").write_text("test\n")
         # nothing interesting
-        (Path(ffp.profile) / "minidumps" / "test.junk").write_text("\n")
+        (ffp.profile.path / "minidumps" / "test.junk").write_text("\n")
         assert not ffp._logs.watching
         assert len(list(ffp._crashreports())) == (3 if is_linux else 2)
         assert ffp._logs.watching
         assert len(list(ffp._crashreports(skip_md=True))) == (2 if is_linux else 1)
         if system() != "Windows":
             # fail to open (for read) and scan sanitizer file
             # not tested on Windows because chmod() does not work
@@ -889,15 +896,14 @@
 
 def test_ffpuppet_31(mocker):
     """test _terminate()"""
     procs = [
         mocker.Mock(spec_set=Process, pid=123),
         mocker.Mock(spec_set=Process, pid=124),
     ]
-    mocker.patch("ffpuppet.core.get_processes", autospec=True)
     fake_wait_procs = mocker.patch("ffpuppet.core.wait_procs", autospec=True)
     # successful call to terminate
     fake_wait_procs.side_effect = (([], []),)
     FFPuppet._terminate(procs)
     assert sum(x.terminate.call_count for x in procs) == 2
     assert not sum(x.kill.call_count for x in procs)
     for proc in procs:
@@ -915,35 +921,37 @@
         FFPuppet._terminate(procs)
     assert sum(x.terminate.call_count for x in procs) == 2
     assert sum(x.kill.call_count for x in procs) == 2
 
 
 def test_ffpuppet_32(mocker, tmp_path):
     """test FFPuppet.close() setting reason"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
 
     class StubbedProc(FFPuppet):
         # pylint: disable=arguments-differ
         def launch(self):
             self.reason = None
             self._bin_path = str(tmp_path)
             self._logs.reset()
             self._logs.add_log("stderr")
             self._proc = mocker.Mock(spec=Popen, pid=123)
             self._proc.poll.return_value = None
             profile = tmp_path / "profile"
             profile.mkdir(exist_ok=True)
-            self.profile = str(profile)
+            self.profile = Profile(working_path=profile)
 
-        def _terminate(self, _procs, _retry_delay=0, _use_kill=False):
+        @staticmethod
+        def _terminate(_procs, _retry_delay=0, _use_kill=False):
             pass
 
     mocker.patch(
         "ffpuppet.core.get_processes",
         autospec=True,
-        return_value=[mocker.Mock(spec_set=Process)],
+        return_value=(mocker.Mock(spec=Process),),
     )
     fake_reports = mocker.patch("ffpuppet.core.FFPuppet._crashreports", autospec=True)
     fake_reports.return_value = ()
     fake_wait_files = mocker.patch("ffpuppet.core.wait_on_files", autospec=True)
     fake_wait_procs = mocker.patch("ffpuppet.core.wait_procs", autospec=True)
     # process exited - no crash
     fake_wait_procs.side_effect = (([], []),)
@@ -1017,11 +1025,52 @@
         assert san_log in ffp._logs.watching
         ffp.close()
         assert ffp.reason == Reason.CLOSED
 
 
 def test_ffpuppet_34(mocker):
     """test secondary process lookup scan in close()"""
-    fake_get_proc = mocker.patch("ffpuppet.core.get_processes", return_value=[])
+    fake_get_proc = mocker.patch("ffpuppet.core.get_processes", return_value=())
     with FFPuppet() as ffp:
         ffp.launch(TESTFF_BIN)
     assert fake_get_proc.call_count == 1
+
+
+@mark.parametrize(
+    "bin_exists, expect_exc",
+    [
+        # failed to execute binary
+        (True, BrowserExecutionError),
+        # missing binary
+        (False, FileNotFoundError),
+    ],
+)
+def test_ffpuppet_35(mocker, tmp_path, bin_exists, expect_exc):
+    """test Popen failure during launch"""
+    bin_fake = tmp_path / "fake_bin"
+    if bin_exists:
+        bin_fake.touch()
+    exc = FileNotFoundError()
+    exc.filename = str(bin_fake)
+    mocker.patch("ffpuppet.core.Popen", autospec=True, side_effect=exc)
+    fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
+    fake_bts.return_value.location = ""
+    with FFPuppet() as ffp:
+        with raises(expect_exc):
+            ffp.launch(TESTFF_BIN)
+        assert not ffp.is_healthy()
+        assert ffp.launches == 0
+
+
+@mark.skipif(system() != "Windows", reason="Only supported on Windows")
+def test_ffpuppet_36(mocker):
+    """test FFPuppet.launch() config_job_object code path"""
+    mocker.patch("ffpuppet.core.files_in_use", autospec=True)
+    fake_bts = mocker.patch("ffpuppet.core.Bootstrapper", autospec=True)
+    fake_bts.return_value.location = ""
+    fake_popen = mocker.patch("ffpuppet.core.Popen", autospec=True)
+    fake_popen.return_value._handle = 123
+    config_job_object = mocker.patch("ffpuppet.core.config_job_object", autospec=True)
+    with FFPuppet() as ffp:
+        ffp.launch(TESTFF_BIN, memory_limit=456)
+    assert config_job_object.call_count == 1
+    assert config_job_object.mock_calls[0] == mocker.call(123, 456)
```

### Comparing `ffpuppet-0.9.2/ffpuppet/test_main.py` & `ffpuppet-0.9.3/src/ffpuppet/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,64 +3,68 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 """ffpuppet main.py tests"""
 
 from pytest import mark, raises
 
 from .core import Reason
+from .exceptions import BrowserExecutionError
 from .main import dump_to_console, main, parse_args
+from .profile import Profile
 
 
 @mark.parametrize(
-    "reason, user_exit, extra_args",
+    "reason, launch, is_healthy, extra_args",
     [
         # browser exit
-        (Reason.EXITED, False, ["-d", "--save-all"]),
+        (Reason.EXITED, None, (False,), ["-d", "--save-all"]),
         # browser exit - more flags
-        (Reason.EXITED, False, ["-a", "token", "--log-level", "DEBUG"]),
+        (Reason.EXITED, None, (False,), ["-a", "token", "--log-level", "DEBUG"]),
+        # cannot launch browser binary
+        (Reason.CLOSED, (BrowserExecutionError(),), None, []),
         # browser crash
-        (Reason.ALERT, False, []),
+        (Reason.ALERT, None, (False,), []),
         # user exit
-        (Reason.CLOSED, True, []),
+        (Reason.CLOSED, None, (True, KeyboardInterrupt()), []),
         # exception
-        (None, False, []),
+        (None, None, (False,), []),
     ],
 )
-def test_main_01(mocker, tmp_path, reason, user_exit, extra_args):
+def test_main_01(mocker, tmp_path, reason, launch, is_healthy, extra_args):
     """test main()"""
+    mocker.patch("ffpuppet.main.sleep", autospec=True)
     fake_ffp = mocker.patch("ffpuppet.main.FFPuppet", autospec=True)
     fake_ffp.return_value.get_pid.return_value = 12345
-    fake_ffp.return_value.is_healthy.return_value = user_exit
-    fake_ffp.return_value.profile = str(tmp_path)
+    fake_ffp.return_value.is_healthy.side_effect = is_healthy
+    fake_ffp.return_value.launch.side_effect = launch
+    fake_ffp.return_value.profile = mocker.Mock(spec_set=Profile, path=tmp_path)
     fake_ffp.return_value.reason = reason
-    mocker.patch("ffpuppet.main.sleep", autospec=True, side_effect=KeyboardInterrupt)
     out_logs = tmp_path / "logs"
     out_logs.mkdir()
     prefs = tmp_path / "prefs.js"
     prefs.touch()
     fake_bin = tmp_path / "fake.bin"
     fake_bin.touch()
     args = [str(fake_bin), "-l", str(out_logs), "-p", str(prefs)]
     main(args + extra_args)
     if "-a" in extra_args:
         assert fake_ffp.return_value.add_abort_token.call_count == 1
     else:
         assert fake_ffp.return_value.add_abort_token.call_count == 0
-    assert fake_ffp.return_value.get_pid.call_count == 1
-    assert fake_ffp.return_value.is_healthy.call_count == 1
     assert fake_ffp.return_value.close.call_count == 1
     if "--save-all" in extra_args or Reason.ALERT:
         assert fake_ffp.return_value.save_logs.call_count == 1
     else:
         assert fake_ffp.return_value.save_logs.call_count == 0
     assert fake_ffp.return_value.clean_up.call_count == 1
 
 
-def test_parse_args_01(tmp_path):
+def test_parse_args_01(mocker, tmp_path):
     """test parse_args()"""
+    certutil_avail = mocker.patch("ffpuppet.main.certutil_available", autospec=True)
     with raises(SystemExit):
         parse_args(["-h"])
     # invalid/missing binary
     with raises(SystemExit):
         parse_args(["fake_bin"])
     fake_bin = tmp_path / "fake.bin"
     fake_bin.touch()
@@ -72,14 +76,22 @@
         parse_args([str(fake_bin), "--memory", "-1"])
     # missing prefs
     with raises(SystemExit):
         parse_args([str(fake_bin), "-p", str(tmp_path / "missing")])
     # missing extension
     with raises(SystemExit):
         parse_args([str(fake_bin), "-e", str(tmp_path / "missing")])
+    # missing certificate
+    certutil_avail.return_value = True
+    with raises(SystemExit):
+        parse_args([str(fake_bin), "--cert", str(tmp_path / "missing")])
+    # missing certutil
+    certutil_avail.return_value = False
+    with raises(SystemExit):
+        parse_args([str(fake_bin), "--cert", str(fake_bin)])
     # multiple debuggers
     with raises(SystemExit):
         parse_args([str(fake_bin), "--gdb", "--valgrind"])
     # invalid log path
     (tmp_path / "junk.log").touch()
     with raises(SystemExit):
         parse_args([str(fake_bin), "--logs", "/missing/path/"])
```

### Comparing `ffpuppet-0.9.2/ffpuppet/test_minidump_parser.py` & `ffpuppet-0.9.3/src/ffpuppet/test_minidump_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,50 +145,60 @@
 
 @mark.parametrize(
     "call_result, result",
     [
         # minidump-stackwalk is available
         ((0,), True),
         # minidump-stackwalk is not available
-        (OSError, False),
+        (OSError("test"), False),
     ],
 )
 def test_minidump_parser_04(mocker, call_result, result):
     """test MinidumpParser.mdsw_available()"""
     mocker.patch("ffpuppet.minidump_parser.call", side_effect=call_result)
-    assert MinidumpParser.mdsw_available() == result
+    assert MinidumpParser.mdsw_available(force_check=True) == result
 
 
 @mark.parametrize(
-    "mdsw, syms, bad_json",
+    "mdsw, syms, md_json_data, raised",
     [
         # loading minidump files - success
-        (True, True, False),
+        (True, True, ["{}"], False),
         # loading minidump files - JSONDecodeError
-        (True, True, True),
+        (True, True, ["bad,json"], True),
+        # loading minidump files - zero byte minidumps
+        (True, True, ["", "{}", ""], False),
         # symbols_path does not exist
-        (True, False, False),
+        (True, False, ["{}"], False),
         # test minidump-stackwalk not available
-        (False, False, False),
+        (False, False, [], False),
     ],
 )
-def test_process_minidumps_01(mocker, tmp_path, mdsw, syms, bad_json):
+def test_process_minidumps_01(mocker, tmp_path, mdsw, syms, md_json_data, raised):
     """test process_minidumps()"""
     fake_mdp = mocker.patch("ffpuppet.minidump_parser.MinidumpParser", autospec=True)
     fake_mdp.mdsw_available.return_value = mdsw
-    (tmp_path / "minidump.dmp").write_text("bad,json" if bad_json else "{}")
-    fake_mdp.return_value.to_json.return_value = tmp_path / "minidump.dmp"
+
+    to_json_results = []
+    for count, md_data in enumerate(md_json_data):
+        md_file = tmp_path / f"minidump{count:02d}.dmp"
+        md_file.write_text(md_data)
+        if md_data:
+            to_json_results.append(md_file)
+    fake_mdp.return_value.to_json.side_effect = to_json_results
+
     try:
         process_minidumps(
             tmp_path,
             tmp_path if syms else tmp_path / "missing",
             mocker.Mock(),
             working_path=str(tmp_path),
         )
     except JSONDecodeError:
-        assert bad_json
+        assert raised
     else:
-        assert not bad_json
+        assert not raised
+
     assert fake_mdp.mdsw_available.call_count == 1
     if mdsw:
         assert fake_mdp.return_value.to_json.call_count == 1
-        assert fake_mdp.return_value.format_output.call_count == (0 if bad_json else 1)
+        assert fake_mdp.return_value.format_output.call_count == (0 if raised else 1)
```

### Comparing `ffpuppet-0.9.2/ffpuppet/test_puppet_logger.py` & `ffpuppet-0.9.3/src/ffpuppet/test_puppet_logger.py`

 * *Files identical despite different names*

### Comparing `ffpuppet-0.9.2/ffpuppet/test_sanitizer_util.py` & `ffpuppet-0.9.3/src/ffpuppet/test_sanitizer_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 from .sanitizer_util import SanitizerOptions
 
 
 @mark.parametrize(
     "init, add, result, overwrite",
     [
         # do nothing
-        ("", dict(), [""], False),
+        ("", {}, [""], False),
         # add single option
         ("", {"a": "1"}, ["a=1"], False),
         # add multiple options
         ("", {"b": "2", "a": "1"}, ["a=1", "b=2"], False),
         # existing
-        ("a=1", dict(), ["a=1"], False),
+        ("a=1", {}, ["a=1"], False),
         # add to existing
         ("a=1", {"b": "2"}, ["a=1", "b=2"], False),
         # no overwrite existing
         ("a=1", {"a": "2"}, ["a=1"], False),
         # overwrite existing
         ("a=1", {"a": "2"}, ["a=2"], True),
         # parse quoted
         (
             "a='C:\\test\\':b=\"/dev/null\"",
-            dict(),
+            {},
             ["a='C:\\test\\'", 'b="/dev/null"'],
             False,
         ),
     ],
 )
 def test_sanitizer_options_01(init, add, result, overwrite):
     """test SanitizerOptions() - parsing and adding"""
```

### Comparing `ffpuppet-0.9.2/ffpuppet.egg-info/PKG-INFO` & `ffpuppet-0.9.3/src/ffpuppet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ffpuppet
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python module that aids in the automation of Firefox at the process level
 Home-page: https://github.com/MozillaSecurity/ffpuppet
 Author: Tyson Smith
 Author-email: twsmith@mozilla.com
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: automation firefox fuzz fuzzing security test testing
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 FFPuppet
 ========
```

### Comparing `ffpuppet-0.9.2/pyproject.toml` & `ffpuppet-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-lines",
     "too-many-locals",
     "too-many-nested-blocks",
     "too-many-statements",
+    "unspecified-encoding",
 ]
 
 [tool.pylint.typecheck]
 ignored-modules = ["pytest"]
 
 [tool.pytest.ini_options]
 log_level = "DEBUG"
```

### Comparing `ffpuppet-0.9.2/setup.cfg` & `ffpuppet-0.9.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 url = https://github.com/MozillaSecurity/ffpuppet
 
 [options]
 include_package_data = True
 install_requires = 
 	psutil >= 4.4.0
 	xvfbwrapper >= 0.2.9; sys_platform == "linux" or sys_platform == "linux2"
+package_dir = 
+	= src
 packages = 
 	ffpuppet
-python_requires = >=3.6
+python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
 	ffpuppet = ffpuppet.main:main
 
 [options.extras_require]
```

### Comparing `ffpuppet-0.9.2/tox.ini` & `ffpuppet-0.9.3/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tox]
-envlist = py{36,37,38,39,310},lint
+envlist = py{38,39,310,311},lint
 skip_missing_interpreters = true
 tox_pip_extensions_ext_venv_update = true
 
 [testenv]
-commands = pytest -v --cache-clear --cov="{toxinidir}" --cov-config="{toxinidir}/pyproject.toml" --cov-report term-missing --basetemp="{envtmpdir}" {posargs} --disable-pytest-warnings
+commands = pytest -v --cache-clear --cov={toxinidir} --cov-config={toxinidir}/pyproject.toml --cov-report=term-missing --basetemp={envtmpdir} {posargs} --disable-pytest-warnings
 deps =
     pytest
     pytest-cov
     pytest-mock
 passenv =
     BUILD_CACHE
     CI
@@ -21,37 +21,38 @@
     VCS_*
 usedevelop = true
 
 [testenv:codecov]
 commands =
     codecov
 deps =
-    codecov
     coverage[toml]
 skip_install = true
+allowlist_externals =
+    codecov
 
 [testenv:lint]
 commands =
     pre-commit run -a {posargs}
 deps =
     pre-commit
 skip_install = true
 
 [testenv:mypy]
 commands =
     mypy --install-types --non-interactive {posargs}
 deps =
-    mypy==v0.942
+    mypy==v0.991
 usedevelop = true
 
 [testenv:pylint]
 commands =
     pylint {posargs}
 deps =
-    pylint==2.9.6
+    pylint==2.15.10
     pytest-mock
 usedevelop = true
 
 [testenv:pypi]
 commands =
     python setup.py sdist bdist_wheel
     twine upload --skip-existing dist/*
@@ -59,15 +60,15 @@
     setuptools>=43
     setuptools_scm[toml]>=3.4
     twine
     wheel
 skip_install = true
 
 [flake8]
+# E203, W503, and W504 are all black compat
 ignore =
-    E203  # black compat
-    W503  # black compat
+    E203
+    W503
 enable =
-    W504  # black compat
+    W504
 max-line-length = 88
 show-source = true
-statistics = true
```

