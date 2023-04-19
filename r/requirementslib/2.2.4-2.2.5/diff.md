# Comparing `tmp/requirementslib-2.2.4.tar.gz` & `tmp/requirementslib-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirementslib-2.2.4.tar", last modified: Fri Mar 17 22:01:12 2023, max compression
+gzip compressed data, was "requirementslib-2.2.5.tar", last modified: Wed Apr 19 10:36:01 2023, max compression
```

## Comparing `requirementslib-2.2.4.tar` & `requirementslib-2.2.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.592600 requirementslib-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35195 2023-03-17 22:00:39.000000 requirementslib-2.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-17 22:00:39.000000 requirementslib-2.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-17 22:00:39.000000 requirementslib-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-17 22:00:39.000000 requirementslib-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-03-17 22:01:12.592600 requirementslib-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-03-17 22:00:39.000000 requirementslib-2.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.588600 requirementslib-2.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.lockfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.pipfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.resolvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.setup_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.models.vcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-17 22:00:39.000000 requirementslib-2.2.4/docs/requirementslib.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-17 22:00:39.000000 requirementslib-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-17 22:01:12.592600 requirementslib-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-17 22:00:39.000000 requirementslib-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.584600 requirementslib-2.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.588600 requirementslib-2.2.4/src/requirementslib/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/funktools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.592600 requirementslib-2.2.4/src/requirementslib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    26748 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44137 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/old_pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/pipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)   119687 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    55401 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/setup_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    34664 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/models/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25755 2023-03-17 22:00:39.000000 requirementslib-2.2.4/src/requirementslib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:01:12.592600 requirementslib-2.2.4/src/requirementslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-03-17 22:01:12.000000 requirementslib-2.2.4/src/requirementslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-17 22:01:12.000000 requirementslib-2.2.4/src/requirementslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:01:12.000000 requirementslib-2.2.4/src/requirementslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-17 22:01:12.000000 requirementslib-2.2.4/src/requirementslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-17 22:01:12.000000 requirementslib-2.2.4/src/requirementslib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:00:43.000000 requirementslib-2.2.4/src/requirementslib.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.765479 requirementslib-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35440 2023-04-19 10:35:19.000000 requirementslib-2.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-19 10:35:19.000000 requirementslib-2.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 10:35:19.000000 requirementslib-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-19 10:35:19.000000 requirementslib-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-19 10:36:01.765479 requirementslib-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-19 10:35:19.000000 requirementslib-2.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.lockfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.pipfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.resolvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.setup_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 10:35:19.000000 requirementslib-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-19 10:36:01.765479 requirementslib-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-19 10:35:19.000000 requirementslib-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.753478 requirementslib-2.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/src/requirementslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/funktools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.765479 requirementslib-2.2.5/src/requirementslib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44137 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/old_pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/pipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119687 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55679 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/setup_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34664 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25755 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/src/requirementslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:35:24.000000 requirementslib-2.2.5/src/requirementslib.egg-info/zip-safe
```

### Comparing `requirementslib-2.2.4/CHANGELOG.rst` & `requirementslib-2.2.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Requirementslib 2.2.5 (2023-04-19)
+==================================
+
+
+Vendored Libraries
+------------------
+
+- Update ``WheelCache`` usage to be compatible with ``pip==23.1``  `#363 <https://github.com/sarugaku/requirementslib/issues/363>`_
+
+
 Requirementslib 2.2.4 (2023-03-17)
 ==================================
 
 
 Requirementslib 2.2.4 (2023-03-17)
 ==================================
```

### Comparing `requirementslib-2.2.4/CONTRIBUTING.rst` & `requirementslib-2.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/LICENSE` & `requirementslib-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/MANIFEST.in` & `requirementslib-2.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/PKG-INFO` & `requirementslib-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.2.4
+Version: 2.2.5
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.2.4/README.rst` & `requirementslib-2.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/docs/Makefile` & `requirementslib-2.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/docs/conf.py` & `requirementslib-2.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/docs/make.bat` & `requirementslib-2.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/docs/requirementslib.models.rst` & `requirementslib-2.2.5/docs/requirementslib.models.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/pyproject.toml` & `requirementslib-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/setup.cfg` & `requirementslib-2.2.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 zip_safe = true
 python_requires = >=3.7
 install_requires = 
 	attrs>=19.2
 	cached_property
 	distlib>=0.2.8
 	pep517>=0.5.0
-	pip>=22.2
+	pip>=23.1
 	platformdirs
 	plette[validation]
 	requests
 	setuptools>=40.8
 	tomlkit>=0.5.3
 	vistir==0.8.0
```

### Comparing `requirementslib-2.2.4/setup.py` & `requirementslib-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/exceptions.py` & `requirementslib-2.2.5/src/requirementslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/funktools.py` & `requirementslib-2.2.5/src/requirementslib/funktools.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/cache.py` & `requirementslib-2.2.5/src/requirementslib/models/cache.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/dependencies.py` & `requirementslib-2.2.5/src/requirementslib/models/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import functools
 import os
 from json import JSONDecodeError
 
 import attr
 import requests
 from pip._internal.cache import WheelCache
-from pip._internal.models.format_control import FormatControl
 from pip._internal.operations.build.build_tracker import get_build_tracker
 from pip._internal.req.constructors import install_req_from_line
 from pip._internal.req.req_install import InstallRequirement
 from pip._internal.req.req_set import RequirementSet
 from pip._internal.utils.temp_dir import TempDirectory, global_tempdir_manager
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.utils import canonicalize_name
@@ -57,15 +56,15 @@
 
 DEPENDENCY_CACHE = DependencyCache()
 
 
 @contextlib.contextmanager
 def _get_wheel_cache():
     with global_tempdir_manager():
-        yield WheelCache(CACHE_DIR, FormatControl(set(), set()))
+        yield WheelCache(CACHE_DIR)
 
 
 def _get_filtered_versions(ireq, versions, prereleases):
     return set(ireq.specifier.filter(versions, prereleases=prereleases))
 
 
 def find_all_matches(finder, ireq, pre=False):
@@ -442,15 +441,15 @@
 def is_python(section):
     return section.startswith("[") and ":" in section
 
 
 def get_resolver(
     finder, build_tracker, pip_options, session, directory, install_command=None
 ):
-    wheel_cache = WheelCache(pip_options.cache_dir, pip_options.format_control)
+    wheel_cache = WheelCache(pip_options.cache_dir)
     if install_command is None:
         install_command = get_pip_command()
     preparer = install_command.make_requirement_preparer(
         temp_build_dir=directory,
         options=pip_options,
         build_tracker=build_tracker,
         session=session,
```

### Comparing `requirementslib-2.2.4/src/requirementslib/models/lockfile.py` & `requirementslib-2.2.5/src/requirementslib/models/lockfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/markers.py` & `requirementslib-2.2.5/src/requirementslib/models/markers.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/metadata.py` & `requirementslib-2.2.5/src/requirementslib/models/metadata.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/pipfile.py` & `requirementslib-2.2.5/src/requirementslib/models/pipfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/project.py` & `requirementslib-2.2.5/src/requirementslib/models/project.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/requirements.py` & `requirementslib-2.2.5/src/requirementslib/models/requirements.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/resolvers.py` & `requirementslib-2.2.5/src/requirementslib/models/resolvers.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/setup_info.py` & `requirementslib-2.2.5/src/requirementslib/models/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from urllib.parse import parse_qs, urlparse, urlunparse
 from weakref import finalize
 
 import attr
 from distlib.wheel import Wheel
 from pep517 import envbuild, wrappers
 from pip._internal.network.download import Downloader
+from pip._internal.operations.prepare import unpack_url
 from pip._internal.utils.temp_dir import global_tempdir_manager
 from pip._internal.utils.urls import url_to_path
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.specifiers import SpecifierSet
 from pip._vendor.packaging.version import parse
 from pip._vendor.pkg_resources import (
     PathMetadata,
@@ -32,15 +33,15 @@
 from platformdirs import user_cache_dir
 from vistir.contextmanagers import cd, temp_path
 from vistir.path import create_tracked_tempdir, rmtree
 
 from ..environment import MYPY_RUNNING
 from ..exceptions import RequirementError
 from ..utils import get_pip_command
-from .old_pip_utils import old_unpack_url
+from .old_pip_utils import _copy_source_tree
 from .utils import (
     get_default_pyproject_backend,
     get_name_variants,
     get_pyproject,
     init_requirement,
     split_vcs_method_from_uri,
     strip_extras_markers_from_requirement,
@@ -1510,24 +1511,30 @@
                 "build_dir": directory,
                 "autodelete": False,
                 "parallel_builds": True,
             }
             build_location_func(**build_kwargs)
             ireq.ensure_has_source_dir(kwargs["src_dir"])
             location = None
-            if getattr(ireq, "source_dir", None):
+            if ireq.source_dir:
                 location = ireq.source_dir
-            old_unpack_url(
-                link=ireq.link,
-                location=location,
-                download=Downloader(session, "off"),
-                verbosity=1,
-                download_dir=download_dir,
-                hashes=ireq.hashes(True),
-            )
+
+            if ireq.link.is_existing_dir():
+                if os.path.isdir(location):
+                    rmtree(location)
+                _copy_source_tree(ireq.link.file_path, location)
+            else:
+                unpack_url(
+                    link=ireq.link,
+                    location=location,
+                    download=Downloader(session, "off"),
+                    verbosity=1,
+                    download_dir=download_dir,
+                    hashes=ireq.hashes(True),
+                )
         created = cls.create(
             ireq.source_dir, subdirectory=subdir, ireq=ireq, kwargs=kwargs, stack=stack
         )
         return created
 
     @classmethod
     def create(
```

### Comparing `requirementslib-2.2.4/src/requirementslib/models/url.py` & `requirementslib-2.2.5/src/requirementslib/models/url.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/utils.py` & `requirementslib-2.2.5/src/requirementslib/models/utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/models/vcs.py` & `requirementslib-2.2.5/src/requirementslib/models/vcs.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib/utils.py` & `requirementslib-2.2.5/src/requirementslib/utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.4/src/requirementslib.egg-info/PKG-INFO` & `requirementslib-2.2.5/src/requirementslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.2.4
+Version: 2.2.5
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.2.4/src/requirementslib.egg-info/SOURCES.txt` & `requirementslib-2.2.5/src/requirementslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

