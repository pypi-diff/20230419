# Comparing `tmp/ansys_fluent_visualization-0.7.dev1.tar.gz` & `tmp/ansys_fluent_visualization-0.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_visualization-0.7.dev1.tar", max compression
+gzip compressed data, was "ansys_fluent_visualization-0.8.dev0.tar", max compression
```

## Comparing `ansys_fluent_visualization-0.7.dev1.tar` & `ansys_fluent_visualization-0.8.dev0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1089 2023-04-13 09:17:37.609464 ansys_fluent_visualization-0.7.dev1/LICENSE
--rw-r--r--   0        0        0     5222 2023-04-13 09:17:37.609464 ansys_fluent_visualization-0.7.dev1/README.rst
--rw-r--r--   0        0        0     1316 2023-04-13 09:17:37.613464 ansys_fluent_visualization-0.7.dev1/pyproject.toml
--rw-r--r--   0        0        0     3774 2023-04-13 09:17:37.965467 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/__init__.py
--rw-r--r--   0        0        0      913 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/_config.py
--rw-r--r--   0        0        0      274 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/__init__.py
--rw-r--r--   0        0        0     2495 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
--rw-r--r--   0        0        0    13270 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
--rw-r--r--   0        0        0     6935 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
--rw-r--r--   0        0        0    14981 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_data_extractor.py
--rw-r--r--   0        0        0     4337 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_windows_manager.py
--rw-r--r--   0        0        0      268 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/__init__.py
--rw-r--r--   0        0        0     6391 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
--rw-r--r--   0        0        0    30842 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
--rw-r--r--   0        0        0     6518 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-19 01:17:51.197746 ansys_fluent_visualization-0.8.dev0/LICENSE
+-rw-r--r--   0        0        0     5469 2023-04-19 01:17:51.197746 ansys_fluent_visualization-0.8.dev0/README.rst
+-rw-r--r--   0        0        0     1316 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3774 2023-04-19 01:17:51.485754 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/_config.py
+-rw-r--r--   0        0        0      274 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/__init__.py
+-rw-r--r--   0        0        0     2495 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
+-rw-r--r--   0        0        0    13270 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
+-rw-r--r--   0        0        0     6935 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
+-rw-r--r--   0        0        0    14981 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_data_extractor.py
+-rw-r--r--   0        0        0     4337 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_windows_manager.py
+-rw-r--r--   0        0        0      268 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/__init__.py
+-rw-r--r--   0        0        0     6391 2023-04-19 01:17:51.205747 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
+-rw-r--r--   0        0        0    30842 2023-04-19 01:17:51.205747 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.8.dev0/PKG-INFO
```

### Comparing `ansys_fluent_visualization-0.7.dev1/LICENSE` & `ansys_fluent_visualization-0.8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/README.rst` & `ansys_fluent_visualization-0.8.dev0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,23 @@
 `Matplotlib <https://matplotlib.org/>`_.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Visualization, see the latest release
 `documentation <https://fluentvisualization.docs.pyansys.com>`_.
 
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
+
 On the `PyFluent Visualization Issues
 <https://github.com/pyansys/pyfluent-visualization/issues>`_ page, you can create
 issues to submit questions, reports burgs, and request new features. To reach
-the support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
 The ``ansys-fluent-visualization`` package supports Python 3.7 through Python
 3.10 on Windows and Linux.
 
 If you are using Python 3.10, download and install the wheel file for the ``vtk`` package from
```

### Comparing `ansys_fluent_visualization-0.7.dev1/pyproject.toml` & `ansys_fluent_visualization-0.8.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-visualization"
-version = "0.7.dev1"
+version = "0.8.dev0"
 description = "A python wrapper for ansys Fluent visualization"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pyfluent-visualization"
 classifiers = [
```

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/__init__.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pkg_resources
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-_VERSION_INFO = "Build date: April 13, 2023 09:17 UTC ShaID: 6c5067a"
+_VERSION_INFO = "Build date: April 19, 2023 01:17 UTC ShaID: 06a4d74"
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 def version_info() -> str:
     """Method returning the version of PyFluent being used.
     Returns
     -------
```

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/_config.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/_config.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_data_extractor.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_data_extractor.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_windows_manager.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_windows_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py` & `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev1/PKG-INFO` & `ansys_fluent_visualization-0.8.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-fluent-visualization
-Version: 0.7.dev1
+Version: 0.8.dev0
 Summary: A python wrapper for ansys Fluent visualization
 Home-page: https://github.com/pyansys/pyfluent-visualization
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
@@ -65,18 +65,23 @@
 `Matplotlib <https://matplotlib.org/>`_.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Visualization, see the latest release
 `documentation <https://fluentvisualization.docs.pyansys.com>`_.
 
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
+
 On the `PyFluent Visualization Issues
 <https://github.com/pyansys/pyfluent-visualization/issues>`_ page, you can create
 issues to submit questions, reports burgs, and request new features. To reach
-the support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
 The ``ansys-fluent-visualization`` package supports Python 3.7 through Python
 3.10 on Windows and Linux.
 
 If you are using Python 3.10, download and install the wheel file for the ``vtk`` package from
```

