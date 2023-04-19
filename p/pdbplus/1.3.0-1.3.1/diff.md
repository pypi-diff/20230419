# Comparing `tmp/pdbplus-1.3.0.tar.gz` & `tmp/pdbplus-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.3.0.tar", last modified: Wed Apr 19 05:36:42 2023, max compression
+gzip compressed data, was "pdbplus-1.3.1.tar", last modified: Wed Apr 19 18:42:35 2023, max compression
```

## Comparing `pdbplus-1.3.0.tar` & `pdbplus-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 05:36:42.337043 pdbplus-1.3.0/
--rw-r--r--   0 michael    (501) staff       (20)    10595 2023-04-19 05:36:42.336835 pdbplus-1.3.0/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     8642 2023-04-19 05:28:37.000000 pdbplus-1.3.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 05:36:42.336683 pdbplus-1.3.0/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    10595 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-19 05:36:42.337071 pdbplus-1.3.0/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-19 05:33:36.000000 pdbplus-1.3.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:42:35.956641 pdbplus-1.3.1/
+-rw-r--r--   0 michael    (501) staff       (20)    10435 2023-04-19 18:42:35.955914 pdbplus-1.3.1/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     8482 2023-04-19 18:41:19.000000 pdbplus-1.3.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:42:35.955773 pdbplus-1.3.1/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    10435 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-19 18:42:35.956681 pdbplus-1.3.1/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-19 18:41:50.000000 pdbplus-1.3.1/setup.py
```

### Comparing `pdbplus-1.3.0/PKG-INFO` & `pdbplus-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.3.0
+Version: 1.3.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -104,17 +104,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbplus-1.3.0/README.md` & `pdbplus-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbplus-1.3.0/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.3.1/pdbplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.3.0
+Version: 1.3.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -104,17 +104,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbplus-1.3.0/setup.py` & `pdbplus-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.3.0',
+    version='1.3.1',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -103,14 +103,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.3.0',
+        'pdbp>=1.3.1',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```

