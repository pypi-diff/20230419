# Comparing `tmp/fijiconvert-1.0.0.tar.gz` & `tmp/fijiconvert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fijiconvert-1.0.0.tar", last modified: Mon Apr 17 20:34:47 2023, max compression
+gzip compressed data, was "fijiconvert-1.0.1.tar", last modified: Wed Apr 19 15:31:44 2023, max compression
```

## Comparing `fijiconvert-1.0.0.tar` & `fijiconvert-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:47.928746 fijiconvert-1.0.0/
--rw-rw-rw-   0        0        0      409 2023-04-17 20:34:47.928746 fijiconvert-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-04-17 20:14:58.000000 fijiconvert-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:47.900370 fijiconvert-1.0.0/fijiconvert/
--rw-rw-rw-   0        0        0       23 2023-04-17 20:16:44.000000 fijiconvert-1.0.0/fijiconvert/__init__.py
--rw-rw-rw-   0        0        0      285 2023-03-28 15:28:28.000000 fijiconvert-1.0.0/fijiconvert/buildsetup.py
--rw-rw-rw-   0        0        0     9498 2023-04-17 20:30:04.000000 fijiconvert-1.0.0/fijiconvert/converter.py
--rw-rw-rw-   0        0        0      294 2023-04-17 20:29:38.000000 fijiconvert-1.0.0/fijiconvert/main.py
--rw-rw-rw-   0        0        0     1899 2023-03-28 15:28:28.000000 fijiconvert-1.0.0/fijiconvert/reader.py
--rw-rw-rw-   0        0        0     1412 2023-03-28 15:28:28.000000 fijiconvert-1.0.0/fijiconvert/setupcheckerr.py
--rw-rw-rw-   0        0        0     3261 2023-03-28 15:28:28.000000 fijiconvert-1.0.0/fijiconvert/tacchkdlg.py
--rw-rw-rw-   0        0        0    24180 2023-04-17 20:29:49.000000 fijiconvert-1.0.0/fijiconvert/ui_fijiconvertdialog.py
--rw-rw-rw-   0        0        0     5281 2023-03-28 15:28:28.000000 fijiconvert-1.0.0/fijiconvert/writer.py
--rw-rw-rw-   0        0        0    15104 2023-04-17 20:30:23.000000 fijiconvert-1.0.0/fijiconvert/xml_gui.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:47.920865 fijiconvert-1.0.0/fijiconvert.egg-info/
--rw-rw-rw-   0        0        0      409 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-17 20:34:47.000000 fijiconvert-1.0.0/fijiconvert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2022-12-22 18:55:48.000000 fijiconvert-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      584 2023-04-17 20:34:47.932741 fijiconvert-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-12-22 18:55:48.000000 fijiconvert-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/
+-rw-rw-rw-   0        0        0      399 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-04-17 20:14:58.000000 fijiconvert-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.368366 fijiconvert-1.0.1/fijiconvert/
+-rw-rw-rw-   0        0        0       23 2023-04-17 20:16:44.000000 fijiconvert-1.0.1/fijiconvert/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/buildsetup.py
+-rw-rw-rw-   0        0        0     9498 2023-04-17 20:30:04.000000 fijiconvert-1.0.1/fijiconvert/converter.py
+-rw-rw-rw-   0        0        0      294 2023-04-17 20:29:38.000000 fijiconvert-1.0.1/fijiconvert/main.py
+-rw-rw-rw-   0        0        0     1899 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/reader.py
+-rw-rw-rw-   0        0        0     1412 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/setupcheckerr.py
+-rw-rw-rw-   0        0        0     3261 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/tacchkdlg.py
+-rw-rw-rw-   0        0        0    24180 2023-04-17 20:29:49.000000 fijiconvert-1.0.1/fijiconvert/ui_fijiconvertdialog.py
+-rw-rw-rw-   0        0        0     5281 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/writer.py
+-rw-rw-rw-   0        0        0    15104 2023-04-17 20:30:23.000000 fijiconvert-1.0.1/fijiconvert/xml_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/fijiconvert.egg-info/
+-rw-rw-rw-   0        0        0      399 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2022-12-22 18:55:48.000000 fijiconvert-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      574 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-12-22 18:55:48.000000 fijiconvert-1.0.1/setup.py
```

### Comparing `fijiconvert-1.0.0/fijiconvert/converter.py` & `fijiconvert-1.0.1/fijiconvert/converter.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/reader.py` & `fijiconvert-1.0.1/fijiconvert/reader.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/setupcheckerr.py` & `fijiconvert-1.0.1/fijiconvert/setupcheckerr.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/tacchkdlg.py` & `fijiconvert-1.0.1/fijiconvert/tacchkdlg.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/ui_fijiconvertdialog.py` & `fijiconvert-1.0.1/fijiconvert/ui_fijiconvertdialog.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/writer.py` & `fijiconvert-1.0.1/fijiconvert/writer.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/fijiconvert/xml_gui.py` & `fijiconvert-1.0.1/fijiconvert/xml_gui.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.0/setup.cfg` & `fijiconvert-1.0.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 696a 6963 6f6e 7665 7274 0d0a   = fijiconvert..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 300d  version = 1.0.0.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 310d  version = 1.0.1.
 00000030: 0a61 7574 686f 7220 3d20 4a65 616e 2046  .author = Jean F
 00000040: 6563 7465 6175 0d0a 6175 7468 6f72 5f65  ecteau..author_e
 00000050: 6d61 696c 203d 206a 6665 6374 6561 7540  mail = jfecteau@
 00000060: 6d62 6662 696f 7363 6965 6e63 652e 636f  mbfbioscience.co
 00000070: 6d0d 0a75 726c 203d 2068 7474 7073 3a2f  m..url = https:/
 00000080: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
 00000090: 742f 6669 6a69 636f 6e76 6572 742f 0d0a  t/fijiconvert/..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 466f  description = Fo
-000000b0: 7220 6163 6365 7373 696e 6720 4d46 2b20  r accessing MF+ 
-000000c0: 636f 6d6d 616e 6420 6c69 6e65 2066 756e  command line fun
-000000d0: 6374 696f 6e61 6c69 7479 0d0a 6c6f 6e67  ctionality..long
-000000e0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000f0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000110: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000120: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a6b  text/markdown..k
-00000130: 6579 776f 7264 7320 3d20 7370 6172 632c  eywords = sparc,
-00000140: 206d 6266 2c20 6269 6f73 6369 656e 6365   mbf, bioscience
-00000150: 2c20 6669 6a69 2c20 786d 6c0d 0a0d 0a5b  , fiji, xml....[
-00000160: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000170: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-00000180: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000190: 332e 360d 0a70 795f 6d6f 6475 6c65 7320  3.6..py_modules 
-000001a0: 3d20 6669 6a69 636f 6e76 6572 740d 0a69  = fijiconvert..i
-000001b0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-000001c0: 3d20 0d0a 0950 7951 7435 0d0a 0d0a 5b6f  = ...PyQt5....[o
-000001d0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000001e0: 6e74 735d 0d0a 6775 695f 7363 7269 7074  nts]..gui_script
-000001f0: 7320 3d20 0d0a 0966 696a 6963 6f6e 7665  s = ...fijiconve
-00000200: 7274 203d 2066 696a 6963 6f6e 7665 7274  rt = fijiconvert
-00000210: 2e6d 6169 6e3a 6d61 696e 0d0a 0d0a 5b65  .main:main....[e
-00000220: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000230: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000240: 203d 2030 0d0a 0d0a                       = 0....
+000000b0: 7220 636f 6e76 6572 7469 6e67 2046 494a  r converting FIJ
+000000c0: 4920 6d61 726b 6572 7320 746f 2058 4d4c  I markers to XML
+000000d0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000f0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000120: 6f77 6e0d 0a6b 6579 776f 7264 7320 3d20  own..keywords = 
+00000130: 7370 6172 632c 206d 6266 2c20 6269 6f73  sparc, mbf, bios
+00000140: 6369 656e 6365 2c20 6669 6a69 2c20 786d  cience, fiji, xm
+00000150: 6c0d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  l....[options]..
+00000160: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000170: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000180: 7320 3d20 3e3d 332e 360d 0a70 795f 6d6f  s = >=3.6..py_mo
+00000190: 6475 6c65 7320 3d20 6669 6a69 636f 6e76  dules = fijiconv
+000001a0: 6572 740d 0a69 6e73 7461 6c6c 5f72 6571  ert..install_req
+000001b0: 7569 7265 7320 3d20 0d0a 0950 7951 7435  uires = ...PyQt5
+000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+000001d0: 7279 5f70 6f69 6e74 735d 0d0a 6775 695f  ry_points]..gui_
+000001e0: 7363 7269 7074 7320 3d20 0d0a 0966 696a  scripts = ...fij
+000001f0: 6963 6f6e 7665 7274 203d 2066 696a 6963  iconvert = fijic
+00000200: 6f6e 7665 7274 2e6d 6169 6e3a 6d61 696e  onvert.main:main
+00000210: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000220: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000230: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

