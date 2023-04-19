# Comparing `tmp/d-popcorn-1.0.0.tar.gz` & `tmp/d-popcorn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d-popcorn-1.0.0.tar", last modified: Wed Apr 19 13:39:03 2023, max compression
+gzip compressed data, was "d-popcorn-1.0.1.tar", last modified: Wed Apr 19 14:21:22 2023, max compression
```

## Comparing `d-popcorn-1.0.0.tar` & `d-popcorn-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 13:39:03.481050 d-popcorn-1.0.0/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.0.0/LICENSE
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 13:39:03.481050 d-popcorn-1.0.0/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     2256 2023-04-19 13:36:33.000000 d-popcorn-1.0.0/README.md
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 13:39:03.481050 d-popcorn-1.0.0/d_popcorn.egg-info/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      285 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/SOURCES.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/dependency_links.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       50 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/entry_points.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/requires.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-04-19 13:39:03.000000 d-popcorn-1.0.0/d_popcorn.egg-info/top_level.txt
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 13:39:03.481050 d-popcorn-1.0.0/popcorn/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    11464 2023-04-18 14:23:23.000000 d-popcorn-1.0.0/popcorn/Popcorn.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       22 2023-04-19 13:38:48.000000 d-popcorn-1.0.0/popcorn/__init__.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3275 2023-04-18 14:16:50.000000 d-popcorn-1.0.0/popcorn/__main__.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-04-19 13:39:03.481050 d-popcorn-1.0.0/setup.cfg
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-19 13:35:05.000000 d-popcorn-1.0.0/setup.py
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 14:21:22.879156 d-popcorn-1.0.1/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.0.1/LICENSE
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 14:21:22.879156 d-popcorn-1.0.1/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     2256 2023-04-19 14:17:01.000000 d-popcorn-1.0.1/README.md
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 14:21:22.879156 d-popcorn-1.0.1/d_popcorn.egg-info/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      285 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       45 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/entry_points.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/requires.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-04-19 14:21:22.000000 d-popcorn-1.0.1/d_popcorn.egg-info/top_level.txt
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-04-19 14:21:22.879156 d-popcorn-1.0.1/popcorn/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       22 2023-04-19 14:21:15.000000 d-popcorn-1.0.1/popcorn/__init__.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3285 2023-04-19 14:17:56.000000 d-popcorn-1.0.1/popcorn/__main__.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    11464 2023-04-18 14:23:23.000000 d-popcorn-1.0.1/popcorn/popcorn.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-04-19 14:21:22.879156 d-popcorn-1.0.1/setup.cfg
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1064 2023-04-19 14:17:01.000000 d-popcorn-1.0.1/setup.py
```

### Comparing `d-popcorn-1.0.0/LICENSE` & `d-popcorn-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.0.0/README.md` & `d-popcorn-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.0.0/popcorn/Popcorn.py` & `d-popcorn-1.0.1/popcorn/popcorn.py`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.0.0/popcorn/__main__.py` & `d-popcorn-1.0.1/popcorn/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import os
-from Popcorn import Popcorn
 
-__version__ = "1.0.0"
+from .popcorn import Popcorn
+from . import __version__
+
 
 def upload_file(args):
     popcorn = Popcorn()
     popcorn.upload(args)
 
 
 def download_file(args):
@@ -77,9 +78,9 @@
         func = args.func
     except AttributeError:
         # Necessary when popcorn is called without any arguments to avoid AttributeError
         parser.error("too few arguments")
     func(args)
 
 
-if __name__ == '__main__':
-    main()
+# if __name__ == '__main__':
+#     main()
```

### Comparing `d-popcorn-1.0.0/setup.py` & `d-popcorn-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     ],
     packages=find_packages(),
     install_requires=[
         'boto3',
     ],
     entry_points={
         'console_scripts': [
-            'popcorn=popcorn.__main__:main',
+            'popcorn=run_popcorn:main',
         ],
     },
 )
```

