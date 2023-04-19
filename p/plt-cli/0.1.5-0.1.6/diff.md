# Comparing `tmp/plt-cli-0.1.5.tar.gz` & `tmp/plt-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plt-cli-0.1.5.tar", last modified: Wed Dec 21 15:54:21 2022, max compression
+gzip compressed data, was "plt-cli-0.1.6.tar", last modified: Wed Apr 19 07:09:45 2023, max compression
```

## Comparing `plt-cli-0.1.5.tar` & `plt-cli-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1061 2022-02-09 12:48:59.000000 plt-cli-0.1.5/LICENSE
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       37 2022-02-09 12:48:59.000000 plt-cli-0.1.5/MANIFEST.in
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      998 2022-12-21 15:54:21.900573 plt-cli-0.1.5/PKG-INFO
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      503 2022-12-16 01:21:22.000000 plt-cli-0.1.5/README.md
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        0 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/__init__.py
--rwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)     4033 2022-12-21 15:31:11.000000 plt-cli-0.1.5/plt/plt
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt/templates/
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt/templates/python/
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt/templates/python/matplotlib/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      858 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/templates/python/matplotlib/density.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      921 2022-12-21 15:48:57.000000 plt-cli-0.1.5/plt/templates/python/matplotlib/histogram.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      614 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/templates/python/matplotlib/line.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      812 2022-12-21 15:24:10.000000 plt-cli-0.1.5/plt/templates/python/matplotlib/normalized_histogram.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      796 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/templates/python/matplotlib/scatter.py
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt/templates/python/plotext/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      583 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/templates/python/plotext/density.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      570 2022-12-21 15:53:45.000000 plt-cli-0.1.5/plt/templates/python/plotext/histogram.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      456 2022-02-09 12:48:59.000000 plt-cli-0.1.5/plt/templates/python/plotext/line.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      596 2022-09-16 18:58:15.000000 plt-cli-0.1.5/plt/templates/python/plotext/scatter.py
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2022-12-21 15:54:21.900573 plt-cli-0.1.5/plt_cli.egg-info/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      998 2022-12-21 15:54:21.000000 plt-cli-0.1.5/plt_cli.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      622 2022-12-21 15:54:21.000000 plt-cli-0.1.5/plt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        1 2022-12-21 15:54:21.000000 plt-cli-0.1.5/plt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       39 2022-12-21 15:54:21.000000 plt-cli-0.1.5/plt_cli.egg-info/requires.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        4 2022-12-21 15:54:21.000000 plt-cli-0.1.5/plt_cli.egg-info/top_level.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      104 2022-02-09 12:48:59.000000 plt-cli-0.1.5/pyproject.toml
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      684 2022-12-21 15:54:21.900573 plt-cli-0.1.5/setup.cfg
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.681040 plt-cli-0.1.6/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1061 2022-02-09 12:48:59.000000 plt-cli-0.1.6/LICENSE
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       37 2022-02-09 12:48:59.000000 plt-cli-0.1.6/MANIFEST.in
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      998 2023-04-19 07:09:45.681040 plt-cli-0.1.6/PKG-INFO
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      503 2022-12-16 01:21:22.000000 plt-cli-0.1.6/README.md
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.681040 plt-cli-0.1.6/plt/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        0 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/__init__.py
+-rwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)     4033 2023-04-19 07:03:24.000000 plt-cli-0.1.6/plt/plt
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.677040 plt-cli-0.1.6/plt/templates/
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.677040 plt-cli-0.1.6/plt/templates/python/
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.681040 plt-cli-0.1.6/plt/templates/python/matplotlib/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      858 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/templates/python/matplotlib/density.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      921 2022-12-21 15:48:57.000000 plt-cli-0.1.6/plt/templates/python/matplotlib/histogram.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      614 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/templates/python/matplotlib/line.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      812 2022-12-21 15:24:10.000000 plt-cli-0.1.6/plt/templates/python/matplotlib/normalized_histogram.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      796 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/templates/python/matplotlib/scatter.py
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.681040 plt-cli-0.1.6/plt/templates/python/plotext/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      583 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/templates/python/plotext/density.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      570 2022-12-21 15:53:45.000000 plt-cli-0.1.6/plt/templates/python/plotext/histogram.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      456 2022-02-09 12:48:59.000000 plt-cli-0.1.6/plt/templates/python/plotext/line.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      596 2022-09-16 18:58:15.000000 plt-cli-0.1.6/plt/templates/python/plotext/scatter.py
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-04-19 07:09:45.681040 plt-cli-0.1.6/plt_cli.egg-info/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      998 2023-04-19 07:09:45.000000 plt-cli-0.1.6/plt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      622 2023-04-19 07:09:45.000000 plt-cli-0.1.6/plt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-04-19 07:09:45.000000 plt-cli-0.1.6/plt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       39 2023-04-19 07:09:45.000000 plt-cli-0.1.6/plt_cli.egg-info/requires.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        4 2023-04-19 07:09:45.000000 plt-cli-0.1.6/plt_cli.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      104 2022-02-09 12:48:59.000000 plt-cli-0.1.6/pyproject.toml
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      684 2023-04-19 07:09:45.681040 plt-cli-0.1.6/setup.cfg
```

### Comparing `plt-cli-0.1.5/LICENSE` & `plt-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/PKG-INFO` & `plt-cli-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plt-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI plotting utility
 Home-page: https://github.com/rlschuller/plt
 Author: Rodrigo Loro Schuller
 Author-email: rloroschuller@gmail.com
 Project-URL: Bug Tracker, https://github.com/rlschuller/plt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `plt-cli-0.1.5/plt/plt` & `plt-cli-0.1.6/plt/plt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -116,21 +116,21 @@
 template = re.sub('<<LABELS:.*>>', str(labels), template)
 template = re.sub('<<HEIGHT:.*>>', str(h), template)
 template = re.sub('<<WIDTH:.*>>', str(w), template)
 template = re.sub('<<DATA:.*>>', str(vv), template)
 if args.alpha:
     template = re.sub('<<ALPHA:.*>>', str(args.alpha), template)
 
-# substitute remaining by default values
-template = re.sub('<<.*:', '', template)
-template = re.sub('>>', '', template)
-
 
 if plot_type == "histogram" or plot_type == "density" or plot_type == "normalized_histogram":
     template = re.sub('<<BINS:.*>>', str(bins), template)
 if plot_type == "scatter":
     template = re.sub('<<SCATTER_SIZE:.*>>', str(scatter_size), template)
 
+# substitute remaining by default values
+template = re.sub('<<.*:', '', template)
+template = re.sub('>>', '', template)
+
 if args.py:
     print(template)
 else:
     exec(template, {})
```

### Comparing `plt-cli-0.1.5/plt/templates/python/matplotlib/density.py` & `plt-cli-0.1.6/plt/templates/python/matplotlib/density.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/matplotlib/histogram.py` & `plt-cli-0.1.6/plt/templates/python/matplotlib/histogram.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/matplotlib/line.py` & `plt-cli-0.1.6/plt/templates/python/matplotlib/line.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/matplotlib/normalized_histogram.py` & `plt-cli-0.1.6/plt/templates/python/matplotlib/normalized_histogram.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/matplotlib/scatter.py` & `plt-cli-0.1.6/plt/templates/python/matplotlib/scatter.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/plotext/density.py` & `plt-cli-0.1.6/plt/templates/python/plotext/density.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/plotext/histogram.py` & `plt-cli-0.1.6/plt/templates/python/plotext/histogram.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt/templates/python/plotext/scatter.py` & `plt-cli-0.1.6/plt/templates/python/plotext/scatter.py`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/plt_cli.egg-info/PKG-INFO` & `plt-cli-0.1.6/plt_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plt-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI plotting utility
 Home-page: https://github.com/rlschuller/plt
 Author: Rodrigo Loro Schuller
 Author-email: rloroschuller@gmail.com
 Project-URL: Bug Tracker, https://github.com/rlschuller/plt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `plt-cli-0.1.5/plt_cli.egg-info/SOURCES.txt` & `plt-cli-0.1.6/plt_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plt-cli-0.1.5/setup.cfg` & `plt-cli-0.1.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plt-cli
-version = 0.1.5
+version = 0.1.6
 author = Rodrigo Loro Schuller
 author_email = rloroschuller@gmail.com
 description = A CLI plotting utility
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rlschuller/plt
 project_urls =
```

