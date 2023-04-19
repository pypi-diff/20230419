# Comparing `tmp/nzshm_common-0.5.1.tar.gz` & `tmp/nzshm_common-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzshm_common-0.5.1.tar", max compression
+gzip compressed data, was "nzshm_common-0.6.0.tar", max compression
```

## Comparing `nzshm_common-0.5.1.tar` & `nzshm_common-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/LICENSE
--rw-r--r--   0        0        0     1109 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/README.md
--rw-r--r--   0        0        0      111 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/__init__.py
--rw-r--r--   0        0        0      799 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/geometry/backarc_polygon.json
--rw-r--r--   0        0        0     1444 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/geometry/geometry.py
--rw-r--r--   0        0        0       47 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/__init__.py
--rw-r--r--   0        0        0      477 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/io.py
--rw-r--r--   0        0        0     2831 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v0.py
--rw-r--r--   0        0        0     3524 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v1.py
--rw-r--r--   0        0        0    47971 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_2_nb_1_1.py
--rw-r--r--   0        0        0     1511 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/region_grid.py
--rw-r--r--   0        0        0    38248 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/wlg_0_01_nb_1_1.py
--rw-r--r--   0        0        0     3260 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/wlg_0_05_nb_1_1.py
--rw-r--r--   0        0        0       41 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/code_location.py
--rw-r--r--   0        0        0     1631 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/location.py
--rw-r--r--   0        0        0  3218277 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/location/locations.json
--rw-r--r--   0        0        0      252 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/location/nz_ids.json
--rw-r--r--   0        0        0       75 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/util/__init__.py
--rw-r--r--   0        0        0     1440 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/util/compression.py
--rw-r--r--   0        0        0     2119 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1760 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_backarc.py
--rw-r--r--   0        0        0     3565 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_coded_location.py
--rw-r--r--   0        0        0     2317 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_compression.py
--rw-r--r--   0        0        0     4500 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_geometry.py
--rw-r--r--   0        0        0     1662 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_location.py
--rw-r--r--   0        0        0     1018 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_region_grid.py
--rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nzshm_common-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1109 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/README.md
+-rw-r--r--   0        0        0      111 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/__init__.py
+-rw-r--r--   0        0        0     1457 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/geometry/geometry.py
+-rw-r--r--   0        0        0       47 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/io.py
+-rw-r--r--   0        0        0     2831 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/nz_0_1_nb_1_v0.py
+-rw-r--r--   0        0        0     3524 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/nz_0_1_nb_1_v1.py
+-rw-r--r--   0        0        0    47971 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/nz_0_2_nb_1_1.py
+-rw-r--r--   0        0        0     1511 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/region_grid.py
+-rw-r--r--   0        0        0    38248 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/wlg_0_01_nb_1_1.py
+-rw-r--r--   0        0        0     3260 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/grids/wlg_0_05_nb_1_1.py
+-rw-r--r--   0        0        0       41 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/location/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/location/code_location.py
+-rw-r--r--   0        0        0     1631 2023-04-19 00:45:45.176668 nzshm_common-0.6.0/nzshm_common/location/location.py
+-rw-r--r--   0        0        0  3218277 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/nzshm_common/location/locations.json
+-rw-r--r--   0        0        0      252 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/nzshm_common/location/nz_ids.json
+-rw-r--r--   0        0        0       75 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/nzshm_common/util/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/nzshm_common/util/compression.py
+-rw-r--r--   0        0        0     2072 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1907 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/tests/test_backarc.py
+-rw-r--r--   0        0        0     3565 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/tests/test_coded_location.py
+-rw-r--r--   0        0        0     2317 2023-04-19 00:45:45.184669 nzshm_common-0.6.0/tests/test_compression.py
+-rw-r--r--   0        0        0     3760 2023-04-19 00:45:45.188669 nzshm_common-0.6.0/tests/test_geometry.py
+-rw-r--r--   0        0        0     1662 2023-04-19 00:45:45.188669 nzshm_common-0.6.0/tests/test_location.py
+-rw-r--r--   0        0        0     1018 2023-04-19 00:45:45.188669 nzshm_common-0.6.0/tests/test_region_grid.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nzshm_common-0.6.0/PKG-INFO
```

### Comparing `nzshm_common-0.5.1/LICENSE` & `nzshm_common-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/README.md` & `nzshm_common-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/geometry/geometry.py` & `nzshm_common-0.6.0/nzshm_common/geometry/geometry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Simple polygon builder methods."""
 
 import math
-from pathlib import Path
 
-import geopandas
-from geopandas.geodataframe import GeoDataFrame
+import shapely.wkt
 from shapely.geometry import Polygon
 
 
 def create_hexagon(edge: float, x: float, y: float):
     """
     Create a hexagon centered on (x, y)
     :param edge: length of the hexagon's edge
@@ -38,14 +36,19 @@
         (x - offset, y - offset),
         (x - offset, y + offset),
         (x + offset, y + offset),
     ]
     return Polygon(c)
 
 
-def create_backarc_polygon() -> GeoDataFrame:
+BA_POLYGON_WKT = (
+    "POLYGON ((177.2 -37.715, 176.2 -38.72, 175.375 -39.27, "
+    "174.25 -40, 173.1 -39.183, 171.7 -34.76, 173.54 -33.22, 177.2 -37.715))"
+)
+
+
+def backarc_polygon() -> Polygon:
     """
-    Retrieve the backarc polygon from json and return geopandas object
+    Retrieve the backarc polygon from json and return shapely Polygon object
     """
 
-    poly_filepath = Path(Path(__file__).parent, 'backarc_polygon.json')
-    return geopandas.read_file(poly_filepath)
+    return shapely.wkt.loads(BA_POLYGON_WKT)
```

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v0.py` & `nzshm_common-0.6.0/nzshm_common/grids/nz_0_1_nb_1_v0.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v1.py` & `nzshm_common-0.6.0/nzshm_common/grids/nz_0_1_nb_1_v1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/nz_0_2_nb_1_1.py` & `nzshm_common-0.6.0/nzshm_common/grids/nz_0_2_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/region_grid.py` & `nzshm_common-0.6.0/nzshm_common/grids/region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/wlg_0_01_nb_1_1.py` & `nzshm_common-0.6.0/nzshm_common/grids/wlg_0_01_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/grids/wlg_0_05_nb_1_1.py` & `nzshm_common-0.6.0/nzshm_common/grids/wlg_0_05_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/location/code_location.py` & `nzshm_common-0.6.0/nzshm_common/location/code_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/location/location.py` & `nzshm_common-0.6.0/nzshm_common/location/location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/location/locations.json` & `nzshm_common-0.6.0/nzshm_common/location/locations.json`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/nzshm_common/util/compression.py` & `nzshm_common-0.6.0/nzshm_common/util/compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/pyproject.toml` & `nzshm_common-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nzshm-common"
-version = "0.5.1"
+version = "0.6.0"
 homepage = "https://github.com/GNS-Science/nzshm-common-py"
 description = "A small pure python library for shared NZ NSHM data like locations."
 authors = ["GNS Science <chrisbc@artisan.co.nz>"]
 readme = "README.md"
 license = "GNU Affero V3"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -23,18 +23,17 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
 
 [tool.poetry.group.geometry.dependencies]
 shapely = {version = "^2.0.1"}
-geopandas = {version = "^0.12.2"}
 
 [tool.poetry.extras]
-geometry = ["geopandas", "shapely"]
+geometry = ["shapely"]
 
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
     "flake8",
```

### Comparing `nzshm_common-0.5.1/tests/test_backarc.py` & `nzshm_common-0.6.0/tests/test_backarc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-from shapely.geometry import Point
+import unittest
 
-from nzshm_common.geometry.geometry import create_backarc_polygon
+try:
+    import shapely  # noqa
+    from shapely.geometry import Point
+    from nzshm_common.geometry.geometry import backarc_polygon
+
+    HAVE_SHAPELY = True
+except ImportError:
+    HAVE_SHAPELY = False
 
 LOCATIONS_W_BACKARC = [
     ("AKL", 174.77, -36.87, 1),
     ("BHE", 173.95, -41.51, 0),
     ("CHC", 172.63, -43.53, 0),
     ("DUD", 170.5, -45.87, 0),
     ("GIS", 178.0, -38.65, 0),
@@ -41,13 +48,13 @@
 ]
 
 LOCATIONS_W_BACKARC_BY_ID = {
     loc[0]: {"id": loc[0], "latitude": loc[2], "longitude": loc[1], "backarc": loc[3]} for loc in LOCATIONS_W_BACKARC
 }
 
 
+@unittest.skipUnless(HAVE_SHAPELY, "Test requires optional shapely module.")
 def test_backarc_polygon():
 
-    backarc_polygon = create_backarc_polygon()
     for location in LOCATIONS_W_BACKARC_BY_ID.values():
-        print(backarc_polygon.contains(Point(location['longitude'], location['latitude']))[0], location['backarc'])
-        assert backarc_polygon.contains(Point(location['longitude'], location['latitude']))[0] == location['backarc']
+        print(backarc_polygon().contains(Point(location['longitude'], location['latitude'])), location['backarc'])
+        assert backarc_polygon().contains(Point(location['longitude'], location['latitude'])) == location['backarc']
```

### Comparing `nzshm_common-0.5.1/tests/test_coded_location.py` & `nzshm_common-0.6.0/tests/test_coded_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/tests/test_compression.py` & `nzshm_common-0.6.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/tests/test_geometry.py` & `nzshm_common-0.6.0/tests/test_geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 import unittest
 import math
-import random
 
 from nzshm_common.grids import load_grid, RegionGrid
 
-
-try:
-    import geopandas as gpd  # noqa
-
-    HAVE_GPD = True
-except ImportError:
-    HAVE_GPD = False
-
 try:
     import shapely  # noqa
     from nzshm_common.geometry.geometry import create_hexagon, create_square_tile  # these require shapely
 
     HAVE_SHAPELY = True
 except ImportError:
     HAVE_SHAPELY = False
@@ -38,28 +29,14 @@
 
         print('centroid spacing', cells[0].centroid.distance(cells[1].centroid))
         print('cell center to boundary', cells[0].centroid.distance(cells[0].boundary))
         print('cell spacing', cells[0].distance(cells[1]))
         print('cell exterior', list(cells[0].exterior.coords))
         self.assertAlmostEqual(cells[0].distance(cells[1]), 0.0)
 
-    @unittest.skipUnless(HAVE_SHAPELY and HAVE_GPD, "Test requires optional modules: shapely + geopandas.")
-    def test_build_geojson_from_squares_pt1(self):
-        grid = RegionGrid['NZ_0_1_NB_1_1']
-        grid_pts = grid.load()
-
-        locs, geometry, values = [], [], []
-        for pt in grid_pts:
-            locs.append((pt[1], pt[0]))
-            geometry.append(create_square_tile(grid.resolution, pt[1], pt[0]))
-            values.append(random.randint(0, 100000))
-
-        gdf = gpd.GeoDataFrame(data=dict(locs=locs, geometry=geometry, values=values))
-        self.assertEqual(gdf.shape[0], len(grid_pts))
-
 
 # TODO: need a different grid layout...
 def create_hexgrid(bbox, side):
     """
     returns an array of Points describing hexagons centers that are inside the given bounding_box
     :param bbox: The containing bounding box. The bbox coordinate should be in Webmercator.
     :param side: The size of the hexagons'
```

### Comparing `nzshm_common-0.5.1/tests/test_location.py` & `nzshm_common-0.6.0/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/tests/test_region_grid.py` & `nzshm_common-0.6.0/tests/test_region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.1/PKG-INFO` & `nzshm_common-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzshm-common
-Version: 0.5.1
+Version: 0.6.0
 Summary: A small pure python library for shared NZ NSHM data like locations.
 Home-page: https://github.com/GNS-Science/nzshm-common-py
 License: GNU Affero V3
 Author: GNS Science
 Author-email: chrisbc@artisan.co.nz
 Requires-Python: >=3.8,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

