# Comparing `tmp/bas_geoplot-0.0.16.tar.gz` & `tmp/bas_geoplot-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bas_geoplot-0.0.16.tar", last modified: Thu Mar 30 14:59:35 2023, max compression
+gzip compressed data, was "bas_geoplot-0.0.17.tar", last modified: Wed Apr 19 10:35:43 2023, max compression
```

## Comparing `bas_geoplot-0.0.16.tar` & `bas_geoplot-0.0.17.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-03-30 14:59:35.780035 bas_geoplot-0.0.16/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.16/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.16/MANIFEST.in
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-03-30 14:59:35.780035 bas_geoplot-0.0.16/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.16/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-03-30 14:59:35.776035 bas_geoplot-0.0.16/bas_geoplot/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-03-30 12:08:17.000000 bas_geoplot-0.0.16/bas_geoplot/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4700 2023-02-23 13:19:23.000000 bas_geoplot-0.0.16/bas_geoplot/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-03-30 14:59:35.780035 bas_geoplot-0.0.16/bas_geoplot/config/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7165 2023-02-23 13:19:23.000000 bas_geoplot-0.0.16/bas_geoplot/config/interactive.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.16/bas_geoplot/config/static.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    34093 2023-03-30 13:09:21.000000 bas_geoplot-0.0.16/bas_geoplot/interactive.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.16/bas_geoplot/static.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2201 2022-10-21 13:21:48.000000 bas_geoplot-0.0.16/bas_geoplot/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-03-30 14:59:35.780035 bas_geoplot-0.0.16/bas_geoplot.egg-info/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-03-30 14:59:35.000000 bas_geoplot-0.0.16/bas_geoplot.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-03-30 14:59:35.780035 bas_geoplot-0.0.16/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.16/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.17/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-04-19 10:35:43.949830 bas_geoplot-0.0.17/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-04-04 13:22:34.000000 bas_geoplot-0.0.17/bas_geoplot/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4821 2023-04-19 10:35:00.000000 bas_geoplot-0.0.17/bas_geoplot/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot/config/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7165 2023-02-23 13:19:23.000000 bas_geoplot-0.0.17/bas_geoplot/config/interactive.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.17/bas_geoplot/config/static.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    34647 2023-04-19 10:35:00.000000 bas_geoplot-0.0.17/bas_geoplot/interactive.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/bas_geoplot/static.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2201 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/bas_geoplot/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot.egg-info/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-04-19 10:35:43.949830 bas_geoplot-0.0.17/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/setup.py
```

### Comparing `bas_geoplot-0.0.16/LICENSE` & `bas_geoplot-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/PKG-INFO` & `bas_geoplot-0.0.17/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas_geoplot
-Version: 0.0.16
+Version: 0.0.17
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.16/README.md` & `bas_geoplot-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/bas_geoplot/cli.py` & `bas_geoplot-0.0.17/bas_geoplot/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,20 @@
     from bas_geoplot.interactive import Map
     import pandas as pd
 
     args = get_args("interactive_plot.html")
     logging.info("{} {}".format(inspect.stack()[0][3][:-4], version))
     info = json.load(args.mesh)
     mesh = pd.DataFrame(info['cellboxes'])
+    region = info['config']['Mesh_info']['Region']
 
     output = ' '.join(args.output.split('/')[-1].split('.')[:-1])
-    output = '{} | Start Date: {}, End Date: {}'.format(output, info['config']['Mesh_info']['Region']['startTime'], info['config']['Mesh_info']['Region']['endTime'])
+    output = '{} | Start Date: {}, End Date: {}'.format(output, region['startTime'], region['endTime'])
+
+    mesh_bounds = [[region["latMin"], region["longMin"]], [region["latMax"], region["longMax"]]]
 
 
     if args.offline_filepath != '':
         logging.debug("offline .js & .css datastore - {}".format(args.offline_filepath))
         if args.coastlines != '':
             mp = Map(title=output,offline_coastlines=args.coastlines,offline_filepath=args.offline_filepath)
         else:
@@ -82,13 +85,14 @@
         mp.Paths(paths,'Routes - Fuel',predefined='Fuel',show=False)
         mp.Paths(paths,'Routes - tCO2e',predefined='tCO2e',show=False)
     if 'waypoints' in info.keys():
         logging.debug('plotting waypoints')
         waypoints = pd.DataFrame(info['waypoints'])
         mp.Points(waypoints,'Waypoints',names={"font_size":10.0})
     mp.MeshInfo(mesh,'Mesh Info',show=False)
+    mp.fit_to_bounds(mesh_bounds)
     logging.info('Saving plot to {}'.format(args.output))
     mp.save(args.output)
```

### Comparing `bas_geoplot-0.0.16/bas_geoplot/config/interactive.json` & `bas_geoplot-0.0.17/bas_geoplot/config/interactive.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/bas_geoplot/config/static.json` & `bas_geoplot-0.0.17/bas_geoplot/config/static.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/bas_geoplot/interactive.py` & `bas_geoplot-0.0.17/bas_geoplot/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from branca.colormap import linear
 from branca.element import MacroElement
 from shapely import wkt
 from shapely.geometry import Polygon
 import geopandas as gpd
 from jinja2 import Template
 from pyproj import Geod
+import logging
 
 
 
 
 def paramsObject(layer,predefined=None,**kwargs):
     # Loading config of standards
     p_file = os.path.join(os.path.dirname(__file__),'config','interactive.json')
@@ -245,14 +246,28 @@
 
             
             
         with open(file,'w') as fp:
             fp.write(html)
             fp.close()
 
+    def fit_to_bounds(self, bounds=None):
+        """
+            Change zoom level to match plotted data
+        """
+        # Use input bounds if provided
+        if bounds:
+            self.map.fit_bounds(bounds)
+        # Otherwise try to retrieve bounds automatically from map
+        else:
+            bounds = self.map.get_bounds()
+            if bounds == [[None, None], [None, None]]:
+                logging.info("No bounds returned, can't fit to layers")
+            else:
+                self.map.fit_bounds(bounds)
 
     def Paths(self,geojson,name,show=True,predefined=None,**kwargs):
         """
             Overlays paths on the interactive plot with layer defined by `name`
 
             Attributes:
                 geojson (dict): A geojson file with several features representing all
@@ -535,15 +550,15 @@
                     config/interactive.json of the package files
         """
 
         p = paramsObject('MeshInfo',predefined=predefined,**kwargs)
 
 
 
-        dataframe_pandas = pd.DataFrame(mesh)
+        dataframe_pandas = copy.copy(pd.DataFrame(mesh))
         dataframe_pandas['geometry'] = dataframe_pandas['geometry'].apply(wkt.loads)
         dataframe_geo = gpd.GeoDataFrame(dataframe_pandas,crs='EPSG:4326', geometry='geometry')
 
         p = p['fields']
 
         column_names = []
         column_names.append('geometry')
```

### Comparing `bas_geoplot-0.0.16/bas_geoplot/static.py` & `bas_geoplot-0.0.17/bas_geoplot/static.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/bas_geoplot/utils.py` & `bas_geoplot-0.0.17/bas_geoplot/utils.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.16/bas_geoplot.egg-info/PKG-INFO` & `bas_geoplot-0.0.17/bas_geoplot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas-geoplot
-Version: 0.0.16
+Version: 0.0.17
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.16/setup.py` & `bas_geoplot-0.0.17/setup.py`

 * *Files identical despite different names*

