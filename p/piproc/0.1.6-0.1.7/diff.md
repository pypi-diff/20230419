# Comparing `tmp/piproc-0.1.6.tar.gz` & `tmp/piproc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piproc-0.1.6.tar", last modified: Wed Apr 12 12:37:11 2023, max compression
+gzip compressed data, was "piproc-0.1.7.tar", last modified: Wed Apr 19 10:39:21 2023, max compression
```

## Comparing `piproc-0.1.6.tar` & `piproc-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.995529 piproc-0.1.6/
--rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      266 2023-04-12 12:37:10.995529 piproc-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.978688 piproc-0.1.6/piproc/
--rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.6/piproc/__init__.py
--rw-rw-rw-   0        0        0    14204 2023-04-12 12:34:42.000000 piproc-0.1.6/piproc/main.py
--rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.6/piproc/tables.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.994487 piproc-0.1.6/piproc.egg-info/
--rw-rw-rw-   0        0        0      266 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      366 2023-04-12 12:37:10.997520 piproc-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.463962 piproc-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-04-19 10:39:21.463962 piproc-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.445192 piproc-0.1.7/piproc/
+-rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.7/piproc/__init__.py
+-rw-rw-rw-   0        0        0    15621 2023-04-17 15:22:00.000000 piproc-0.1.7/piproc/main.py
+-rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.7/piproc/tables.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.462984 piproc-0.1.7/piproc.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      366 2023-04-19 10:39:21.464932 piproc-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.7/setup.py
```

### Comparing `piproc-0.1.6/LICENSE` & `piproc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `piproc-0.1.6/README.md` & `piproc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `piproc-0.1.6/piproc/main.py` & `piproc-0.1.7/piproc/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -258,29 +258,35 @@
                 file.no_fdi += 1
             except TypeError:
                 file.no_fdi = 1
             file.date_fdi = datetime.datetime.now()
             file.fdi_path = yaml_path
         self.session.commit()
 
-    def check_prediction(self):
+    def check_prediction(self, satellite='sentinel2'):
         '''
         A function to check in the Plastic-i processing db if a tile has already had
         a plastic prediction tile created from it.
         '''
-        files = self.session.query(Processing).filter(Processing.indexed == 2,
-                                                Processing.prediction == 0).limit(1)
 
-        for file in files:
-            output = {'x': file.lons,
-                    'y': file.lats,
-                    'date': file.tile_date,
-                    'tile': file.tile,
-                    'crs': file.crs,
-                    'id': file.id
+        if satellite == 'sentinel2':
+            file = self.session.query(Processing).filter(Processing.indexed == 2,
+                                                Processing.prediction == 0).first()
+            tile = file.tile
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProc).filter(PlanetProc.indexed == 2, 
+                                                PlanetProc.prediction == 0).first()
+            tile = file.crs # Planet scenes don't have tiles so we use the crs to distinguish them
+        
+        output = {'x': file.lons,
+                  'y': file.lats,
+                  'date': file.tile_date,
+                  'tile': tile,
+                  'crs': file.crs,
+                  'id': file.id
                 }
         return output
 
     def mq_unet(self, product_id):
         '''
         A function to get data from the Plastic-i processing db for a tile supplied an id for running a unet.
         Used in production with a message queue and kubernetes.
@@ -291,56 +297,71 @@
                   'date': file.tile_date,
                   'tile': file.tile,
                   'crs': file.crs,
                   'id': file.id
             }
         return output
 
-    def update_unet(self, output, it, yaml_path=None, model=None, result=None, env=None):
+    def update_unet(self, output, it, satellite='sentinel2', yaml_path=None, model=None, result=None, env=None):
         '''
         Update the product db with the status of an apply_unet process.
         '''
-        file = self.session.query(Processing).get(output['id'])
+        if satellite == 'sentinel2':
+            file = self.session.query(Processing).get(output['id'])
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProc).get(output['id'])
+
         file.prediction = result
         file.pred_path = yaml_path
         file.model = model
 
         try:
-            new_file = Products(id=f'{output["id"]}_{it}', base_id=output['id'], tile=file.tile, 
-                lons=str(output['lons']), lats=str(output['lats']), tile_date=file.tile_date, 
-                crs=file.crs, prediction=0, avg=float(output['avg']), min=float(output['min']), 
-                max=float(output['max']), std=float(output['std']), area=output['area'], 
-                length=output['length'])
+            if satellite == 'sentinel2':
+                new_file = Products(id=f'{output["id"]}_{it}', base_id=output['id'], tile=file.tile, 
+                    lons=str(output['lons']), lats=str(output['lats']), tile_date=file.tile_date, 
+                    crs=file.crs, prediction=0, avg=float(output['avg']), min=float(output['min']), 
+                    max=float(output['max']), std=float(output['std']), area=output['area'], 
+                    length=output['length'])
+            elif satellite == 'planet':
+                new_file = PlanetProd(id=f'{output["id"]}_{it}', base_id=output['id'], 
+                    lons=str(output['lons']), lats=str(output['lats']), tile_date=file.tile_date,
+                    crs=file.crs, prediction=0, avg=float(output['avg']), min=float(output['min']),
+                    max=float(output['max']), std=float(output['std']), area=output['area'], 
+                    length=output['length'])
             self.session.add(new_file)
         except KeyError:
             # If no plastic files found, nothing to add to products db.
             pass
 
         if env == 'k8s':
             # Notify message queue that file has been downloaded when running with kubernetes.
             self.notify(f'{output["id"]}_{it}', 'pifind_prediction')
 
         self.session.commit()
 
-    def check_xgboost(self):
+    def check_xgboost(self, satellite='sentinel2'):
         '''
         A function to check in the Plastic-i processing db if a tile has already had
         a plastic prediction tile created from it.
         '''
-        files = self.session.query(Products).filter(Products.prediction == 0).limit(1)
-
-        for file in files:
-            output = {'x': file.lons,
-                    'y': file.lats,
-                    'date': file.tile_date,
-                    'crs': file.crs,
-                    'id': file.id,
-                    'tile': file.tile
-                }
-
+        if satellite == 'sentinel2':
+            file = self.session.query(Products).filter(Products.prediction == 0).first()
+            tile = file.tile
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProd).filter(PlanetProd.prediction == 0).first()
+            tile = file.crs
+
+        output = {
+            'x': file.lons,
+            'y': file.lats,
+            'date': file.tile_date,
+            'crs': file.crs,
+            'id': file.id,
+            'tile': tile
+        }
         return output
 
     def mq_xgboost(self, product_id):
         '''
         A function to get data from the Plastic-i processing db for a tile supplied an id for running xgboost.
         Used in production with a message queue and kubernetes.
         '''
@@ -350,19 +371,22 @@
                   'date': file.tile_date,
                   'crs': file.crs,
                   'id': file.id,
                   'tile': file.tile
             }
         return output
 
-    def update_xgboost(self, product_id, yaml_path, model, result=2):
+    def update_xgboost(self, product_id, yaml_path, model, satellite='sentinel2', result=2):
         '''
         Update the processing db with the status of an apply_models process.
         '''
-        file = self.session.query(Products).get(product_id)
+        if satellite == 'sentinel2':
+            file = self.session.query(Products).get(product_id)
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProd).get(product_id)
         
         file.prediction = result
         if result == 2:
             # Only update number of times downloaded if download was successful
             try:
                 file.no_prediction += 1
             except TypeError:
```

### Comparing `piproc-0.1.6/piproc/tables.py` & `piproc-0.1.7/piproc/tables.py`

 * *Files identical despite different names*

