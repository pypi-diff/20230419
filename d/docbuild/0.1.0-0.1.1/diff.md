# Comparing `tmp/docbuild-0.1.0.tar.gz` & `tmp/docbuild-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.0.tar", last modified: Wed Apr 19 09:12:46 2023, max compression
+gzip compressed data, was "docbuild-0.1.1.tar", last modified: Wed Apr 19 14:38:00 2023, max compression
```

## Comparing `docbuild-0.1.0.tar` & `docbuild-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 09:12:46.997613 docbuild-0.1.0/
--rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 09:12:46.997132 docbuild-0.1.0/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.0/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 09:12:46.992778 docbuild-0.1.0/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       61 2023-04-19 06:11:50.000000 docbuild-0.1.0/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      408 2023-04-19 09:10:09.000000 docbuild-0.1.0/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.0/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.0/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     6942 2023-04-19 09:11:18.000000 docbuild-0.1.0/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 09:12:46.995222 docbuild-0.1.0/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.0/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.0/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-19 06:25:05.000000 docbuild-0.1.0/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.0/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.0/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-19 06:25:19.000000 docbuild-0.1.0/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.0/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 09:12:46.996647 docbuild-0.1.0/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.0/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 09:11:07.000000 docbuild-0.1.0/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      158 2023-04-19 09:10:38.000000 docbuild-0.1.0/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16376 2023-04-19 09:12:11.000000 docbuild-0.1.0/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 09:12:46.993857 docbuild-0.1.0/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 09:12:46.000000 docbuild-0.1.0/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-19 09:12:46.000000 docbuild-0.1.0/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-19 09:12:46.000000 docbuild-0.1.0/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       28 2023-04-19 09:12:46.000000 docbuild-0.1.0/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-19 09:12:46.000000 docbuild-0.1.0/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-19 09:12:46.997696 docbuild-0.1.0/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      753 2023-04-19 09:12:44.000000 docbuild-0.1.0/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.504817 docbuild-0.1.1/
+-rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 14:38:00.504651 docbuild-0.1.1/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.1/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.500513 docbuild-0.1.1/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-19 14:36:50.000000 docbuild-0.1.1/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      408 2023-04-19 09:10:09.000000 docbuild-0.1.1/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.1/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.1/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     6942 2023-04-19 09:11:18.000000 docbuild-0.1.1/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.503093 docbuild-0.1.1/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.1/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.1/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-19 06:25:05.000000 docbuild-0.1.1/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.1/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.1/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-19 06:25:19.000000 docbuild-0.1.1/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.1/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.504291 docbuild-0.1.1/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.1/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.1/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      158 2023-04-19 09:10:38.000000 docbuild-0.1.1/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16376 2023-04-19 09:12:11.000000 docbuild-0.1.1/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.501829 docbuild-0.1.1/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-19 14:38:00.504858 docbuild-0.1.1/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      830 2023-04-19 14:37:56.000000 docbuild-0.1.1/setup.py
```

### Comparing `docbuild-0.1.0/PKG-INFO` & `docbuild-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.0/docbuild/graph.py` & `docbuild-0.1.1/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/hocr_parser.py` & `docbuild-0.1.1/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/page_creator.py` & `docbuild-0.1.1/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.1/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.1/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.1/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/textract_parser.py` & `docbuild-0.1.1/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/utils.py` & `docbuild-0.1.1/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.1/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.1/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.1/docbuild.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.0/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.1/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.0/setup.py` & `docbuild-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.0",
+    version="0.1.1",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
     install_requires=[
         "attrs>=22.0.0",
         "numpy==1.23.2",
+        "beautifulsoup4>=4.11.1",
+        "opencv-contrib-python==4.6.0.66",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

