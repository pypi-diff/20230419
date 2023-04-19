# Comparing `tmp/hhcm_forest-1.1.5.tar.gz` & `tmp/hhcm_forest-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhcm_forest-1.1.5.tar", last modified: Tue Oct 25 12:09:42 2022, max compression
+gzip compressed data, was "hhcm_forest-1.1.6.tar", last modified: Wed Apr 19 12:35:16 2023, max compression
```

## Comparing `hhcm_forest-1.1.5.tar` & `hhcm_forest-1.1.6.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.613563 hhcm_forest-1.1.5/
--rw-rw-r--   0 root         (0) root         (0)     1073 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      134 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4760 2022-10-25 12:09:42.613563 hhcm_forest-1.1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4238 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/README.md
--rw-rw-r--   0 root         (0) root         (0)      111 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      774 2022-10-25 12:09:42.613563 hhcm_forest-1.1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      237 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/forest/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       54 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/forest/cmake_tools/
--rw-rw-r--   0 root         (0) root         (0)     1649 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/cmake_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1605 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/cmake_tools/_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/forest/cmake_tools/template/
--rw-rw-r--   0 root         (0) root         (0)      101 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/cmake_tools/template/find_package.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/forest/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8418 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/build_handler.py
--rw-rw-r--   0 root         (0) root         (0)      419 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/config_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4994 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/eval_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7930 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/fetch_handler.py
--rw-rw-r--   0 root         (0) root         (0)      206 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/forest_dirs.py
--rw-rw-r--   0 root         (0) root         (0)     8100 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/install.py
--rw-rw-r--   0 root         (0) root         (0)     3124 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/package.py
--rw-rw-r--   0 root         (0) root         (0)      923 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/print_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2521 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/proc_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/recipe.py
--rw-rw-r--   0 root         (0) root         (0)      683 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/setup.bash
--rw-rw-r--   0 root         (0) root         (0)     1842 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/common/sudo_refresh.py
--rw-rw-r--   0 root         (0) root         (0)       45 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/forest.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.609563 hhcm_forest-1.1.5/src/forest/git_tools/
--rw-rw-r--   0 root         (0) root         (0)     1975 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/git_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/git_tools/_impl.py
--rwxrwxr-x   0 root         (0) root         (0)     9830 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/src/forest/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.613563 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4760 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1011 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-25 12:09:42.000000 hhcm_forest-1.1.5/src/hhcm_forest.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 12:09:42.613563 hhcm_forest-1.1.5/test/
--rw-rw-r--   0 root         (0) root         (0)      703 2022-10-25 12:08:48.000000 hhcm_forest-1.1.5/test/test_run_bash_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/
+-rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4238 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/README.md
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)      787 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      237 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:15.997381 hhcm_forest-1.1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:15.997381 hhcm_forest-1.1.6/src/forest/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:15.997381 hhcm_forest-1.1.6/src/forest/cmake_tools/
+-rw-rw-r--   0 root         (0) root         (0)     1649 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/cmake_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1754 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/cmake_tools/_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:15.997381 hhcm_forest-1.1.6/src/forest/cmake_tools/template/
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/cmake_tools/template/find_package.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/src/forest/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8418 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/build_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      419 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/config_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4994 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/eval_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7930 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/fetch_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/forest_dirs.py
+-rw-rw-r--   0 root         (0) root         (0)     8100 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/install.py
+-rw-rw-r--   0 root         (0) root         (0)     3124 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/package.py
+-rw-rw-r--   0 root         (0) root         (0)     3027 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/parser.py
+-rw-rw-r--   0 root         (0) root         (0)      923 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/print_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3851 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/proc_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/recipe.py
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/setup.bash
+-rw-rw-r--   0 root         (0) root         (0)     1842 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/common/sudo_refresh.py
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/forest.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/src/forest/git_tools/
+-rw-rw-r--   0 root         (0) root         (0)     1975 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/git_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/git_tools/_impl.py
+-rwxrwxr-x   0 root         (0) root         (0)     9830 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/src/forest/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 12:35:15.000000 hhcm_forest-1.1.6/src/hhcm_forest.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:35:16.001381 hhcm_forest-1.1.6/test/
+-rw-rw-r--   0 root         (0) root         (0)      703 2023-04-19 12:34:07.000000 hhcm_forest-1.1.6/test/test_run_bash_tests.py
```

### Comparing `hhcm_forest-1.1.5/LICENSE` & `hhcm_forest-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/PKG-INFO` & `hhcm_forest-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm_forest
-Version: 1.1.5
+Version: 1.1.6
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.5/README.md` & `hhcm_forest-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/setup.cfg` & `hhcm_forest-1.1.6/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hhcm_forest
-version = 1.1.5
+version = 1.1.6
 author = Arturo Laurenzi
 author_email = arturo.laurenzi@iit.it
 description = A minimalistic tool to automate source code cloning and building
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://none
 project_urls = 
@@ -21,14 +21,15 @@
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
 	argcomplete
 	parse
 	pyyaml
 	psutil
+	progressbar
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	forest = forest.main:main
```

### Comparing `hhcm_forest-1.1.5/src/forest/cmake_tools/__init__.py` & `hhcm_forest-1.1.6/src/forest/cmake_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/cmake_tools/_impl.py` & `hhcm_forest-1.1.6/src/forest/cmake_tools/_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tempfile import TemporaryDirectory
 import os 
 
 from forest.common import proc_utils
+from forest.common.parser import update_progess_bar
 
 cmake_command = 'cmake'
 default_args = list()
 
 def _construct(self, srcdir, builddir):
     self.srcdir = srcdir
     self.builddir = builddir
@@ -30,15 +31,17 @@
 
     return _call_cmake(['--build', self.builddir, '--target', target, '--', '-j', jobs])
 
 
 def _call_cmake(args, cwd='.', print_on_error=True):
 
     args_str = list(map(str, args))
-    return proc_utils.call_process(args=[cmake_command] + args_str, cwd=cwd, print_on_error=print_on_error)
+    return proc_utils.call_process(args=[cmake_command] + args_str,
+                                                cwd=cwd, 
+                                                print_on_error=print_on_error)
 
 
 def _find_package(pkg_name: str):
         
     with TemporaryDirectory(prefix="foresttmp-") as tmpdir:
 
         # dir of current file
```

### Comparing `hhcm_forest-1.1.5/src/forest/common/build_handler.py` & `hhcm_forest-1.1.6/src/forest/common/build_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/eval_handler.py` & `hhcm_forest-1.1.6/src/forest/common/eval_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/fetch_handler.py` & `hhcm_forest-1.1.6/src/forest/common/fetch_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/install.py` & `hhcm_forest-1.1.6/src/forest/common/install.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/package.py` & `hhcm_forest-1.1.6/src/forest/common/package.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/print_utils.py` & `hhcm_forest-1.1.6/src/forest/common/print_utils.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/recipe.py` & `hhcm_forest-1.1.6/src/forest/common/recipe.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/setup.bash` & `hhcm_forest-1.1.6/src/forest/common/setup.bash`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/common/sudo_refresh.py` & `hhcm_forest-1.1.6/src/forest/common/sudo_refresh.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/git_tools/__init__.py` & `hhcm_forest-1.1.6/src/forest/git_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/forest/main.py` & `hhcm_forest-1.1.6/src/forest/main.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.5/src/hhcm_forest.egg-info/PKG-INFO` & `hhcm_forest-1.1.6/src/hhcm_forest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm-forest
-Version: 1.1.5
+Version: 1.1.6
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.5/src/hhcm_forest.egg-info/SOURCES.txt` & `hhcm_forest-1.1.6/src/hhcm_forest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/forest/common/build_handler.py
 src/forest/common/config_handler.py
 src/forest/common/eval_handler.py
 src/forest/common/fetch_handler.py
 src/forest/common/forest_dirs.py
 src/forest/common/install.py
 src/forest/common/package.py
+src/forest/common/parser.py
 src/forest/common/print_utils.py
 src/forest/common/proc_utils.py
 src/forest/common/recipe.py
 src/forest/common/setup.bash
 src/forest/common/sudo_refresh.py
 src/forest/git_tools/__init__.py
 src/forest/git_tools/_impl.py
```

### Comparing `hhcm_forest-1.1.5/test/test_run_bash_tests.py` & `hhcm_forest-1.1.6/test/test_run_bash_tests.py`

 * *Files identical despite different names*

