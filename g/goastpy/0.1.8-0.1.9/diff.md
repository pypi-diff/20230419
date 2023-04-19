# Comparing `tmp/goastpy-0.1.8.tar.gz` & `tmp/goastpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.8.tar", last modified: Wed Apr 19 12:33:22 2023, max compression
+gzip compressed data, was "goastpy-0.1.9.tar", last modified: Wed Apr 19 13:13:18 2023, max compression
```

## Comparing `goastpy-0.1.8.tar` & `goastpy-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 12:33:09.000000 goastpy-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:33:22.370063 goastpy-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 12:33:09.000000 goastpy-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/goastpy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser.h
--rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser.so
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Darwin.h
--rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Linux.h
--rw-r--r--   0 runner    (1001) docker     (123)  2858760 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_Linux.so
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastparser_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 12:33:09.000000 goastpy-0.1.8/goastpy/goastpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/goastpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:33:22.000000 goastpy-0.1.8/goastpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 12:33:22.370063 goastpy-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 12:33:09.000000 goastpy-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:33:22.370063 goastpy-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 12:33:09.000000 goastpy-0.1.8/tests/test_go_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:13:18.896335 goastpy-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 13:13:07.000000 goastpy-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 13:13:18.896335 goastpy-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-19 13:13:07.000000 goastpy-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:13:18.896335 goastpy-0.1.9/goastpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser_Darwin.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2831794 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser_Darwin.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser_Linux.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2858760 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser_Linux.so
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastparser_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 13:13:07.000000 goastpy-0.1.9/goastpy/goastpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:13:18.896335 goastpy-0.1.9/goastpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 13:13:18.000000 goastpy-0.1.9/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 13:13:18.000000 goastpy-0.1.9/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:13:18.000000 goastpy-0.1.9/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 13:13:18.000000 goastpy-0.1.9/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 13:13:18.896335 goastpy-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-19 13:13:07.000000 goastpy-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:13:18.896335 goastpy-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 13:13:07.000000 goastpy-0.1.9/tests/test_go_parser.py
```

### Comparing `goastpy-0.1.8/LICENSE` & `goastpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser.h` & `goastpy-0.1.9/goastpy/goastparser.h`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser.so` & `goastpy-0.1.9/goastpy/goastparser.so`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser_Darwin.h` & `goastpy-0.1.9/goastpy/goastparser_Darwin.h`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser_Darwin.so` & `goastpy-0.1.9/goastpy/goastparser_Darwin.so`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser_Linux.h` & `goastpy-0.1.9/goastpy/goastparser_Linux.h`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser_Linux.so` & `goastpy-0.1.9/goastpy/goastparser_Linux.so`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastparser_wrapper.py` & `goastpy-0.1.9/goastpy/goastparser_wrapper.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/goastpy/goastpy.py` & `goastpy-0.1.9/goastpy/goastpy.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.8/setup.py` & `goastpy-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="goastpy",
-    version="0.1.8",
+    version="0.1.9",
     include_package_data=True,
     packages=find_packages(),
     package_dir={"": "."},
     package_data={"goastpy": ["*.h", "*.so"]},
     install_requires=[],
-    description='a python wrapper for the built-in go parser using c-types',
+    description='Python Wrapper for Go AST Parser',
     author='Itay Gersten',
     author_email='Itay.Gersten@gmail.com',
     url='https://github.com/itayg25/goastpy',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords=['GO', 'GOLANG', 'PYTHON', 'AST',
               'GOPY', 'PYGO', 'PARSER', 'ASTPARSER'],
```

