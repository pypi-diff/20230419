# Comparing `tmp/dvis-0.8.7.2-py3-none-any.whl.zip` & `tmp/dvis-0.8.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18349 bytes, number of entries: 11
+Zip file size: 18348 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx       35 b- defN 22-Aug-10 15:03 dvis/__init__.py
 -rw-rw-r--  2.0 unx    38101 b- defN 23-Jan-02 11:02 dvis/dvis.py
 -rw-rw-r--  2.0 unx     1525 b- defN 23-Jan-04 10:29 dvis/dvis_cli.py
 -rw-rw-r--  2.0 unx     8263 b- defN 23-Jan-02 10:43 dvis/dvis_client.py
 -rw-rw-r--  2.0 unx     6060 b- defN 22-Aug-10 15:03 dvis/dvis_client_old.py
 -rw-rw-r--  2.0 unx     5519 b- defN 23-Feb-23 09:32 dvis/utils.py
--rw-rw-r--  2.0 unx     4228 b- defN 23-Mar-08 18:46 dvis-0.8.7.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-08 18:46 dvis-0.8.7.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-08 18:46 dvis-0.8.7.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Mar-08 18:46 dvis-0.8.7.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Mar-08 18:46 dvis-0.8.7.2.dist-info/RECORD
-11 files, 64747 bytes uncompressed, 16967 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx     4228 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/RECORD
+11 files, 64747 bytes uncompressed, 16966 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: dvis/dvis_client_old.py
 Comment: 
 
 Filename: dvis/utils.py
 Comment: 
 
-Filename: dvis-0.8.7.2.dist-info/METADATA
+Filename: dvis-0.8.7.3.dist-info/METADATA
 Comment: 
 
-Filename: dvis-0.8.7.2.dist-info/WHEEL
+Filename: dvis-0.8.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: dvis-0.8.7.2.dist-info/entry_points.txt
+Filename: dvis-0.8.7.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: dvis-0.8.7.2.dist-info/top_level.txt
+Filename: dvis-0.8.7.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dvis-0.8.7.2.dist-info/RECORD
+Filename: dvis-0.8.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dvis-0.8.7.2.dist-info/METADATA` & `dvis-0.8.7.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvis
-Version: 0.8.7.2
+Version: 0.8.7.3
 Summary: The best web-based visualizer
 Home-page: https://github.com/SirWyver/dvis
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `dvis-0.8.7.2.dist-info/RECORD` & `dvis-0.8.7.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dvis/__init__.py,sha256=bfwoJN9nz_CchjmbhA9LJ0RKF1sHsInHrU4y79KfKpg,35
 dvis/dvis.py,sha256=C_yURtfDco7HbU-fUU7Cbe9B4oj-RcWd0TiISLhFHdo,38101
 dvis/dvis_cli.py,sha256=ON6Hgf4fZLldr2kRYlcDszVr5aONASkJOv3fhW_B5cE,1525
 dvis/dvis_client.py,sha256=IuyqDe6B2K0pc9gJv0zCH3xUBKGuJTnPZRrJlFmmv-w,8263
 dvis/dvis_client_old.py,sha256=kJCMvv9fMB0o2xT1rXeFknTlYwxVipsmtR4XZD6jgHM,6060
 dvis/utils.py,sha256=s2q78zNtycRXMCSyk14_iALqUAnRoX6BvamKuIuVJMQ,5519
-dvis-0.8.7.2.dist-info/METADATA,sha256=tkJLdD0_OXOy5k0QX_CaSTJ1o6MlfGMFAI1LAxl6TF4,4228
-dvis-0.8.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dvis-0.8.7.2.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
-dvis-0.8.7.2.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
-dvis-0.8.7.2.dist-info/RECORD,,
+dvis-0.8.7.3.dist-info/METADATA,sha256=DxSCFJr_JLPhE62RndkVztxG4dI9cEbcAl3jMurqa7s,4228
+dvis-0.8.7.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dvis-0.8.7.3.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
+dvis-0.8.7.3.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
+dvis-0.8.7.3.dist-info/RECORD,,
```

