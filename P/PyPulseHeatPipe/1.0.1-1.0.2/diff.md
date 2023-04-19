# Comparing `tmp/PyPulseHeatPipe-1.0.1.tar.gz` & `tmp/PyPulseHeatPipe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPulseHeatPipe-1.0.1.tar", last modified: Wed Apr 19 00:07:50 2023, max compression
+gzip compressed data, was "PyPulseHeatPipe-1.0.2.tar", last modified: Wed Apr 19 00:25:17 2023, max compression
```

## Comparing `PyPulseHeatPipe-1.0.1.tar` & `PyPulseHeatPipe-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:07:50.695750 PyPulseHeatPipe-1.0.1/
--rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.1/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     1791 2023-04-19 00:07:50.695792 PyPulseHeatPipe-1.0.1/PKG-INFO
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:07:50.694506 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe/
--rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)    11083 2023-04-15 10:09:07.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe/analysis.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:07:50.695420 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     1791 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      337 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       72 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       16 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)     1443 2023-04-19 00:06:54.000000 PyPulseHeatPipe-1.0.1/README.md
--rw-r--r--   0 nirmal     (501) staff       (20)       79 2023-04-19 00:07:50.695957 PyPulseHeatPipe-1.0.1/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      772 2023-04-19 00:06:58.000000 PyPulseHeatPipe-1.0.1/setup.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:07:50.695539 PyPulseHeatPipe-1.0.1/test/
--rw-r--r--   0 nirmal     (501) staff       (20)       88 2023-04-18 21:04:27.000000 PyPulseHeatPipe-1.0.1/test/test.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776937 PyPulseHeatPipe-1.0.2/
+-rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.2/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     1872 2023-04-19 00:25:17.776985 PyPulseHeatPipe-1.0.2/PKG-INFO
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.775547 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/
+-rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)    11083 2023-04-15 10:09:07.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776584 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     1872 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      337 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       72 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       16 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)     1524 2023-04-19 00:17:50.000000 PyPulseHeatPipe-1.0.2/README.md
+-rw-r--r--   0 nirmal     (501) staff       (20)       79 2023-04-19 00:25:17.777170 PyPulseHeatPipe-1.0.2/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      772 2023-04-19 00:24:56.000000 PyPulseHeatPipe-1.0.2/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776718 PyPulseHeatPipe-1.0.2/test/
+-rw-r--r--   0 nirmal     (501) staff       (20)       88 2023-04-18 21:04:27.000000 PyPulseHeatPipe-1.0.2/test/test.py
```

### Comparing `PyPulseHeatPipe-1.0.1/LICENSE` & `PyPulseHeatPipe-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.1/PKG-INFO` & `PyPulseHeatPipe-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PulseHeatPipe
 
-[PyPulseHeatPipe]() is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
+[PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
-pip install pyphp
+pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from pyphp import PulsHeatPipe
+    from PyPulseHeatPipe import PulsHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
@@ -39,16 +39,16 @@
 7. plot_all_data
 8. plot_Te_Tc
 9. plot_eu
 
 Example:
 ```
 # importing module
-from pyphp import PulseHeatPipe
-from pyphp import DataVisualisation
+from PyPulseHeatPipe import PulseHeatPipe
+from PyPulseHeatPipe import DataVisualisation
 
 analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
 visual = DataVisualisation('Al2O3_DI_60FR')
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
```

### Comparing `PyPulseHeatPipe-1.0.1/PyPulseHeatPipe/analysis.py` & `PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/analysis.py`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.1/PyPulseHeatPipe.egg-info/PKG-INFO` & `PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PulseHeatPipe
 
-[PyPulseHeatPipe]() is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
+[PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
-pip install pyphp
+pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from pyphp import PulsHeatPipe
+    from PyPulseHeatPipe import PulsHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
@@ -39,16 +39,16 @@
 7. plot_all_data
 8. plot_Te_Tc
 9. plot_eu
 
 Example:
 ```
 # importing module
-from pyphp import PulseHeatPipe
-from pyphp import DataVisualisation
+from PyPulseHeatPipe import PulseHeatPipe
+from PyPulseHeatPipe import DataVisualisation
 
 analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
 visual = DataVisualisation('Al2O3_DI_60FR')
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
```

### Comparing `PyPulseHeatPipe-1.0.1/README.md` & `PyPulseHeatPipe-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # PulseHeatPipe
 
-[PyPulseHeatPipe]() is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
+[PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
-pip install pyphp
+pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from pyphp import PulsHeatPipe
+    from PyPulseHeatPipe import PulsHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
@@ -28,16 +28,16 @@
 7. plot_all_data
 8. plot_Te_Tc
 9. plot_eu
 
 Example:
 ```
 # importing module
-from pyphp import PulseHeatPipe
-from pyphp import DataVisualisation
+from PyPulseHeatPipe import PulseHeatPipe
+from PyPulseHeatPipe import DataVisualisation
 
 analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
 visual = DataVisualisation('Al2O3_DI_60FR')
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
```

### Comparing `PyPulseHeatPipe-1.0.1/setup.py` & `PyPulseHeatPipe-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='PyPulseHeatPipe',
-        version='1.0.1',
+        version='1.0.2',
         license='GNU',
         url='https://github.com/nirmalparmarphd/PyPulseHeatPipe',
         description='The data analysis Python package for the Pulsating Heat Pipe experimental data', 
         long_description=long_description,
         long_description_content_type='text/markdown',
         author='Nirmal Parmar',
         author_email='nirmalparmarphd@gmail.com',
```

