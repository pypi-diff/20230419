# Comparing `tmp/xlibs-0.0.3-py3-none-any.whl.zip` & `tmp/xlibs-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1527 bytes, number of entries: 6
+Zip file size: 1633 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-18 09:56 x/__init__.py
--rw-rw-rw-  2.0 fat      103 b- defN 23-Apr-18 09:43 x/_ver.py
--rw-rw-rw-  2.0 fat      198 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      422 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/RECORD
-6 files, 1111 bytes uncompressed, 765 bytes compressed:  31.1%
+-rw-rw-rw-  2.0 fat      210 b- defN 23-Apr-19 00:37 x/_ver.py
+-rw-rw-rw-  2.0 fat      292 b- defN 23-Apr-19 00:40 xlibs-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 00:40 xlibs-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-19 00:40 xlibs-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      422 b- defN 23-Apr-19 00:40 xlibs-0.0.4.dist-info/RECORD
+6 files, 1312 bytes uncompressed, 871 bytes compressed:  33.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: x/__init__.py
 Comment: 
 
 Filename: x/_ver.py
 Comment: 
 
-Filename: xlibs-0.0.3.dist-info/METADATA
+Filename: xlibs-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xlibs-0.0.3.dist-info/WHEEL
+Filename: xlibs-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xlibs-0.0.3.dist-info/top_level.txt
+Filename: xlibs-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xlibs-0.0.3.dist-info/RECORD
+Filename: xlibs-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## x/_ver.py

```diff
@@ -1,6 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from importlib.metadata import version
-__version__ = version('xlibs')
+import sys
+
+if sys.version_info >= (3, 8):
+    from importlib import metadata
+else:
+    import importlib_metadata as metadata
+    
+__version__ = metadata.version('xlibs')
```

