# Comparing `tmp/xgridfit-3.2.8.tar.gz` & `tmp/xgridfit-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgridfit-3.2.8.tar", last modified: Fri Jan 13 22:34:03 2023, max compression
+gzip compressed data, was "xgridfit-3.2.9.tar", last modified: Sun Jan 15 21:58:54 2023, max compression
```

## Comparing `xgridfit-3.2.8.tar` & `xgridfit-3.2.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.795465 xgridfit-3.2.8/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11326 2022-02-15 21:27:56.000000 xgridfit-3.2.8/LICENSE.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      194 2022-11-13 00:11:12.000000 xgridfit-3.2.8/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-13 22:34:03.795324 xgridfit-3.2.8/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1201 2022-12-20 02:07:53.000000 xgridfit-3.2.8/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      647 2023-01-13 22:21:09.000000 xgridfit-3.2.8/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-13 22:34:03.795508 xgridfit-3.2.8/setup.cfg
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.783523 xgridfit-3.2.8/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.785200 xgridfit-3.2.8/src/xgridfit/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.788885 xgridfit-3.2.8/src/xgridfit/Schemas/
--rw-r--r--   0 peterbaker   (504) staff       (20)    18674 2022-05-10 00:34:15.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit-sh.rnc
--rw-r--r--   0 peterbaker   (504) staff       (20)    53112 2022-05-10 00:36:20.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit-sh.rng
--rw-r--r--   0 peterbaker   (504) staff       (20)    19791 2022-05-10 00:37:24.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.rnc
--rw-r--r--   0 peterbaker   (504) staff       (20)    52399 2022-05-10 00:38:33.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.rng
--rw-r--r--   0 peterbaker   (504) staff       (20)    67775 2022-02-22 18:45:54.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.xsd
--rw-r--r--   0 peterbaker   (504) staff       (20)      634 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xi.xsd
--rw-r--r--   0 peterbaker   (504) staff       (20)      520 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/Schemas/xml.xsd
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.794895 xgridfit-3.2.8/src/xgridfit/XSL/
--rw-r--r--   0 peterbaker   (504) staff       (20)    14150 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/arithmetic.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    12610 2022-05-10 00:19:09.000000 xgridfit-3.2.8/src/xgridfit/XSL/compact.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     6397 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/delta.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    13321 2022-05-10 00:16:13.000000 xgridfit-3.2.8/src/xgridfit/XSL/expand.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    10023 2022-02-19 04:54:24.000000 xgridfit-3.2.8/src/xgridfit/XSL/expressions.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     4225 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/flow.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    30297 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/func-predef.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    38781 2022-02-22 20:39:35.000000 xgridfit-3.2.8/src/xgridfit/XSL/function.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    49445 2022-05-14 11:42:12.000000 xgridfit-3.2.8/src/xgridfit/XSL/graphics.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3271 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/measure.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3286 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/messages.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     2922 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/misc.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    52891 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/move-els.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    22545 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/move-lib.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)   109795 2022-05-07 00:22:27.000000 xgridfit-3.2.8/src/xgridfit/XSL/numbers.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    54518 2022-10-27 22:28:02.000000 xgridfit-3.2.8/src/xgridfit/XSL/points.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    13472 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/prep.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    11443 2022-02-15 21:27:56.000000 xgridfit-3.2.8/src/xgridfit/XSL/primitives.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3041 2023-01-13 22:23:16.000000 xgridfit-3.2.8/src/xgridfit/XSL/std-vars.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    15661 2022-03-01 10:36:15.000000 xgridfit-3.2.8/src/xgridfit/XSL/xgfdata.xml
--rw-r--r--   0 peterbaker   (504) staff       (20)    22383 2022-10-28 03:23:36.000000 xgridfit-3.2.8/src/xgridfit/XSL/xgridfit-ft.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)      494 2022-11-09 05:09:18.000000 xgridfit-3.2.8/src/xgridfit/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       22 2023-01-13 22:21:57.000000 xgridfit-3.2.8/src/xgridfit/version.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    43925 2023-01-13 22:29:40.000000 xgridfit-3.2.8/src/xgridfit/xgridfit.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    17067 2022-12-31 00:16:25.000000 xgridfit-3.2.8/src/xgridfit/ygridfit.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-13 22:34:03.786232 xgridfit-3.2.8/src/xgridfit.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1218 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       52 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       61 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        9 2023-01-13 22:34:03.000000 xgridfit-3.2.8/src/xgridfit.egg-info/top_level.txt
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.490590 xgridfit-3.2.9/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11326 2022-02-15 21:27:56.000000 xgridfit-3.2.9/LICENSE.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      194 2022-11-13 00:11:12.000000 xgridfit-3.2.9/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-15 21:58:54.490454 xgridfit-3.2.9/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1201 2022-12-20 02:07:53.000000 xgridfit-3.2.9/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      647 2023-01-15 21:57:10.000000 xgridfit-3.2.9/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-15 21:58:54.490625 xgridfit-3.2.9/setup.cfg
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.476892 xgridfit-3.2.9/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.479380 xgridfit-3.2.9/src/xgridfit/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.483377 xgridfit-3.2.9/src/xgridfit/Schemas/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    18674 2022-05-10 00:34:15.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rnc
+-rw-r--r--   0 peterbaker   (504) staff       (20)    53112 2022-05-10 00:36:20.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rng
+-rw-r--r--   0 peterbaker   (504) staff       (20)    19791 2022-05-10 00:37:24.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rnc
+-rw-r--r--   0 peterbaker   (504) staff       (20)    52399 2022-05-10 00:38:33.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rng
+-rw-r--r--   0 peterbaker   (504) staff       (20)    67775 2022-02-22 18:45:54.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.xsd
+-rw-r--r--   0 peterbaker   (504) staff       (20)      634 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xi.xsd
+-rw-r--r--   0 peterbaker   (504) staff       (20)      520 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xml.xsd
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.490065 xgridfit-3.2.9/src/xgridfit/XSL/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    14150 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/arithmetic.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12610 2022-05-10 00:19:09.000000 xgridfit-3.2.9/src/xgridfit/XSL/compact.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6397 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/delta.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13321 2022-05-10 00:16:13.000000 xgridfit-3.2.9/src/xgridfit/XSL/expand.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10023 2022-02-19 04:54:24.000000 xgridfit-3.2.9/src/xgridfit/XSL/expressions.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4225 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/flow.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    30297 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/func-predef.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    38781 2022-02-22 20:39:35.000000 xgridfit-3.2.9/src/xgridfit/XSL/function.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    49445 2022-05-14 11:42:12.000000 xgridfit-3.2.9/src/xgridfit/XSL/graphics.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3271 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/measure.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3286 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/messages.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2922 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/misc.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    52891 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/move-els.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22545 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/move-lib.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)   109795 2022-05-07 00:22:27.000000 xgridfit-3.2.9/src/xgridfit/XSL/numbers.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    54518 2022-10-27 22:28:02.000000 xgridfit-3.2.9/src/xgridfit/XSL/points.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13472 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/prep.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11443 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/primitives.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3041 2023-01-15 21:57:51.000000 xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15661 2022-03-01 10:36:15.000000 xgridfit-3.2.9/src/xgridfit/XSL/xgfdata.xml
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22383 2022-10-28 03:23:36.000000 xgridfit-3.2.9/src/xgridfit/XSL/xgridfit-ft.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)      494 2022-11-09 05:09:18.000000 xgridfit-3.2.9/src/xgridfit/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       22 2023-01-15 21:57:30.000000 xgridfit-3.2.9/src/xgridfit/version.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    43941 2023-01-15 04:58:44.000000 xgridfit-3.2.9/src/xgridfit/xgridfit.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    17067 2022-12-31 00:16:25.000000 xgridfit-3.2.9/src/xgridfit/ygridfit.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.480623 xgridfit-3.2.9/src/xgridfit.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1218 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       52 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       61 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        9 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/top_level.txt
```

### Comparing `xgridfit-3.2.8/LICENSE.txt` & `xgridfit-3.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/PKG-INFO` & `xgridfit-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgridfit
-Version: 3.2.8
+Version: 3.2.9
 Summary: An XML-based hinting language for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xgridfit-3.2.8/README.md` & `xgridfit-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/pyproject.toml` & `xgridfit-3.2.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xgridfit"
-version = "3.2.8"
+version = "3.2.9"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "An XML-based hinting language for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit-sh.rnc` & `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rnc`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit-sh.rng` & `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rng`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.rnc` & `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rnc`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.rng` & `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rng`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xgridfit.xsd` & `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xi.xsd` & `xgridfit-3.2.9/src/xgridfit/Schemas/xi.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/Schemas/xml.xsd` & `xgridfit-3.2.9/src/xgridfit/Schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/arithmetic.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/arithmetic.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/compact.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/compact.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/delta.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/delta.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/expand.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/expand.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/expressions.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/expressions.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/flow.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/flow.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/func-predef.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/func-predef.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/function.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/function.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/graphics.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/graphics.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/measure.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/measure.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/messages.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/messages.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/misc.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/misc.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/move-els.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/move-els.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/move-lib.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/move-lib.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/numbers.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/numbers.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/points.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/points.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/prep.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/prep.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/primitives.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/primitives.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/std-vars.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl`

 * *Files 0% similar despite different names*

#### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/std-vars.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform" xmlns:xgf="http://xgridfit.sourceforge.net/Xgridfit2" version="1.0" exclude-result-prefixes="xgf">
   <!--
       This file is part of xgridfit, version 3.
       Licensed under the Apache License, Version 2.0.
       Copyright (c) 2006-20 by Peter S. Baker
   -->
-  <xsl:variable name="xgf-version" select="'3.2.8'"/>
+  <xsl:variable name="xgf-version" select="'3.2.9'"/>
   <!--
       First in the Storage Area is a block of locations used by legacy
       code (e.g. from ttfautohint). Next come some
       reserved locations used by Xgridfit to track state
       information. Next is the global variable area and finally a
       growable variable frame area.
   -->
```

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/xgfdata.xml` & `xgridfit-3.2.9/src/xgridfit/XSL/xgfdata.xml`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/XSL/xgridfit-ft.xsl` & `xgridfit-3.2.9/src/xgridfit/XSL/xgridfit-ft.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit/xgridfit.py` & `xgridfit-3.2.9/src/xgridfit/xgridfit.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,15 +651,15 @@
             for entry in etransform.error_log:
                 print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
             failed_glyph_list.append(g)
     try:
         # New procedure: grab the font, subset it with just the one glyph we're
         # previewing, and write it to a spooled temporary file.
         tf = SpooledTemporaryFile(max_size=1000000, mode='b')
-        options = subset.Options()
+        options = subset.Options(glyph_names=True)
         options.layout_features = []
         subsetter = subset.Subsetter(options)
         subsetter.populate(glyphs=glyph_list)
         subsetter.subset(thisFont)
         glyph_id = {}
         for g in glyph_list:
             glyph_id[g] = thisFont.getGlyphID(g)
```

### Comparing `xgridfit-3.2.8/src/xgridfit/ygridfit.py` & `xgridfit-3.2.9/src/xgridfit/ygridfit.py`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.8/src/xgridfit.egg-info/PKG-INFO` & `xgridfit-3.2.9/src/xgridfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgridfit
-Version: 3.2.8
+Version: 3.2.9
 Summary: An XML-based hinting language for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xgridfit-3.2.8/src/xgridfit.egg-info/SOURCES.txt` & `xgridfit-3.2.9/src/xgridfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

