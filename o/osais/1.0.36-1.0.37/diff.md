# Comparing `tmp/osais-1.0.36.tar.gz` & `tmp/osais-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-n6xscl2h\osais-1.0.36.tar", last modified: Fri Apr 14 09:43:00 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-y1x8hkis\osais-1.0.37.tar", last modified: Wed Apr 19 06:17:56 2023, max compression
```

## Comparing `osais-1.0.36.tar` & `osais-1.0.37.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.929769 osais-1.0.36/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.36/LICENSE
--rw-rw-rw-   0        0        0     1113 2023-04-14 09:43:00.928772 osais-1.0.36/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.36/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.923769 osais-1.0.36/osais/
--rw-rw-rw-   0        0        0      652 2023-04-14 09:42:35.000000 osais-1.0.36/osais/__init__.py
--rw-rw-rw-   0        0        0    41525 2023-04-14 09:42:13.000000 osais-1.0.36/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.927770 osais-1.0.36/osais.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.36/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 09:43:00.929769 osais-1.0.36/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-14 09:42:41.000000 osais-1.0.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:17:56.706027 osais-1.0.37/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.37/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-04-19 06:17:56.706027 osais-1.0.37/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.37/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 06:17:56.701025 osais-1.0.37/osais/
+-rw-rw-rw-   0        0        0      652 2023-04-19 06:16:57.000000 osais-1.0.37/osais/__init__.py
+-rw-rw-rw-   0        0        0    42040 2023-04-19 06:16:50.000000 osais-1.0.37/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:17:56.705026 osais-1.0.37/osais.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-19 06:17:56.000000 osais-1.0.37/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-19 06:17:56.000000 osais-1.0.37/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:17:56.000000 osais-1.0.37/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-19 06:17:56.000000 osais-1.0.37/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 06:17:56.000000 osais-1.0.37/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.37/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:17:56.706027 osais-1.0.37/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-04-19 06:16:39.000000 osais-1.0.37/setup.py
```

### Comparing `osais-1.0.36/LICENSE` & `osais-1.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.36/PKG-INFO` & `osais-1.0.37/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.36
+Version: 1.0.37
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.36/osais/__init__.py` & `osais-1.0.37/osais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.36"
+__version__="1.0.37"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
```

### Comparing `osais-1.0.36/osais/osais.py` & `osais-1.0.37/osais/osais.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.36"
+__version__="1.0.37"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -492,28 +492,42 @@
 def osais_getEnv(_filename):
     global gUsername
     global gIsVirtualAI
     global gIsLocal
     global gName
 
     ## read env from config file
-    with open(_filename, "r") as f:
-        content = f.read()
-    variables = content.split("\n")
-    for var in variables:
-        if var!="":
-            key, value = var.split("=")
-            if key == "USERNAME":
-                gUsername = value
-            elif key == "IS_LOCAL":
-                gIsLocal = (value=="True")
-            elif key == "IS_VIRTUALAI":
-                gIsVirtualAI = (value=="True")
-            elif key == "ENGINE":
-                gName = value
+    try:
+        with open(_filename, "r") as f:
+            content = f.read()
+        variables = content.split("\n")
+        for var in variables:
+            if var!="":
+                key, value = var.split("=")
+                if key == "USERNAME":
+                    gUsername = value
+                elif key == "IS_LOCAL":
+                    gIsLocal = (value=="True")
+                elif key == "IS_VIRTUALAI":
+                    gIsVirtualAI = (value=="True")
+                elif key == "ENGINE":
+                    gName = value
+    except Exception as err: 
+        print(f'No env file {_filename}')
+
+    # overload with env settings if any
+    if os.environ.get('IS_LOCAL'):
+        gIsLocal=os.environ.get('IS_LOCAL')
+    if os.environ.get('IS_VIRTUALAI'):
+        gIsVirtualAI=os.environ.get('IS_VIRTUALAI')
+    if os.environ.get('ENGINE'):
+        gName=os.environ.get('ENGINE')
+    if os.environ.get('USERNAME'):
+        gUsername=os.environ.get('USERNAME')
+
     return {
         "username": gUsername,
         "isLocal": gIsLocal,
         "isVirtualAI": gIsVirtualAI,
         "name": gName
     }
```

### Comparing `osais-1.0.36/osais.egg-info/PKG-INFO` & `osais-1.0.37/osais.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.36
+Version: 1.0.37
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.36/setup.py` & `osais-1.0.37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.36',
+    version='1.0.37',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

