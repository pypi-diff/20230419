# Comparing `tmp/living-figures-0.1.2.tar.gz` & `tmp/living-figures-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.1.2.tar", last modified: Wed Apr 19 18:16:06 2023, max compression
+gzip compressed data, was "living-figures-0.1.3.tar", last modified: Wed Apr 19 18:33:30 2023, max compression
```

## Comparing `living-figures-0.1.2.tar` & `living-figures-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 18:15:11.000000 living-figures-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 18:15:11.000000 living-figures-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:16:06.180855 living-figures-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 18:15:11.000000 living-figures-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-19 18:15:11.000000 living-figures-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:15:11.000000 living-figures-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:16:06.180855 living-figures-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 18:15:11.000000 living-figures-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.176855 living-figures-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.176855 living-figures-0.1.2/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/epigenome/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/epigenome/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/pacbio_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/epigenome/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/epigenome/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 18:15:11.000000 living-figures-0.1.2/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:16:06.000000 living-figures-0.1.2/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 18:16:06.000000 living-figures-0.1.2/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:16:06.000000 living-figures-0.1.2/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:16:06.000000 living-figures-0.1.2/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 18:16:06.000000 living-figures-0.1.2/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:16:06.180855 living-figures-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 18:15:11.000000 living-figures-0.1.2/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 18:32:43.000000 living-figures-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 18:32:43.000000 living-figures-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:33:30.743426 living-figures-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 18:32:43.000000 living-figures-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-19 18:32:43.000000 living-figures-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:32:43.000000 living-figures-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:33:30.743426 living-figures-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 18:32:43.000000 living-figures-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.739426 living-figures-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 18:32:43.000000 living-figures-0.1.3/tests/test_import.py
```

### Comparing `living-figures-0.1.2/LICENSE` & `living-figures-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/PKG-INFO` & `living-figures-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.2
+Version: 0.1.3
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.2/README.md` & `living-figures-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/pyproject.toml` & `living-figures-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py` & `living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/pacbio_file.py` & `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,28 @@
         value=None,
         label="PacBio Motifs",
         help: Union[str, None] = None,
         disabled: bool = False,
         label_visibility: str = "visible",
         sidebar=True,
         show_uploader=True,
-        cname_map={},
+        cname_map={
+            "Motif": "motifString",
+            "Modified Position": "centerPos",
+            "Motification Type": "modificationType",
+            "% of Motifs Detected": "fraction",
+            "# of Motifs Detected": "nDetected",
+            "# of Motifs in Genome": "nGenome",
+            "Mean QV": "meanScore",
+            "Mean Coverage": "meanCoverage",
+            "Partner Motif": "partnerMotifString",
+            "Mean IPD ratio": "meanIpdRatio",
+            "Group Tag": "groupTag",
+            "Objective Score": "objectiveScore"
+        },
         **kwargs
     ):
         """
         Args:
             id (str):       The unique key for the resource.
             label (str):    (optional) Label used for user input display
                             elements.
```

### Comparing `living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/parse_rebase.py` & `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/epigenome/utilities/rebase_file.py` & `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/epigenome/widgets/panepibrowser.py` & `living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/volcano/app.py` & `living-figures-0.1.3/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.1.3/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures/helpers/sorting.py` & `living-figures-0.1.3/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.1.3/src/living_figures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.2
+Version: 0.1.3
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.2/src/living_figures.egg-info/SOURCES.txt` & `living-figures-0.1.3/src/living_figures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.2/tests/test_import.py` & `living-figures-0.1.3/tests/test_import.py`

 * *Files identical despite different names*

