# Comparing `tmp/runmanager-3.2.0.tar.gz` & `tmp/runmanager-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runmanager-3.2.0.tar", last modified: Wed Apr 19 19:38:08 2023, max compression
+gzip compressed data, was "runmanager-3.2.0rc1.tar", last modified: Thu Apr 13 00:42:01 2023, max compression
```

## Comparing `runmanager-3.2.0.tar` & `runmanager-3.2.0rc1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.517686 runmanager-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.505686 runmanager-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.505686 runmanager-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-19 19:37:50.000000 runmanager-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-19 19:37:50.000000 runmanager-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 19:37:50.000000 runmanager-3.2.0/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-19 19:37:50.000000 runmanager-3.2.0/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 19:37:50.000000 runmanager-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-19 19:38:08.517686 runmanager-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-19 19:37:50.000000 runmanager-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.505686 runmanager-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.509686 runmanager-3.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.509686 runmanager-3.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.509686 runmanager-3.2.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.509686 runmanager-3.2.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.513687 runmanager-3.2.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106126 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager.ico
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113429 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_axes.png
--rw-r--r--   0 runner    (1001) docker     (123)   217480 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_bools.png
--rw-r--r--   0 runner    (1001) docker     (123)   243887 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_complex_globals.png
--rw-r--r--   0 runner    (1001) docker     (123)   250190 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_eval_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   200741 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_groups.png
--rw-r--r--   0 runner    (1001) docker     (123)   239956 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_interface.png
--rw-r--r--   0 runner    (1001) docker     (123)   131423 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runmanager_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    28615 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)   245000 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/using_runmanager.docx
--rw-r--r--   0 runner    (1001) docker     (123)   679785 2023-04-19 19:37:50.000000 runmanager-3.2.0/docs/using_runmanager.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 19:37:50.000000 runmanager-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 19:37:50.000000 runmanager-3.2.0/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.517686 runmanager-3.2.0/runmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    48648 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189841 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/batch_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/globals_diff.bat
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/globals_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/group.ui
--rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)   167461 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/runmanager.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-04-19 19:37:50.000000 runmanager-3.2.0/runmanager/runmanager.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:08.517686 runmanager-3.2.0/runmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 19:38:08.000000 runmanager-3.2.0/runmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 19:38:08.517686 runmanager-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 19:37:50.000000 runmanager-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.817341 runmanager-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.825341 runmanager-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106126 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113429 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_axes.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217480 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_bools.png
+-rw-r--r--   0 runner    (1001) docker     (123)   243887 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_complex_globals.png
+-rw-r--r--   0 runner    (1001) docker     (123)   250190 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_eval_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   200741 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_groups.png
+-rw-r--r--   0 runner    (1001) docker     (123)   239956 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_interface.png
+-rw-r--r--   0 runner    (1001) docker     (123)   131423 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    28615 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   245000 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/using_runmanager.docx
+-rw-r--r--   0 runner    (1001) docker     (123)   679785 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/using_runmanager.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/runmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    48648 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189841 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/batch_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/globals_diff.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/globals_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/group.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167461 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/runmanager.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/runmanager.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/runmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/setup.py
```

### Comparing `runmanager-3.2.0/.github/workflows/release.yml` & `runmanager-3.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/.gitignore` & `runmanager-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/BSD-2-CLAUSE-LICENSE.txt` & `runmanager-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/BSD-3-CLAUSE-LICENSE.txt` & `runmanager-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/LICENSE.txt` & `runmanager-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/PKG-INFO` & `runmanager-3.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runmanager
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Graphical control of parameterised experiments composed in labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runmanager
 Project-URL: Download, https://github.com/labscript-suite/runmanager/releases
```

### Comparing `runmanager-3.2.0/README.md` & `runmanager-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/Makefile` & `runmanager-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/make.bat` & `runmanager-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/_static/custom.css` & `runmanager-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/_templates/autosummary-class.rst` & `runmanager-3.2.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/_templates/autosummary-module.rst` & `runmanager-3.2.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/_templates/components.rst` & `runmanager-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/conf.py` & `runmanager-3.2.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/blacs_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/labscript_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/lyse_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager.ico` & `runmanager-3.2.0rc1/docs/source/img/runmanager.ico`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_64x64.svg` & `runmanager-3.2.0rc1/docs/source/img/runmanager_64x64.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_axes.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_axes.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_bools.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_bools.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_complex_globals.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_complex_globals.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_eval_error.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_eval_error.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_groups.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_groups.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_interface.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_interface.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runmanager_overview.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_overview.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/img/runviewer_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/index.rst` & `runmanager-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/introduction.rst` & `runmanager-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/pyqt5-modified-objects.inv` & `runmanager-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/source/usage.rst` & `runmanager-3.2.0rc1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/using_runmanager.docx` & `runmanager-3.2.0rc1/docs/using_runmanager.docx`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/docs/using_runmanager.pdf` & `runmanager-3.2.0rc1/docs/using_runmanager.pdf`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/readthedocs.yaml` & `runmanager-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/__init__.py` & `runmanager-3.2.0rc1/runmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/__main__.py` & `runmanager-3.2.0rc1/runmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/__version__.py` & `runmanager-3.2.0rc1/runmanager/__version__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/batch_compiler.py` & `runmanager-3.2.0rc1/runmanager/batch_compiler.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/functions.py` & `runmanager-3.2.0rc1/runmanager/functions.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/group.ui` & `runmanager-3.2.0rc1/runmanager/group.ui`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/main.ui` & `runmanager-3.2.0rc1/runmanager/main.ui`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/remote.py` & `runmanager-3.2.0rc1/runmanager/remote.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/runmanager.ico` & `runmanager-3.2.0rc1/runmanager/runmanager.ico`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager/runmanager.svg` & `runmanager-3.2.0rc1/runmanager/runmanager.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/runmanager.egg-info/PKG-INFO` & `runmanager-3.2.0rc1/runmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runmanager
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Graphical control of parameterised experiments composed in labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runmanager
 Project-URL: Download, https://github.com/labscript-suite/runmanager/releases
```

### Comparing `runmanager-3.2.0/runmanager.egg-info/SOURCES.txt` & `runmanager-3.2.0rc1/runmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.2.0/setup.cfg` & `runmanager-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*

