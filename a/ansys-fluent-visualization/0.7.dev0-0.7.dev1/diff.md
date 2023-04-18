# Comparing `tmp/ansys_fluent_visualization-0.7.dev0.tar.gz` & `tmp/ansys_fluent_visualization-0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_visualization-0.7.dev0.tar", max compression
+gzip compressed data, was "ansys_fluent_visualization-0.7.dev1.tar", max compression
```

## Comparing `ansys_fluent_visualization-0.7.dev0.tar` & `ansys_fluent_visualization-0.7.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1089 2023-01-31 18:39:22.296802 ansys_fluent_visualization-0.7.dev0/LICENSE
--rw-r--r--   0        0        0     5222 2023-01-31 18:39:22.296802 ansys_fluent_visualization-0.7.dev0/README.rst
--rw-r--r--   0        0        0     1316 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/pyproject.toml
--rw-r--r--   0        0        0     3776 2023-01-31 18:39:22.592802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/__init__.py
--rw-r--r--   0        0        0      913 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/_config.py
--rw-r--r--   0        0        0      274 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/__init__.py
--rw-r--r--   0        0        0     2495 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
--rw-r--r--   0        0        0    13272 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
--rw-r--r--   0        0        0     6935 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
--rw-r--r--   0        0        0    14981 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/post_data_extractor.py
--rw-r--r--   0        0        0     4337 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/post_windows_manager.py
--rw-r--r--   0        0        0      268 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/pyvista/__init__.py
--rw-r--r--   0        0        0     5221 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
--rw-r--r--   0        0        0    26092 2023-01-31 18:39:22.300802 ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
--rw-r--r--   0        0        0     6518 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-13 09:17:37.609464 ansys_fluent_visualization-0.7.dev1/LICENSE
+-rw-r--r--   0        0        0     5222 2023-04-13 09:17:37.609464 ansys_fluent_visualization-0.7.dev1/README.rst
+-rw-r--r--   0        0        0     1316 2023-04-13 09:17:37.613464 ansys_fluent_visualization-0.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3774 2023-04-13 09:17:37.965467 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/_config.py
+-rw-r--r--   0        0        0      274 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/__init__.py
+-rw-r--r--   0        0        0     2495 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
+-rw-r--r--   0        0        0    13270 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
+-rw-r--r--   0        0        0     6935 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
+-rw-r--r--   0        0        0    14981 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_data_extractor.py
+-rw-r--r--   0        0        0     4337 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_windows_manager.py
+-rw-r--r--   0        0        0      268 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/__init__.py
+-rw-r--r--   0        0        0     6391 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
+-rw-r--r--   0        0        0    30842 2023-04-13 09:17:37.617464 ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
+-rw-r--r--   0        0        0     6518 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.7.dev1/PKG-INFO
```

### Comparing `ansys_fluent_visualization-0.7.dev0/LICENSE` & `ansys_fluent_visualization-0.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/README.rst` & `ansys_fluent_visualization-0.7.dev1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-PyFluent Visualization
+PyFluent-Visualization
 ======================
 |pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
```

### Comparing `ansys_fluent_visualization-0.7.dev0/pyproject.toml` & `ansys_fluent_visualization-0.7.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-visualization"
-version = "0.7.dev0"
+version = "0.7.dev1"
 description = "A python wrapper for ansys Fluent visualization"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pyfluent-visualization"
 classifiers = [
```

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/__init__.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pkg_resources
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-_VERSION_INFO = "Build date: January 31, 2023 18:39 UTC ShaID: 3149d03"
+_VERSION_INFO = "Build date: April 13, 2023 09:17 UTC ShaID: 6c5067a"
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 def version_info() -> str:
     """Method returning the version of PyFluent being used.
     Returns
     -------
```

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/_config.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/_config.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for matplotlib windows management."""
 import itertools
 import multiprocessing as mp
 from typing import Dict, List, Optional, Union
 
-from ansys.fluent.core.fluent_connection import _FluentConnection
+from ansys.fluent.core.fluent_connection import FluentConnection
 from ansys.fluent.core.post_objects.post_object_definitions import (
     MonitorDefn,
     PlotDefn,
     XYPlotDefn,
 )
 from ansys.fluent.core.utils.generic import AbstractSingletonMeta, in_notebook
 
@@ -34,15 +34,15 @@
         self._closed = False
         self.plot_pipe, plotter_pipe = mp.Pipe()
         self.plotter = ProcessPlotter(window_id, curves, title, xlabel, ylabel)
         self.plot_process = mp.Process(
             target=self.plotter, args=(plotter_pipe,), daemon=True
         )
         self.plot_process.start()
-        _FluentConnection._monitor_thread.cbs.append(self.close)
+        FluentConnection._monitor_thread.cbs.append(self.close)
 
     def plot(self, data):
         self.plot_pipe.send(data)
 
     def set_properties(self, properties):
         self.plot_pipe.send({"properties": properties})
```

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/post_data_extractor.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_data_extractor.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/post_windows_manager.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/post_windows_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py`

 * *Files 25% similar despite different names*

```diff
@@ -55,24 +55,29 @@
         mesh1 = graphics_session.Meshes["mesh-1"]
         mesh1.show_edges = True
         mesh1.surfaces_list = ['wall']
         mesh1.display("window-0")
     """
 
     @Command
-    def display(self, window_id: Optional[str] = None):
+    def display(self, window_id: Optional[str] = None, overlay: Optional[bool] = False):
         """Display mesh graphics.
 
         Parameters
         ----------
         window_id : str, optional
             Window ID. If an ID is not specified, a unique ID is used.
             The default is ``None``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         """
-        pyvista_windows_manager.plot(self, window_id)
+        pyvista_windows_manager.plot(
+            self, window_id=window_id, overlay=overlay, fetch_data=True
+        )
 
 
 class Pathlines(PathlinesDefn):
     """Pathlines definition for PyVista.
 
     .. code-block:: python
 
@@ -82,24 +87,29 @@
         pathlines1 = graphics_session.Pathlines["pathlines-1"]
         pathlines1.field = "velocity-magnitude"
         pathlines1.surfaces_list = ['inlet']
         pathlines1.display("window-0")
     """
 
     @Command
-    def display(self, window_id: Optional[str] = None):
+    def display(self, window_id: Optional[str] = None, overlay: Optional[bool] = False):
         """Display mesh graphics.
 
         Parameters
         ----------
         window_id : str, optional
             Window ID. If an ID is not specified, a unique ID is used.
             The default is ``None``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         """
-        pyvista_windows_manager.plot(self, window_id)
+        pyvista_windows_manager.plot(
+            self, window_id=window_id, overlay=overlay, fetch_data=True
+        )
 
 
 class Surface(SurfaceDefn):
     """Provides for displaying surface graphics.
 
     Parameters
     ----------
@@ -120,24 +130,29 @@
         surface1.definition.iso_surface.field= "velocity-magnitude"
         surface1.definition.iso_surface.rendering= "contour"
         surface1.definition.iso_surface.iso_value = 0.0
         surface1.display("window-0")
     """
 
     @Command
-    def display(self, window_id: Optional[str] = None):
+    def display(self, window_id: Optional[str] = None, overlay: Optional[bool] = False):
         """Display surface graphics.
 
         Parameters
         ----------
         window_id : str, optional
             Window ID. If an ID is not specified, a unique ID is used.
             The default is ``None``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         """
-        pyvista_windows_manager.plot(self, window_id)
+        pyvista_windows_manager.plot(
+            self, window_id=window_id, overlay=overlay, fetch_data=True
+        )
 
 
 class Contour(ContourDefn):
     """Provides for displaying contour graphics.
 
     Parameters
     ----------
@@ -156,24 +171,29 @@
         contour1 = graphics_session.Contours["contour-1"]
         contour1.field = "velocity-magnitude"
         contour1.surfaces_list = ['wall']
         contour1.display("window-0")
     """
 
     @Command
-    def display(self, window_id: Optional[str] = None):
+    def display(self, window_id: Optional[str] = None, overlay: Optional[bool] = False):
         """Display contour graphics.
 
         Parameters
         ----------
         window_id : str, optional
             Window ID. If an ID is not specified, a unique ID is used.
             The default is ``None``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         """
-        pyvista_windows_manager.plot(self, window_id)
+        pyvista_windows_manager.plot(
+            self, window_id=window_id, overlay=overlay, fetch_data=True
+        )
 
 
 class Vector(VectorDefn):
     """Provides for displaying vector graphics.
 
     Parameters
     ----------
@@ -193,17 +213,22 @@
         vector1.surfaces_list  = ['symmetry']
         vector1.scale = 4.0
         vector1.skip = 4
         vector1.display("window-0")
     """
 
     @Command
-    def display(self, window_id: Optional[str] = None):
+    def display(self, window_id: Optional[str] = None, overlay: Optional[bool] = False):
         """Display vector graphics.
 
         Parameters
         ----------
         window_id : str, optional
             Window ID. If an ID is not specified, a unique ID is used.
             The default is ``None``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         """
-        pyvista_windows_manager.plot(self, window_id)
+        pyvista_windows_manager.plot(
+            self, window_id=window_id, overlay=overlay, fetch_data=True
+        )
```

### Comparing `ansys_fluent_visualization-0.7.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py` & `ansys_fluent_visualization-0.7.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Module for pyVista windows management."""
+from enum import Enum
 import itertools
 import threading
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
-from ansys.fluent.core.fluent_connection import _FluentConnection
+from ansys.fluent.core.fluent_connection import FluentConnection
 from ansys.fluent.core.post_objects.post_object_definitions import GraphicsDefn
 from ansys.fluent.core.utils.generic import AbstractSingletonMeta, in_notebook
 import numpy as np
 import pyvista as pv
 from pyvistaqt import BackgroundPlotter
 
 from ansys.fluent.visualization import get_config
 from ansys.fluent.visualization.post_data_extractor import FieldDataExtractor
 from ansys.fluent.visualization.post_windows_manager import (
     PostWindow,
     PostWindowsManager,
 )
 
 
+class FieldDataType(Enum):
+    """Provides surface data types."""
+
+    Meshes = 1
+    Vectors = 2
+    Contours = 3
+    Pathlines = 4
+
+
 class PyVistaWindow(PostWindow):
     """Provides for managing PyVista windows."""
 
     def __init__(self, id: str, post_object: GraphicsDefn):
         """Instantiate a PyVista window.
 
         Parameters
@@ -34,32 +44,76 @@
         self.post_object: GraphicsDefn = post_object
         self.id: str = id
         self.plotter: Union[BackgroundPlotter, pv.Plotter] = (
             pv.Plotter(title=f"PyFluent ({self.id})")
             if in_notebook() or get_config()["blocking"]
             else BackgroundPlotter(title=f"PyFluent ({self.id})")
         )
+        self.overlay: bool = False
+        self.fetch_data: bool = False
+        self.show_window: bool = True
         self.animate: bool = False
         self.close: bool = False
         self.refresh: bool = False
         self.update: bool = False
         self._visible: bool = False
         self._init_properties()
+        self._data = {}
+        self._colors = {
+            "red": [255, 0, 0],
+            "lime": [0, 255, 0],
+            "blue": [0, 0, 255],
+            "yellow": [255, 255, 0],
+            "cyan": [0, 255, 255],
+            "magenta": [255, 0, 255],
+            "silver": [192, 192, 192],
+            "gray": [128, 128, 128],
+            "maroon": [128, 0, 0],
+            "olive": [128, 128, 0],
+            "green": [0, 128, 0],
+            "purple": [128, 0, 128],
+            "teal": [0, 128, 128],
+            "navy": [0, 0, 128],
+            "orange": [255, 165, 0],
+            "brown": [210, 105, 30],
+            "white": [255, 255, 255],
+        }
+
+    def set_data(self, data_type: FieldDataType, data: Dict[int, Dict[str, np.array]]):
+        """Set data for graphics."""
+        self._data[data_type] = data
 
-    def plot(self):
-        """Plot graphics."""
+    def fetch(self):
+        """Fetch data for graphics."""
+        if not self.post_object:
+            return
+        obj = self.post_object
+        if obj.__class__.__name__ == "Mesh":
+            self._fetch_mesh(obj)
+        elif obj.__class__.__name__ == "Surface":
+            self._fetch_surface(obj)
+        elif obj.__class__.__name__ == "Contour":
+            self._fetch_contour(obj)
+        elif obj.__class__.__name__ == "Vector":
+            self._fetch_vector(obj)
+        elif obj.__class__.__name__ == "Pathlines":
+            self._fetch_pathlines(obj)
+
+    def render(self):
+        """Render graphics."""
         if not self.post_object:
             return
         obj = self.post_object
         plotter = self.plotter
         camera = plotter.camera.copy()
-        if in_notebook() and self.plotter.theme._jupyter_backend == "pythreejs":
-            plotter.remove_actor(plotter.renderer.actors.copy())
-        else:
-            plotter.clear()
+        if not self.overlay:
+            if in_notebook() and self.plotter.theme._jupyter_backend == "pythreejs":
+                plotter.remove_actor(plotter.renderer.actors.copy())
+            else:
+                plotter.clear()
         if obj.__class__.__name__ == "Mesh":
             self._display_mesh(obj, plotter)
         elif obj.__class__.__name__ == "Surface":
             self._display_surface(obj, plotter)
         elif obj.__class__.__name__ == "Contour":
             self._display_contour(obj, plotter)
         elif obj.__class__.__name__ == "Vector":
@@ -78,18 +132,23 @@
             "zy": plotter.view_zy,
             "isometric": plotter.view_isometric,
         }.get(view)
         if view_fun:
             view_fun()
         else:
             plotter.camera = camera.copy()
-        if not self._visible:
+        if not self._visible and self.show_window:
             plotter.show()
             self._visible = True
 
+    def plot(self):
+        """Display graphics."""
+        self.fetch()
+        self.render()
+
     # private methods
 
     def _init_properties(self):
         self.plotter.theme.cmap = "jet"
         self.plotter.background_color = "white"
         self.plotter.theme.font.color = "black"
 
@@ -101,27 +160,29 @@
             fmt="%.6e",
             font_family="arial",
             vertical=True,
             position_x=0.06,
             position_y=0.3,
         )
 
-    def _display_vector(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
+    def _fetch_vector(self, obj):
+        if self._data.get(FieldDataType.Vectors) is None or self.fetch_data:
+            self._data[FieldDataType.Vectors] = FieldDataExtractor(obj).fetch_data()
 
-        vector_field_data = FieldDataExtractor(obj).fetch_data()
+    def _display_vector(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
         field_info = obj._api_helper.field_info()
         vectors_of = obj.vectors_of()
         # scalar bar properties
         scalar_bar_args = self._scalar_bar_default_properties()
 
         field = obj.field()
         field_unit = obj._api_helper.get_field_unit(field)
         field = f"{field}\n[{field_unit}]" if field_unit else field
 
-        for surface_id, mesh_data in vector_field_data.items():
+        for surface_id, mesh_data in self._data[FieldDataType.Vectors].items():
             if "vertices" not in mesh_data or "faces" not in mesh_data:
                 continue
             mesh_data["vertices"].shape = mesh_data["vertices"].size // 3, 3
             mesh_data[obj.vectors_of()].shape = (
                 mesh_data[obj.vectors_of()].size // 3,
                 3,
             )
@@ -148,15 +209,15 @@
                         velocity_magnitude,
                         auto_range_off.minimum(),
                         auto_range_off.maximum(),
                     ).filled(fill_value=0)
             else:
                 auto_range_on = obj.range.auto_range_on
                 if auto_range_on.global_range():
-                    range = field_info.get_range(obj.field(), False)
+                    range = field_info.get_scalar_fields_range(obj.field(), False)
                 else:
                     range = [np.min(scalar_field), np.max(scalar_field)]
 
             if obj.skip():
                 vmag = np.zeros(velocity_magnitude.size)
                 vmag[:: obj.skip() + 1] = velocity_magnitude[:: obj.skip() + 1]
                 velocity_magnitude = vmag
@@ -173,26 +234,29 @@
                 scalars=field,
                 scalar_bar_args=scalar_bar_args,
                 clim=range,
             )
             if obj.show_edges():
                 plotter.add_mesh(mesh, show_edges=True, color="white")
 
+    def _fetch_pathlines(self, obj):
+        if self._data.get(FieldDataType.Pathlines) is None or self.fetch_data:
+            self._data[FieldDataType.Pathlines] = FieldDataExtractor(obj).fetch_data()
+
     def _display_pathlines(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
         field = obj.field()
         field_unit = obj._api_helper.get_field_unit(field)
         field = f"{field}\n[{field_unit}]" if field_unit else field
         node_values = True
 
         # scalar bar properties
         scalar_bar_args = self._scalar_bar_default_properties()
-        data = FieldDataExtractor(obj).fetch_data()
 
         # loop over all meshes
-        for surface_id, surface_data in data.items():
+        for surface_id, surface_data in self._data[FieldDataType.Pathlines].items():
             if "vertices" not in surface_data or "lines" not in surface_data:
                 continue
             surface_data["vertices"].shape = surface_data["vertices"].size // 3, 3
 
             mesh = pv.PolyData(
                 surface_data["vertices"],
                 lines=surface_data["lines"],
@@ -204,31 +268,34 @@
                 mesh.cell_data[field] = surface_data[obj.field()]
             plotter.add_mesh(
                 mesh,
                 scalars=field,
                 scalar_bar_args=scalar_bar_args,
             )
 
+    def _fetch_contour(self, obj):
+        if self._data.get(FieldDataType.Contours) is None or self.fetch_data:
+            self._data[FieldDataType.Contours] = FieldDataExtractor(obj).fetch_data()
+
     def _display_contour(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
         # contour properties
         field = obj.field()
         field_unit = obj._api_helper.get_field_unit(field)
         field = f"{field}\n[{field_unit}]" if field_unit else field
         range_option = obj.range.option()
         filled = obj.filled()
         contour_lines = obj.contour_lines()
         node_values = obj.node_values()
         boundary_values = obj.boundary_values()
 
         # scalar bar properties
         scalar_bar_args = self._scalar_bar_default_properties()
-        scalar_field_data = FieldDataExtractor(obj).fetch_data()
 
         # loop over all meshes
-        for surface_id, surface_data in scalar_field_data.items():
+        for surface_id, surface_data in self._data[FieldDataType.Contours].items():
             if "vertices" not in surface_data or "faces" not in surface_data:
                 continue
             surface_data["vertices"].shape = surface_data["vertices"].size // 3, 3
             topology = "line" if surface_data["faces"][0] == 2 else "face"
             if topology == "line":
                 mesh = pv.PolyData(
                     surface_data["vertices"],
@@ -289,15 +356,15 @@
             else:
                 auto_range_on = obj.range.auto_range_on
                 if auto_range_on.global_range():
                     if filled:
                         field_info = obj._api_helper.field_info()
                         plotter.add_mesh(
                             mesh,
-                            clim=field_info.get_range(obj.field(), False),
+                            clim=field_info.get_scalar_fields_range(obj.field(), False),
                             scalars=field,
                             show_edges=obj.show_edges(),
                             scalar_bar_args=scalar_bar_args,
                         )
                     if (not filled or contour_lines) and (
                         np.min(mesh[field]) != np.max(mesh[field])
                     ):
@@ -312,57 +379,84 @@
                             scalar_bar_args=scalar_bar_args,
                         )
                     if (not filled or contour_lines) and (
                         np.min(mesh[field]) != np.max(mesh[field])
                     ):
                         plotter.add_mesh(mesh.contour(isosurfaces=20))
 
-    def _display_surface(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
+    def _fetch_surface(self, obj):
         surface_api = obj._api_helper.surface_api
         surface_api.create_surface_on_server()
         dummy_object = "dummy_object"
         post_session = obj._get_top_most_parent()
         if (
             obj.definition.type() == "iso-surface"
             and obj.definition.iso_surface.rendering() == "contour"
         ):
             contour = post_session.Contours[dummy_object]
             contour.field = obj.definition.iso_surface.field()
             contour.surfaces_list = [obj._name]
             contour.show_edges = obj.show_edges()
             contour.range.auto_range_on.global_range = True
+            contour.boundary_values = True
+            self._fetch_contour(contour)
+            del post_session.Contours[dummy_object]
+        else:
+            mesh = post_session.Meshes[dummy_object]
+            mesh.surfaces_list = [obj._name]
+            mesh.show_edges = obj.show_edges()
+            self._fetch_mesh(mesh)
+            del post_session.Meshes[dummy_object]
+        surface_api.delete_surface_on_server()
+
+    def _display_surface(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
+        dummy_object = "dummy_object"
+        post_session = obj._get_top_most_parent()
+        if (
+            obj.definition.type() == "iso-surface"
+            and obj.definition.iso_surface.rendering() == "contour"
+        ):
+            contour = post_session.Contours[dummy_object]
+            contour.field = obj.definition.iso_surface.field()
+            contour.surfaces_list = [obj._name]
+            contour.show_edges = obj.show_edges()
+            contour.range.auto_range_on.global_range = True
+            contour.boundary_values = True
             self._display_contour(contour, plotter)
             del post_session.Contours[dummy_object]
         else:
             mesh = post_session.Meshes[dummy_object]
             mesh.surfaces_list = [obj._name]
             mesh.show_edges = obj.show_edges()
             self._display_mesh(mesh, plotter)
             del post_session.Meshes[dummy_object]
-        surface_api.delete_surface_on_server()
 
-    def _display_mesh(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
+    def _fetch_mesh(self, obj):
+        if self._data.get(FieldDataType.Meshes) is None or self.fetch_data:
+            self._data[FieldDataType.Meshes] = FieldDataExtractor(obj).fetch_data()
 
-        surfaces_data = FieldDataExtractor(obj).fetch_data()
-        for surface_id, mesh_data in surfaces_data.items():
+    def _display_mesh(self, obj, plotter: Union[BackgroundPlotter, pv.Plotter]):
+        for surface_id, mesh_data in self._data[FieldDataType.Meshes].items():
             if "vertices" not in mesh_data or "faces" not in mesh_data:
                 continue
             mesh_data["vertices"].shape = mesh_data["vertices"].size // 3, 3
             topology = "line" if mesh_data["faces"][0] == 2 else "face"
             if topology == "line":
                 mesh = pv.PolyData(
                     mesh_data["vertices"],
                     lines=mesh_data["faces"],
                 )
             else:
                 mesh = pv.PolyData(
                     mesh_data["vertices"],
                     faces=mesh_data["faces"],
                 )
-            plotter.add_mesh(mesh, show_edges=obj.show_edges(), color="lightgrey")
+            color_size = len(self._colors.values())
+            color = list(self._colors.values())[surface_id % color_size]
+            plotter.add_mesh(mesh, show_edges=obj.show_edges(), color=color)
 
     def _get_refresh_for_plotter(self, window: "PyVistaWindow"):
         def refresh():
 
             with PyVistaWindowsManager._condition:
                 plotter = window.plotter
                 if window.close:
@@ -390,14 +484,30 @@
         self._post_windows: Dict[str:PyVistaWindow] = {}
         self._plotter_thread: threading.Thread = None
         self._post_object: GraphicsDefn = None
         self._window_id: str = None
         self._exit_thread: bool = False
         self._app = None
 
+    def get_window(self, window_id: str) -> PyVistaWindow:
+        """Get the PyVista window.
+
+        Parameters
+        ----------
+        window_id : str
+            Window ID.
+
+        Returns
+        -------
+        PyVistaWindow
+            PyVista window.
+        """
+        with self._condition:
+            return self._post_windows.get(window_id, None)
+
     def get_plotter(self, window_id: str) -> Union[BackgroundPlotter, pv.Plotter]:
         """Get the PyVista plotter.
 
         Parameters
         ----------
         window_id : str
             Window ID for the plotter.
@@ -424,15 +534,15 @@
         str
             ID for the new window.
         """
         with self._condition:
             if not window_id:
                 window_id = self._get_unique_window_id()
             if in_notebook() or get_config()["blocking"]:
-                self._open_window_notebook(window_id)
+                window = self._open_window_notebook(window_id)
             else:
                 self._open_and_plot_console(None, window_id)
             return window_id
 
     def set_object_for_window(self, object: GraphicsDefn, window_id: str) -> None:
         """Associate a visualization object with a running window instance.
 
@@ -451,39 +561,49 @@
         if not isinstance(object, GraphicsDefn):
             raise RuntimeError("Object type currently not supported.")
         with self._condition:
             window = self._post_windows.get(window_id)
             if window:
                 window.post_object = object
 
-    def plot(self, object: GraphicsDefn, window_id: Optional[str] = None) -> None:
+    def plot(
+        self,
+        object: GraphicsDefn,
+        window_id: Optional[str] = None,
+        fetch_data: Optional[bool] = False,
+        overlay: Optional[bool] = False,
+    ) -> None:
         """Draw a plot.
 
         Parameters
         ----------
         object: GraphicsDefn
             Object to plot.
         window_id : str, optional
             Window ID for the plot. The default is ``None``, in which
             case a unique ID is assigned.
-
+        fetch_data : bool, optional
+            Whether to fetch data. The default is ``False``.
+        overlay : bool, optional
+            Whether to overlay graphics over existing graphics.
+            The default is ``False``.
         Raises
         ------
         RuntimeError
             If the window does not support the object.
         """
         if not isinstance(object, GraphicsDefn):
             raise RuntimeError("Object type currently not supported.")
         with self._condition:
             if not window_id:
                 window_id = self._get_unique_window_id()
             if in_notebook() or get_config()["blocking"]:
-                self._plot_notebook(object, window_id)
+                self._plot_notebook(object, window_id, fetch_data, overlay)
             else:
-                self._open_and_plot_console(object, window_id)
+                self._open_and_plot_console(object, window_id, fetch_data, overlay)
 
     def save_graphic(
         self,
         window_id: str,
         format: str,
     ) -> None:
         """Save a graphic.
@@ -602,38 +722,48 @@
                         plotter = window.plotter
                         self._app = plotter.app
                         plotter.add_callback(
                             window._get_refresh_for_plotter(window),
                             100,
                         )
                     window.post_object = self._post_object
+                    window.fetch_data = self._fetch_data
+                    window.overlay = self._overlay
                     window.animate = animate
                     window.update = True
                     self._post_windows[self._window_id] = window
                     self._post_object = None
                     self._window_id = None
             self._app.processEvents()
         with self._condition:
             for window in self._post_windows.values():
                 plotter = window.plotter
                 plotter.close()
                 plotter.app.quit()
             self._post_windows.clear()
             self._condition.notify()
 
-    def _open_and_plot_console(self, obj: object, window_id: str) -> None:
+    def _open_and_plot_console(
+        self,
+        obj: object,
+        window_id: str,
+        fetch_data: bool = False,
+        overlay: bool = False,
+    ) -> None:
         if self._exit_thread:
             return
         with self._condition:
             self._window_id = window_id
             self._post_object = obj
+            self._fetch_data = fetch_data
+            self._overlay = overlay
 
         if not self._plotter_thread:
-            if _FluentConnection._monitor_thread:
-                _FluentConnection._monitor_thread.cbs.append(self._exit)
+            if FluentConnection._monitor_thread:
+                FluentConnection._monitor_thread.cbs.append(self._exit)
             self._plotter_thread = threading.Thread(target=self._display, args=())
             self._plotter_thread.start()
 
         with self._condition:
             self._condition.wait()
 
     def _open_window_notebook(self, window_id: str) -> pv.Plotter:
@@ -642,17 +772,21 @@
         if window and not window.close and window.refresh:
             window.refresh = False
         else:
             window = PyVistaWindow(window_id, None)
             self._post_windows[window_id] = window
         return window
 
-    def _plot_notebook(self, obj: object, window_id: str) -> None:
+    def _plot_notebook(
+        self, obj: object, window_id: str, fetch_data: bool, overlay: bool
+    ) -> None:
         window = self._open_window_notebook(window_id)
         window.post_object = obj
+        window.fetch_data = fetch_data
+        window.overlay = overlay
         plotter = window.plotter
         window.plot()
 
     def _get_windows_id(
         self,
         session_id: Optional[str] = "",
         windows_id: Optional[List[str]] = [],
```

### Comparing `ansys_fluent_visualization-0.7.dev0/PKG-INFO` & `ansys_fluent_visualization-0.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-fluent-visualization
-Version: 0.7.dev0
+Version: 0.7.dev1
 Summary: A python wrapper for ansys Fluent visualization
 Home-page: https://github.com/pyansys/pyfluent-visualization
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
@@ -25,15 +25,15 @@
 Requires-Dist: pyside6 (>=6.2.3)
 Requires-Dist: pyvista (>=0.33.2)
 Requires-Dist: pyvistaqt (>=0.7.0)
 Requires-Dist: vtk (>=9.0.3) ; python_full_version <= "3.9.0"
 Project-URL: Repository, https://github.com/pyansys/pyfluent-visualization
 Description-Content-Type: text/x-rst
 
-PyFluent Visualization
+PyFluent-Visualization
 ======================
 |pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
```

