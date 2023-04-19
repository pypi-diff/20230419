# Comparing `tmp/goastpy-0.1.6.tar.gz` & `tmp/goastpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.6.tar", last modified: Mon Apr 17 11:06:05 2023, max compression
+gzip compressed data, was "goastpy-0.1.7.tar", last modified: Wed Apr 19 12:10:39 2023, max compression
```

## Comparing `goastpy-0.1.6.tar` & `goastpy-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:06:05.382165 goastpy-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 11:05:54.000000 goastpy-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-17 11:06:05.382165 goastpy-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 11:05:54.000000 goastpy-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:06:05.378164 goastpy-0.1.6/goastpy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 11:05:54.000000 goastpy-0.1.6/goastpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-17 11:05:54.000000 goastpy-0.1.6/goastpy/goastparser.h
--rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-17 11:05:54.000000 goastpy-0.1.6/goastpy/goastparser.so
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-17 11:05:54.000000 goastpy-0.1.6/goastpy/goastparser_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-17 11:05:54.000000 goastpy-0.1.6/goastpy/goastpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:06:05.382165 goastpy-0.1.6/goastpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-17 11:06:05.000000 goastpy-0.1.6/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-17 11:06:05.000000 goastpy-0.1.6/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:06:05.000000 goastpy-0.1.6/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 11:06:05.000000 goastpy-0.1.6/goastpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 11:06:05.382165 goastpy-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-17 11:05:54.000000 goastpy-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:06:05.382165 goastpy-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-17 11:05:54.000000 goastpy-0.1.6/tests/test_go_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 12:10:24.000000 goastpy-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:10:39.903713 goastpy-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 12:10:24.000000 goastpy-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/goastpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser.so
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/goastpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 12:10:39.907714 goastpy-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-19 12:10:24.000000 goastpy-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 12:10:24.000000 goastpy-0.1.7/tests/test_go_parser.py
```

### Comparing `goastpy-0.1.6/LICENSE` & `goastpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.6/goastpy/goastparser.h` & `goastpy-0.1.7/goastpy/goastparser.h`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.6/goastpy/goastparser.so` & `goastpy-0.1.7/goastpy/goastparser.so`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.6/goastpy/goastparser_wrapper.py` & `goastpy-0.1.7/goastpy/goastparser_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
+import platform
 import sys
 import ctypes
 import subprocess
 from ctypes import c_char_p
 from threading import Lock, Thread
 
-GO_LIBRARY = f"goastparser.so"
+GO_SHARED_LIB_NAME = "goastparser"
 
 
 class SingletonMeta(type):
     """
     This is a thread-safe implementation of Singleton.
     """
 
@@ -42,47 +43,63 @@
                 cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class GoAstLib(metaclass=SingletonMeta):
 
     @staticmethod
+    def get_lib_name():
+        os_name = platform.system()
+        return f"goastparser_{os_name}.so" 
+    
+    @staticmethod
     def __find_go_executable():
         go_executable = "go" + (".exe" if sys.platform == "win32" else "")
         for path in os.environ["PATH"].split(os.pathsep):
             executable_path = os.path.join(path.strip('"'), go_executable)
             if os.path.isfile(executable_path) and os.access(executable_path, os.X_OK):
                 return executable_path
         raise FileNotFoundError("Go executable not found in the system's PATH")
 
     @staticmethod
-    def __build_go_library_if_not_exists():
-        if not os.path.exists(GO_LIBRARY):
-            print("Building Go shared library...")
-            try:
-                go_executable = GoAstLib.__find_go_executable()
-            except FileNotFoundError as e:
-                print(f"Error finding Go in path: {e}, trying to use default homebrew path")
-                go_executable = '/opt/homebrew/bin/go'
-            try:
-                subprocess.check_call([go_executable, "build", "-o", GO_LIBRARY, "-buildmode=c-shared", "main.go",
-                                       "goastparser_export.go"])
-            except subprocess.CalledProcessError as e:
-                print(f"Error building Go shared library: {e}")
-                raise
+    def build_go_library(output_file_name = None):
+        if output_file_name is None:
+            output_file_name = GoAstLib.get_lib_name()
+            
+        print("Building Go shared library...")
+        try:
+            go_executable = GoAstLib.__find_go_executable()
+        except FileNotFoundError as e:
+            print(f"Error finding Go in path: {e}, trying to use default homebrew path")
+            go_executable = '/opt/homebrew/bin/go'
+        try:
+            os.chdir(os.path.dirname(__file__))
+            subprocess.check_call([go_executable, "build", "-o", output_file_name, "-buildmode=c-shared", "main.go",
+                                    "goastparser_export.go"])
+        except subprocess.CalledProcessError as e:
+            print(f"Error building Go shared library: {e}")
+            raise
 
     @staticmethod
     def __configure_go_function(go_lib):
         go_lib.ParseSourceCode.restype = c_char_p
         go_lib.ParseSourceCode.argtypes = [c_char_p]
 
     @staticmethod
-    def __load_go_library():
-        return ctypes.CDLL(os.path.join(os.path.dirname(__file__), GO_LIBRARY))
+    def __load_go_library(build_lib = False):
+        if build_lib:
+             GoAstLib.build_go_library()
+        
+        return ctypes.CDLL(os.path.join(os.path.dirname(__file__), GoAstLib.get_lib_name()))
 
     def __init__(self):
         self.lib = self.__load_go_library()
         self.__configure_go_function(self.lib)
 
     @staticmethod
     def lib():
         return GoAstLib().lib
+
+if __name__ == "__main__":
+    GoAstLib.build_go_library()    
+
+
```

### Comparing `goastpy-0.1.6/goastpy/goastpy.py` & `goastpy-0.1.7/goastpy/goastpy.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.6/setup.py` & `goastpy-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="goastpy",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     package_dir={"goastpy": "./goastpy"},
     include_package_data=True,
     package_data={"goastpy": ['./goastpy/goastparser.h', './goastpy/goastparser.so']},
     data_files=[('goastpy', ['./goastpy/goastparser.h', './goastpy/goastparser.so'])],
     install_requires=[],
     description='a python wrapper for the built-in go parser using c-types',
```

