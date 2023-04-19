# Comparing `tmp/aplanat-0.6.8.tar.gz` & `tmp/aplanat-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplanat-0.6.8.tar", last modified: Tue Apr 26 09:27:10 2022, max compression
+gzip compressed data, was "aplanat-0.6.9.tar", last modified: Tue May 31 18:53:26 2022, max compression
```

## Comparing `aplanat-0.6.8.tar` & `aplanat-0.6.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.470740 aplanat-0.6.8/
--rw-rw-rw-   0 root         (0) root         (0)    15820 2022-04-26 08:45:38.000000 aplanat-0.6.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-04-26 08:45:38.000000 aplanat-0.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4552 2022-04-26 09:27:10.470740 aplanat-0.6.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4264 2022-04-26 08:45:38.000000 aplanat-0.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.466740 aplanat-0.6.8/aplanat/
--rw-rw-rw-   0 root         (0) root         (0)     6080 2022-04-26 09:25:32.000000 aplanat-0.6.8/aplanat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2336 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/annot.py
--rw-rw-rw-   0 root         (0) root         (0)     5707 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/bars.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/bio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.466740 aplanat-0.6.8/aplanat/components/
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7395 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/bcfstats.py
--rw-rw-rw-   0 root         (0) root         (0)     8466 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/clonevalidation.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     7347 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/depthcoverage.py
--rw-rw-rw-   0 root         (0) root         (0)     5943 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)    22300 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/mapula.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/components/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.470740 aplanat-0.6.8/aplanat/data/
--rw-rw-rw-   0 root         (0) root         (0)   159515 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)     3700 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/custom-epi2me.css
--rw-rw-rw-   0 root         (0) root         (0)     3953 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/custom-ond.css
--rw-rw-rw-   0 root         (0) root         (0)     3955 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/custom-ont.css
--rw-rw-rw-   0 root         (0) root         (0)    34092 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   204580 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)    71482 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/fontawesome.css
--rw-rw-rw-   0 root         (0) root         (0)    72372 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/jquery-3.6.0.slim.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1236 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)    33283 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/ond_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/ont_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)      876 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/report_template.html
--rw-rw-rw-   0 root         (0) root         (0)     3067 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/simple-datatables_latest.css
--rw-rw-rw-   0 root         (0) root         (0)    37980 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/data/simple-datatables_latest.js
--rw-rw-rw-   0 root         (0) root         (0)     5548 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/graphics.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/hist.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/layouts.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.470740 aplanat-0.6.8/aplanat/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/parsers/bcfstats.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/points.py
--rw-rw-rw-   0 root         (0) root         (0)    13587 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/report.py
--rw-rw-rw-   0 root         (0) root         (0)     6030 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/spatial.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2022-04-26 08:45:38.000000 aplanat-0.6.8/aplanat/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 09:27:10.466740 aplanat-0.6.8/aplanat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4552 2022-04-26 09:27:09.000000 aplanat-0.6.8/aplanat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1286 2022-04-26 09:27:10.000000 aplanat-0.6.8/aplanat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-26 09:27:10.000000 aplanat-0.6.8/aplanat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2022-04-26 09:27:10.000000 aplanat-0.6.8/aplanat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-26 09:26:42.000000 aplanat-0.6.8/aplanat.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       95 2022-04-26 09:27:10.000000 aplanat-0.6.8/aplanat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-04-26 09:27:10.000000 aplanat-0.6.8/aplanat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-04-26 08:45:38.000000 aplanat-0.6.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-26 09:27:10.470740 aplanat-0.6.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2348 2022-04-26 08:45:38.000000 aplanat-0.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.019333 aplanat-0.6.9/
+-rw-rw-rw-   0 root         (0) root         (0)    15820 2022-05-31 15:31:18.000000 aplanat-0.6.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       91 2022-05-31 15:31:18.000000 aplanat-0.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4515 2022-05-31 18:53:26.019333 aplanat-0.6.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4264 2022-05-31 15:31:18.000000 aplanat-0.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.015332 aplanat-0.6.9/aplanat/
+-rw-rw-rw-   0 root         (0) root         (0)     6080 2022-05-31 18:52:19.000000 aplanat-0.6.9/aplanat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2336 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/annot.py
+-rw-rw-rw-   0 root         (0) root         (0)     5707 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/bars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/bio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.015332 aplanat-0.6.9/aplanat/components/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7395 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/bcfstats.py
+-rw-rw-rw-   0 root         (0) root         (0)     8466 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/clonevalidation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7347 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/depthcoverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    22300 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/mapula.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/components/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.019333 aplanat-0.6.9/aplanat/data/
+-rw-rw-rw-   0 root         (0) root         (0)   159515 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/custom-epi2me.css
+-rw-rw-rw-   0 root         (0) root         (0)     3953 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/custom-ond.css
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/custom-ont.css
+-rw-rw-rw-   0 root         (0) root         (0)    34092 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   204580 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    71482 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/fontawesome.css
+-rw-rw-rw-   0 root         (0) root         (0)    72372 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/jquery-3.6.0.slim.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/ond_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/ont_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)      876 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/report_template.html
+-rw-rw-rw-   0 root         (0) root         (0)     3067 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/simple-datatables_latest.css
+-rw-rw-rw-   0 root         (0) root         (0)    37980 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/data/simple-datatables_latest.js
+-rw-rw-rw-   0 root         (0) root         (0)     5548 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/graphics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/hist.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/layouts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.019333 aplanat-0.6.9/aplanat/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/parsers/bcfstats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/points.py
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     6030 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/spatial.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2022-05-31 15:31:18.000000 aplanat-0.6.9/aplanat/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:53:26.015332 aplanat-0.6.9/aplanat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4515 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1286 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-31 18:53:04.000000 aplanat-0.6.9/aplanat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-05-31 18:53:25.000000 aplanat-0.6.9/aplanat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-05-31 15:31:18.000000 aplanat-0.6.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-05-31 18:53:26.019333 aplanat-0.6.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2022-05-31 15:31:18.000000 aplanat-0.6.9/setup.py
```

### Comparing `aplanat-0.6.8/LICENSE.md` & `aplanat-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/PKG-INFO` & `aplanat-0.6.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: aplanat
-Version: 0.6.8
+Version: 0.6.9
 Summary: Bokeh plotting API.
 Home-page: https://github.com/epi2me-labs/aplanat
 Author: cwright
 Author-email: cwright@nanoporetech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Aplanat
 =======
 
 Aplanat provides a wrappers (templates) around the bokeh library to simplify
@@ -133,9 +131,7 @@
         y_facet_heading='Y Facet label',
         x_axis_label='x-axis plot label',
         y_axis_label='y-axis plot label')
 
 
 The `transform` callback functions can be used to transform the x and y data
 for each subplot after it has been selected, allowing arbitrary manipulation.
-
-
```

### Comparing `aplanat-0.6.8/README.md` & `aplanat-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/__init__.py` & `aplanat-0.6.9/aplanat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from bokeh.colors import RGB
 from bokeh.embed.util import OutputDocumentFor, standalone_docs_json
 import bokeh.io as bkio
 from bokeh.layouts import gridplot
 from bokeh.plotting import Figure
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 # we don't run a comprehensive test suite and mostly in notebooks,
 # so show warnings all the time.
 warnings.simplefilter('always', DeprecationWarning)
 
 
 class Grid(list):
```

### Comparing `aplanat-0.6.8/aplanat/annot.py` & `aplanat-0.6.9/aplanat/annot.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/bars.py` & `aplanat-0.6.9/aplanat/bars.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/base.py` & `aplanat-0.6.9/aplanat/base.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/bio.py` & `aplanat-0.6.9/aplanat/bio.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/bcfstats.py` & `aplanat-0.6.9/aplanat/components/bcfstats.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/clonevalidation.py` & `aplanat-0.6.9/aplanat/components/clonevalidation.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/demo.py` & `aplanat-0.6.9/aplanat/components/demo.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/depthcoverage.py` & `aplanat-0.6.9/aplanat/components/depthcoverage.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/fastcat.py` & `aplanat-0.6.9/aplanat/components/fastcat.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     return plot
 
 
 _full_report_header = """
 ### Read summary
 
 The following tables and figures are derived from
-the output of [fastcat](https://github.com/epi2me-labs/fastcat)`.
+the output of [fastcat](https://github.com/epi2me-labs/fastcat).
 """
 
 
 def full_report(
         stats, header=_full_report_header, report=None,
         sample_counts=False, min_len=None, max_len=None):
     """Create a report section from the output of fastcat.
```

### Comparing `aplanat-0.6.8/aplanat/components/mapula.py` & `aplanat-0.6.9/aplanat/components/mapula.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/nextclade.py` & `aplanat-0.6.9/aplanat/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/components/simple.py` & `aplanat-0.6.9/aplanat/components/simple.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/bootstrap.min.css` & `aplanat-0.6.9/aplanat/data/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/custom-epi2me.css` & `aplanat-0.6.9/aplanat/data/custom-epi2me.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/custom-ond.css` & `aplanat-0.6.9/aplanat/data/custom-ond.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/custom-ont.css` & `aplanat-0.6.9/aplanat/data/custom-ont.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/fa-regular-400.ttf` & `aplanat-0.6.9/aplanat/data/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/fa-solid-900.ttf` & `aplanat-0.6.9/aplanat/data/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/fontawesome.css` & `aplanat-0.6.9/aplanat/data/fontawesome.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/jquery-3.6.0.slim.min.js` & `aplanat-0.6.9/aplanat/data/jquery-3.6.0.slim.min.js`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/nextclade.html` & `aplanat-0.6.9/aplanat/data/nextclade.html`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/ond_logo.txt` & `aplanat-0.6.9/aplanat/data/ond_logo.txt`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/ont_logo.txt` & `aplanat-0.6.9/aplanat/data/ont_logo.txt`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/report_template.html` & `aplanat-0.6.9/aplanat/data/report_template.html`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/simple-datatables_latest.css` & `aplanat-0.6.9/aplanat/data/simple-datatables_latest.css`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/data/simple-datatables_latest.js` & `aplanat-0.6.9/aplanat/data/simple-datatables_latest.js`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/graphics.py` & `aplanat-0.6.9/aplanat/graphics.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/hist.py` & `aplanat-0.6.9/aplanat/hist.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/layouts.py` & `aplanat-0.6.9/aplanat/layouts.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/lines.py` & `aplanat-0.6.9/aplanat/lines.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/parsers/bcfstats.py` & `aplanat-0.6.9/aplanat/parsers/bcfstats.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/points.py` & `aplanat-0.6.9/aplanat/points.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/report.py` & `aplanat-0.6.9/aplanat/report.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/spatial.py` & `aplanat-0.6.9/aplanat/spatial.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat/util.py` & `aplanat-0.6.9/aplanat/util.py`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/aplanat.egg-info/PKG-INFO` & `aplanat-0.6.9/aplanat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: aplanat
-Version: 0.6.8
+Version: 0.6.9
 Summary: Bokeh plotting API.
 Home-page: https://github.com/epi2me-labs/aplanat
 Author: cwright
 Author-email: cwright@nanoporetech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Aplanat
 =======
 
 Aplanat provides a wrappers (templates) around the bokeh library to simplify
@@ -133,9 +131,7 @@
         y_facet_heading='Y Facet label',
         x_axis_label='x-axis plot label',
         y_axis_label='y-axis plot label')
 
 
 The `transform` callback functions can be used to transform the x and y data
 for each subplot after it has been selected, allowing arbitrary manipulation.
-
-
```

### Comparing `aplanat-0.6.8/aplanat.egg-info/SOURCES.txt` & `aplanat-0.6.9/aplanat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aplanat-0.6.8/setup.py` & `aplanat-0.6.9/setup.py`

 * *Files identical despite different names*

