# Comparing `tmp/tupa123-1.3.8.tar.gz` & `tmp/tupa123-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.8.tar", last modified: Tue Apr 18 11:59:24 2023, max compression
+gzip compressed data, was "tupa123-1.3.9.tar", last modified: Tue Apr 18 13:59:36 2023, max compression
```

## Comparing `tupa123-1.3.8.tar` & `tupa123-1.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2094 2023-04-18 11:59:24.769330 tupa123-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-04-18 11:58:24.000000 tupa123-1.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 11:59:24.784951 tupa123-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-18 11:54:21.000000 tupa123-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.8/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.8/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2094 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.358947 tupa123-1.3.9/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-04-18 13:59:36.357591 tupa123-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:59:36.358947 tupa123-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-18 13:54:58.000000 tupa123-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.346616 tupa123-1.3.9/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.9/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.9/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.355558 tupa123-1.3.9/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.8/LICENSE.txt` & `tupa123-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.8/PKG-INFO` & `tupa123-1.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.8
+Version: 1.3.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<b>----------------------------------------------------------------</b> <br> 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 Fast, robust and very simple to use, <i> this is the way </i> <br>
+(As long as python exists this project will exist) <br>
+<b>----------------------------------------------------------------</b> <br> 
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
 #Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
-#-----FILE TO MACHINE LEARNING <br>
+#-----FILE TO MACHINE LEARNING----------------------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
 y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
-#-----FILE TO APPLICATION OF MACHINE LEARNING <br>
+#-----FILE TO APPLICATION OF MACHINE LEARNING-------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
 y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
```

### Comparing `tupa123-1.3.8/README.md` & `tupa123-1.3.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+<b>----------------------------------------------------------------</b> <br> 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 Fast, robust and very simple to use, <i> this is the way </i> <br>
+(As long as python exists this project will exist) <br>
+<b>----------------------------------------------------------------</b> <br> 
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
 #Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
-#-----FILE TO MACHINE LEARNING <br>
+#-----FILE TO MACHINE LEARNING----------------------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
 y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
-#-----FILE TO APPLICATION OF MACHINE LEARNING <br>
+#-----FILE TO APPLICATION OF MACHINE LEARNING-------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
 y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
```

### Comparing `tupa123-1.3.8/setup.py` & `tupa123-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.8',
+    version='1.3.9',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.8/tupa123/tupa123.py` & `tupa123-1.3.9/tupa123/tupa123.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.8/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.9/tupa123.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.8
+Version: 1.3.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<b>----------------------------------------------------------------</b> <br> 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 Fast, robust and very simple to use, <i> this is the way </i> <br>
+(As long as python exists this project will exist) <br>
+<b>----------------------------------------------------------------</b> <br> 
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
 #Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
-#-----FILE TO MACHINE LEARNING <br>
+#-----FILE TO MACHINE LEARNING----------------------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
 y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
-#-----FILE TO APPLICATION OF MACHINE LEARNING <br>
+#-----FILE TO APPLICATION OF MACHINE LEARNING-------------- <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(nn1c=5, nn2c=7, nn3c=5, nn4c=2, namenet='tupa01') <br>
 X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
 y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
```

