# Comparing `tmp/vtmmpy-1.0.1.tar.gz` & `tmp/vtmmpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.1.tar", last modified: Sat Mar 18 15:28:03 2023, max compression
+gzip compressed data, was "vtmmpy-1.0.2.tar", last modified: Wed Apr 19 13:12:14 2023, max compression
```

## Comparing `vtmmpy-1.0.1.tar` & `vtmmpy-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 locutus   (1000) locutus   (1000)        0 2023-03-18 15:28:03.808001 vtmmpy-1.0.1/
--rw-r--r--   0 locutus   (1000) locutus   (1000)     4496 2023-03-18 15:28:03.808001 vtmmpy-1.0.1/PKG-INFO
--rw-r--r--   0 locutus   (1000) locutus   (1000)     4041 2023-03-18 15:26:09.000000 vtmmpy-1.0.1/README.md
--rw-r--r--   0 locutus   (1000) locutus   (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.1/pyproject.toml
--rw-r--r--   0 locutus   (1000) locutus   (1000)      613 2023-03-18 15:28:03.809001 vtmmpy-1.0.1/setup.cfg
-drwxr-xr-x   0 locutus   (1000) locutus   (1000)        0 2023-03-18 15:28:03.808001 vtmmpy-1.0.1/src/
-drwxr-xr-x   0 locutus   (1000) locutus   (1000)        0 2023-03-18 15:28:03.808001 vtmmpy-1.0.1/src/vtmmpy/
--rw-r--r--   0 locutus   (1000) locutus   (1000)     7327 2023-03-17 14:28:36.000000 vtmmpy-1.0.1/src/vtmmpy/__init__.py
-drwxr-xr-x   0 locutus   (1000) locutus   (1000)        0 2023-03-18 15:28:03.808001 vtmmpy-1.0.1/src/vtmmpy.egg-info/
--rw-r--r--   0 locutus   (1000) locutus   (1000)     4496 2023-03-18 15:28:03.000000 vtmmpy-1.0.1/src/vtmmpy.egg-info/PKG-INFO
--rw-r--r--   0 locutus   (1000) locutus   (1000)      193 2023-03-18 15:28:03.000000 vtmmpy-1.0.1/src/vtmmpy.egg-info/SOURCES.txt
--rw-r--r--   0 locutus   (1000) locutus   (1000)        1 2023-03-18 15:28:03.000000 vtmmpy-1.0.1/src/vtmmpy.egg-info/dependency_links.txt
--rw-r--r--   0 locutus   (1000) locutus   (1000)        7 2023-03-18 15:28:03.000000 vtmmpy-1.0.1/src/vtmmpy.egg-info/top_level.txt
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/
+-rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.2/LICENSE
+-rw-rw-r--   0 tony      (1000) tony      (1000)     3933 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     3458 2023-04-18 14:37:28.000000 vtmmpy-1.0.2/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.2/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/setup.cfg
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.446843 vtmmpy-1.0.2/src/
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/src/vtmmpy/
+-rw-r--r--   0 tony      (1000) tony      (1000)     8279 2023-04-18 14:04:08.000000 vtmmpy-1.0.2/src/vtmmpy/__init__.py
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/src/vtmmpy.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3933 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/top_level.txt
```

### Comparing `vtmmpy-1.0.1/setup.cfg` & `vtmmpy-1.0.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = vtmmpy
-version = 1.0.1
+version = 1.0.2
 author = Tony
 author_email = tk_87@hotmail.com
 description = A vectorized implementation of the transfer matrix method
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/AI-Tony/vtmmpy/tree/master
+url = https://github.com/AI-Tony/vtmmpy/tree/main
 project_urls = 
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
```

### Comparing `vtmmpy-1.0.1/src/vtmmpy/__init__.py` & `vtmmpy-1.0.2/src/vtmmpy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,64 @@
 import numpy as np
+import pandas as pd
+import refidx as ri 
+from IPython.display import clear_output 
+
+
+class RefractiveIndex:
+    def __init__(self):
+        # self.shelf = "main"
+        self.__shelfs = ["main", "organic", "glass", "other"] 
+        self.__db = ri.DataBase()
+
+    def index(self, symbol): 
+        if symbol=="air": return 1
+        return self.__refractiveIndexInfo(symbol) 
+
+    def epsilon(self, symbol):
+        return self.index(symbol)**2
+
+    def __refractiveIndexInfo(self, book): 
+        wavelength = 1e6 * 2 * np.pi * 3e8 / self.w 
+        df = pd.DataFrame(columns=["Page", "Wavelength Range (μm)", "Comments"]) 
+        for shelf in self.__shelfs:
+            try:
+                pages = self.__db.materials[shelf][book]
+                print("{} found in {}".format(book, shelf))
+                break
+            except:
+                print("{} not in {}".format(book, shelf)) 
+                for parentbook in self.__db.materials[shelf].keys():
+                    try:
+                        pages = self.__db.materials[shelf][parentbook][book] 
+                        print("{} found in {}/{}".format(book, shelf, parentbook))
+                        break
+                    except:
+                        continue
+        for i, (key, value) in enumerate(pages.items()): 
+            df.loc[i] = [key, pages[key].wavelength_range, pages[key].info["comments"]] 
+        print("\nSelect an index [0-{}] for {} and press enter. Check refractiveindex.info for more details.\n".format(len(df)-1, book)) 
+        display(df) 
+        i = int(input()) 
+        clear_output()
+        mat = pages[df.iloc[i].Page] 
+        index = mat.get_index(wavelength) 
+        return np.conjugate(index) 
 
-class TMM:
+
+class TMM(RefractiveIndex): 
     def __init__(self, 
             freq, 
             theta, 
             f_scale=1e12, 
             l_scale=1e-9, 
             incident_medium="air", 
             transmitted_medium="air"): 
 
+        RefractiveIndex.__init__(self) 
         self.__theta = theta * np.pi/180 
         self.__freq = freq * f_scale 
         self.__f_scale = f_scale
         self.__l_scale = l_scale
         self.__materialsProperties = {} 
         self.__incident_medium = incident_medium 
         self.__transmitted_medium = transmitted_medium 
@@ -27,15 +73,15 @@
                 nt = self.__materialsProperties[self.__transmitted_medium][0] 
             bi = self.__materialsProperties[self.__incident_medium][1] 
             bt = self.__materialsProperties[self.__transmitted_medium][1] 
             M  = self.__transferMatrix(polarization) 
             M  = self.__inverse(M) 
             r  = -(M[0,0,:,:,:]*bi*nt*nt - M[1,1,:,:,:]*bt*ni*ni + 1j*(M[1,0,:,:,:]*nt*nt*ni*ni + M[0,1,:,:,:]*bi*bt))/\
                   (M[0,0,:,:,:]*bi*nt*nt + M[1,1,:,:,:]*bt*ni*ni - 1j*(M[1,0,:,:,:]*nt*nt*ni*ni - M[0,1,:,:,:]*bi*bt)) 
-            return r 
+            return r
         except:
             raise Exception("no designs present. Use addDesign() method to add a design") 
 
     def transmission(self, polarization):
         try:
             if polarization == "TE":
                 ni = 1 
@@ -44,15 +90,15 @@
                 ni = self.__materialsProperties[self.__incident_medium][0] 
                 nt = self.__materialsProperties[self.__transmitted_medium][0] 
             bi = self.__materialsProperties[self.__incident_medium][1] 
             bt = self.__materialsProperties[self.__transmitted_medium][1] 
             M  = self.__transferMatrix(polarization) 
             M  = self.__inverse(M) 
             t  = -2*ni*nt*bi / (M[0,0,:,:,:]*bi*nt*nt + M[1,1,:,:,:]*bt*ni*ni - 1j*(M[1,0,:,:,:]*nt*nt*ni*ni - M[0,1,:,:,:]*bi*bt)) 
-            return t 
+            return t
         except:
             raise Exception("no designs present. Use addDesign() method to add a design") 
 
     def addDesign(self, materials, thicknesses): 
         materials = np.array(materials) 
         thicknesses = np.array(thicknesses) * self.__l_scale 
         if len(materials) != len(thicknesses):
@@ -66,39 +112,26 @@
             self.__materials = materials[None,:] 
             self.__thicknesses = thicknesses[None,:] 
         self.__dims = ( len(self.__materials), len(self.__freq), len(self.__theta) ) 
         self.__layers = self.__materials.shape[1] 
         self.__calculateMaterialProperties() 
 
     def __calculateMaterialProperties(self): 
-        w = 2*np.pi*self.__freq[:,None] * np.ones(self.__dims[1:]) 
-        k0 = w / 3e8 
+        self.w = 2*np.pi*self.__freq[:,None] * np.ones(self.__dims[1:]) 
+        k0 = self.w / 3e8 
         kx = k0 * np.sin( self.__theta ) 
         material_set = set( self.__materials.flatten() )
         material_set.add( self.__incident_medium )
         material_set.add( self.__transmitted_medium ) 
         for mat in material_set:
             if mat not in self.__materialsProperties.keys(): 
-                n  = self.__refractiveIindex(mat, w) 
+                n = self.index(mat) 
                 beta = np.sqrt( k0**2 * n**2 - kx**2 ) 
                 self.__materialsProperties["{}".format(mat)] = (n, beta) 
 
-    def __refractiveIindex(self, mat, omega):
-        ri = np.ones( self.__dims[1:] ) 
-        if mat=="air": return 1.0 * ri 
-        elif mat=="sio2": return 1.45 * ri 
-        elif mat=="tio2": return 2.45 * ri 
-        elif mat=="sin": return 1.99 * ri
-        elif mat=="ito": 
-            w, gamma, E_inf, wp2 =  omega, 2.05e14, 3.91, 2.65e15**2 
-            eps = E_inf - wp2 / ( w**2 + 1j*gamma*w )
-            n = np.sqrt(  eps.real + np.sqrt( eps.real**2 + eps.imag**2 ) ) / np.sqrt(2) 
-            k = np.sqrt( -eps.real + np.sqrt( eps.real**2 + eps.imag**2 ) ) / np.sqrt(2) 
-            return ( n + 1j*k ) * ri
-
     def __transferMatrix(self, polarization):
         M            = np.zeros((2, 2, *self.__dims), dtype='cfloat') 
         M[0,0,:,:,:] = np.ones(self.__dims, dtype='cfloat') 
         M[1,1,:,:,:] = np.ones(self.__dims, dtype='cfloat') 
         for i in np.arange(self.__layers-1, -1, -1):
             m = self.__subMatrix( self.__materials[:,i], self.__thicknesses[:,i], polarization ) 
             M = self.__matmul(M, m) 
@@ -124,24 +157,20 @@
         A = M[0,0,:,:,:]*m[0,0,:,:,:] + M[0,1,:,:,:]*m[1,0,:,:,:] 
         B = M[0,0,:,:,:]*m[0,1,:,:,:] + M[0,1,:,:,:]*m[1,1,:,:,:] 
         C = M[1,0,:,:,:]*m[0,0,:,:,:] + M[1,1,:,:,:]*m[1,0,:,:,:] 
         D = M[1,0,:,:,:]*m[0,1,:,:,:] + M[1,1,:,:,:]*m[1,1,:,:,:] 
         return np.array( [ [A, B], [C, D] ], dtype='cfloat' ) 
 
     def __inverse(self, M):
-        try:
-            det = M[0,0,:,:,:]*M[1,1,:,:,:] - M[0,1,:,:,:]*M[1,0,:,:,:] 
-            A   = M[0,0,:,:,:] 
-            B   = M[0,1,:,:,:] 
-            C   = M[1,0,:,:,:] 
-            D   = M[1,1,:,:,:] 
-            return np.array( [ [D, -B], [-C, A] ], dtype='cfloat' ) / det 
-        except ZeroDivisionError: 
-            print("Warning: division by zero") 
-            return np.array( [ [0, -0], [-0, 0] ], dtype='cfloat' ) 
+        det = M[0,0,:,:,:]*M[1,1,:,:,:] - M[0,1,:,:,:]*M[1,0,:,:,:] 
+        A   = M[0,0,:,:,:] 
+        B   = M[0,1,:,:,:] 
+        C   = M[1,0,:,:,:] 
+        D   = M[1,1,:,:,:] 
+        return np.array( [ [D, -B], [-C, A] ], dtype='cfloat' ) / (det+1e-99) 
 
     def summary(self):
         print("\n Summary")
         print(" --------------------------------------------") 
         print("  Number of designs:        ", len(self.__materials)) 
         print("  Frequency range (THz):    ", self.__freq[0]*1e-12, "-", self.__freq[-1]*1e-12) 
         print("  Angles of incidence:      ", np.rint(self.__theta[0]*180/np.pi), "-", np.rint(self.__theta[-1]*180/np.pi)) 
@@ -149,10 +178,10 @@
         print("  Transmitted medium:       ", self.__transmitted_medium) 
         print("") 
 
     def designs(self):
         try:
             zipped = zip(self.__materials,self.__thicknesses) 
             for pair in zipped:
-                print(pair)
+                print(pair) 
         except:
-            raise Exception("add designs with addDesign() before trying to call designs() method")
+            raise Exception("No designs found. Add designs with the addDesign() method.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

