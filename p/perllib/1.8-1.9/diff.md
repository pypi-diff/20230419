# Comparing `tmp/perllib-1.8.tar.gz` & `tmp/perllib-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perllib-1.8.tar", last modified: Mon Oct 31 20:08:13 2022, max compression
+gzip compressed data, was "perllib-1.9.tar", last modified: Thu Nov  3 15:31:37 2022, max compression
```

## Comparing `perllib-1.8.tar` & `perllib-1.9.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.453791 perllib-1.8/
--rw-rw-rw-   0        0        0      165 2022-02-15 05:42:28.000000 perllib-1.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     4321 2022-08-16 20:21:59.000000 perllib-1.8/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.403692 perllib-1.8/Config/
--rw-rw-rw-   0        0        0      736 2022-10-27 00:58:34.000000 perllib-1.8/Config/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.403692 perllib-1.8/File/
--rw-rw-rw-   0        0        0    29233 2022-10-27 00:58:34.000000 perllib-1.8/File/Path.py
--rw-rw-rw-   0        0        0        0 2022-04-13 21:47:41.000000 perllib-1.8/File/__init__.py
--rw-rw-rw-   0        0        0     6725 2022-10-31 18:53:07.000000 perllib-1.8/HISTORY.rst
--rw-rw-rw-   0        0        0     8841 2022-02-15 05:48:09.000000 perllib-1.8/LICENSE
--rw-rw-rw-   0        0        0      273 2022-02-17 05:13:46.000000 perllib-1.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.403692 perllib-1.8/Math/
--rw-rw-rw-   0        0        0    60812 2022-10-27 00:58:34.000000 perllib-1.8/Math/Complex.py
--rw-rw-rw-   0        0        0        0 2022-03-30 04:31:19.000000 perllib-1.8/Math/__init__.py
--rw-rw-rw-   0        0        0     9099 2022-10-31 20:08:13.453791 perllib-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1586 2022-02-15 14:34:07.000000 perllib-1.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.403692 perllib-1.8/Sys/
--rw-rw-rw-   0        0        0     7611 2022-10-27 00:58:34.000000 perllib-1.8/Sys/Hostname.py
--rw-rw-rw-   0        0        0        0 2022-03-14 14:32:45.000000 perllib-1.8/Sys/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.403692 perllib-1.8/charnames/
--rw-rw-rw-   0        0        0     3491 2022-10-27 00:58:34.000000 perllib-1.8/charnames/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.437155 perllib-1.8/docs/
--rw-rw-rw-   0        0        0      151 2022-03-14 14:27:04.000000 perllib-1.8/docs/Config.rst
--rw-rw-rw-   0        0        0      298 2022-04-13 21:51:30.000000 perllib-1.8/docs/File.rst
--rw-rw-rw-   0        0        0      628 2022-02-15 05:42:29.000000 perllib-1.8/docs/Makefile
--rw-rw-rw-   0        0        0      304 2022-03-31 19:36:28.000000 perllib-1.8/docs/Math.rst
--rw-rw-rw-   0        0        0      301 2022-03-14 14:33:07.000000 perllib-1.8/docs/Sys.rst
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.387058 perllib-1.8/docs/_build/
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.387058 perllib-1.8/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.437155 perllib-1.8/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-09-04 15:44:39.000000 perllib-1.8/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-09-04 15:44:39.000000 perllib-1.8/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-09-04 15:44:39.000000 perllib-1.8/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2022-02-15 05:42:28.000000 perllib-1.8/docs/authors.rst
--rw-rw-rw-   0        0        0      160 2022-03-14 14:27:03.000000 perllib-1.8/docs/charnames.rst
--rw-rw-rw-   0        0        0     4928 2022-02-15 05:42:28.000000 perllib-1.8/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-02-15 05:42:28.000000 perllib-1.8/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-02-15 05:42:28.000000 perllib-1.8/docs/history.rst
--rw-rw-rw-   0        0        0      324 2022-02-15 05:42:28.000000 perllib-1.8/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2022-02-17 04:05:44.000000 perllib-1.8/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2022-02-15 05:42:29.000000 perllib-1.8/docs/make.bat
--rw-rw-rw-   0        0        0      373 2022-04-13 21:48:44.000000 perllib-1.8/docs/modules.rst
--rw-rw-rw-   0        0        0      154 2022-10-31 20:07:56.000000 perllib-1.8/docs/perllib.rst
--rw-rw-rw-   0        0        0       28 2022-02-15 05:42:29.000000 perllib-1.8/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2022-02-15 05:42:29.000000 perllib-1.8/docs/usage.rst
--rw-rw-rw-   0        0        0    10169 2022-01-14 23:59:45.000000 perllib-1.8/license.html
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.437155 perllib-1.8/perllib/
--rw-rw-rw-   0        0        0   119011 2022-10-31 18:56:35.000000 perllib-1.8/perllib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-31 20:08:13.452786 perllib-1.8/perllib.egg-info/
--rw-rw-rw-   0        0        0     9099 2022-10-31 20:08:13.000000 perllib-1.8/perllib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2022-10-31 20:08:13.000000 perllib-1.8/perllib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 20:08:13.000000 perllib-1.8/perllib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-31 20:08:13.000000 perllib-1.8/perllib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2022-10-31 20:08:13.000000 perllib-1.8/perllib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2022-10-31 20:08:13.453791 perllib-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1420 2022-10-27 00:58:34.000000 perllib-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.230850 perllib-1.9/
+-rw-rw-rw-   0        0        0      165 2022-02-15 05:42:28.000000 perllib-1.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     4321 2022-08-16 20:21:59.000000 perllib-1.9/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.180946 perllib-1.9/Config/
+-rw-rw-rw-   0        0        0      736 2022-10-31 21:11:50.000000 perllib-1.9/Config/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.180946 perllib-1.9/File/
+-rw-rw-rw-   0        0        0    29233 2022-10-31 21:11:50.000000 perllib-1.9/File/Path.py
+-rw-rw-rw-   0        0        0        0 2022-04-13 21:47:41.000000 perllib-1.9/File/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.180946 perllib-1.9/FindBin/
+-rw-rw-rw-   0        0        0     7284 2022-10-31 22:02:37.000000 perllib-1.9/FindBin/__init__.py
+-rw-rw-rw-   0        0        0     6836 2022-11-02 04:09:32.000000 perllib-1.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     8841 2022-02-15 05:48:09.000000 perllib-1.9/LICENSE
+-rw-rw-rw-   0        0        0      273 2022-02-17 05:13:46.000000 perllib-1.9/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.180946 perllib-1.9/Math/
+-rw-rw-rw-   0        0        0    60812 2022-10-31 21:11:50.000000 perllib-1.9/Math/Complex.py
+-rw-rw-rw-   0        0        0        0 2022-03-30 04:31:19.000000 perllib-1.9/Math/__init__.py
+-rw-rw-rw-   0        0        0     9262 2022-11-03 15:31:37.230850 perllib-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1586 2022-02-15 14:34:07.000000 perllib-1.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.180946 perllib-1.9/Sys/
+-rw-rw-rw-   0        0        0     7611 2022-10-31 21:11:50.000000 perllib-1.9/Sys/Hostname.py
+-rw-rw-rw-   0        0        0        0 2022-03-14 14:32:45.000000 perllib-1.9/Sys/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.196576 perllib-1.9/charnames/
+-rw-rw-rw-   0        0        0     3491 2022-10-31 21:11:50.000000 perllib-1.9/charnames/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.214215 perllib-1.9/docs/
+-rw-rw-rw-   0        0        0      151 2022-03-14 14:27:04.000000 perllib-1.9/docs/Config.rst
+-rw-rw-rw-   0        0        0      298 2022-04-13 21:51:30.000000 perllib-1.9/docs/File.rst
+-rw-rw-rw-   0        0        0      154 2022-11-03 15:28:56.000000 perllib-1.9/docs/FindBin.rst
+-rw-rw-rw-   0        0        0      628 2022-02-15 05:42:29.000000 perllib-1.9/docs/Makefile
+-rw-rw-rw-   0        0        0      304 2022-03-31 19:36:28.000000 perllib-1.9/docs/Math.rst
+-rw-rw-rw-   0        0        0      301 2022-03-14 14:33:07.000000 perllib-1.9/docs/Sys.rst
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.164313 perllib-1.9/docs/_build/
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.164313 perllib-1.9/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.214215 perllib-1.9/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-09-04 15:44:39.000000 perllib-1.9/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-09-04 15:44:39.000000 perllib-1.9/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-09-04 15:44:39.000000 perllib-1.9/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2022-02-15 05:42:28.000000 perllib-1.9/docs/authors.rst
+-rw-rw-rw-   0        0        0      160 2022-03-14 14:27:03.000000 perllib-1.9/docs/charnames.rst
+-rw-rw-rw-   0        0        0     4928 2022-02-15 05:42:28.000000 perllib-1.9/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-02-15 05:42:28.000000 perllib-1.9/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2022-02-15 05:42:28.000000 perllib-1.9/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2022-02-15 05:42:28.000000 perllib-1.9/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2022-02-17 04:05:44.000000 perllib-1.9/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2022-02-15 05:42:29.000000 perllib-1.9/docs/make.bat
+-rw-rw-rw-   0        0        0      440 2022-11-03 15:27:38.000000 perllib-1.9/docs/modules.rst
+-rw-rw-rw-   0        0        0      154 2022-11-03 15:29:04.000000 perllib-1.9/docs/perllib.rst
+-rw-rw-rw-   0        0        0       28 2022-02-15 05:42:29.000000 perllib-1.9/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2022-02-15 05:42:29.000000 perllib-1.9/docs/usage.rst
+-rw-rw-rw-   0        0        0    10169 2022-01-14 23:59:45.000000 perllib-1.9/license.html
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.214215 perllib-1.9/perllib/
+-rw-rw-rw-   0        0        0   123721 2022-11-03 14:55:12.000000 perllib-1.9/perllib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-03 15:31:37.230850 perllib-1.9/perllib.egg-info/
+-rw-rw-rw-   0        0        0     9262 2022-11-03 15:31:37.000000 perllib-1.9/perllib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2022-11-03 15:31:37.000000 perllib-1.9/perllib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-03 15:31:37.000000 perllib-1.9/perllib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-03 15:31:37.000000 perllib-1.9/perllib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2022-11-03 15:31:37.000000 perllib-1.9/perllib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2022-11-03 15:31:37.230850 perllib-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1482 2022-10-31 22:09:52.000000 perllib-1.9/setup.py
```

### Comparing `perllib-1.8/CONTRIBUTING.rst` & `perllib-1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `perllib-1.8/Config/__init__.py` & `perllib-1.9/Config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation of perl Config package"""
 
 __author__ = """Joe Cool"""
 ___email__ = 'snoopyjc@gmail.com'
-__version__ = '1.008'
+__version__ = '1.009'
 
 import perllib
 import subprocess
 import traceback
 perllib.init_package('Config')
 
 def config_sh():
```

### Comparing `perllib-1.8/File/Path.py` & `perllib-1.9/File/Path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # Generated by "pythonizer -aM -v3 -d5 Path.pm" v0.971 run by JO2742 on Thu Apr 14 15:50:18 2022
 """Implementation of perl File::Path package"""
 __author__ = """Joe Cool"""
 __email__ = "snoopyjc@gmail.com"
-__version__ = "1.008"
+__version__ = "1.009"
 import builtins, perllib, os, re
 
 _str = lambda s: "" if s is None else str(s)
 _locals_stack = []
 
 
 class LoopControl_ROOT_DIR(Exception):
```

### Comparing `perllib-1.8/HISTORY.rst` & `perllib-1.9/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+1.009 (2022-10-31)
+------------------
+
+* issue s128: Added _readlink, FindBin, issue s129: Added _switch
+
 1.008 (2022-10-26)
 ------------------
 
 * (no library changes)
 
 1.007 (2022-10-24)
 ------------------
```

### Comparing `perllib-1.8/LICENSE` & `perllib-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perllib-1.8/Math/Complex.py` & `perllib-1.9/Math/Complex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """Implementation of perl Math::Complex package"""
 
 __author__ = """Pythonizer"""
 ___email__ = 'snoopyjc@gmail.com'
-__version__ = '1.008'
+__version__ = '1.009'
 
 # Generated by "pythonizer -v3 -d5 ../Math/Complex.pm" v0.966 run by JO2742 on Tue Mar 29 17:57:14 2022
 #
 # Complex numbers and associated mathematical functions
 # -- Raphael Manfredi	Since Sep 1996
 # -- Jarkko Hietaniemi	Since Mar 1997
 # -- Daniel S. Lewart	Since Sep 1997
```

### Comparing `perllib-1.8/PKG-INFO` & `perllib-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: perllib
-Version: 1.8
+Version: 1.9
 Summary: Library functions to support pythonizer
 Home-page: https://github.com/snoopyjc/pythonizer
 Author: Joe Cool
 Author-email: snoopyjc@gmail.com
 License: Artistic License 2.0 - The Perl Foundation
 Keywords: perllib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Artistic License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: license.html
 License-File: AUTHORS.rst
 
 =======
 perllib
@@ -59,14 +60,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+1.009 (2022-10-31)
+------------------
+
+* issue s128: Added _readlink, FindBin, issue s129: Added _switch
+
 1.008 (2022-10-26)
 ------------------
 
 * (no library changes)
 
 1.007 (2022-10-24)
 ------------------
```

### Comparing `perllib-1.8/README.rst` & `perllib-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `perllib-1.8/Sys/Hostname.py` & `perllib-1.9/Sys/Hostname.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # Generated by "pythonizer -M -v 0 -s ./PyModules/Sys/Hostname.pm" v0.964 run by JO2742 on Sat Mar 12 16:24:25 2022
 # Edited by snoopyjc
 
 __author__ = """Joe Cool"""
 ___email__ = 'snoopyjc@gmail.com'
-__version__ = '1.008'
+__version__ = '1.009'
 
 import signal, re, perllib, builtins, os
 
 _str = lambda s: "" if s is None else str(s)
 _locals_stack = []
 perllib.init_package("Sys.Hostname")
```

### Comparing `perllib-1.8/charnames/__init__.py` & `perllib-1.9/charnames/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation of perl charnames functions"""
 
 __author__ = """Joe Cool"""
 ___email__ = 'snoopyjc@gmail.com'
-__version__ = '1.008'
+__version__ = '1.009'
 
 import perllib
 import unicodedata
 import re
 perllib.init_package('charnames')
 
 def string_vianame(name):
```

### Comparing `perllib-1.8/docs/Makefile` & `perllib-1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `perllib-1.8/docs/conf.py` & `perllib-1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `perllib-1.8/docs/installation.rst` & `perllib-1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `perllib-1.8/docs/make.bat` & `perllib-1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `perllib-1.8/license.html` & `perllib-1.9/license.html`

 * *Files identical despite different names*

### Comparing `perllib-1.8/perllib/__init__.py` & `perllib-1.9/perllib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# perllib module for pythonizer, generated by makelib.py on Mon Oct 31 14:56:35 2022
+# perllib module for pythonizer, generated by makelib.py on Thu Nov  3 10:55:12 2022
 #
 # WARNING: Do not edit this file - to change the functions or add new ones, edit them in the pyf directory,
 #          then re-run makelib.py
 #
 __author__ = """Joe Cool"""
 ___email__ = 'snoopyjc@gmail.com'
-__version__ = '1.008'
+__version__ = '1.009'
 
 import sys,os,re,fileinput,subprocess,collections.abc,warnings,inspect,itertools,signal,traceback,io,tempfile,calendar,types,random,dataclasses,builtins,codecs,struct,pprint,functools
 import time as tm_py
 import stat as st_py
 _str = lambda s: "" if s is None else str(s)
 try:
     import fcntl as fc_py
@@ -18,32 +18,32 @@
 
 class Die(Exception):
     def __init__(self, *args,suppress_traceback=None):
         super().__init__(*args)
         if TRACEBACK and not suppress_traceback:
             cluck()
 
-OS_ERROR = ''
-OUTPUT_LAYERS = ''
-INPUT_LAYERS = ''
-OUTPUT_FIELD_SEPARATOR = ''
+BASETIME = tm_py.time()
+WARNING = 0
+LIST_SEPARATOR = ' '
 INPUT_RECORD_SEPARATOR = "\n"
-_DUP_MAP = dict(STDIN=0, STDOUT=1, STDERR=2)
-TRACEBACK = 0
 OUTPUT_RECORD_SEPARATOR = ''
-_OPEN_MODE_MAP = {'<': 'r', '>': 'w', '+<': 'r+', '+>': 'w+', '>>': 'a', '+>>': 'a+', '|': '|-'}
 TRACE_RUN = 0
-AUTODIE = 0
-OUTPUT_AUTOFLUSH = 0
-LIST_SEPARATOR = ' '
 CHILD_ERROR = 0
-BASETIME = tm_py.time()
-WARNING = 0
+OUTPUT_AUTOFLUSH = 0
+_DUP_MAP = dict(STDIN=0, STDOUT=1, STDERR=2)
+OS_ERROR = ''
+OUTPUT_FIELD_SEPARATOR = ''
+AUTODIE = 0
 EVAL_ERROR = ''
 INPUT_LINE_NUMBER = 0
+INPUT_LAYERS = ''
+TRACEBACK = 0
+_OPEN_MODE_MAP = {'<': 'r', '>': 'w', '+<': 'r+', '+>': 'w+', '>>': 'a', '+>>': 'a+', '|': '|-'}
+OUTPUT_LAYERS = ''
 
 
 def init_package(name, is_class=False, isa=(), autovivification=True):
     """Initialize a package by creating a namespace for it"""
     pieces = name.split('.')
     parent = builtins
     parent_name = ''
@@ -2589,14 +2589,28 @@
         INPUT_LINE_NUMBER = fh._lno = 1
     else:
         fh._lno += 1
         INPUT_LINE_NUMBER = fh._lno
     return result
 
 
+def readlink(path):
+    """Returns the value of a symbolic link.  If there is a system error, returns the undefined value and sets OS_ERROR (errno)."""
+    global OS_ERROR, TRACEBACK, AUTODIE
+    try:
+        return os.readlink(path)
+    except Exception as _e:
+        OS_ERROR = str(_e)
+        if TRACEBACK:
+            cluck(f"readlink({path}) failed: {OS_ERROR}",skip=2)
+        if AUTODIE:
+            raise
+        return None
+
+
 def ref(r):
     """ref function in perl - called when NOT followed by a backslash"""
     _ref_map = {"<class 'int'>": 'SCALAR', "<class 'str'>": 'SCALAR',
                 "<class 'float'>": 'SCALAR', "<class 'NoneType'>": 'SCALAR',
                 "<class 'list'>": 'ARRAY', "<class 'tuple'>": 'ARRAY',
                 "<class 'dict'>": 'HASH'}
     tr = type(r)
@@ -3093,14 +3107,102 @@
     except TypeError:
         if isinstance(value, int) or isinstance(value, float):
             base[index] = num(base[index]) - value
         elif value is not None:
             raise
     return base[index]
 
+def switch(s_val):
+    """Implementation of switch/given statement in perl.  This
+    returns a function that is called for each case."""
+    def iter_to_bool(i):
+        try:
+            v = next(i)
+            return True
+        except StopIteration:
+            return False
+
+    if callable(s_val):
+        def f_switch(c_val):
+            if callable(c_val):
+                return s_val == c_val
+            if isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str):
+                return s_val(*c_val)
+            return s_val(c_val)
+        return f_switch
+    elif isinstance(s_val, int) or isinstance(s_val, float):
+        def n_switch(c_val):
+            if isinstance(c_val, int) or isinstance(c_val, float):
+                return s_val == c_val
+            if callable(c_val):
+                return c_val(s_val)
+            if isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str):
+                if hasattr(c_val, 'isHash') and c_val.isHash:
+                    return str(s_val) in c_val
+                return s_val in c_val
+            if isinstance(c_val, re.Pattern):
+                return re.search(c_val, str(s_val))
+            if isinstance(c_val, dict):
+                return str(s_val) in c_val
+            return str(s_val) == str(c_val)
+        return n_switch
+    elif isinstance(s_val, str):
+        def s_switch(c_val):
+            if (isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str)) or isinstance(c_val, dict):
+                return s_val in c_val       # list, Array, or Hash
+            if callable(c_val):
+                return c_val(s_val)
+            if isinstance(c_val, re.Pattern):
+                return re.search(c_val, s_val)
+            return s_val == str(c_val)
+        return s_switch
+    elif isinstance(s_val, dict) and (not hasattr(s_val, 'isHash') or s_val.isHash):
+        def h_switch(c_val):
+            if isinstance(c_val, dict) and (not hasattr(c_val, 'isHash') or c_val.isHash):
+                return s_val == c_val
+            if isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str):
+                return iter_to_bool(filter(lambda _d: _d in s_val and s_val[_d], c_val))
+            if callable(c_val):
+                return c_val(s_val)
+            if isinstance(c_val, re.Pattern):
+                return iter_to_bool(filter(lambda _d: re.search(c_val, _d) and _d in s_val and s_val[_d], s_val.keys()))
+            return str(c_val) in s_val and s_val[str(c_val)]
+        return h_switch
+    elif isinstance(s_val, collections.abc.Iterable) and (not hasattr(s_val, 'isHash') or not s_val.isHash):
+        def a_switch(c_val):
+            if isinstance(c_val, dict) and (not hasattr(c_val, 'isHash') or c_val.isHash):
+                return iter_to_bool(filter(lambda _d: str(_d) in c_val and c_val[str(_d)], s_val))
+            if isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str):
+                for item in s_val:
+                    if item not in c_val:
+                        return False
+                return True
+            if callable(c_val):
+                return c_val(*(map(str, s_val)))
+            if isinstance(c_val, re.Pattern):
+                return iter_to_bool(filter(lambda _d: re.search(c_val, _d), map(str, s_val)))
+            return c_val in s_val
+        return a_switch
+    elif isinstance(s_val, re.Pattern):
+        def r_switch(c_val):
+            if isinstance(c_val, dict) and (not hasattr(c_val, 'isHash') or c_val.isHash):
+                return iter_to_bool(filter(lambda _d: re.search(s_val, _d) and c_val[_d], c_val.keys()))
+            if isinstance(c_val, collections.abc.Iterable) and not isinstance(c_val, str):
+                return iter_to_bool(filter(lambda _d: re.search(s_val, _d), map(str, c_val)))
+            if callable(c_val):
+                return c_val(s_val)
+            if isinstance(c_val, re.Pattern):
+                return s_val.pattern == c_val.pattern
+            return re.search(s_val, str(c_val))
+        return r_switch
+    else:
+        def n_switch(c_val):
+            return False
+        return n_switch
+
 def sysread(fh, var, length, offset=0, need_len=False):
     """Read length bytes from the fh, and return the result to store in var
        if need_len is False, else return a tuple with the result
        and the length read"""
     global OS_ERROR, TRACEBACK, AUTODIE
     if var is None:
         var = ''
```

### Comparing `perllib-1.8/perllib.egg-info/PKG-INFO` & `perllib-1.9/perllib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: perllib
-Version: 1.8
+Version: 1.9
 Summary: Library functions to support pythonizer
 Home-page: https://github.com/snoopyjc/pythonizer
 Author: Joe Cool
 Author-email: snoopyjc@gmail.com
 License: Artistic License 2.0 - The Perl Foundation
 Keywords: perllib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Artistic License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: license.html
 License-File: AUTHORS.rst
 
 =======
 perllib
@@ -59,14 +60,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+1.009 (2022-10-31)
+------------------
+
+* issue s128: Added _readlink, FindBin, issue s129: Added _switch
+
 1.008 (2022-10-26)
 ------------------
 
 * (no library changes)
 
 1.007 (2022-10-24)
 ------------------
```

### Comparing `perllib-1.8/perllib.egg-info/SOURCES.txt` & `perllib-1.9/perllib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 README.rst
 license.html
 setup.cfg
 setup.py
 Config/__init__.py
 File/Path.py
 File/__init__.py
+FindBin/__init__.py
 Math/Complex.py
 Math/__init__.py
 Sys/Hostname.py
 Sys/__init__.py
 charnames/__init__.py
 docs/Config.rst
 docs/File.rst
+docs/FindBin.rst
 docs/Makefile
 docs/Math.rst
 docs/Sys.rst
 docs/authors.rst
 docs/charnames.rst
 docs/conf.py
 docs/contributing.rst
```

### Comparing `perllib-1.8/setup.py` & `perllib-1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,23 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Artistic License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="Library functions to support pythonizer",
     install_requires=requirements,
     license="Artistic License 2.0 - The Perl Foundation",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='perllib',
     name='perllib',
-    packages=find_packages(include=['perllib', 'perllib.*', 'charnames', 'Config', 'Sys', 'Sys.*', 'Math', 'Math.*', 'File', 'File.*']),
+    packages=find_packages(include=['perllib', 'perllib.*', 'charnames', 'Config', 'Sys', 'Sys.*', 'Math', 'Math.*', 'File', 'File.*', 'FindBin']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/snoopyjc/pythonizer',
-    version='1.008',
+    version='1.009',
     zip_safe=False,
 )
```

