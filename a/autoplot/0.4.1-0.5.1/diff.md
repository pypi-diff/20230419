# Comparing `tmp/autoplot-0.4.1.tar.gz` & `tmp/autoplot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplot-0.4.1.tar", last modified: Wed Apr 12 17:05:33 2023, max compression
+gzip compressed data, was "autoplot-0.5.1.tar", last modified: Wed Apr 19 17:01:01 2023, max compression
```

## Comparing `autoplot-0.4.1.tar` & `autoplot-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.4.1/LICENSE.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1887 2023-04-12 17:05:33.371171 autoplot-0.4.1/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.4.1/README.rst
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      273 2023-04-12 16:41:46.000000 autoplot-0.4.1/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    21685 2023-04-12 16:24:38.000000 autoplot-0.4.1/autoplot/autoplot.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/autoplot.egg-info/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1887 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/requires.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/top_level.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-12 17:05:33.371171 autoplot-0.4.1/setup.cfg
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-12 16:51:15.000000 autoplot-0.4.1/setup.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.5.1/LICENSE.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:01:01.231355 autoplot-0.5.1/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.5.1/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      271 2023-04-19 17:00:38.000000 autoplot-0.5.1/autoplot/__init__.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    22041 2023-04-19 17:00:38.000000 autoplot-0.5.1/autoplot/autoplot.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-19 17:01:01.231355 autoplot-0.5.1/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-19 17:00:38.000000 autoplot-0.5.1/setup.py
```

### Comparing `autoplot-0.4.1/LICENSE.txt` & `autoplot-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoplot-0.4.1/PKG-INFO` & `autoplot-0.5.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: autoplot
-Version: 0.4.1
-Summary: Interface to Autoplot Java library
-Home-page: https://github.com/autoplot/python/
-Author: Jeremy Faden
-Author-email: faden@cottagesystems.com
-License: LICENSE.txt
-License-File: LICENSE.txt
-
 Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
 Helper procedures from the autoplot package convert QDataSets into ndarrays.
```

### Comparing `autoplot-0.4.1/README.rst` & `autoplot-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
-Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
-
-Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
-These URIs can be created using the Autoplot application, available at http://autoplot.org/.
-Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the autoplot package convert QDataSets into ndarrays.
-
-Autoplot/Python Interface Tools
--------------------------------
-
-Install using `pip install autoplot`
-
-.. code:: python
-
-  from autoplot import *
-
-  # Download autoplot.jar if needed and return Python bridge object
-  javaaddpath('http://autoplot.org/latest/autoplot.jar')
-  
-  # Create Autoplot Data Set
-  apds = APDataSet()
-
-  # Set URI
-  apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
-
-  # Get the data
-  apds.doGetDataSet()
-
-  print(apds.toString())
-  # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
-  # data: data[dep0=288] (dimensionless)
-  # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
-
-  # Extract data values
-  vv = to_ndarray(apds, 'data')
-  tt = to_ndarray(apds, 'dep0')
-
-  from matplotlib import pyplot as plt
-  plt.plot(tt,vv)
-  plt.show()
-
-Contact
--------------------------------
-Jeremy Faden <faden@cottagesystems.com>
-
+Metadata-Version: 1.0
+Name: autoplot
+Version: 0.5.1
+Summary: Interface to Autoplot Java library
+Home-page: https://github.com/autoplot/python/
+Author: Jeremy Faden
+Author-email: faden@cottagesystems.com
+License: LICENSE.txt
+Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+        Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
+        
+        Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
+        These URIs can be created using the Autoplot application, available at http://autoplot.org/.
+        Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
+        Helper procedures from the autoplot package convert QDataSets into ndarrays.
+        
+        Autoplot/Python Interface Tools
+        -------------------------------
+        
+        Install using `pip install autoplot`
+        
+        .. code:: python
+        
+          from autoplot import *
+        
+          # Download autoplot.jar if needed and return Python bridge object
+          javaaddpath('http://autoplot.org/latest/autoplot.jar')
+          
+          # Create Autoplot Data Set
+          apds = APDataSet()
+        
+          # Set URI
+          apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
+        
+          # Get the data
+          apds.doGetDataSet()
+        
+          print(apds.toString())
+          # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
+          # data: data[dep0=288] (dimensionless)
+          # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
+        
+          # Extract data values
+          vv = to_ndarray(apds, 'data')
+          tt = to_ndarray(apds, 'dep0')
+        
+          from matplotlib import pyplot as plt
+          plt.plot(tt,vv)
+          plt.show()
+        
+        Contact
+        -------------------------------
+        Jeremy Faden <faden@cottagesystems.com>
+        
+        
+Platform: UNKNOWN
```

### Comparing `autoplot-0.4.1/autoplot/autoplot.py` & `autoplot-0.5.1/autoplot/autoplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,14 +481,29 @@
     print('tryPortConnect')
     import socket
     s = socket.socket()
     s.connect(('localhost',port))
     s.close()
 
 
+def load( uri ):
+    """tell Autoplot to load a .vap or plot an Autoplot URI.  Autoplot must be running and its optional server must be listening 
+on port 12345."""
+    port= 12345
+
+    import socket
+    s = socket.socket()
+    s.connect(('localhost',port))
+
+    cmd= "load( \'"+uri+"\')\n"
+
+    foo= sendCommand( s, cmd )
+    s.shutdown(1)
+    s.close()
+
 def sendCommand( s, cmd ):
     s.send( bytes(cmd,'utf8') )
     print('done')
 
 def applot( x=None, y=None, z=None, z4=None, xunits='', ylabel='', tmpfile=None, noplot=0, respawn=0, delta_plus=None, delta_minus=None ):
     """
 NAME:
```

### Comparing `autoplot-0.4.1/autoplot.egg-info/PKG-INFO` & `autoplot-0.5.1/autoplot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: autoplot
-Version: 0.4.1
+Version: 0.5.1
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
-License-File: LICENSE.txt
-
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
-Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
-
-Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
-These URIs can be created using the Autoplot application, available at http://autoplot.org/.
-Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the autoplot package convert QDataSets into ndarrays.
-
-Autoplot/Python Interface Tools
--------------------------------
-
-Install using `pip install autoplot`
-
-.. code:: python
-
-  from autoplot import *
-
-  # Download autoplot.jar if needed and return Python bridge object
-  javaaddpath('http://autoplot.org/latest/autoplot.jar')
-  
-  # Create Autoplot Data Set
-  apds = APDataSet()
-
-  # Set URI
-  apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
-
-  # Get the data
-  apds.doGetDataSet()
-
-  print(apds.toString())
-  # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
-  # data: data[dep0=288] (dimensionless)
-  # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
-
-  # Extract data values
-  vv = to_ndarray(apds, 'data')
-  tt = to_ndarray(apds, 'dep0')
-
-  from matplotlib import pyplot as plt
-  plt.plot(tt,vv)
-  plt.show()
-
-Contact
--------------------------------
-Jeremy Faden <faden@cottagesystems.com>
-
+Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+        Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
+        
+        Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
+        These URIs can be created using the Autoplot application, available at http://autoplot.org/.
+        Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
+        Helper procedures from the autoplot package convert QDataSets into ndarrays.
+        
+        Autoplot/Python Interface Tools
+        -------------------------------
+        
+        Install using `pip install autoplot`
+        
+        .. code:: python
+        
+          from autoplot import *
+        
+          # Download autoplot.jar if needed and return Python bridge object
+          javaaddpath('http://autoplot.org/latest/autoplot.jar')
+          
+          # Create Autoplot Data Set
+          apds = APDataSet()
+        
+          # Set URI
+          apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
+        
+          # Get the data
+          apds.doGetDataSet()
+        
+          print(apds.toString())
+          # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
+          # data: data[dep0=288] (dimensionless)
+          # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
+        
+          # Extract data values
+          vv = to_ndarray(apds, 'data')
+          tt = to_ndarray(apds, 'dep0')
+        
+          from matplotlib import pyplot as plt
+          plt.plot(tt,vv)
+          plt.show()
+        
+        Contact
+        -------------------------------
+        Jeremy Faden <faden@cottagesystems.com>
+        
+        
+Platform: UNKNOWN
```

### Comparing `autoplot-0.4.1/setup.py` & `autoplot-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.4.1',
+    version='0.5.1',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
     url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
```

