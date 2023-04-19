# Comparing `tmp/hacking-5.0.0.tar.gz` & `tmp/hacking-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hacking-5.0.0.tar", last modified: Thu Oct  6 09:45:47 2022, max compression
+gzip compressed data, was "hacking-6.0.0.tar", last modified: Wed Apr 19 08:05:44 2023, max compression
```

## Comparing `hacking-5.0.0.tar` & `hacking-6.0.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-10-06 09:45:12.000000 hacking-5.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2022-10-06 09:45:12.000000 hacking-5.0.0/.pre-commit-hooks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2022-10-06 09:45:12.000000 hacking-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2022-10-06 09:45:12.000000 hacking-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7203 2022-10-06 09:45:47.000000 hacking-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2022-10-06 09:45:12.000000 hacking-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37754 2022-10-06 09:45:47.000000 hacking-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14411 2022-10-06 09:45:12.000000 hacking-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-10-06 09:45:12.000000 hacking-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-10-06 09:45:12.000000 hacking-5.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7682 2022-10-06 09:45:47.739091 hacking-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5312 2022-10-06 09:45:12.000000 hacking-5.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/user/hacking.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-10-06 09:45:12.000000 hacking-5.0.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/hacking/checks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6556 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/comments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/dictlist.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6193 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10691 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/except_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/imports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4695 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/localization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6411 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/mock_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2082 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/other.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7284 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/python23.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/checks/vim_check.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/hacking/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2195 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/hacking/tests/checks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/checks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7419 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/checks/test_comments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8010 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/checks/test_except_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/checks/test_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/checks/test_other.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2771 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/test_doctest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2022-10-06 09:45:12.000000 hacking-5.0.0/hacking/tests/test_import_exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/hacking.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7682 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-10-06 09:45:47.000000 hacking-5.0.0/hacking.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/integration-test/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1135 2022-10-06 09:45:12.000000 hacking-5.0.0/integration-test/test.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-10-06 09:45:12.000000 hacking-5.0.0/py35-upper-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.735091 hacking-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/drop-py-2-7-c2bcdd28e4513532.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/drop-python36-834bb59e53d5fd71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/flake8-3-x-support-cd478de79fe7b63d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/migrating-most-common-hacking-checks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/rocky-intermediate-release-60db6e8f66539e4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/notes/start-of-queens-c3024ebbb49aef6f.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:47.739091 hacking-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8902 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/v1.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/v1.1.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/v2.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/v3.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-06 09:45:12.000000 hacking-5.0.0/releasenotes/source/v4.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2022-10-06 09:45:12.000000 hacking-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-10-06 09:45:47.739091 hacking-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-10-06 09:45:12.000000 hacking-5.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-10-06 09:45:12.000000 hacking-5.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1534 2022-10-06 09:45:12.000000 hacking-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-04-19 08:05:13.000000 hacking-6.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-04-19 08:05:13.000000 hacking-6.0.0/.pre-commit-hooks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-04-19 08:05:13.000000 hacking-6.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-04-19 08:05:13.000000 hacking-6.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7203 2023-04-19 08:05:43.000000 hacking-6.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-04-19 08:05:13.000000 hacking-6.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37836 2023-04-19 08:05:43.000000 hacking-6.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14411 2023-04-19 08:05:13.000000 hacking-6.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-19 08:05:13.000000 hacking-6.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-19 08:05:13.000000 hacking-6.0.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7682 2023-04-19 08:05:44.141833 hacking-6.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5312 2023-04-19 08:05:13.000000 hacking-6.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/user/hacking.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-04-19 08:05:13.000000 hacking-6.0.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/hacking/checks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6556 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/comments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/dictlist.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6193 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10691 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/except_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/imports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4695 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/localization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6411 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/mock_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2082 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/other.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7308 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/python23.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/checks/vim_check.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/hacking/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2195 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/hacking/tests/checks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/checks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7419 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/checks/test_comments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8010 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/checks/test_except_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/checks/test_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/checks/test_other.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2825 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/test_doctest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-04-19 08:05:13.000000 hacking-6.0.0/hacking/tests/test_import_exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/hacking.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7682 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-04-19 08:05:44.000000 hacking-6.0.0/hacking.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2023-04-19 08:05:43.000000 hacking-6.0.0/hacking.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/integration-test/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1135 2023-04-19 08:05:13.000000 hacking-6.0.0/integration-test/test.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-04-19 08:05:13.000000 hacking-6.0.0/py35-upper-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.137833 hacking-6.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/drop-py-2-7-c2bcdd28e4513532.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/drop-python36-834bb59e53d5fd71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/flake8-3-x-support-cd478de79fe7b63d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/migrating-most-common-hacking-checks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/rocky-intermediate-release-60db6e8f66539e4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/notes/start-of-queens-c3024ebbb49aef6f.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:44.141833 hacking-6.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8902 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/v1.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/v1.1.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/v2.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/v3.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-19 08:05:13.000000 hacking-6.0.0/releasenotes/source/v4.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-04-19 08:05:13.000000 hacking-6.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2023-04-19 08:05:44.145833 hacking-6.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-04-19 08:05:13.000000 hacking-6.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2023-04-19 08:05:13.000000 hacking-6.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2023-04-19 08:05:13.000000 hacking-6.0.0/tox.ini
```

### Comparing `hacking-5.0.0/.zuul.yaml` & `hacking-6.0.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/AUTHORS` & `hacking-6.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/CONTRIBUTING.rst` & `hacking-6.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/ChangeLog` & `hacking-6.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+6.0.0
+-----
+
+* Bump flake8 to 5.0 to pick up fixes
+* Make tox.ini 4.0 compatible
+
 5.0.0
 -----
 
 * Drop py36 and py37 support
 * Add support for flake8 4.x
 * Fix test errors with python3.10
 * Use TOX\_CONSTRAINTS\_FILE
```

### Comparing `hacking-5.0.0/HACKING.rst` & `hacking-6.0.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/LICENSE` & `hacking-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/PKG-INFO` & `hacking-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hacking
-Version: 5.0.0
+Version: 6.0.0
 Summary: OpenStack Hacking Guideline Enforcement
 Home-page: https://docs.openstack.org/hacking/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://bugs.launchpad.net/hacking
 Project-URL: Reviews, https://review.opendev.org/q/p:openstack/hacking+status:open
```

### Comparing `hacking-5.0.0/README.rst` & `hacking-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/doc/source/conf.py` & `hacking-6.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/doc/source/contributor/contributing.rst` & `hacking-6.0.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/doc/source/index.rst` & `hacking-6.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/comments.py` & `hacking-6.0.0/hacking/checks/comments.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/dictlist.py` & `hacking-6.0.0/hacking/checks/dictlist.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/docstrings.py` & `hacking-6.0.0/hacking/checks/docstrings.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/except_checks.py` & `hacking-6.0.0/hacking/checks/except_checks.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/imports.py` & `hacking-6.0.0/hacking/checks/imports.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/localization.py` & `hacking-6.0.0/hacking/checks/localization.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/mock_checks.py` & `hacking-6.0.0/hacking/checks/mock_checks.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/other.py` & `hacking-6.0.0/hacking/checks/other.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/checks/python23.py` & `hacking-6.0.0/hacking/checks/python23.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,19 @@
     H236: class Foo(object):\n    '''docstr.'''\n    __metaclass__ = Meta
     H236: class Foo(object):\n    __metaclass__ = \\n        Meta
     Okay: class Foo(object):\n    __metaclass__ = Meta  # noqa
     """
     if noqa:
         return
     split_line = logical_line.split()
-    if(len(split_line) > 2 and split_line[0] == '__metaclass__' and
-       split_line[1] == '='):
+    if (
+        len(split_line) > 2
+        and split_line[0] == '__metaclass__'
+        and split_line[1] == '='
+    ):
         yield (logical_line.find('__metaclass__'),
                "H236: Python 3.x incompatible __metaclass__, "
                "use six.add_metaclass()")
 
 
 # NOTE(guochbo): This is removed module list:
 # http://python3porting.com/stdlib.html#removed-modules
```

### Comparing `hacking-5.0.0/hacking/checks/vim_check.py` & `hacking-6.0.0/hacking/checks/vim_check.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/config.py` & `hacking-6.0.0/hacking/config.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/core.py` & `hacking-6.0.0/hacking/core.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/__init__.py` & `hacking-6.0.0/hacking/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/checks/test_comments.py` & `hacking-6.0.0/hacking/tests/checks/test_comments.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/checks/test_except_checks.py` & `hacking-6.0.0/hacking/tests/checks/test_except_checks.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/checks/test_mock.py` & `hacking-6.0.0/hacking/tests/checks/test_mock.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/checks/test_other.py` & `hacking-6.0.0/hacking/tests/checks/test_other.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/test_config.py` & `hacking-6.0.0/hacking/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking/tests/test_doctest.py` & `hacking-6.0.0/hacking/tests/test_doctest.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,26 +36,28 @@
 
     def test_flake8(self):
 
         with tempfile.NamedTemporaryFile(mode='w', delete=False) as f:
             f.write(''.join(self.lines))
 
         cmd = [sys.executable, '-mflake8', '--isolated',
-               '--select=%s' % self.code, '--ignore=F',
+               '--select=%s' % self.code,
+               '--enable-extensions=%s' % self.code, '--ignore=F',
                '--format=%(code)s\t%(path)s\t%(row)d', f.name]
         out, _ = subprocess.Popen(cmd, stdout=subprocess.PIPE).communicate()
 
         out = out.decode('utf-8')
 
         if self.code == 'Okay':
             self.assertEqual('', out)
         else:
             self.addDetail('reason',
                            content.text_content("Failed to trigger rule %s" %
                                                 self.code))
+
             self.assertNotEqual('', out)
             self.assertEqual(self.code, out.split('\t')[0].rstrip(':'), out)
 
         os.remove(f.name)
 
 
 def _get_lines(check):
```

### Comparing `hacking-5.0.0/hacking/tests/test_import_exceptions.py` & `hacking-6.0.0/hacking/tests/test_import_exceptions.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking.egg-info/PKG-INFO` & `hacking-6.0.0/hacking.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hacking
-Version: 5.0.0
+Version: 6.0.0
 Summary: OpenStack Hacking Guideline Enforcement
 Home-page: https://docs.openstack.org/hacking/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://bugs.launchpad.net/hacking
 Project-URL: Reviews, https://review.opendev.org/q/p:openstack/hacking+status:open
```

### Comparing `hacking-5.0.0/hacking.egg-info/SOURCES.txt` & `hacking-6.0.0/hacking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/hacking.egg-info/entry_points.txt` & `hacking-6.0.0/hacking.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/integration-test/test.sh` & `hacking-6.0.0/integration-test/test.sh`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/releasenotes/notes/migrating-most-common-hacking-checks.yaml` & `hacking-6.0.0/releasenotes/notes/migrating-most-common-hacking-checks.yaml`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/releasenotes/notes/rocky-intermediate-release-60db6e8f66539e4b.yaml` & `hacking-6.0.0/releasenotes/notes/rocky-intermediate-release-60db6e8f66539e4b.yaml`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/releasenotes/source/conf.py` & `hacking-6.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/setup.cfg` & `hacking-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/setup.py` & `hacking-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/test-requirements.txt` & `hacking-6.0.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `hacking-5.0.0/tox.ini` & `hacking-6.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [tox]
 minversion = 3.18.0
-skipsdist = True
 envlist = py39,pep8
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 usedevelop = True
 deps =
```

