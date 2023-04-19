# Comparing `tmp/wafermap-0.2.1.tar.gz` & `tmp/wafermap-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-0.2.1.tar", max compression
+gzip compressed data, was "wafermap-0.2.2.tar", max compression
```

## Comparing `wafermap-0.2.1.tar` & `wafermap-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.1/LICENSE
--rw-r--r--   0        0        0      897 2023-04-18 22:39:53.903967 wafermap-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7920 2023-04-18 22:34:33.741285 wafermap-0.2.1/README.md
--rw-r--r--   0        0        0      169 2023-04-18 13:32:08.195020 wafermap-0.2.1/wafermap/__init__.py
--rw-r--r--   0        0        0     3033 2023-04-17 22:16:54.410477 wafermap-0.2.1/wafermap/utils.py
--rw-r--r--   0        0        0    25669 2023-04-18 22:16:09.161641 wafermap-0.2.1/wafermap/wafermap.py
--rw-r--r--   0        0        0     8575 1970-01-01 00:00:00.000000 wafermap-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.2/LICENSE
+-rw-r--r--   0        0        0      897 2023-04-19 14:06:18.046113 wafermap-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7982 2023-04-19 13:29:46.122469 wafermap-0.2.2/README.md
+-rw-r--r--   0        0        0      171 2023-04-19 10:42:08.837188 wafermap-0.2.2/wafermap/__init__.py
+-rw-r--r--   0        0        0     3033 2023-04-17 22:16:54.410477 wafermap-0.2.2/wafermap/utils.py
+-rw-r--r--   0        0        0    26339 2023-04-19 13:53:53.176550 wafermap-0.2.2/wafermap/wafermap.py
+-rw-r--r--   0        0        0     8633 1970-01-01 00:00:00.000000 wafermap-0.2.2/PKG-INFO
```

### Comparing `wafermap-0.2.1/LICENSE` & `wafermap-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wafermap-0.2.1/pyproject.toml` & `wafermap-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wafermap"
-version = "0.2.1"
+version = "0.2.2"
 description = "A python package to plot maps of semiconductor wafers."
 authors = ["Sotiris Thomas <sothomas88@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/cap1tan/wafermap"
 keywords = ["semiconductor", "wafer", "layout", "plot"]
```

### Comparing `wafermap-0.2.1/README.md` & `wafermap-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,19 +99,23 @@
             ]
 colors = ['green', 'red', 'blue', 'black']
 for color, (cell, vector) in zip(colors, vectors):
     wm.add_vector(vector_points=vector, cell=cell, vector_style={'color': color}, root_style={'radius': 1, 'color': color})
 ```
 
 Let's throw in some points in a normal distribution for good measure too:
+
 ```python
 # add 50 points per cell, in a random distribution
 import random as rnd
+
 cell_size = (10e-3, 20e-3)
-cell_points = [(cell, [(rnd.gauss(cell_size[1]/2, cell_size[1]/6), rnd.gauss(cell_size[0]/2, cell_size[0]/6)) for _ in range(50)]) for cell in wm.cell_map.keys()]
+cell_points = [(cell, [(rnd.gauss(cell_size[1] / 2, cell_size[1] / 6),
+                        rnd.gauss(cell_size[0] / 2, cell_size[0] / 6)) for _ in
+                       range(50)]) for cell in wm._cell_map.keys()]
 for cell, cell_points_ in cell_points:
     for cell_point in cell_points_:
         wm.add_point(cell=cell, offset=cell_point)
 ```
 
 Finally, nothing would matter if we couldn't see the result:
 ```python
```

### Comparing `wafermap-0.2.1/wafermap/utils.py` & `wafermap-0.2.2/wafermap/utils.py`

 * *Files identical despite different names*

### Comparing `wafermap-0.2.1/wafermap/wafermap.py` & `wafermap-0.2.2/wafermap/wafermap.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,92 +21,81 @@
     webdriver = None
 
 
 class WaferMap:
     """Main WaferMap class. Represents a circular wafer layout, with a grid, an edge
     exclusion, cells and several types of markers (points, vectors, images)."""
 
-    MAP_CONVERSION = 1e-3  # MAP_CONVERSION meters equal to 1 map meter
-    NOTCH_HEIGHT = 1e-3 / MAP_CONVERSION
-    NOTCH_WIDTH = 2.8284e-3 / MAP_CONVERSION
+    NOTCH_HEIGHT = 1
+    NOTCH_WIDTH = 2.8284
     DEFAULT_MARKER_STYLE = {"color": "#ff0000", "fill": True}
     DEFAULT_VECTOR_STYLE = {"color": "#009900", "weight": 1}
     DEFAULT_POINT_STYLE = {"radius": 0.5, "fill": True}
     DEFAULT_LABEL_HTML_STYLE = "font-size: 8pt; color: black; text-align: center;"
     IMAGE_SIZE_IN_POPUP = (400, 400)
     IMAGE_FOLDER = "\\_images\\"
     MAP_PADDING = (100, 100)  # in pixels (x, y)
 
     def __init__(
         self,
         wafer_radius: float,
         cell_size: Tuple[float, float],
         cell_margin=(0.0, 0.0),
         grid_offset=(0.0, 0.0),
-        edge_exclusion=2.2e-3,
+        edge_exclusion=3,
         coverage="full",
         notch_orientation=270,
         bg_color=(1, 1, 1),
         conversion_factor=1,
     ):
         """
         The wafermap origin is always the central die.
-        :param wafer_radius: Wafer diameter in m
-        :param cell_size: Cell size in m, (x, y)
-        :param cell_margin: Distance between cells in m, (x, y)
-        :param grid_offset: Grid offset in m, (x, y)
+        :param wafer_radius: Wafer diameter in mm
+        :param cell_size: Cell size in mm, (x, y)
+        :param cell_margin: Distance between cells in mm, (x, y)
+        :param grid_offset: Grid offset in mm, (x, y)
         :param edge_exclusion: Margin from the wafer edge where a red edge exclusion
-        ring is drawn.
+        ring is drawn in mm.
         :param coverage: Options of 'full', 'inner'. Option 'full' will cover wafer with
          cells, partial cells allowed, 'inner' will only allow full cells
         :param bg_color: Tuple of (r, g, b), 0-255.
         :param conversion_factor: Factor to multiply input dimensions with.
         """
 
         assert cell_size[0] > 0
         assert cell_size[1] > 0
         assert coverage.lower() in ["full", "inner"]
 
         self.coverage = coverage.lower()
-        self.cell_size_x = conversion_factor * cell_size[0] / WaferMap.MAP_CONVERSION
-        self.cell_size_y = conversion_factor * cell_size[1] / WaferMap.MAP_CONVERSION
-        self.cell_margin_x = (
-            conversion_factor * cell_margin[0] / WaferMap.MAP_CONVERSION
-        )
-        self.cell_margin_y = (
-            conversion_factor * cell_margin[1] / WaferMap.MAP_CONVERSION
-        )
-        self.wafer_radius = conversion_factor * wafer_radius / WaferMap.MAP_CONVERSION
-        self.edge_exclusion = (
-            conversion_factor * edge_exclusion / WaferMap.MAP_CONVERSION
-        )
-        self.grid_offset_x = (
-            conversion_factor * grid_offset[0] / WaferMap.MAP_CONVERSION
-        )
-        self.grid_offset_y = (
-            conversion_factor * grid_offset[1] / WaferMap.MAP_CONVERSION
-        )
+        self.cell_size_x = conversion_factor * cell_size[0]
+        self.cell_size_y = conversion_factor * cell_size[1]
+        self.cell_margin_x = conversion_factor * cell_margin[0]
+        self.cell_margin_y = conversion_factor * cell_margin[1]
+        self.wafer_radius = conversion_factor * wafer_radius
+        self.edge_exclusion = conversion_factor * edge_exclusion
+        self.grid_offset_x = conversion_factor * grid_offset[0]
+        self.grid_offset_y = conversion_factor * grid_offset[1]
         self._num_of_cells_x = math.ceil(2 * self.wafer_radius / self.cell_size_x)
         self._num_of_cells_y = math.ceil(2 * self.wafer_radius / self.cell_size_y)
         self.notch_orientation = notch_orientation
         wafer_edge_color = utils.rgb_to_html(*utils.complementary(*bg_color))
 
-        # init the cell map
+        # init the _cell_map
         # the cell map is a dict that corresponds the pixel coordinates of the bounding
         # box of each cell to the cell index:
         # {(cell_y, cell_x): ((y_lower_left, x_lower_left),
         #                     (y_lower_right, x_lower_right),
         #                     (y_upper_left, x_upper_left),
         #                     (y_upper_right, x_upper_right),
         #                     (y_cell_center, x_cell_center),
         #                     folium.vector_layers.Rectangle
         #                     )}
         # We consider the cell origin to be its lower left corner
         # y is latitude, x is longitude
-        self.cell_map = {}
+        self._cell_map = {}
 
         # Init the folium map
         folium_map = folium.Map(
             tiles=None,
             crs="Simple",
             prefer_canvas=True,
             control_scale=False,
@@ -237,26 +226,26 @@
                         )
                     )
                 )
 
                 if (self.coverage == "full" and in_for_full) or (
                     self.coverage == "inner" and in_for_inner
                 ):
-                    self.cell_map[cell_label] = bounds + (center,)
-                    self.cell_map[cell_label] += (
+                    self._cell_map[cell_label] = bounds + (center,)  # in (y,x)
+                    self._cell_map[cell_label] += (
                         folium.vector_layers.Rectangle(
                             [lower_left, upper_right],
                             popup=None,
                             tooltip=None,
-                            color="#404040",
-                            weight=0.1,
+                            color="#142d2d",
+                            weight=0.2,
                             fill=False,
                         ),
                     )
-                    self.cell_map[cell_label][5].add_to(self._grid_layer)
+                    self._cell_map[cell_label][5].add_to(self._grid_layer)
 
                     # print labels
                     folium.map.Marker(
                         [
                             lower_left[0] + (0.5 * self.cell_size_y),
                             lower_left[1] + (0.5 * self.cell_size_x),
                         ],
@@ -283,19 +272,39 @@
             [
                 (-self.wafer_radius, -self.wafer_radius),
                 (self.wafer_radius, self.wafer_radius),
             ],
             padding=(WaferMap.MAP_PADDING[0], WaferMap.MAP_PADDING[1]),
         )  # padding is in pixels while the zoom box is in (long, lat)
 
+    @property
+    def cell_map(self):
+        # Internal attribute _cell_map uses (y,x) convention while WaferMap interfaces
+        # with (x,y). Therefore, we provide cell_map as a property to interface with
+        # outside the class, which fully converts _cell_map from (y,x) to (x,y)
+        cell_map = {}
+        for _cell_idx, _cell in self._cell_map.items():
+            cell_idx = _cell_idx[1], _cell_idx[0]
+            cell = ()
+            for _cell_item in _cell:
+                if type(_cell_item) is tuple:
+                    cell += ((_cell_item[1], _cell_item[0]),)
+                else:
+                    cell += (_cell_item,)
+            cell_map[cell_idx] = cell
+        return cell_map
+
     def save_html(self, output_file="wafermap.html") -> str:
         """Save current Folium Map to HTML."""
         assert os.path.splitext(output_file)[1].lower() == ".html"
-        # add extra controls to the html map
+        # turn on/off relevant layers/controls
+        self._cell_labels_layer.show = False
+        self._labels_layer.show = False
         self.map.options["zoomControl"] = True
+        # add extra controls to the html map
         plugins.MousePosition(
             position="topright",
             separator=" | ",
             empty_string="NaN",
             lng_first=True,
             prefix="Wafer Coordinates:",
         ).add_to(self.map)
@@ -306,21 +315,18 @@
     def save_png(self, output_file="wafermap.png") -> Union[str, None]:
         """Save current Folium Map to a PNG image. Selenium is required."""
         if webdriver is None or selenium is None:
             raise EnvironmentError(
                 "Error: Selenium is required to export to png and is not installed."
             )
         assert os.path.splitext(output_file)[1].lower() == ".png"
-        self._cell_labels_layer.show = (
-            False  # turn off cell_labels_layer before screenshot
-        )
-        self._labels_layer.show = True  # turn on cell_labels_layer before screenshot
-        self.map.options[
-            "zoomControl"
-        ] = False  # turn off zoom controls before screenshot
+        # turn on/off relevant layers/controls
+        self._cell_labels_layer.show = False
+        self._labels_layer.show = True
+        self.map.options["zoomControl"] = False
         try:
             options = webdriver.edge.options.Options()
             options.add_argument("--headless=new")
             edge_driver = webdriver.Edge(options=options)
             png_image = self.map._to_png(delay=1, driver=edge_driver)
         except selenium.common.exceptions.SessionNotCreatedException as exc:
             raise EnvironmentError(
@@ -356,67 +362,79 @@
         Add an image at the location specified by cell + offset. If marker_style flag is
          an empty dict, the image will be embedded directly on the wafermap, else a
          marker with a popup will be created.
         :param image_source_file: The path to the image file.
         :param marker_style: if not empty, a marker will be created with the defined
         style that when clicked, opens the image in a popup. If empty the image will be
         embedded directly on the wafermap and the image will be resized to fit the cell.
-        :param cell: Tuple of cell index.  If None is passed, the offset is interpreted
-        as wafer coordinates.
-        :param offset: Tuple of (y,x) offset from cell origin in meters.  Cell origin is
+        :param cell: Tuple of cell index (x,y).  If None is passed, the offset is
+        interpreted as (x,y) wafer coordinates.
+        :param offset: Tuple of (x,y) offset from cell origin in mm.  Cell origin is
          the bottom left corner.
         """
 
         if marker_style is None:
             marker_style = WaferMap.DEFAULT_MARKER_STYLE
-        if not os.path.isfile(image_source_file) or cell not in self.cell_map:
+        if not os.path.isfile(image_source_file) or cell not in self._cell_map:
             return
 
+        # given in (x,y) but internally we use (y,x) = (long, lat)
+        if cell:
+            cell = cell[1], cell[0]
+        offset = offset[1], offset[0]
+
         if cell:
-            if cell in self.cell_map:
+            if cell in self._cell_map:
                 # offset is cell coordinates
-                origin = self.cell_map[cell][0]  # already converted to MAP coordinates
+                origin = self._cell_map[cell][0]
                 image_origin = (
-                    offset[0] / WaferMap.MAP_CONVERSION + origin[0],
-                    offset[1] / WaferMap.MAP_CONVERSION + origin[1],
+                    offset[0] + origin[0],
+                    offset[1] + origin[1],
                 )
             else:
                 raise ValueError(f"{str(cell)} does not exist in wafermap.")
         else:
             # offset is wafer coordinates
             image_origin = (
-                offset[0] / WaferMap.MAP_CONVERSION,
-                offset[1] / WaferMap.MAP_CONVERSION,
+                offset[0],
+                offset[1],
             )
 
         # Open and read image
         with Image.open(image_source_file) as imf:
             try:
                 imf.thumbnail(WaferMap.IMAGE_SIZE_IN_POPUP)
                 image_width, image_height = imf.size
                 buffered = BytesIO()
                 imf.save(buffered, "JPEG")
                 image_file = base64.b64encode(buffered.getvalue())
             except IOError:
                 print(f"Error: Cannot create thumbnail for {image_source_file}")
         # find position to put image
-        image_coordinates = (
-            image_origin[0] + offset[0],
-            image_origin[1] + offset[1],
-        )
+        if cell:
+            image_coordinates = (
+                image_origin[0] + offset[0],
+                image_origin[1] + offset[1],
+            )
+        else:
+            # offset is wafer coordinates
+            image_coordinates = (
+                image_origin[0],
+                image_origin[1],
+            )
         image_bounds = [
             (image_coordinates[0], image_coordinates[1]),
             (
                 image_coordinates[0] + image_height * 1 / 10,
                 image_coordinates[1] + image_width * 1 / 10,
             ),
         ]
         cell_bounds = [
             (image_coordinates[0], image_coordinates[1]),
-            (self.cell_map[cell][3][0], self.cell_map[cell][3][1]),
+            (self._cell_map[cell][3][0], self._cell_map[cell][3][1]),
         ]
         if not marker_style:
             # add image as ImageOverlay
             folium.raster_layers.ImageOverlay(
                 image=image_source_file,
                 bounds=utils.bounded_rectangle(rect=image_bounds, bounds=cell_bounds),
                 origin="lower",
@@ -445,79 +463,81 @@
         vector_style=None,
         root_style=None,
     ):
         """
         Add a vector to the map.
         :param root_style: If given, the vector will have a point as root with the given
          style.
-        :param vector_points: [(y_start, x_start), (y_end, x_end)] in meters. Cell
-        origin is the bottom left corner.
+        :param vector_points: [(x_start, y_start), (x_end, y_end)] in mm. Cell origin is
+         the bottom left corner.
         :param vector_length_scale: Value to multiply the vector length by
-        :param cell: Tuple of cell index (y, x). If None is passed, the vector_points
+        :param cell: Tuple of cell index (x, y). If None is passed, the vector_points
         are interpreted as wafer coordinates.
         :param vector_style: A dict with style options.
         """
 
         if root_style is None:
             root_style = {}
         if vector_style is None:
             vector_style = WaferMap.DEFAULT_VECTOR_STYLE
         if not len(vector_points) == 2:
             return
         if vector_style != WaferMap.DEFAULT_VECTOR_STYLE:
             vector_style = {**WaferMap.DEFAULT_VECTOR_STYLE, **vector_style}
 
+        # given in (x,y) but internally we use (y,x) = (long, lat)
+        if cell:
+            cell = cell[1], cell[0]
+        for i, vector_point in enumerate(vector_points):
+            vector_points[i] = vector_point[1], vector_point[0]
+
         if cell:
-            if cell in self.cell_map:
+            if cell in self._cell_map:
                 # vector_points is cell coordinates
-                origin = self.cell_map[cell][0]  # already converted to MAP coordinates
+                origin = self._cell_map[cell][0]  # already converted to MAP coordinates
                 vector_points = [
                     (
-                        vector_points[0][0] / WaferMap.MAP_CONVERSION + origin[0],
-                        vector_points[0][1] / WaferMap.MAP_CONVERSION + origin[1],
+                        vector_points[0][0] + origin[0],
+                        vector_points[0][1] + origin[1],
                     ),
                     (
                         (
                             vector_points[0][0]
                             + vector_length_scale
                             * (vector_points[1][0] - vector_points[0][0])
                         )
-                        / WaferMap.MAP_CONVERSION
                         + origin[0],
                         (
                             vector_points[0][1]
                             + vector_length_scale
                             * (vector_points[1][1] - vector_points[0][1])
                         )
-                        / WaferMap.MAP_CONVERSION
                         + origin[1],
                     ),
                 ]
             else:
                 return  # do nothing when cell doesn't exist
         else:
             # vector_points is wafer coordinates
             vector_points = [
                 (
-                    vector_points[0][0] / WaferMap.MAP_CONVERSION,
-                    vector_points[0][1] / WaferMap.MAP_CONVERSION,
+                    vector_points[0][0],
+                    vector_points[0][1],
                 ),
                 (
                     (
                         vector_points[0][0]
                         + vector_length_scale
                         * (vector_points[1][0] - vector_points[0][0])
-                    )
-                    / WaferMap.MAP_CONVERSION,
+                    ),
                     (
                         vector_points[0][1]
                         + vector_length_scale
                         * (vector_points[1][1] - vector_points[0][1])
-                    )
-                    / WaferMap.MAP_CONVERSION,
+                    ),
                 ),
             ]
 
         if root_style:
             root_point = vector_points[0]
             folium.CircleMarker(location=root_point, **root_style).add_to(
                 self._vectors_layer
@@ -535,42 +555,47 @@
         cell: Union[Tuple[int, int], None] = (0, 0),
         offset: Tuple[float, float] = (0.0, 0.0),
         point_style=None,
         popup_text=None,
     ):
         """
         :param point_style: Draw a point with the given style
-        :param offset: Tuple of (y,x) offset from cell origin in meters.  Cell origin is
+        :param offset: Tuple of (x,y) offset from cell origin in mm.  Cell origin is
          the bottom left corner.
-        :param cell: Tuple of cell index. If None is passed, the offset is interpreted
+        :param cell: Tuple of cell index (x,y). If None is passed, the offset is interpreted
         as wafer coordinates.
         :param popup_text: The text to display as a popup upon clicking the point. If
         None, no popup will be shown.
         """
 
         if point_style is None:
             point_style = WaferMap.DEFAULT_POINT_STYLE
         if point_style != WaferMap.DEFAULT_POINT_STYLE:
             point_style = {**WaferMap.DEFAULT_POINT_STYLE, **point_style}
 
+        # given in (x,y) but internally we use (y,x) = (long, lat)
         if cell:
-            if cell in self.cell_map:
+            cell = cell[1], cell[0]
+        offset = offset[1], offset[0]
+
+        if cell:
+            if cell in self._cell_map:
                 # offset is cell coordinates
-                origin = self.cell_map[cell][0]  # already converted to MAP coordinates
+                origin = self._cell_map[cell][0]
                 point_origin = (
-                    offset[0] / WaferMap.MAP_CONVERSION + origin[0],
-                    offset[1] / WaferMap.MAP_CONVERSION + origin[1],
+                    offset[0] + origin[0],
+                    offset[1] + origin[1],
                 )
             else:
                 raise ValueError(f"{str(cell)} does not exist in wafermap.")
         else:
             # offset is wafer coordinates
             point_origin = (
-                offset[0] / WaferMap.MAP_CONVERSION,
-                offset[1] / WaferMap.MAP_CONVERSION,
+                offset[0],
+                offset[1],
             )
 
         folium.CircleMarker(
             location=point_origin, popup=popup_text, **point_style
         ).add_to(self._markers_layer)
 
     def add_label(
@@ -580,41 +605,46 @@
         label_text="",
         label_html_style=None,
         popup_text=None,
     ):
         """
         :param label_html_style: Write a label with the given HTML style, e.g:
         'font-size: 8pt; color: black; text-align: center'
-        :param offset: Tuple of (y,x) offset from cell origin in meters.  Cell origin is
-         the bottom left corner.
+        :param offset: Tuple of (x,y) offset from cell origin in mm. Cell origin is the
+        bottom left corner.
         :param label_text: The text of the label.
-        :param cell: Tuple of cell index. If None is passed, the offset is interpreted
-        as wafer coordinates.
+        :param cell: Tuple of cell index (x,y). If None is passed, the offset is
+        interpreted as wafer coordinates.
         :param popup_text: The text to display as a popup upon clicking the label. If
         None, no popup will be shown.
         """
 
         if label_html_style is None:
             label_html_style = WaferMap.DEFAULT_LABEL_HTML_STYLE
 
+        # given in (x,y) but internally we use (y,x) = (long, lat)
         if cell:
-            if cell in self.cell_map:
+            cell = cell[1], cell[0]
+        offset = offset[1], offset[0]
+
+        if cell:
+            if cell in self._cell_map:
                 # offset is cell coordinates
-                origin = self.cell_map[cell][0]  # already converted to MAP coordinates
+                origin = self._cell_map[cell][0]  # already converted to MAP coordinates
                 label_origin = (
-                    offset[0] / WaferMap.MAP_CONVERSION + origin[0],
-                    offset[1] / WaferMap.MAP_CONVERSION + origin[1],
+                    offset[0] + origin[0],
+                    offset[1] + origin[1],
                 )
             else:
                 raise ValueError(f"{str(cell)} does not exist in wafermap.")
         else:
             # offset is wafer coordinates. Origin is the center
             label_origin = (
-                offset[0] / WaferMap.MAP_CONVERSION,
-                offset[1] / WaferMap.MAP_CONVERSION,
+                offset[0],
+                offset[1],
             )
         # we multiply by 5 so that we have some scaling the label size with the
         # cell size but still, it is not 1-1 conversion to pixel size.
         label_size_px = (self.cell_size_x * 4, self.cell_size_y * 3)
         label_anchor_px = (label_size_px[0] / 2, label_size_px[1] / 2)
         folium.map.Marker(
             location=label_origin,
@@ -629,19 +659,23 @@
     def style_cell(
         self,
         cell: Union[Tuple[int, int], None] = (0, 0),
         cell_style=dict,
     ):
         """
         :param cell_style: Define the cell style
-        :param cell: Tuple of cell index. If None is passed, all cells are styled.
+        :param cell: Tuple of cell index (x,y). If None is passed, all cells are styled.
         """
 
+        # given in (x,y) but internally we use (y,x) = (long, lat)
+        if cell:
+            cell = cell[1], cell[0]
+
         if not cell:
-            cells_to_style = [c for c in self.cell_map]
+            cells_to_style = [c for c in self._cell_map]
         else:
-            if cell not in self.cell_map:
+            if cell not in self._cell_map:
                 raise ValueError(f"{str(cell)} does not exist in wafermap.")
             cells_to_style = [cell]
 
         for cell_to_style in cells_to_style:
-            self.cell_map[cell_to_style][5].options |= cell_style
+            self._cell_map[cell_to_style][5].options |= cell_style
```

### Comparing `wafermap-0.2.1/PKG-INFO` & `wafermap-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafermap
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package to plot maps of semiconductor wafers.
 Home-page: https://github.com/cap1tan/wafermap
 License: MIT
 Keywords: semiconductor,wafer,layout,plot
 Author: Sotiris Thomas
 Author-email: sothomas88@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -123,19 +123,23 @@
             ]
 colors = ['green', 'red', 'blue', 'black']
 for color, (cell, vector) in zip(colors, vectors):
     wm.add_vector(vector_points=vector, cell=cell, vector_style={'color': color}, root_style={'radius': 1, 'color': color})
 ```
 
 Let's throw in some points in a normal distribution for good measure too:
+
 ```python
 # add 50 points per cell, in a random distribution
 import random as rnd
+
 cell_size = (10e-3, 20e-3)
-cell_points = [(cell, [(rnd.gauss(cell_size[1]/2, cell_size[1]/6), rnd.gauss(cell_size[0]/2, cell_size[0]/6)) for _ in range(50)]) for cell in wm.cell_map.keys()]
+cell_points = [(cell, [(rnd.gauss(cell_size[1] / 2, cell_size[1] / 6),
+                        rnd.gauss(cell_size[0] / 2, cell_size[0] / 6)) for _ in
+                       range(50)]) for cell in wm._cell_map.keys()]
 for cell, cell_points_ in cell_points:
     for cell_point in cell_points_:
         wm.add_point(cell=cell, offset=cell_point)
 ```
 
 Finally, nothing would matter if we couldn't see the result:
 ```python
```

