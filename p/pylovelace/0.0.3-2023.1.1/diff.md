# Comparing `tmp/pylovelace-0.0.3.zip` & `tmp/pylovelace-2023.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,11 @@
-Zip file size: 125544 bytes, number of entries: 21
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 17:03 pylovelace-0.0.3/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 17:03 pylovelace-0.0.3/source/
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/LICENSE
--rw-rw-rw-  2.0 fat     3179 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/PKG-INFO
--rw-rw-rw-  2.0 fat     2617 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/README.md
--rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/setup.cfg
--rw-rw-rw-  2.0 fat     1157 b- defN 23-Apr-18 17:02 pylovelace-0.0.3/setup.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       58 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat     3179 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      371 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-18 17:03 pylovelace-0.0.3/pylovelace.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 17:03 pylovelace-0.0.3/source/core/
--rw-rw-rw-  2.0 fat     3422 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/pylovelace.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 17:03 pylovelace-0.0.3/source/core/cryptography/
--rw-rw-rw-  2.0 fat      324 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/core/configuration.py
--rw-rw-rw-  2.0 fat   180224 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/core/lovelace.pyd
--rw-rw-rw-  2.0 fat      136 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/core/__init__.py
--rw-rw-rw-  2.0 fat    61952 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/core/cryptography/PFC256.pyd
--rw-rw-rw-  2.0 fat       82 b- defN 23-Apr-08 19:33 pylovelace-0.0.3/source/core/cryptography/__init__.py
-21 files, 291904 bytes uncompressed, 122334 bytes compressed:  58.1%
+Zip file size: 17984 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-19 00:09 pylovelace/__init__.py
+-rw-rw-rw-  2.0 fat     8097 b- defN 23-Apr-19 03:40 pylovelace/__main__.py
+-rw-rw-rw-  2.0 fat     4382 b- defN 23-Apr-19 03:40 pylovelace/protect.py
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1596 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/RECORD
+9 files, 50364 bytes uncompressed, 16678 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,64 +1,28 @@
-Filename: pylovelace-0.0.3/
+Filename: pylovelace/__init__.py
 Comment: 
 
-Filename: pylovelace-0.0.3/pylovelace.egg-info/
+Filename: pylovelace/__main__.py
 Comment: 
 
-Filename: pylovelace-0.0.3/source/
+Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-0.0.3/LICENSE
+Filename: pylovelace-2023.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-0.0.3/PKG-INFO
+Filename: pylovelace-2023.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-0.0.3/README.md
+Filename: pylovelace-2023.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-0.0.3/setup.cfg
+Filename: pylovelace-2023.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-0.0.3/setup.py
+Filename: pylovelace-2023.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-0.0.3/pylovelace.egg-info/dependency_links.txt
-Comment: 
-
-Filename: pylovelace-0.0.3/pylovelace.egg-info/entry_points.txt
-Comment: 
-
-Filename: pylovelace-0.0.3/pylovelace.egg-info/PKG-INFO
-Comment: 
-
-Filename: pylovelace-0.0.3/pylovelace.egg-info/SOURCES.txt
-Comment: 
-
-Filename: pylovelace-0.0.3/pylovelace.egg-info/top_level.txt
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/
-Comment: 
-
-Filename: pylovelace-0.0.3/source/pylovelace.py
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/cryptography/
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/configuration.py
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/lovelace.pyd
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/__init__.py
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/cryptography/PFC256.pyd
-Comment: 
-
-Filename: pylovelace-0.0.3/source/core/cryptography/__init__.py
+Filename: pylovelace-2023.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `pylovelace-0.0.3/LICENSE` & `pylovelace-2023.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

