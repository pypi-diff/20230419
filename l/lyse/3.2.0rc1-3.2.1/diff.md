# Comparing `tmp/lyse-3.2.0rc1.tar.gz` & `tmp/lyse-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyse-3.2.0rc1.tar", last modified: Wed Apr 12 23:58:15 2023, max compression
+gzip compressed data, was "lyse-3.2.1.tar", last modified: Wed Apr 19 19:29:55 2023, max compression
```

## Comparing `lyse-3.2.0rc1.tar` & `lyse-3.2.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    41708 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/gui.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/header.tex
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_3.py
--rw-r--r--   0 runner    (1001) docker     (123)   131235 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/lyse.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/lyse.tex
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/minted.sty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54825 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/gui.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/lyse/
--rw-r--r--   0 runner    (1001) docker     (123)    49690 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109625 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/analysis_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/dataframe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/edit_columns.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/figure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/filebox.ui
--rw-r--r--   0 runner    (1001) docker     (123)   160912 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (123)   236310 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/lyse.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/plot_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/routinebox.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/tempfile2clipboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/lyse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.724458 lyse-3.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.712458 lyse-3.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-19 19:29:42.000000 lyse-3.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-19 19:29:42.000000 lyse-3.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 19:29:42.000000 lyse-3.2.1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-19 19:29:42.000000 lyse-3.2.1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-19 19:29:42.000000 lyse-3.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-19 19:29:42.000000 lyse-3.2.1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-19 19:29:55.724458 lyse-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-19 19:29:42.000000 lyse-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    41708 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/gui.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/header.tex
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/listing_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/listing_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/listing_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131235 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/lyse.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/lyse.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/minted.sty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.716458 lyse-3.2.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.720458 lyse-3.2.1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54825 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/gui.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/lyse.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/lyse_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-19 19:29:42.000000 lyse-3.2.1/docs/source/pyqt5-modified-objects.inv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.720458 lyse-3.2.1/lyse/
+-rw-r--r--   0 runner    (1001) docker     (123)    52737 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109625 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/analysis_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/dataframe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/edit_columns.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/figure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/filebox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   160912 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/lyse.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   236310 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/lyse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/plot_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/routinebox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-19 19:29:42.000000 lyse-3.2.1/lyse/tempfile2clipboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:29:55.720458 lyse-3.2.1/lyse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 19:29:55.000000 lyse-3.2.1/lyse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 19:29:42.000000 lyse-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 19:29:42.000000 lyse-3.2.1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 19:29:55.724458 lyse-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 19:29:42.000000 lyse-3.2.1/setup.py
```

### Comparing `lyse-3.2.0rc1/.github/workflows/release.yml` & `lyse-3.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/.gitignore` & `lyse-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt` & `lyse-3.2.1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt` & `lyse-3.2.1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/LICENSE.txt` & `lyse-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/NEWS.md` & `lyse-3.2.1/NEWS.md`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/PKG-INFO` & `lyse-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.2.0rc1
+Version: 3.2.1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
```

### Comparing `lyse-3.2.0rc1/README.md` & `lyse-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/Makefile` & `lyse-3.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/gui.pdf` & `lyse-3.2.1/docs/gui.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/header.tex` & `lyse-3.2.1/docs/header.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/listing_2.py` & `lyse-3.2.1/docs/listing_2.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/listing_3.py` & `lyse-3.2.1/docs/listing_3.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/lyse.pdf` & `lyse-3.2.1/docs/lyse.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/lyse.tex` & `lyse-3.2.1/docs/lyse.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/make.bat` & `lyse-3.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/minted.sty` & `lyse-3.2.1/docs/minted.sty`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/_static/custom.css` & `lyse-3.2.1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/_templates/autosummary-class.rst` & `lyse-3.2.1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/_templates/autosummary-module.rst` & `lyse-3.2.1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/_templates/components.rst` & `lyse-3.2.1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/conf.py` & `lyse-3.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/examples.rst` & `lyse-3.2.1/docs/source/examples.rst`

 * *Files 20% similar despite different names*

```diff
@@ -49,14 +49,46 @@
 	# figures replace old ones, rather than you getting new window popping
 	# up every time your script runs.
 
 	# We might wish to save this result so that we can compare it across
 	# shots in a multishot analysis:
 	run.save_result('mot loadrate', c)
 
+Single shot analysis with global file opening
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+	from lyse import *
+
+	# Instantiate Run object and open
+	# Globally opening the shot keeps the h5 file open
+	# This prevents excessive opening and closing of the file
+	# which can slow down the analysis
+	with Run(path).open('r+') as shot:
+
+		# Obtaining a trace:
+		t, mot_fluorecence = shot.get_trace('mot fluorecence')
+
+		# Now we might do some analysis on this data. Say we've written a
+		# linear fit function (or we're calling some other libaries linear
+		# fit function):
+		m, c = linear_fit(t, mot_fluorecence)
+		int_tot = mot_fluorecence.sum()
+		mf_min = mot_fluorecence.min()
+		mf_max = mot_fluorecence.max()
+
+		normalised_fluorecence = normalise_response(mot_fluorecence)
+
+		# We might wish to save this result so that we can compare it across
+		# shots in a multishot analysis:
+		shot.save_result('mot loadrate', c)
+		shot.save_result('mot integrated', int_tot)
+		shot.save_results('mot fl min', mf_min, 'mot fl max', mf_max)
+		shot.save_result_array('norm mot fluorecence', normalised_fluorecence)
 
 An analysis on multiple shots
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
 	from lyse import *
```

### Comparing `lyse-3.2.0rc1/docs/source/img/blacs_32nx32n.svg` & `lyse-3.2.1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/gui.svg` & `lyse-3.2.1/docs/source/img/gui.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/labscript_32nx32n.svg` & `lyse-3.2.1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/lyse.ico` & `lyse-3.2.1/docs/source/img/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/lyse_32nx32n.svg` & `lyse-3.2.1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/lyse_64x64.svg` & `lyse-3.2.1/docs/source/img/lyse_64x64.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg` & `lyse-3.2.1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg` & `lyse-3.2.1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/index.rst` & `lyse-3.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/introduction.rst` & `lyse-3.2.1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/docs/source/pyqt5-modified-objects.inv` & `lyse-3.2.1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/__init__.py` & `lyse-3.2.1/lyse/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 """
 
 from lyse.dataframe_utilities import get_series_from_shot as _get_singleshot
 from labscript_utils.dict_diff import dict_diff
 import os
 import socket
 import pickle as pickle
-import inspect
+from pathlib import Path
 import sys
 import threading
+import functools
+import contextlib
 
 import labscript_utils.h5_lock, h5py
 from labscript_utils.labconfig import LabConfig
 import pandas
 from numpy import array, ndarray, where
 import types
 
@@ -219,14 +221,61 @@
     Returns:
         dict: Dictionary of differences between globals in the form `key:[val1,val2]`
         pairs. Keys unique to either dictionary are returned as `key:[val1,'-']` or
         `key:['-',val2]`.
     """
     return dict_diff(run1.get_globals(group), run2.get_globals(group))
  
+def open_file(mode):
+    """Decorator for lyse functions to allow using previously opened file with context manager.
+    
+    If multiple read/write operations happen on a Run in a single shot,
+    opening the h5file once via the context manager `open`
+    can speed up the analysis execution time by limiting the number of times
+    the file must be opened/closed.
+
+    Note that an opened :class:`h5py:h5py.File` can only be in modes `'r'` or `'r+'`.
+    All other mode opening options differ in file creation logic only.
+    In particular, all mode opening options except `'r'` are considered
+    `'r+'` once the file is open.
+
+    Args:
+        mode (str): which :class:`h5py:h5py.File` mode to open the h5 file with.
+            Must be 'r', 'a', 'r+', 'w', 'w-', or 'x'.
+            Lyse typically only uses 'r' and 'r+'.
+
+    Returns:
+        Decorator for :class:`~.Run` methods that need to read/write the shot file
+
+    Raises:
+        PermissionError: If the Run is set as read-only but a write mode is requested
+    """
+    def decorator_open_file(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+
+            if self.no_write and mode != 'r':
+                msg = f'Cannot perform operation {func.__name__:s}; this run is read-only'
+                raise PermissionError(msg)
+
+            if self.h5_file is None:
+                with self.open(mode):
+                    return func(self, *args, **kwargs)
+            else:
+                if (self.h5_file.mode == 'r') and (mode != 'r'):
+                    msg = (f"Cannot perform operation {func.__name__:s}; "
+                        + f"requested mode {mode:s} not compatible with "
+                        + f"h5_file's mode {self.h5_file.mode:s}")
+                    raise PermissionError(msg)
+                else:
+                    return func(self, *args, **kwargs)
+            
+        return wrapper
+    return decorator_open_file
+
 class Run(object):
     """A class for saving/retrieving data to/from a shot's hdf5 file.
 
     This class implements methods that allow the user to retrieve data from a
     shot's hdf5 file such as images, traces, and the values of globals. It also
     provides methods for saving and retrieving results from analysis.
 
@@ -236,70 +285,117 @@
         no_write (bool, optional): Set to `True` to prevent editing the shot's
             hdf5 file. Note that doing so prohibits the ability to save results
             to the file. Defaults to `False`.
     """
     def __init__(self,h5_path,no_write=False):
         self.__h5_path = h5_path
         self.__no_write = no_write
+        self.__h5_file = None
         self.__group = None
         if not self.no_write:
             self._create_group_if_not_exists(h5_path, '/', 'results')
                      
-        try:
-            if not self.no_write:
-                # The group where this run's results will be stored in the h5
-                # file will be the name of the python script which is
-                # instantiating this Run object. Iterate from innermost caller
-                # to outermost. The name of the script will be one frame in
-                # from analysis_subprocess.py.
-                analysis_subprocess_path = os.path.join(
-                    LYSE_DIR,
-                    'analysis_subprocess.py',
-                )
-                group = None
-                inner_frame = inspect.currentframe()
-                inner_path = self._frame_to_path(inner_frame)
-                inner_file_name = self._path_to_file_name(inner_path)
-                while group is None:
-                    # self._frame_to_path() will raise a KeyError if this loop
-                    # reaches the outermost caller.
-                    outer_frame = inner_frame.f_back
-                    outer_path = self._frame_to_path(outer_frame)
-                    outer_file_name = self._path_to_file_name(outer_path)
-                    if outer_path == analysis_subprocess_path:
-                        group = inner_file_name
-                    inner_frame = outer_frame
-                    inner_path = outer_path
-                    inner_file_name = outer_file_name
-                self.set_group(group)
-        except KeyError:
-            # sys.stderr.write('Warning: to write results, call '
-            # 'Run.set_group(groupname), specifying the name of the group '
-            # 'you would like to save results to. This normally comes from '
-            # 'the filename of your script, but since you\'re in interactive '
-            # 'mode, there is no script name.\n')
-            pass
-
-    def _frame_to_path(self, frame):
-        path = frame.f_globals['__file__']
-        return path
-
-    def _path_to_file_name(self, path):
-        file_name = os.path.basename(path).split('.py')[0]
-        return file_name
+        # The group where this run's results will be stored in the h5 file will be the
+        # name of the python script which is instantiating this Run object. If the user
+        # is running interactively or in an unusual environment such that the __main__
+        # module isn't in sys.modules or doesn't have a non-None __file__ attribute,
+        # then self.group will not be set.
+        main_module_path = getattr(sys.modules.get('__main__'), '__file__', None)
+        if not self.no_write and main_module_path is not None:
+            self.set_group(Path(main_module_path).stem)
 
     @property
     def h5_path(self):
         """str: The value provided for `h5_path` during instantiation."""
         return self.__h5_path
 
     @property
     def no_write(self):
         """bool: The value provided for `no_write` during instantiation."""
         return self.__no_write
+    
+    @property
+    def h5_file(self):
+        """h5py.File: opened h5py file handle for the shot"""
+        return self.__h5_file
+    
+    @contextlib.contextmanager
+    def open(self, mode):
+        """Context manager to open the Run's h5 file for successive reads/writes.
+
+        Supports all h5 modes, though only `'r'` and `'r+'`/`'a'` are typically
+        used within lyse itself.
+
+        Args:
+            mode (str): which :class:`h5py:h5py.File` mode to open the h5 file with.
+                Must be 'r', 'a', 'r+', 'w', 'w-', or 'x'.
+                Lyse typically only uses 'r' and 'r+'.
+
+        Yields:
+            :class:`~.Run`: Handle to opened `Run` object.
+
+        Raises:
+            PermissionError: If the Run is set as read-only but a write mode is requested
+
+        Examples:
+            
+            Trivial example that selectively opens the file during analysis.
+            For better performance, it would be better to combine
+            these two openings into one.
+
+            >>> from lyse import *
+            >>> shot = Run(path)
+            >>> with shot.open('r'):
+            >>>     # shot processing that requires reads/writes
+            >>>     _, vals = shot.get_trace('my_trace')
+            >>> with shot.open('r+'):
+            >>>     results = vals**2
+            >>>     shot.save_result_array('my_result', results)
+            >>>     _, vals2 = shot.get_trace('my_other_trace')
+            >>>     shot.save_result('my_result2', vals2.mean())
+            >>> # Shot processing that doesn't require h5 reads/writes
+            >>> print(f'Max of results is {results.max():.3f}')
+            Max of results is 5.003
+
+            Open and create the shot handle for the whole analysis
+            in a single line.
+
+            >>> from lyse import *
+            >>> with Run(path).open('r+') as shot:
+            >>>     # shot processing that requires reads/writes
+            >>>     t, vals = shot.get_trace('my_trace')
+            >>>     results = vals**2
+            >>>     shot.save_result_array('my_result', results)
+            >>>     # Shot processing that doesn't require h5 reads/writes
+            >>>     # could be outside the context
+            >>>     print(f'Max of results is {results.max():.3f}')
+            Max of results is 5.003
+
+        """
+
+        # ensure no_write is respected
+        if self.no_write and mode != 'r':
+            msg = 'Cannot open file with a write mode; this run is read-only'
+            raise PermissionError(msg)
+            
+        # check if file is already open, do nothing if modes compatible
+        if self.__h5_file is not None:
+            # ensure no-write is respected
+            if (self.__h5_file.mode == 'r') and (mode != 'r'):
+                msg = 'Cannot open file with a write mode; this run is read-only'
+                raise PermissionError(msg)
+            yield self
+            return
+        
+        with h5py.File(self.h5_path, mode) as f:
+            self.__h5_file = f
+            try:
+                yield self
+            finally:
+                self.__h5_file = None
 
     @property
     def group(self):
         """str: The group in the hdf5 file in which results are saved by default.
         
         When a `Run` instance is created from within a lyse singleshot or
         multishot routine, `group` will be set to the name of the running
@@ -322,15 +418,15 @@
         """Creates a group in the HDF5 file at `location` if it does not exist.
         
         Only opens the h5 file in write mode if a group must be created.
         This ensures the last modified time of the file is only updated if
         the file is actually written to."""
         create_group = False
         with h5py.File(h5_path, 'r') as h5_file:
-            if not groupname in h5_file[location]:
+            if groupname not in h5_file[location]:
                 create_group = True
         if create_group:
             if self.no_write:
                 msg = "Cannot create group; this run is read-only."
                 raise PermissionError(msg)
             with h5py.File(h5_path, 'r+') as h5_file:
                 # Catch the ValueError raised if the group was created by
@@ -352,46 +448,47 @@
             groupname (str): The name of the hdf5 file group in which to save
                 results by default. The group will be created in the
                 `'/results'` group of the hdf5 file.
         """
         self._create_group_if_not_exists(self.h5_path, '/results', groupname)
         self.__group = groupname
 
+    @open_file('r')
     def trace_names(self):
         """Return a list of all saved data traces in Run.
 
         Raises:
             KeyError: If the group `'/data/traces/'` does not yet exist.
 
         Returns:
             list: List of keys in the h5 file's `'/data/traces/'` group.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            try:
-                return list(h5_file['data']['traces'].keys())
-            except KeyError:
-                return []
-                
+        try:
+            return list(self.h5_file['data']['traces'].keys())
+        except KeyError:
+            return []
+
+    @open_file('r')                
     def get_attrs(self, group):
         """Returns all attributes of the specified group as a dictionary.
 
         Args:
             group (str): Group for which attributes are desired.
 
         Raises:
             Exception: If the `group` does not exist.
 
         Returns:
             dict: Dictionary of attributes.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not group in h5_file:
-                raise Exception('The group \'%s\' does not exist'%group)
-            return get_attributes(h5_file[group])
+        if group not in self.h5_file:
+            raise Exception('The group \'%s\' does not exist'%group)
+        return get_attributes(self.h5_file[group])
 
+    @open_file('r')
     def get_trace(self, name, raw_data=False):
         """Return the saved data trace `name`.
         
         Args:
             name (str): Name of saved data trace to get.
             raw_data (bool, optional): option to return the h5_data directly 
                 without interpreting it as a 2-D time trace.
@@ -399,84 +496,84 @@
         Raises:
             Exception: If `name` trace does not exist.
 
         Returns:
             :obj:`numpy:numpy.ndarray`: Returns 2-D timetrace of times `'t'`
             and values `'values'`.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not name in h5_file['data']['traces']:
-                raise Exception('The trace \'%s\' does not exist'%name)
-            trace = h5_file['data']['traces'][name]
-            
-            if raw_data:
-                data = trace[()]
-            else:
-                data = array(trace['t'],dtype=float),array(trace['values'],dtype=float)  
-            
-            return data
+        if name not in self.h5_file['data']['traces']:
+            raise Exception('The trace \'%s\' does not exist'%name)
+        trace = self.h5_file['data']['traces'][name]
+        
+        if raw_data:
+            data = trace[()]
+        else:
+            data = array(trace['t'],dtype=float),array(trace['values'],dtype=float)  
+        
+        return data
 
-    def get_wait(self,name):
+    @open_file('r')
+    def get_wait(self, name):
         """Returns the wait paramteres: label, timeout, duration, and time out status.
 
         Args:
             name (str): Name of the wait to get.
 
         Raises:
             KeyError if `name` wait does not exist.
 
         Returns:
             tuple: Tuple of the wait parameters.
         """
-        with h5py.File(self.h5_path,'r') as h5_file:
-            if not 'data' in h5_file:
-                raise Exception('The shot has no data group')
-            name=name.encode()
-            if not name in h5_file['data']['waits']['label']:
-                raise Exception('The wait \'%s\' does not exist'%name.decode())
-            name_index, =where(h5_file['data']['waits']['label']==name)[0]
-            return h5_file['data']['waits'][name_index]
+        if not 'data' in self.h5_file:
+            raise Exception('The shot has no data group')
+        name=name.encode()
+        if name not in self.h5_file['data']['waits']['label']:
+            raise Exception('The wait \'%s\' does not exist'%name.decode())
+        name_index, =where(self.h5_file['data']['waits']['label']==name)[0]
+        return self.h5_file['data']['waits'][name_index]
 
+    @open_file('r')
     def get_waits(self):
         """Returns the parameters of all waits in the experiment.
 
         Raises:
             Exception: If the experiment has no waits.
 
         Returns:
             :obj:`numpy:numpy.ndarray`: Returns 2D structured numpy array of the waits and their parameters.
         """
-        with h5py.File(self.h5_path,'r') as h5_file:
-            if not 'data' in h5_file:
-                raise Exception('The shot has no data group')
-            if not 'waits' in h5_file['data']:
-                raise Exception('The shot has no waits')
-            return h5_file['data']['waits'][()]
-        
-    def get_result_array(self,group,name):
+        if 'data' not in self.h5_file:
+            raise Exception('The shot has no data group')
+        if 'waits' not in self.h5_file['data']:
+            raise Exception('The shot has no waits')
+        return self.h5_file['data']['waits'][()]
+
+    @open_file('r')        
+    def get_result_array(self, group, name):
         """Returns saved results data.
 
         Args:
             group (str): Group to look in for the array. Typically the name of
                 the analysis script that created it.
             name (str): Name of the results array to return.
 
         Raises:
             Exception: If `group` or `name` do not already exist.
 
         Returns:
             :obj:`numpy:numpy.ndarray`: Numpy array of the saved data.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not group in h5_file['results']:
-                raise Exception('The result group \'%s\' does not exist'%group)
-            if not name in h5_file['results'][group]:
-                raise Exception('The result array \'%s\' does not exist'%name)
-            return array(h5_file['results'][group][name])
-            
+        if group not in self.h5_file['results']:
+            raise Exception('The result group \'%s\' does not exist'%group)
+        if name not in self.h5_file['results'][group]:
+            raise Exception('The result array \'%s\' does not exist'%name)
+        return array(self.h5_file['results'][group][name])
+
+    @open_file('r')            
     def get_result(self, group, name):
         """Retrieve result from prior calculation.
 
         Args:
             group (str): Group to look in for the result. Typically the name of
                 the analysis script that created it.
             name (str): Name of the result.
@@ -484,21 +581,21 @@
         Raises:
             Exception: If `group` or `name` do not already exist.
 
         Returns:
             : Result with appropriate type, as determined by 
             :obj:`labscript-utils:labscript_utils.properties.get_attribute`.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not group in h5_file['results']:
-                raise Exception('The result group \'%s\' does not exist'%group)
-            if not name in h5_file['results'][group].attrs.keys():
-                raise Exception('The result \'%s\' does not exist'%name)
-            return get_attribute(h5_file['results'][group], name)
-            
+        if group not in self.h5_file['results']:
+            raise Exception('The result group \'%s\' does not exist'%group)
+        if name not in self.h5_file['results'][group].attrs.keys():
+            raise Exception('The result \'%s\' does not exist'%name)
+        return get_attribute(self.h5_file['results'][group], name)
+
+    @open_file('r')            
     def get_results(self, group, *names):
         """Return multiple results from the same group.
 
         Iteratively calls get_result(group,name) for each name provided.
         
         Args:
             group (str): Group to look in for the results. Typically the name of
@@ -508,16 +605,17 @@
         Returns:
             list: List of the results, in the same order as specified by names.
             If `names` does not preserve order, return order is not guaranteed.
         """
         results = []
         for name in names:
             results.append(self.get_result(group,name))
-        return results        
-            
+        return results
+
+    @open_file('r+')            
     def save_result(self, name, value, group=None, overwrite=True):
         """Save a result to the hdf5 file.
 
         With the default argument values this method saves to `self.group` in
         the `'/results'` group and overwrites any existing value. Note that the
         result is saved as an attribute and overwriting attributes causes hdf5
         file size bloat.
@@ -549,47 +647,44 @@
                 `True` because saving the result would edit the file.
             ValueError: A `ValueError` is raised if `self.group` is `None` and
                 no value is provided for `group` because the method then doesn't
                 know where to save the result.
             PermissionError: A `PermissionError` is raised if an attribute with
                 name `name` already exists but `overwrite` is set to `False`.
         """
-        if self.no_write:
-            msg = "Cannot save result; this instance is read-only."
-            raise PermissionError(msg)
-        with h5py.File(self.h5_path,'a') as h5_file:
-            if not group:
-                if self.group is None:
-                    msg = """Cannot save result; no default group set. Either
-                        specify a value for this method's optional group
-                        argument, or set a default value using the set_group()
-                        method."""
-                    raise ValueError(dedent(msg))
-                # Save to analysis results group by default
-                group = 'results/' + self.group
-            elif not group in h5_file:
-                # Create the group if it doesn't exist
-                h5_file.create_group(group) 
-            if name in h5_file[group].attrs and not overwrite:
-                msg = """Cannot save result; group '{group}' already has
-                    attribute '{name}' and overwrite is set to False. Set
-                    overwrite=True to overwrite the existing value.""".format(
-                        group=group,
-                        name=name,
-                    )
-                raise PermissionError(dedent(msg))
-            set_attributes(h5_file[group], {name: value})
+        if not group:
+            if self.group is None:
+                msg = """Cannot save result; no default group set. Either
+                    specify a value for this method's optional group
+                    argument, or set a default value using the set_group()
+                    method."""
+                raise ValueError(dedent(msg))
+            # Save to analysis results group by default
+            group = 'results/' + self.group
+        elif group not in self.h5_file:
+            # Create the group if it doesn't exist
+            self.h5_file.create_group(group) 
+        if name in self.h5_file[group].attrs and not overwrite:
+            msg = """Cannot save result; group '{group}' already has
+                attribute '{name}' and overwrite is set to False. Set
+                overwrite=True to overwrite the existing value.""".format(
+                    group=group,
+                    name=name,
+                )
+            raise PermissionError(dedent(msg))
+        set_attributes(self.h5_file[group], {name: value})
             
         if spinning_top:
             if self.h5_path not in _updated_data:
                 _updated_data[self.h5_path] = {}
             if group.startswith('results'):
                 toplevel = group.replace('results/', '', 1)
                 _updated_data[self.h5_path][toplevel, name] = value
 
+    @open_file('r+')
     def save_result_array(self, name, data, group=None, 
                           overwrite=True, keep_attrs=False, **kwargs):
         """Save an array of data to the hdf5 h5 file.
 
         With the default argument values this method saves to `self.group` in
         the `'/results'` group and overwrites any existing value without keeping
         the dataset's previous attributes. Additional keyword arguments are
@@ -611,76 +706,75 @@
             overwrite (bool, optional): Sets whether or not to overwrite the
                 previous value if the dataset already exists. If set to
                 `False` and the dataset already exists, a `PermissionError` is
                 raised. Defaults to `True`.
             keep_attrs (bool, optional): Whether or not to keep the dataset's
                 attributes when overwriting it, i.e. if the dataset already
                 existed. Defaults to `False`.
+            **kwargs: Optional kwargs passed directly to h5_file.create_dataset()
 
         Raises:
             PermissionError: A `PermissionError` is raised if `self.no_write` is
                 `True` because saving the result would edit the file.
             ValueError: A `ValueError` is raised if `self.group` is `None` and
                 no value is provided for `group` because the method then doesn't
                 know where to save the result.
             PermissionError: A `PermissionError` is raised if a dataset with
                 name `name` already exists but `overwrite` is set to `False`.
         """
-        if self.no_write:
-            msg = "Cannot save result; this instance is read-only."
-            raise PermissionError(msg)
-        with h5py.File(self.h5_path, 'a') as h5_file:
-            attrs = {}
-            if not group:
-                if self.group is None:
-                    msg = """Cannot save result; no default group set. Either
-                        specify a value for this method's optional group
-                        argument, or set a default value using the set_group()
-                        method."""
-                    raise ValueError(dedent(msg))
-                # Save dataset to results group by default
-                group = 'results/' + self.group
-            elif not group in h5_file:
-                # Create the group if it doesn't exist
-                h5_file.create_group(group) 
-            if name in h5_file[group]:
-                if overwrite:
-                    # Overwrite if dataset already exists
-                    if keep_attrs:
-                        attrs = dict(h5_file[group][name].attrs)
-                    del h5_file[group][name]
-                else:
-                    msg = """Cannot save result; group '{group}' already has
-                        dataset '{name}' and overwrite is set to False. Set
-                        overwrite=True to overwrite the existing
-                        value.""".format(
-                            group=group,
-                            name=name,
-                        )
-                    raise PermissionError(dedent(msg))
-            h5_file[group].create_dataset(name, data=data, **kwargs)
-            for key, val in attrs.items():
-                h5_file[group][name].attrs[key] = val
+        attrs = {}
+        if not group:
+            if self.group is None:
+                msg = """Cannot save result; no default group set. Either
+                    specify a value for this method's optional group
+                    argument, or set a default value using the set_group()
+                    method."""
+                raise ValueError(dedent(msg))
+            # Save dataset to results group by default
+            group = 'results/' + self.group
+        elif group not in self.h5_file:
+            # Create the group if it doesn't exist
+            self.h5_file.create_group(group) 
+        if name in self.h5_file[group]:
+            if overwrite:
+                # Overwrite if dataset already exists
+                if keep_attrs:
+                    attrs = dict(self.h5_file[group][name].attrs)
+                del self.h5_file[group][name]
+            else:
+                msg = """Cannot save result; group '{group}' already has
+                    dataset '{name}' and overwrite is set to False. Set
+                    overwrite=True to overwrite the existing
+                    value.""".format(
+                        group=group,
+                        name=name,
+                    )
+                raise PermissionError(dedent(msg))
+        self.h5_file[group].create_dataset(name, data=data, **kwargs)
+        for key, val in attrs.items():
+            self.h5_file[group][name].attrs[key] = val
 
-    def get_traces(self, *names):
+    @open_file('r')
+    def get_traces(self, *names,):
         """Retrieve multiple data traces.
 
         Iteratively calls :obj:`get_trace`.
 
         Args:
             \*names (str): Names of traces to retrieve
 
         Returns:
             list: List of numpy arrays.
         """
         traces = []
         for name in names:
             traces.extend(self.get_trace(name))
         return traces
-             
+
+    @open_file('r')             
     def get_result_arrays(self, group, *names):
         """Retrieve multiple result arrays from the same group.
 
         Iteratively calls :obj:`self.get_result_array(group,name) <get_result_array>`
         with default arguments.
 
         Args:
@@ -690,15 +784,16 @@
         Returns:
             list: List of results.
         """
         results = []
         for name in names:
             results.append(self.get_result_array(group, name))
         return results
-        
+
+    @open_file('r+')        
     def save_results(self, *args, **kwargs):
         """Save multiple results to the hdf5 file.
 
         This method iteratively calls 
         :obj:`self.save_result() <save_result>` on multiple results.
         It assumes arguments are ordered such that each result to be saved is
         preceded by the name of the attribute to save it under. Keywords
@@ -722,15 +817,16 @@
             >>> b = 2.48
             >>> run.save_results('result', a, 'other_result', b, overwrite=False)  # doctest: +SKIP
         """
         names = args[::2]
         values = args[1::2]
         for name, value in zip(names, values):
             self.save_result(name, value, **kwargs)
-            
+
+    @open_file('r+')            
     def save_results_dict(self, results_dict, uncertainties=False, **kwargs):
         """Save results dictionary.
 
         Iteratively calls :obj:`self.save_result(key,value) <save_result>` on
         the provided dictionary. If uncertainties is `True`, `value` is a two-element
         list where the second element is the uncertainty in the result and saved with
         to the same key with `u_` prepended.
@@ -744,14 +840,15 @@
         for name, value in results_dict.items():
             if not uncertainties:
                 self.save_result(name, value, **kwargs)
             else:
                 self.save_result(name, value[0], **kwargs)
                 self.save_result('u_' + name, value[1], **kwargs)
 
+    @open_file('r+')
     def save_result_arrays(self, *args, **kwargs):
         """Save multiple result arrays.
 
         Iteratively calls :obj:`save_result_array() <save_result_array>` on multiple data sets. 
         Assumes arguments are ordered such that each dataset to be saved is 
         preceded by the name to save it as. 
         All keyword arguments are passed to each call of save_result_array().
@@ -761,15 +858,16 @@
                 preceded by the name to save it as.
             **kwargs: Passed through to `save_result_array` as kwargs.
         """
         names = args[::2]
         values = args[1::2]
         for name, value in zip(names, values):
             self.save_result_array(name, value, **kwargs)
-    
+
+    @open_file('r')    
     def get_image(self, orientation, label, image):
         """Get previously saved image from the h5 file.
 
         h5 path to saved image is `/images/orientation/label/image`
 
         Args:
             orientation (str): Orientation label for saved image.
@@ -778,25 +876,25 @@
 
         Raises:
             Exception: If the image or paths do not exist.
 
         Returns:
             :obj:`numpy:numpy.ndarray`: 2-D image array.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not 'images' in h5_file:
-                raise Exception('File does not contain any images')
-            if not orientation in h5_file['images']:
-                raise Exception('File does not contain any images with orientation \'%s\''%orientation)
-            if not label in h5_file['images'][orientation]:
-                raise Exception('File does not contain any images with label \'%s\''%label)
-            if not image in h5_file['images'][orientation][label]:
-                raise Exception('Image \'%s\' not found in file'%image)
-            return array(h5_file['images'][orientation][label][image])
-    
+        if 'images' not in self.h5_file:
+            raise Exception('File does not contain any images')
+        if orientation not in self.h5_file['images']:
+            raise Exception('File does not contain any images with orientation \'%s\''%orientation)
+        if label not in self.h5_file['images'][orientation]:
+            raise Exception('File does not contain any images with label \'%s\''%label)
+        if image not in self.h5_file['images'][orientation][label]:
+            raise Exception('Image \'%s\' not found in file'%image)
+        return array(self.h5_file['images'][orientation][label][image])
+
+    @open_file('r')    
     def get_images(self, orientation, label, *images):
         """Get multiple saved images from orientation and label.
 
         Iteratively calls :obj:`self.get_image(orientation,label,image) <get_image>` for
         each image argument.
 
         Args:
@@ -808,14 +906,15 @@
             :obj:`list` of :obj:`numpy:numpy.ndarray`: List of 2-D images.
         """
         results = []
         for image in images:
             results.append(self.get_image(orientation,label,image))
         return results
 
+    @open_file('r')
     def get_images_dict(self, orientation, label, *images):
         """Get multiple saved images from orientation and label.
 
         Iteratively calls :obj:`self.get_image(orientation,label,image) <get_image>` for
         each image argument.
 
         Args:
@@ -826,81 +925,82 @@
         Returns:
             :obj:`dict` of :obj:`numpy:numpy.ndarray`: Dictionary of 2-D images.
         """
         results = self.get_images(orientation,label, *images)
 
         return {k:v for k,v in zip(images, results)}
 
-
+    @open_file('r')
     def get_all_image_labels(self):
         """Return all existing images labels in the h5 file.
 
         Returns:
             dict: Dictionary of the form `{orientation:[label1,label2]}`
         """
         images_list = {}
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            for orientation in h5_file['/images'].keys():
-                images_list[orientation] = list(h5_file['/images'][orientation].keys())               
-        return images_list                
-    
+        for orientation in self.h5_file['/images'].keys():
+            images_list[orientation] = list(self.h5_file['/images'][orientation].keys())               
+        return images_list
+
+    @open_file('r')    
     def get_image_attributes(self, orientation):
         """Return the attributes of a saved orientation image group.
 
         Args:
             orientation (str): Orientation label to get attributes of.
 
         Raises:
             Exception: If images or orientation group do not exist.
         Returns:
             dict: Dictionary of attributes and their values.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if not 'images' in h5_file:
-                raise Exception('File does not contain any images')
-            if not orientation in h5_file['images']:
-                raise Exception('File does not contain any images with orientation \'%s\''%orientation)
-            return get_attributes(h5_file['images'][orientation])
+        if 'images' not in self.h5_file:
+            raise Exception('File does not contain any images')
+        if orientation not in self.h5_file['images']:
+            raise Exception('File does not contain any images with orientation \'%s\''%orientation)
+        return get_attributes(self.h5_file['images'][orientation])
 
-    def get_globals(self,group=None):
+    @open_file('r')
+    def get_globals(self, group=None):
         """Get globals from the shot.
 
         Args:
             group (str, optional): If `None`, return all global variables.
                 If defined, only return globals from `group`.
 
         Returns:
             dict: Dictionary of globals and their values.
         """
         if not group:
-            with h5py.File(self.h5_path, 'r') as h5_file:
-                return dict(h5_file['globals'].attrs)
+            return dict(self.h5_file['globals'].attrs)
         else:
             try:
-                with h5py.File(self.h5_path, 'r') as h5_file:
-                    return dict(h5_file['globals'][group].attrs)
+                return dict(self.h5_file['globals'][group].attrs)
             except KeyError:
                 return {}
 
+    @open_file('r')
     def get_globals_raw(self, group=None):
         """Get the raw global values from the shot.
 
         Args:
             group (str, optional): If `None`, return all global variables.
-                If defined, only return globals from `group`. 
+                If defined, only return globals from `group`.
+
+        Returns:
+            dict: Dictionary of raw globals and their values
         """
         globals_dict = {}
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            if group == None:
-                for obj in h5_file['globals'].values():
-                    temp_dict = dict(obj.attrs)
-                    for key, val in temp_dict.items():
-                        globals_dict[key] = val
-            else:
-                globals_dict = dict(h5_file['globals'][group].attrs)
+        if group == None:
+            for obj in self.h5_file['globals'].values():
+                temp_dict = dict(obj.attrs)
+                for key, val in temp_dict.items():
+                    globals_dict[key] = val
+        else:
+            globals_dict = dict(self.h5_file['globals'][group].attrs)
         return globals_dict
         
     # def iterable_globals(self, group=None):
         # raw_globals = self.get_globals_raw(group)
         # print raw_globals.items()
         # iterable_globals = {}
         # for global_name, expression in raw_globals.items():
@@ -917,35 +1017,42 @@
                # # iterable_globals[global_name] = [tuple(value)]
             # # elif isinstance(value, ndarray) or  isinstance(value, list):
                # # print global_name + ' is iterable.'            
                # # iterable_globals[global_name] = value
             # # else:
                 # # print global_name + ' is not iterable.'
             # return raw_globals
-            
+
+    @open_file('r')            
     def get_globals_expansion(self):
         """Get the expansion type of each global.
 
         This will skip global variables that do not have
         an expansion.
 
+        Args:
+            h5_file (h5py.File, optional): Allows passing in a handle
+                to an already opened h5 file. If None, will open in
+                read only mode and close after operation.
+
         Returns:
             dict: Dcitionary of globals with their expansion type.
         """
         expansion_dict = {}
         def append_expansion(name, obj):
             if 'expansion' in name:
                 temp_dict = dict(obj.attrs)
                 for key, val in temp_dict.items():
                     if val:
                         expansion_dict[key] = val
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            h5_file['globals'].visititems(append_expansion)
+        
+        self.h5_file['globals'].visititems(append_expansion)
         return expansion_dict
-                   
+
+    @open_file('r')                   
     def get_units(self, group=None):
         """Get the units of globals.
 
         This method retrieves the values in the "Units" column of runmanager for
         this shot. The values are returned in a dictionary where the keys are
         the names of globals and the values are the corresponding units.
 
@@ -971,31 +1078,30 @@
         units = {}
         # Define method that when applied to an hdf5 group adds all of its
         # globals and units to the units dict.
         def append_units(name, obj):
             if 'units' in name:
                 units.update(dict(obj.attrs))
         try:
-            with h5py.File(self.h5_path, 'r') as h5_file:
-                h5_file[path].visititems(append_units)
+            self.h5_file[path].visititems(append_units)
         except KeyError:
             pass
         return units
 
+    @open_file('r')
     def globals_groups(self):
         """Get names of all the globals groups.
 
         Returns:
             list: List of global group names.
         """
-        with h5py.File(self.h5_path, 'r') as h5_file:
-            try:
-                return list(h5_file['globals'].keys())
-            except KeyError:
-                return []   
+        try:
+            return list(self.h5_file['globals'].keys())
+        except KeyError:
+            return []
                 
     def globals_diff(self, other_run, group=None):
         """Take a diff between this run and another run.
 
         This calls :obj:`globals_diff(self, other_run, group) <globals_diff>`.
 
         Args:
@@ -1111,15 +1217,15 @@
         **kwargs: Passed to `figure.savefig()` as kwargs.
     """
     
     import matplotlib.pyplot as plt
     from zprocess import start_daemon
     import tempfile
 
-    if not 'bbox_inches' in kwargs:
+    if 'bbox_inches' not in kwargs:
         kwargs['bbox_inches'] = 'tight'
                
     if figure is None:
         figure = plt.gcf()
 
     with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as f:
         tempfile_name = f.name
```

### Comparing `lyse-3.2.0rc1/lyse/__main__.py` & `lyse-3.2.1/lyse/__main__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/__version__.py` & `lyse-3.2.1/lyse/__version__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/analysis_subprocess.py` & `lyse-3.2.1/lyse/analysis_subprocess.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/dataframe_utilities.py` & `lyse-3.2.1/lyse/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/edit_columns.ui` & `lyse-3.2.1/lyse/edit_columns.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/figure_manager.py` & `lyse-3.2.1/lyse/figure_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,8 @@
     global figuremanager
     import matplotlib.pyplot
     import matplotlib.figure
 
     figuremanager = FigureManager()
     matplotlib.pyplot.figure = figuremanager
     matplotlib.pyplot.close = figuremanager.close
-    matplotlib.pyplot.show = lambda: figuremanager.show
+    matplotlib.pyplot.show = lambda: figuremanager.show()
```

### Comparing `lyse-3.2.0rc1/lyse/filebox.ui` & `lyse-3.2.1/lyse/filebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/lyse.ico` & `lyse-3.2.1/lyse/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/lyse.svg` & `lyse-3.2.1/lyse/lyse.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/main.ui` & `lyse-3.2.1/lyse/main.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/plot_window.ui` & `lyse-3.2.1/lyse/plot_window.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/routinebox.ui` & `lyse-3.2.1/lyse/routinebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse/tempfile2clipboard.py` & `lyse-3.2.1/lyse/tempfile2clipboard.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/lyse.egg-info/PKG-INFO` & `lyse-3.2.1/lyse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.2.0rc1
+Version: 3.2.1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
```

### Comparing `lyse-3.2.0rc1/lyse.egg-info/SOURCES.txt` & `lyse-3.2.1/lyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/readthedocs.yaml` & `lyse-3.2.1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0rc1/setup.cfg` & `lyse-3.2.1/setup.cfg`

 * *Files identical despite different names*

