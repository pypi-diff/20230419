# Comparing `tmp/goastpy-0.1.7.tar.gz` & `tmp/goastpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.7.tar", last modified: Wed Apr 19 12:10:39 2023, max compression
+gzip compressed data, was "goastpy-0.1.8.tar", last modified: Wed Apr 19 12:33:22 2023, max compression
```

## Comparing `goastpy-0.1.7.tar` & `goastpy-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 12:10:24.000000 goastpy-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:10:39.903713 goastpy-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 12:10:24.000000 goastpy-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/goastpy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser.h
--rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser.so
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastparser_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-19 12:10:24.000000 goastpy-0.1.7/goastpy/goastpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/goastpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:10:39.000000 goastpy-0.1.7/goastpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 12:10:39.907714 goastpy-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-19 12:10:24.000000 goastpy-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:10:39.903713 goastpy-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 12:10:24.000000 goastpy-0.1.7/tests/test_go_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 12:33:09.000000 goastpy-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:33:22.370063 goastpy-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 12:33:09.000000 goastpy-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/goastpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Darwin.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Darwin.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Linux.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2858760 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Linux.so
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/goastpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 12:33:22.370063 goastpy-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 12:33:09.000000 goastpy-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 12:33:09.000000 goastpy-0.1.8/tests/test_go_parser.py
```

### Comparing `goastpy-0.1.7/LICENSE` & `goastpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.7/PKG-INFO` & `goastpy-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `goastpy-0.1.7/README.md` & `goastpy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.7/goastpy/goastparser.h` & `goastpy-0.1.8/goastpy/goastparser.h`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.7/goastpy/goastparser.so` & `goastpy-0.1.8/goastpy/goastparser.so`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.7/goastpy/goastparser_wrapper.py` & `goastpy-0.1.8/goastpy/goastparser_wrapper.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.7/goastpy/goastpy.py` & `goastpy-0.1.8/goastpy/goastpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-import goastparser_wrapper
+from goastpy import goastparser_wrapper
 
 
 class GoAst:
     def __init__(self, go_code):
         self.__ast_json = self.parse_source_code_to_json(go_code)
         self.ast = json.loads(self.__ast_json)
```

### Comparing `goastpy-0.1.7/goastpy.egg-info/PKG-INFO` & `goastpy-0.1.8/goastpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `goastpy-0.1.7/setup.py` & `goastpy-0.1.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="goastpy",
-    version="0.1.7",
-    packages=find_packages(),
-    package_dir={"goastpy": "./goastpy"},
+    version="0.1.8",
     include_package_data=True,
-    package_data={"goastpy": ['./goastpy/goastparser.h', './goastpy/goastparser.so']},
-    data_files=[('goastpy', ['./goastpy/goastparser.h', './goastpy/goastparser.so'])],
+    packages=find_packages(),
+    package_dir={"": "."},
+    package_data={"goastpy": ["*.h", "*.so"]},
     install_requires=[],
     description='a python wrapper for the built-in go parser using c-types',
     author='Itay Gersten',
     author_email='Itay.Gersten@gmail.com',
     url='https://github.com/itayg25/goastpy',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    keywords=['GO', 'GOLANG', 'PYTHON', 'AST', 'GOPY', 'PYGO', 'PARSER', 'ASTPARSER'],
+    keywords=['GO', 'GOLANG', 'PYTHON', 'AST',
+              'GOPY', 'PYGO', 'PARSER', 'ASTPARSER'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

