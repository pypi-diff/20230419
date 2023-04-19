# Comparing `tmp/saltext.elasticsearch8-1.0.10.tar.gz` & `tmp/saltext.elasticsearch8-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.elasticsearch8-1.0.10.tar", last modified: Wed Apr 19 20:43:02 2023, max compression
+gzip compressed data, was "saltext.elasticsearch8-1.0.9.tar", last modified: Wed Apr 19 19:04:56 2023, max compression
```

## Comparing `saltext.elasticsearch8-1.0.10.tar` & `saltext.elasticsearch8-1.0.9.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/
--rw-r--r--   0 root         (0) root         (0)      722 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.779205 saltext.elasticsearch8-1.0.10/.github/
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.github/release-notes.yml
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.github/release.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.779205 saltext.elasticsearch8-1.0.10/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1886 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     8324 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.github/workflows/test.yml
--rw-r--r--   0 root         (0) root         (0)     1940 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8538 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.779205 saltext.elasticsearch8-1.0.10/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     2090 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)    11755 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/.tagpr
--rw-r--r--   0 root         (0) root         (0)     3646 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/LICENSE.new
--rw-r--r--   0 root         (0) root         (0)     1295 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/README.md
--rw-r--r--   0 root         (0) root         (0)      983 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/README.new
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)     5443 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/ref/saltext.elasticsearch8.modules.rst
--rw-r--r--   0 root         (0) root         (0)      657 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/ref/saltext.elasticsearch8.rst
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/ref/saltext.elasticsearch8.states.rst
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/ref/saltext.rst
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    15417 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/noxfile.py
--rw-r--r--   0 root         (0) root         (0)      708 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/requirements/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/crypto.txt
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/darwin.txt
--rw-r--r--   0 root         (0) root         (0)      384 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/pytest.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/requirements/static/
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.783205 saltext.elasticsearch8-1.0.10/requirements/static/ci/
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/changelog.in
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/cloud.in
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/common.in
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/crypto.in
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/darwin.in
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/docs.in
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/freebsd.in
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/invoke.in
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/lint.in
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/linux.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.787205 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/
--rw-r--r--   0 root         (0) root         (0)      796 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/changelog.txt
--rw-r--r--   0 root         (0) root         (0)    22639 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/cloud.txt
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/darwin-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    22134 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/darwin.txt
--rw-r--r--   0 root         (0) root         (0)     2843 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/docs.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/freebsd-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    22415 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)      452 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/invoke.txt
--rw-r--r--   0 root         (0) root         (0)    21913 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/lint.txt
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/linux-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/linux.txt
--rw-r--r--   0 root         (0) root         (0)     1112 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/tools.txt
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/windows-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    10106 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.787205 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/
--rw-r--r--   0 root         (0) root         (0)    23074 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/cloud.txt
--rw-r--r--   0 root         (0) root         (0)     3008 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/docs.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/invoke.txt
--rw-r--r--   0 root         (0) root         (0)    22483 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/lint.txt
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/linux-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    24071 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/linux.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.787205 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/
--rw-r--r--   0 root         (0) root         (0)    23685 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/cloud.txt
--rw-r--r--   0 root         (0) root         (0)     3007 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/docs.txt
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/freebsd-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    23368 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/invoke.txt
--rw-r--r--   0 root         (0) root         (0)    23050 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/lint.txt
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/linux-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    24558 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/linux.txt
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/windows-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    10428 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.787205 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/changelog.txt
--rw-r--r--   0 root         (0) root         (0)    23376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/cloud.txt
--rw-r--r--   0 root         (0) root         (0)     2912 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/docs.txt
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/freebsd-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    23089 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/invoke.txt
--rw-r--r--   0 root         (0) root         (0)    22698 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/lint.txt
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/linux-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    24253 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/linux.txt
--rw-r--r--   0 root         (0) root         (0)      377 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/windows-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    10112 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/changelog.txt
--rw-r--r--   0 root         (0) root         (0)    23498 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/cloud.txt
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/darwin-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    22932 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/darwin.txt
--rw-r--r--   0 root         (0) root         (0)     3023 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/docs.txt
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/freebsd-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    23213 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/invoke.txt
--rw-r--r--   0 root         (0) root         (0)    22775 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/lint.txt
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/linux-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    24414 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/linux.txt
--rw-r--r--   0 root         (0) root         (0)     1110 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/tools.txt
--rw-r--r--   0 root         (0) root         (0)      377 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/windows-crypto.txt
--rw-r--r--   0 root         (0) root         (0)    10182 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/windows.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/tools.in
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/ci/windows.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/darwin.in
--rw-r--r--   0 root         (0) root         (0)      394 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/freebsd.in
--rw-r--r--   0 root         (0) root         (0)      390 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/linux.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/
--rw-r--r--   0 root         (0) root         (0)     2911 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/darwin.txt
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)     2559 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/linux.txt
--rw-r--r--   0 root         (0) root         (0)     3343 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.6/
--rw-r--r--   0 root         (0) root         (0)     2769 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.6/linux.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/
--rw-r--r--   0 root         (0) root         (0)     2545 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)     2537 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/linux.txt
--rw-r--r--   0 root         (0) root         (0)     3459 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/
--rw-r--r--   0 root         (0) root         (0)     2488 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/linux.txt
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/windows.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/
--rw-r--r--   0 root         (0) root         (0)     2909 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/darwin.txt
--rw-r--r--   0 root         (0) root         (0)     2568 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/freebsd.txt
--rw-r--r--   0 root         (0) root         (0)     2558 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/linux.txt
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/windows.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/static/pkg/windows.in
--rw-r--r--   0 root         (0) root         (0)      670 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/windows.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/requirements/zeromq.txt
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      271 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.779205 saltext.elasticsearch8-1.0.10/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.779205 saltext.elasticsearch8-1.0.10/src/saltext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/
--rw-r--r--   0 root         (0) root         (0)      863 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/__init__.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111097 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/modules/elasticsearch8_mod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/returners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/returners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/returners/elasticsearch8_mod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/states/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23247 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/states/elasticsearch8_mod.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.791205 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1295 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5348 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 20:43:02.000000 saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/support/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/support/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)    18976 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/support/elasticsearch/elasticsearch_mock8.py
--rw-r--r--   0 root         (0) root         (0)    16517 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/support/mock.py
--rw-r--r--   0 root         (0) root         (0)    11065 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/support/unit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/unit/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/unit/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59646 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/unit/modules/test_elasticsearch8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:02.795205 saltext.elasticsearch8-1.0.10/tests/unit/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/unit/states/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-04-19 20:42:30.000000 saltext.elasticsearch8-1.0.10/tests/unit/states/test_elasticsearch8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/.github/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.github/release-notes.yml
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.github/release.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)    11755 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/.tagpr
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/LICENSE.new
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      983 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/README.new
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)     5443 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.893701 saltext.elasticsearch8-1.0.9/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/ref/saltext.elasticsearch8.modules.rst
+-rw-r--r--   0 root         (0) root         (0)      657 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/ref/saltext.elasticsearch8.rst
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/ref/saltext.elasticsearch8.states.rst
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/ref/saltext.rst
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    15417 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)      708 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.893701 saltext.elasticsearch8-1.0.9/requirements/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/crypto.txt
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/darwin.txt
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/pytest.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.893701 saltext.elasticsearch8-1.0.9/requirements/static/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.893701 saltext.elasticsearch8-1.0.9/requirements/static/ci/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/changelog.in
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/cloud.in
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/common.in
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/crypto.in
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/darwin.in
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/docs.in
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/freebsd.in
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/invoke.in
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/lint.in
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/linux.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.893701 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/
+-rw-r--r--   0 root         (0) root         (0)      796 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)    22639 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/cloud.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/darwin-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    22134 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/darwin.txt
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/freebsd-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    22415 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/invoke.txt
+-rw-r--r--   0 root         (0) root         (0)    21913 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/linux-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/tools.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/windows-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    10106 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.897702 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/
+-rw-r--r--   0 root         (0) root         (0)    23074 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/cloud.txt
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/invoke.txt
+-rw-r--r--   0 root         (0) root         (0)    22483 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/linux-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    24071 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/linux.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.897702 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/
+-rw-r--r--   0 root         (0) root         (0)    23685 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/cloud.txt
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/freebsd-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    23368 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/invoke.txt
+-rw-r--r--   0 root         (0) root         (0)    23050 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/linux-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    24558 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/linux.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/windows-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    10428 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.897702 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)    23376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/cloud.txt
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/freebsd-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    23089 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/invoke.txt
+-rw-r--r--   0 root         (0) root         (0)    22698 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/linux-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    24253 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/linux.txt
+-rw-r--r--   0 root         (0) root         (0)      377 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/windows-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    10112 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)    23498 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/cloud.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/darwin-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    22932 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/darwin.txt
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/freebsd-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    23213 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/invoke.txt
+-rw-r--r--   0 root         (0) root         (0)    22775 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/lint.txt
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/linux-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    24414 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/tools.txt
+-rw-r--r--   0 root         (0) root         (0)      377 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/windows-crypto.txt
+-rw-r--r--   0 root         (0) root         (0)    10182 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/windows.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/tools.in
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/ci/windows.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/darwin.in
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/freebsd.in
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/linux.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/darwin.txt
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.6/
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.6/linux.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/windows.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/darwin.txt
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/freebsd.txt
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/linux.txt
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/windows.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/static/pkg/windows.in
+-rw-r--r--   0 root         (0) root         (0)      670 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/windows.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/requirements/zeromq.txt
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      271 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.889701 saltext.elasticsearch8-1.0.9/src/saltext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111097 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/modules/elasticsearch8_mod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/returners/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/returners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/returners/elasticsearch8_mod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23247 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/states/elasticsearch8_mod.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.901702 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:04:56.000000 saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/support/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/support/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)    18976 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/support/elasticsearch/elasticsearch_mock8.py
+-rw-r--r--   0 root         (0) root         (0)    16517 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/support/mock.py
+-rw-r--r--   0 root         (0) root         (0)    11065 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/support/unit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/unit/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/unit/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59646 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/unit/modules/test_elasticsearch8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:04:56.905702 saltext.elasticsearch8-1.0.9/tests/unit/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/unit/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-04-19 19:04:22.000000 saltext.elasticsearch8-1.0.9/tests/unit/states/test_elasticsearch8.py
```

### Comparing `saltext.elasticsearch8-1.0.10/.coveragerc` & `saltext.elasticsearch8-1.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.github/workflows/release.yml` & `saltext.elasticsearch8-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.github/workflows/test.yml` & `saltext.elasticsearch8-1.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.gitignore` & `saltext.elasticsearch8-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.pre-commit-config.yaml` & `saltext.elasticsearch8-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.pre-commit-hooks/check-cli-examples.py` & `saltext.elasticsearch8-1.0.9/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.pre-commit-hooks/make-autodocs.py` & `saltext.elasticsearch8-1.0.9/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.pylintrc` & `saltext.elasticsearch8-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/.tagpr` & `saltext.elasticsearch8-1.0.9/.tagpr`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/CHANGELOG.md` & `saltext.elasticsearch8-1.0.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # Changelog
 
-## [1.0.10](https://github.com/cesan3/salt-ext-elasticsearch8/compare/1.0.9...1.0.10) - 2023-04-19
-- fix: downgrade package python requirement to 3.6 and salt to 3003 by @cesan3 in https://github.com/cesan3/salt-ext-elasticsearch8/pull/35
-
 ## [1.0.9](https://github.com/cesan3/salt-ext-elasticsearch8/compare/1.0.8...1.0.9) - 2023-04-19
 - fix: update semver after package is published by @cesan3 in https://github.com/cesan3/salt-ext-elasticsearch8/pull/33
 
 ## [1.0.8](https://github.com/cesan3/salt-ext-elasticsearch8/compare/1.0.7...1.0.8) - 2023-04-19
 - fix: testing by @cesan3 in https://github.com/cesan3/salt-ext-elasticsearch8/pull/31
 
 ## [1.0.7](https://github.com/cesan3/salt-ext-elasticsearch8/compare/1.0.6...1.0.7) - 2023-04-18
```

### Comparing `saltext.elasticsearch8-1.0.10/LICENSE` & `saltext.elasticsearch8-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/LICENSE.new` & `saltext.elasticsearch8-1.0.9/LICENSE.new`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/PKG-INFO` & `saltext.elasticsearch8-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: saltext.elasticsearch8
-Version: 1.0.10
+Version: 1.0.9
 Summary: Module to manage Eleasticsearch8
 Home-page: https://github.com/cesan3/salt-ext-elasticsearch8
 Author: Cesar Sanchez
 Author-email: cesan3@gmail.com
 License: Apache Software License
 Project-URL: Source, https://github.com/cesan3/salt-ext-elasticsearch8
 Project-URL: Tracker, https://github.com/cesan3/salt-ext-elasticsearch8/issues
 Keywords: salt-extension
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: docsauto
 License-File: LICENSE
 License-File: LICENSE.new
```

### Comparing `saltext.elasticsearch8-1.0.10/README.new` & `saltext.elasticsearch8-1.0.9/README.new`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/docs/Makefile` & `saltext.elasticsearch8-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/docs/conf.py` & `saltext.elasticsearch8-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/docs/make.bat` & `saltext.elasticsearch8-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/docs/ref/saltext.elasticsearch8.rst` & `saltext.elasticsearch8-1.0.9/docs/ref/saltext.elasticsearch8.rst`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/noxfile.py` & `saltext.elasticsearch8-1.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/pyproject.toml` & `saltext.elasticsearch8-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/README.rst` & `saltext.elasticsearch8-1.0.9/requirements/static/README.rst`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/common.in` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/common.in`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/changelog.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/changelog.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/cloud.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/cloud.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/darwin.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/darwin.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/docs.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/docs.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/lint.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/lint.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/tools.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/tools.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.10/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.10/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/cloud.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/cloud.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/docs.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/docs.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/lint.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/lint.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.6/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.6/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/cloud.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/cloud.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/docs.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/docs.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/lint.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/lint.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.7/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.7/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/changelog.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/changelog.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/cloud.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/cloud.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/docs.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/docs.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/lint.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/lint.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.8/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.8/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/changelog.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/changelog.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/cloud.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/cloud.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/darwin.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/darwin.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/docs.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/docs.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/lint.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/lint.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/tools.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/tools.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/ci/py3.9/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/ci/py3.9/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/darwin.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/darwin.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.10/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.10/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.6/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.6/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.7/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.7/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.8/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.8/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/darwin.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/darwin.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/freebsd.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/freebsd.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/linux.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/linux.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/static/pkg/py3.9/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/static/pkg/py3.9/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/requirements/windows.txt` & `saltext.elasticsearch8-1.0.9/requirements/windows.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/setup.cfg` & `saltext.elasticsearch8-1.0.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -12,37 +12,34 @@
 	Tracker=https://github.com/cesan3/salt-ext-elasticsearch8/issues
 license = Apache Software License
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 platforms = any
 
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find_namespace:
-python_requires = >= 3.6
+python_requires = >= 3.9
 setup_requires = 
 	wheel
 	setuptools>=50.3.2
 	setuptools_scm[toml]>=3.4
 	setuptools-declarative-requirements
 install_requires = 
-	salt>=3003
+	salt>=3005
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.entry_points]
```

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/__init__.py` & `saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/loader.py` & `saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/loader.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/modules/elasticsearch8_mod.py` & `saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/modules/elasticsearch8_mod.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext/elasticsearch8/states/elasticsearch8_mod.py` & `saltext.elasticsearch8-1.0.9/src/saltext/elasticsearch8/states/elasticsearch8_mod.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/PKG-INFO` & `saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: saltext.elasticsearch8
-Version: 1.0.10
+Version: 1.0.9
 Summary: Module to manage Eleasticsearch8
 Home-page: https://github.com/cesan3/salt-ext-elasticsearch8
 Author: Cesar Sanchez
 Author-email: cesan3@gmail.com
 License: Apache Software License
 Project-URL: Source, https://github.com/cesan3/salt-ext-elasticsearch8
 Project-URL: Tracker, https://github.com/cesan3/salt-ext-elasticsearch8/issues
 Keywords: salt-extension
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: docsauto
 License-File: LICENSE
 License-File: LICENSE.new
```

### Comparing `saltext.elasticsearch8-1.0.10/src/saltext.elasticsearch8.egg-info/SOURCES.txt` & `saltext.elasticsearch8-1.0.9/src/saltext.elasticsearch8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/conftest.py` & `saltext.elasticsearch8-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/support/elasticsearch/elasticsearch_mock8.py` & `saltext.elasticsearch8-1.0.9/tests/support/elasticsearch/elasticsearch_mock8.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/support/mock.py` & `saltext.elasticsearch8-1.0.9/tests/support/mock.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/support/unit.py` & `saltext.elasticsearch8-1.0.9/tests/support/unit.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/unit/modules/test_elasticsearch8.py` & `saltext.elasticsearch8-1.0.9/tests/unit/modules/test_elasticsearch8.py`

 * *Files identical despite different names*

### Comparing `saltext.elasticsearch8-1.0.10/tests/unit/states/test_elasticsearch8.py` & `saltext.elasticsearch8-1.0.9/tests/unit/states/test_elasticsearch8.py`

 * *Files identical despite different names*

