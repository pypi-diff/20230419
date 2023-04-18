# Comparing `tmp/historical_timelines-0.2.1.tar.gz` & `tmp/historical_timelines-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "historical_timelines-0.2.1.tar", last modified: Wed Mar 29 04:12:13 2023, max compression
+gzip compressed data, was "historical_timelines-0.2.2.tar", last modified: Tue Apr 18 22:44:42 2023, max compression
```

## Comparing `historical_timelines-0.2.1.tar` & `historical_timelines-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,50 @@
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      409 2023-03-29 04:11:40.000000 historical_timelines-0.2.1/.bumpversion.cfg
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     9826 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/CONTRIBUTING.md
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1063 2023-03-05 02:18:16.000000 historical_timelines-0.2.1/LICENSE
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      527 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/MANIFEST.in
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2314 2023-03-08 12:54:50.000000 historical_timelines-0.2.1/Makefile
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2462 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/PKG-INFO
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2169 2023-03-29 04:07:09.000000 historical_timelines-0.2.1/README.md
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/doc/
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/doc/_static/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    39113 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/doc/_static/random_timeline.png
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/historical_timelines/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      112 2023-03-29 04:11:40.000000 historical_timelines-0.2.1/historical_timelines/__init__.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     4391 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/historical_timelines/date.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     5529 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/historical_timelines/event.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3173 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/historical_timelines/graphics.py
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/historical_timelines/tests/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-05 02:42:04.000000 historical_timelines-0.2.1/historical_timelines/tests/__init__.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1053 2023-03-28 21:29:29.000000 historical_timelines-0.2.1/historical_timelines/tests/test_dates.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      986 2023-03-28 21:29:29.000000 historical_timelines-0.2.1/historical_timelines/tests/test_events.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      252 2023-03-28 21:29:29.000000 historical_timelines-0.2.1/historical_timelines/tests/test_graphics.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3208 2023-03-28 21:29:29.000000 historical_timelines-0.2.1/historical_timelines/tests/test_integration.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      947 2023-03-28 21:29:29.000000 historical_timelines-0.2.1/historical_timelines/tests/test_timelines.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-03-07 23:11:00.000000 historical_timelines-0.2.1/historical_timelines/tests/timeline_egypt.csv
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     6186 2023-03-29 03:29:39.000000 historical_timelines-0.2.1/historical_timelines/timeline.py
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/historical_timelines.egg-info/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2462 2023-03-29 04:12:13.000000 historical_timelines-0.2.1/historical_timelines.egg-info/PKG-INFO
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      808 2023-03-29 04:12:13.000000 historical_timelines-0.2.1/historical_timelines.egg-info/SOURCES.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        1 2023-03-29 04:12:13.000000 historical_timelines-0.2.1/historical_timelines.egg-info/dependency_links.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        6 2023-03-29 04:12:13.000000 historical_timelines-0.2.1/historical_timelines.egg-info/requires.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       21 2023-03-29 04:12:13.000000 historical_timelines-0.2.1/historical_timelines.egg-info/top_level.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2247 2023-03-29 04:11:40.000000 historical_timelines-0.2.1/pyproject.toml
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       38 2023-03-29 04:12:13.957911 historical_timelines-0.2.1/setup.cfg
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      528 2023-03-29 04:11:40.000000 historical_timelines-0.2.1/setup.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      409 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/.bumpversion.cfg
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      716 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/.readthedocs.yaml
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     9826 2023-03-29 03:29:39.000000 historical_timelines-0.2.2/CONTRIBUTING.md
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1066 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/LICENSE
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      581 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/MANIFEST.in
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2314 2023-03-08 12:54:50.000000 historical_timelines-0.2.2/Makefile
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2755 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/PKG-INFO
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2462 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/README.md
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.002106 historical_timelines-0.2.2/docs/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      638 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/Makefile
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/binder/
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/binder/.ipynb_checkpoints/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2678 2023-04-18 22:26:22.000000 historical_timelines-0.2.2/docs/binder/.ipynb_checkpoints/tutorial-checkpoint.ipynb
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/binder/timeline_egypt.csv
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3034 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/binder/tutorial.ipynb
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      804 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/make.bat
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      173 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/requirements.txt
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/source/
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/source/_static/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    39113 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/_static/random_timeline.png
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1029 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/conf.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      426 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/date.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      441 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/event.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/graphics.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/index.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      396 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/timeline.rst
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/historical_timelines/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      112 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/historical_timelines/__init__.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     4391 2023-03-29 03:29:39.000000 historical_timelines-0.2.2/historical_timelines/date.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     6302 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/event.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     7437 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/graphics.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/historical_timelines/tests/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-05 02:42:04.000000 historical_timelines-0.2.2/historical_timelines/tests/__init__.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1053 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_dates.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      986 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_events.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      252 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_graphics.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3208 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_integration.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      947 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_timelines.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-03-07 23:11:00.000000 historical_timelines-0.2.2/historical_timelines/tests/timeline_egypt.csv
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     8017 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/timeline.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/historical_timelines.egg-info/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2755 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/PKG-INFO
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1134 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        1 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        6 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/requires.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       21 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/top_level.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2247 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/pyproject.toml
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       38 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/setup.cfg
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      528 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/setup.py
```

### Comparing `historical_timelines-0.2.1/CONTRIBUTING.md` & `historical_timelines-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/LICENSE` & `historical_timelines-0.2.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Shaina
+Copyright (c) 2023 darthbeep
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `historical_timelines-0.2.1/MANIFEST.in` & `historical_timelines-0.2.2/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 graft historical_timelines
 
 include LICENSE
 include README.md
 include CONTRIBUTING.md
 include MANIFEST.in
+include .readthedocs.yaml
 
 include .bumpversion.cfg
 include pyproject.toml
 include Makefile
 
-include doc/_static/*
-
 prune .github
 exclude .gitignore
 exclude .gitattributes
 
 # Patterns to exclude from any directory
 global-exclude *~
 global-exclude *.pyc
 global-exclude *.pyo
 global-exclude .git
 global-exclude .ipynb_checkpoints
 global-exclude .DS_Store
 global-exclude .coverage
 global-exclude .pytest_cache/*
-global-exclude .pytest_cache/v/cache/*
+global-exclude .pytest_cache/v/cache/*
+
+# Docs:
+recursive-include docs *
+prune docs/build
```

### Comparing `historical_timelines-0.2.1/Makefile` & `historical_timelines-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/PKG-INFO` & `historical_timelines-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historical_timelines
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for making historical timelines
 Home-page: UNKNOWN
 Author: darthbeep
 Author-email: darthbeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 Python package for creating timelines of historical events.
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
- 
+[![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
 Install with `pip install historical_timelines`
@@ -43,15 +44,15 @@
 timeline = HistoricalTimeline("Random Timeline")
 timeline.populate_random_timeline()
 timeline.render_timeline("timeline.html")
 ```
 
 This will produce something that looks like this:
 
-![Sample timeline](doc/_static/random_timeline.png)
+![Sample timeline](docs/source/_static/random_timeline.png)
 
 If you have a csv that you want to convert to a timeline, you can do that too. Suppose you have a csv with the path `timeline.csv`, and five columns entitled `Name`, `Description`, `Label`, `Start`, and `End`. It would be imported like this.
 
 ```python
 from historical_timelines import HistoricalTimeline
 
 timeline = HistoricalTimeline("Timeline from my csv")
@@ -64,7 +65,11 @@
     "End",
 )
 
 timeline.populate_timeline_from_dict(timeline_json)
 timeline.render_timeline("timeline.html")
 ```
 
+## Documentation
+
+The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
+
```

### Comparing `historical_timelines-0.2.1/README.md` & `historical_timelines-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Python package for creating timelines of historical events.
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
- 
+[![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
 Install with `pip install historical_timelines`
@@ -31,15 +32,15 @@
 timeline = HistoricalTimeline("Random Timeline")
 timeline.populate_random_timeline()
 timeline.render_timeline("timeline.html")
 ```
 
 This will produce something that looks like this:
 
-![Sample timeline](doc/_static/random_timeline.png)
+![Sample timeline](docs/source/_static/random_timeline.png)
 
 If you have a csv that you want to convert to a timeline, you can do that too. Suppose you have a csv with the path `timeline.csv`, and five columns entitled `Name`, `Description`, `Label`, `Start`, and `End`. It would be imported like this.
 
 ```python
 from historical_timelines import HistoricalTimeline
 
 timeline = HistoricalTimeline("Timeline from my csv")
@@ -50,8 +51,12 @@
     "Label",
     "Start",
     "End",
 )
 
 timeline.populate_timeline_from_dict(timeline_json)
 timeline.render_timeline("timeline.html")
-```
+```
+
+## Documentation
+
+The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
```

### Comparing `historical_timelines-0.2.1/doc/_static/random_timeline.png` & `historical_timelines-0.2.2/docs/source/_static/random_timeline.png`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/date.py` & `historical_timelines-0.2.2/historical_timelines/date.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/event.py` & `historical_timelines-0.2.2/historical_timelines/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,26 +121,48 @@
                 if char_counter != prev_stop:
                     ret_title += " "
                 ret_title += word
                 char_counter = next_break + 1
 
         return ret_title
 
-    def get_label_or_default(self, default='default'):
+    def get_label_or_default(self, default: str = 'default') -> str:
+        """Get get the label if it exists, otherwise return a default string
+
+        Args:
+            default (str, optional): The string to use if the label isn't found. Defaults to 'default'.
+
+        Returns:
+            str: The label or default string
+        """
         if self.label:
             return self.label
         return default
 
     def get_adjusted_year(self):
+        """Get the year adjusted for the AD/BC timeline.
+        Returns an int if the event is an event, and a tuple if the event is a period.
+
+        Returns:
+            int | tuple[int, int]: The year(s), adjusted for AD/BC.
+        """
         if self.event_type is EventType.Event:
             return self.start.get_adjudged_year()
-        return [self.start.get_adjudged_year(), self.end.get_adjudged_year()]
+        return (self.start.get_adjudged_year(), self.end.get_adjudged_year())
 
     @staticmethod
     def event_from_dict(event_dict: object) -> "HistoricalEvent":
+        """Takes in a dictionary entry and turns it into a HistoricalEvent
+
+        Args:
+            event_dict (object): A dictionary representing a HistoricalEvent
+
+        Returns:
+            HistoricalEvent: The converted event
+        """
         start = HistoricalDate(event_dict["start"], era=event_dict["era"])
         label = None
         end = None
         if event_dict["label"]:
             label = event_dict["label"]
         if event_dict["end"]:
             end = HistoricalDate(event_dict["end"], era=event_dict["era"])
```

### Comparing `historical_timelines-0.2.1/historical_timelines/tests/test_dates.py` & `historical_timelines-0.2.2/historical_timelines/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/tests/test_events.py` & `historical_timelines-0.2.2/historical_timelines/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/tests/test_integration.py` & `historical_timelines-0.2.2/historical_timelines/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/tests/test_timelines.py` & `historical_timelines-0.2.2/historical_timelines/tests/test_timelines.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines/tests/timeline_egypt.csv` & `historical_timelines-0.2.2/docs/binder/timeline_egypt.csv`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.1/historical_timelines.egg-info/PKG-INFO` & `historical_timelines-0.2.2/historical_timelines.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historical-timelines
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for making historical timelines
 Home-page: UNKNOWN
 Author: darthbeep
 Author-email: darthbeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 Python package for creating timelines of historical events.
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
- 
+[![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
 Install with `pip install historical_timelines`
@@ -43,15 +44,15 @@
 timeline = HistoricalTimeline("Random Timeline")
 timeline.populate_random_timeline()
 timeline.render_timeline("timeline.html")
 ```
 
 This will produce something that looks like this:
 
-![Sample timeline](doc/_static/random_timeline.png)
+![Sample timeline](docs/source/_static/random_timeline.png)
 
 If you have a csv that you want to convert to a timeline, you can do that too. Suppose you have a csv with the path `timeline.csv`, and five columns entitled `Name`, `Description`, `Label`, `Start`, and `End`. It would be imported like this.
 
 ```python
 from historical_timelines import HistoricalTimeline
 
 timeline = HistoricalTimeline("Timeline from my csv")
@@ -64,7 +65,11 @@
     "End",
 )
 
 timeline.populate_timeline_from_dict(timeline_json)
 timeline.render_timeline("timeline.html")
 ```
 
+## Documentation
+
+The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
+
```

### Comparing `historical_timelines-0.2.1/historical_timelines.egg-info/SOURCES.txt` & `historical_timelines-0.2.2/historical_timelines.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 .bumpversion.cfg
+.readthedocs.yaml
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.py
-doc/_static/random_timeline.png
+docs/Makefile
+docs/make.bat
+docs/requirements.txt
+docs/binder/timeline_egypt.csv
+docs/binder/tutorial.ipynb
+docs/binder/.ipynb_checkpoints/tutorial-checkpoint.ipynb
+docs/source/conf.py
+docs/source/date.rst
+docs/source/event.rst
+docs/source/graphics.rst
+docs/source/index.rst
+docs/source/timeline.rst
+docs/source/_static/random_timeline.png
 historical_timelines/__init__.py
 historical_timelines/date.py
 historical_timelines/event.py
 historical_timelines/graphics.py
 historical_timelines/timeline.py
 historical_timelines.egg-info/PKG-INFO
 historical_timelines.egg-info/SOURCES.txt
```

### Comparing `historical_timelines-0.2.1/pyproject.toml` & `historical_timelines-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "historical-timelines"
 authors = [{name = "darthbeep", email = "darthbeep@gmail.com"}]
 description="A python project to make historical timelines"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">=3.7"
 
 dependencies = [
     "bokeh >= 3.1.0"
 ]
 
 classifiers = [
```

### Comparing `historical_timelines-0.2.1/setup.py` & `historical_timelines-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='historical_timelines',
-    version='0.2.1',
+    version='0.2.2',
     description='A Python package for making historical timelines',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='darthbeep',
     author_email='darthbeep@gmail.com',
     packages=['historical_timelines'],
     install_requires=[
```

