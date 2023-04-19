# Comparing `tmp/Geode_Conversion-5.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2269 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-13 12:40 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-13 12:40 geode_conversion/model.py
--rw-rw-rw-  2.0 fat     2048 b- defN 23-Apr-13 12:41 Geode_Conversion-5.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 12:41 Geode_Conversion-5.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-13 12:41 Geode_Conversion-5.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      499 b- defN 23-Apr-13 12:41 Geode_Conversion-5.0.0.dist-info/RECORD
-6 files, 2933 bytes uncompressed, 1357 bytes compressed:  53.7%
+Zip file size: 1210123 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-19 16:37 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-19 16:37 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  2396672 b- defN 23-Apr-19 16:38 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150528 b- defN 23-Apr-19 16:38 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2048 b- defN 23-Apr-19 16:38 Geode_Conversion-5.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-19 16:38 Geode_Conversion-5.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-19 16:38 Geode_Conversion-5.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      730 b- defN 23-Apr-19 16:38 Geode_Conversion-5.0.1.dist-info/RECORD
+8 files, 2550364 bytes uncompressed, 1208835 bytes compressed:  52.6%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: Geode_Conversion-5.0.0.dist-info/METADATA
+Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
-Filename: Geode_Conversion-5.0.0.dist-info/WHEEL
+Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.0.0.dist-info/top_level.txt
+Filename: Geode_Conversion-5.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.0.0.dist-info/RECORD
+Filename: Geode_Conversion-5.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Conversion-5.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Conversion-5.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Geode_Conversion-5.0.0.dist-info/METADATA` & `Geode_Conversion-5.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 5.0.0
+Version: 5.0.1
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.0 Summary: Conversion
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.1 Summary: Conversion
 module for Geode-solutions OpenGeode modules Home-page: https://github.com/
 Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0)
 Requires-Dist: opengeode-core (==14.*,>=14.0.0)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
```

