# Comparing `tmp/stackview-0.6.1.tar.gz` & `tmp/stackview-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.6.1.tar", last modified: Sat Apr 15 09:29:08 2023, max compression
+gzip compressed data, was "stackview-0.6.2.tar", last modified: Wed Apr 19 19:49:46 2023, max compression
```

## Comparing `stackview-0.6.1.tar` & `stackview-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.228073 stackview-0.6.1/
--rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    10414 2023-04-15 09:29:08.228073 stackview-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     9830 2023-04-15 09:27:34.000000 stackview-0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 09:29:08.228073 stackview-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-04-15 09:27:34.000000 stackview-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.201527 stackview-0.6.1/stackview/
--rw-rw-rw-   0        0        0      586 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/__init__.py
--rw-rw-rw-   0        0        0     7781 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.6.1/stackview/_assist.py
--rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_colormaps.py
--rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.6.1/stackview/_context.py
--rw-rw-rw-   0        0        0     5487 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_crop.py
--rw-rw-rw-   0        0        0     4684 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_curtain.py
--rw-rw-rw-   0        0        0     4070 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     7597 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_interact.py
--rw-rw-rw-   0        0        0     2124 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     3384 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_picker.py
--rw-rw-rw-   0        0        0     5023 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     2149 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_slice.py
--rw-rw-rw-   0        0        0     2350 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8266 2023-01-15 16:10:46.000000 stackview-0.6.1/stackview/_static_view.py
--rw-rw-rw-   0        0        0     6146 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.6.1/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.6.1/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.225590 stackview-0.6.1/stackview.egg-info/
--rw-rw-rw-   0        0        0    10414 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-15 09:29:08.000000 stackview-0.6.1/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.926694 stackview-0.6.2/
+-rw-rw-rw-   0        0        0     1549 2023-04-19 19:02:17.000000 stackview-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0    10414 2023-04-19 19:49:46.926694 stackview-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9830 2023-04-19 19:02:17.000000 stackview-0.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 19:49:46.926694 stackview-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-04-19 19:49:26.000000 stackview-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.905159 stackview-0.6.2/stackview/
+-rw-rw-rw-   0        0        0      586 2023-04-19 19:49:26.000000 stackview-0.6.2/stackview/__init__.py
+-rw-rw-rw-   0        0        0     7781 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_assist.py
+-rw-rw-rw-   0        0        0     5467 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_context.py
+-rw-rw-rw-   0        0        0     5487 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_crop.py
+-rw-rw-rw-   0        0        0     4684 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4070 2023-04-19 19:44:22.000000 stackview-0.6.2/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     7544 2023-04-19 19:49:26.000000 stackview-0.6.2/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2124 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3384 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5023 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2149 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2350 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8266 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6146 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     2567 2023-04-19 19:02:18.000000 stackview-0.6.2/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:49:46.925626 stackview-0.6.2/stackview.egg-info/
+-rw-rw-rw-   0        0        0    10414 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 19:49:46.000000 stackview-0.6.2/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.6.1/LICENSE` & `stackview-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/PKG-INFO` & `stackview-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.1
+Version: 0.6.2
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `stackview-0.6.1/README.md` & `stackview-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/setup.py` & `stackview-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.6.1",
+    version="0.6.2",
     author="Robert Haase",
     author_email="robert.haase@tu-dresden.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
```

### Comparing `stackview-0.6.1/stackview/__init__.py` & `stackview-0.6.2/stackview/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
```

### Comparing `stackview-0.6.1/stackview/_annotate.py` & `stackview-0.6.2/stackview/_annotate.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_assist.py` & `stackview-0.6.2/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_colormaps.py` & `stackview-0.6.2/stackview/_colormaps.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_context.py` & `stackview-0.6.2/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_crop.py` & `stackview-0.6.2/stackview/_crop.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_curtain.py` & `stackview-0.6.2/stackview/_curtain.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_image_widget.py` & `stackview-0.6.2/stackview/_image_widget.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_interact.py` & `stackview-0.6.2/stackview/_interact.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,18 +143,17 @@
             else:
                 command = command + ", " + key + "=" + str(kwargs[key])
         command = command + ")"
         command_label.value = command.replace("(,", "(")
 
         if not execution_blocked:
             if image_passed:
-                viewer.view.data = func(image, *args, **kwargs)
+                viewer.image = func(image, *args, **kwargs)
             else:
-                viewer.view.data = func(*args, **kwargs)
-            viewer.image = viewer.view.data
+                viewer.image = func(*args, **kwargs)
 
         viewer.slice_slider.max = viewer.image.shape[0] - 1
         viewer.configuration_updated(None)
 
 
     worker_function.__signature__ = inspect.Signature(exposable_parameters)
     inter = ipywidgets.interactive(worker_function, dict(manual=False, auto_display=False))
```

### Comparing `stackview-0.6.1/stackview/_orthogonal.py` & `stackview-0.6.2/stackview/_orthogonal.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_picker.py` & `stackview-0.6.2/stackview/_picker.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_side_by_side.py` & `stackview-0.6.2/stackview/_side_by_side.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_slice.py` & `stackview-0.6.2/stackview/_slice.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_slice_viewer.py` & `stackview-0.6.2/stackview/_slice_viewer.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_static_view.py` & `stackview-0.6.2/stackview/_static_view.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_switch.py` & `stackview-0.6.2/stackview/_switch.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_uint_field.py` & `stackview-0.6.2/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview/_utilities.py` & `stackview-0.6.2/stackview/_utilities.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.1/stackview.egg-info/PKG-INFO` & `stackview-0.6.2/stackview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.1
+Version: 0.6.2
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `stackview-0.6.1/stackview.egg-info/SOURCES.txt` & `stackview-0.6.2/stackview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

