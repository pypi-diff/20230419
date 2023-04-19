# Comparing `tmp/actipy-2.0.3.tar.gz` & `tmp/actipy-2.0.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-2.0.3.tar", last modified: Tue Mar 21 20:43:56 2023, max compression
+gzip compressed data, was "actipy-2.0.3.post0.tar", last modified: Wed Apr 19 17:25:20 2023, max compression
```

## Comparing `actipy-2.0.3.tar` & `actipy-2.0.3.post0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-x---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:43:56.892965 actipy-2.0.3/
--rw-r-----   0 vtx027   (37039) doherty  (30011)     6177 2022-09-30 04:04:48.000000 actipy-2.0.3/LICENSE.md
--rw-r--r--   0 vtx027   (37039) doherty  (30011)       71 2022-07-19 08:25:58.000000 actipy-2.0.3/MANIFEST.in
--rw-r-----   0 vtx027   (37039) doherty  (30011)     3347 2023-03-21 20:43:56.891965 actipy-2.0.3/PKG-INFO
--rw-r-----   0 vtx027   (37039) doherty  (30011)     2788 2022-12-17 06:52:20.000000 actipy-2.0.3/README.md
-drwxr-x---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:43:56.885965 actipy-2.0.3/actipy/
--rw-r-----   0 vtx027   (37039) doherty  (30011)    11487 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy/ActigraphReader.class
--rw-r-----   0 vtx027   (37039) doherty  (30011)    30928 2023-02-15 13:19:08.000000 actipy-2.0.3/actipy/ActigraphReader.java
--rw-r-----   0 vtx027   (37039) doherty  (30011)     7013 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy/AxivityReader.class
--rw-r-----   0 vtx027   (37039) doherty  (30011)    11228 2023-02-15 13:19:08.000000 actipy-2.0.3/actipy/AxivityReader.java
--rw-r-----   0 vtx027   (37039) doherty  (30011)     5980 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy/GENEActivReader.class
--rw-r-----   0 vtx027   (37039) doherty  (30011)     9656 2023-02-15 13:19:08.000000 actipy-2.0.3/actipy/GENEActivReader.java
--rw-r-----   0 vtx027   (37039) doherty  (30011)     8445 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy/NpyWriter.class
--rw-r--r--   0 vtx027   (37039) doherty  (30011)     7615 2022-07-19 08:25:56.000000 actipy-2.0.3/actipy/NpyWriter.java
--rw-r-----   0 vtx027   (37039) doherty  (30011)      226 2023-03-21 20:43:36.000000 actipy-2.0.3/actipy/__init__.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)    14774 2023-03-21 20:40:14.000000 actipy-2.0.3/actipy/processing.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)    12454 2023-02-17 15:50:19.000000 actipy-2.0.3/actipy/reader.py
-drwxr-x---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:43:56.890965 actipy-2.0.3/actipy.egg-info/
--rw-r-----   0 vtx027   (37039) doherty  (30011)     3347 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy.egg-info/PKG-INFO
--rw-r-----   0 vtx027   (37039) doherty  (30011)      459 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy.egg-info/SOURCES.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)        1 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy.egg-info/dependency_links.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)      210 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy.egg-info/requires.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)        7 2023-03-21 20:43:56.000000 actipy-2.0.3/actipy.egg-info/top_level.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)       38 2023-03-21 20:43:56.892965 actipy-2.0.3/setup.cfg
--rw-r-----   0 vtx027   (37039) doherty  (30011)     1782 2022-10-01 05:46:26.000000 actipy-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.731829 actipy-2.0.3.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/versioneer.py
```

### Comparing `actipy-2.0.3/LICENSE.md` & `actipy-2.0.3.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/PKG-INFO` & `actipy-2.0.3.post0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: actipy
-Version: 2.0.3
-Summary: Python package to process wearable accelerometer data
-Home-page: https://github.com/activityMonitoring/actipy
-Author: Shing Chan, Aiden Doherty
-Author-email: shing.chan@ndph.ox.ac.uk, aiden.doherty@ndph.ox.ac.uk
-License: See LICENSE.md
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
 # actipy
 
 A Python package to process accelerometer data.
 
 Axivity3 (`.cwa`), Actigraph (`.gt3x`), and GENEActiv (`.bin`) files are supported,
 as well as custom CSV files.
```

### Comparing `actipy-2.0.3/actipy/ActigraphReader.class` & `actipy-2.0.3.post0/src/actipy/ActigraphReader.class`

 * *Files 9% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,156 +1,156 @@
-  SHA-256 checksum 702be00b57dec25840895191a4eb78d311599cf6648f3bf6db1e67adafb7c4c3
+  SHA-256 checksum df41148f264ca4f3f77b03db4289635abc6080c55c5daf6c5fd1a0a03df12d52
   Compiled from "ActigraphReader.java"
 public class ActigraphReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #36                         // ActigraphReader
   super_class: #152                       // java/lang/Object
   interfaces: 0, fields: 5, methods: 20, attributes: 1
 Constant pool:
-    #1 = Methodref          #152.#221     // java/lang/Object."<init>":()V
-    #2 = Methodref          #36.#222      // ActigraphReader.read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
-    #3 = Class              #223          // java/util/HashMap
-    #4 = Methodref          #3.#221       // java/util/HashMap."<init>":()V
+    #1 = Methodref          #152.#227     // java/lang/Object."<init>":()V
+    #2 = Methodref          #36.#228      // ActigraphReader.read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
+    #3 = Class              #229          // java/util/HashMap
+    #4 = Methodref          #3.#227       // java/util/HashMap."<init>":()V
     #5 = Double             -1.0d
-    #7 = Class              #224          // NpyWriter
-    #8 = Fieldref           #36.#225      // ActigraphReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-    #9 = Methodref          #7.#226       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
-   #10 = Class              #227          // java/util/zip/ZipFile
-   #11 = Class              #228          // java/io/File
-   #12 = Methodref          #11.#229      // java/io/File."<init>":(Ljava/lang/String;)V
-   #13 = Methodref          #10.#230      // java/util/zip/ZipFile."<init>":(Ljava/io/File;I)V
-   #14 = Methodref          #36.#231      // ActigraphReader.getGT3XVersion:(Ljava/util/zip/ZipFile;)I
-   #15 = Fieldref           #232.#233     // java/lang/System.err:Ljava/io/PrintStream;
-   #16 = Class              #234          // java/lang/StringBuilder
-   #17 = Methodref          #16.#221      // java/lang/StringBuilder."<init>":()V
-   #18 = String             #235          // file
-   #19 = Methodref          #16.#236      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #20 = String             #237          //  is not a valid V1 or V2 g3tx file
-   #21 = Methodref          #16.#238      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #22 = Methodref          #239.#240     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #23 = Methodref          #10.#241      // java/util/zip/ZipFile.entries:()Ljava/util/Enumeration;
-   #24 = InterfaceMethodref #179.#242     // java/util/Enumeration.hasMoreElements:()Z
-   #25 = InterfaceMethodref #179.#243     // java/util/Enumeration.nextElement:()Ljava/lang/Object;
-   #26 = Class              #244          // java/util/zip/ZipEntry
-   #27 = Methodref          #26.#238      // java/util/zip/ZipEntry.toString:()Ljava/lang/String;
-   #28 = String             #245          // info.txt
-   #29 = Methodref          #176.#246     // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #30 = Class              #247          // java/io/BufferedReader
-   #31 = Class              #248          // java/io/InputStreamReader
-   #32 = Methodref          #10.#249      // java/util/zip/ZipFile.getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-   #33 = Methodref          #31.#250      // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
-   #34 = Methodref          #30.#251      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
-   #35 = String             #252          // activity.bin
-   #36 = Class              #253          // ActigraphReader
-   #37 = String             #254          // log.bin
+    #7 = Class              #230          // NpyWriter
+    #8 = Fieldref           #36.#231      // ActigraphReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+    #9 = Methodref          #7.#232       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
+   #10 = Class              #233          // java/util/zip/ZipFile
+   #11 = Class              #234          // java/io/File
+   #12 = Methodref          #11.#235      // java/io/File."<init>":(Ljava/lang/String;)V
+   #13 = Methodref          #10.#236      // java/util/zip/ZipFile."<init>":(Ljava/io/File;I)V
+   #14 = Methodref          #36.#237      // ActigraphReader.getGT3XVersion:(Ljava/util/zip/ZipFile;)I
+   #15 = Fieldref           #238.#239     // java/lang/System.err:Ljava/io/PrintStream;
+   #16 = Class              #240          // java/lang/StringBuilder
+   #17 = Methodref          #16.#227      // java/lang/StringBuilder."<init>":()V
+   #18 = String             #241          // file
+   #19 = Methodref          #16.#242      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #20 = String             #243          //  is not a valid V1 or V2 g3tx file
+   #21 = Methodref          #16.#244      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #22 = Methodref          #245.#246     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #23 = Methodref          #10.#247      // java/util/zip/ZipFile.entries:()Ljava/util/Enumeration;
+   #24 = InterfaceMethodref #248.#249     // java/util/Enumeration.hasMoreElements:()Z
+   #25 = InterfaceMethodref #248.#250     // java/util/Enumeration.nextElement:()Ljava/lang/Object;
+   #26 = Class              #251          // java/util/zip/ZipEntry
+   #27 = Methodref          #26.#244      // java/util/zip/ZipEntry.toString:()Ljava/lang/String;
+   #28 = String             #252          // info.txt
+   #29 = Methodref          #253.#254     // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #30 = Class              #255          // java/io/BufferedReader
+   #31 = Class              #256          // java/io/InputStreamReader
+   #32 = Methodref          #10.#257      // java/util/zip/ZipFile.getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+   #33 = Methodref          #31.#258      // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
+   #34 = Methodref          #30.#259      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
+   #35 = String             #260          // activity.bin
+   #36 = Class              #261          // ActigraphReader
+   #37 = String             #262          // log.bin
    #38 = Long               -1l
-   #40 = String             #255          //
-   #41 = String             #256          // 00:00:00
-   #42 = Methodref          #30.#257      // java/io/BufferedReader.ready:()Z
-   #43 = Methodref          #30.#258      // java/io/BufferedReader.readLine:()Ljava/lang/String;
-   #44 = String             #259          // :
-   #45 = Methodref          #176.#260     // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #46 = Methodref          #176.#261     // java/lang/String.trim:()Ljava/lang/String;
-   #47 = String             #262          // Sample Rate
-   #48 = Methodref          #119.#263     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
-   #49 = String             #264          // Start Date
-   #50 = Methodref          #265.#266     // java/lang/Long.parseLong:(Ljava/lang/String;)J
-   #51 = Methodref          #36.#267      // ActigraphReader.GT3XfromTickToMillisecond:(J)J
-   #52 = String             #268          // Acceleration Scale
-   #53 = Methodref          #269.#270     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #54 = String             #271          // Acceleration Min
-   #55 = String             #272          // Acceleration Max
-   #56 = String             #273          // Stop Date
-   #57 = String             #274          // Serial Number
-   #58 = String             #275          // TimeZone
-   #59 = Methodref          #36.#276      // ActigraphReader.setAccelerationScale:(Ljava/lang/String;)D
-   #60 = String             #277          // Error parsing
-   #61 = String             #278          // , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
-   #62 = Methodref          #36.#279      // ActigraphReader.setSampleDelta:(D)D
-   #63 = Methodref          #36.#280      // ActigraphReader.readG3TXv1Pairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
-   #64 = Methodref          #36.#281      // ActigraphReader.readG3TXv2:(Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
-   #65 = Methodref          #10.#282      // java/util/zip/ZipFile.close:()V
-   #66 = Methodref          #178.#282     // java/io/InputStream.close:()V
-   #67 = Methodref          #30.#282      // java/io/BufferedReader.close:()V
-   #68 = Methodref          #7.#282       // NpyWriter.close:()V
-   #69 = Class              #283          // java/lang/Exception
-   #70 = Methodref          #69.#284      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-   #71 = Class              #285          // java/io/IOException
-   #72 = Methodref          #71.#284      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
-   #73 = String             #286          // Error reading/writing file
-   #74 = Methodref          #71.#238      // java/io/IOException.toString:()Ljava/lang/String;
-   #75 = String             #287          // ReadOK
-   #76 = Methodref          #176.#288     // java/lang/String.valueOf:(I)Ljava/lang/String;
-   #77 = InterfaceMethodref #177.#289     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-   #78 = String             #290          // ReadErrors
-   #79 = String             #291          // SampleRate
-   #80 = Methodref          #176.#292     // java/lang/String.valueOf:(D)Ljava/lang/String;
-   #81 = Methodref          #178.#293     // java/io/InputStream.read:()I
-   #82 = Methodref          #36.#294      // ActigraphReader.isPayload:(III)Z
-   #83 = Methodref          #36.#295      // ActigraphReader.isAccelScale:([B)Z
-   #84 = Methodref          #36.#296      // ActigraphReader.decodePara:(I)D
-   #85 = Methodref          #36.#297      // ActigraphReader.processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
-   #86 = Methodref          #36.#298      // ActigraphReader.processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
-   #87 = Methodref          #36.#299      // ActigraphReader.checkChecksum:(IIIIJII)V
-   #88 = Methodref          #36.#300      // ActigraphReader.readAccelPair:([BD)[D
+   #40 = String             #263          //
+   #41 = String             #264          // 00:00:00
+   #42 = Methodref          #30.#265      // java/io/BufferedReader.ready:()Z
+   #43 = Methodref          #30.#266      // java/io/BufferedReader.readLine:()Ljava/lang/String;
+   #44 = String             #267          // :
+   #45 = Methodref          #253.#268     // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #46 = Methodref          #253.#269     // java/lang/String.trim:()Ljava/lang/String;
+   #47 = String             #270          // Sample Rate
+   #48 = Methodref          #119.#271     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
+   #49 = String             #272          // Start Date
+   #50 = Methodref          #273.#274     // java/lang/Long.parseLong:(Ljava/lang/String;)J
+   #51 = Methodref          #36.#275      // ActigraphReader.GT3XfromTickToMillisecond:(J)J
+   #52 = String             #276          // Acceleration Scale
+   #53 = Methodref          #277.#278     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #54 = String             #279          // Acceleration Min
+   #55 = String             #280          // Acceleration Max
+   #56 = String             #281          // Stop Date
+   #57 = String             #282          // Serial Number
+   #58 = String             #283          // TimeZone
+   #59 = Methodref          #36.#284      // ActigraphReader.setAccelerationScale:(Ljava/lang/String;)D
+   #60 = String             #285          // Error parsing
+   #61 = String             #286          // , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
+   #62 = Methodref          #36.#287      // ActigraphReader.setSampleDelta:(D)D
+   #63 = Methodref          #36.#288      // ActigraphReader.readG3TXv1Pairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
+   #64 = Methodref          #36.#289      // ActigraphReader.readG3TXv2:(Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
+   #65 = Methodref          #10.#290      // java/util/zip/ZipFile.close:()V
+   #66 = Methodref          #291.#290     // java/io/InputStream.close:()V
+   #67 = Methodref          #30.#290      // java/io/BufferedReader.close:()V
+   #68 = Methodref          #7.#290       // NpyWriter.close:()V
+   #69 = Class              #292          // java/lang/Exception
+   #70 = Methodref          #69.#293      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+   #71 = Class              #294          // java/io/IOException
+   #72 = Methodref          #71.#293      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
+   #73 = String             #295          // Error reading/writing file
+   #74 = Methodref          #71.#244      // java/io/IOException.toString:()Ljava/lang/String;
+   #75 = String             #296          // ReadOK
+   #76 = Methodref          #253.#297     // java/lang/String.valueOf:(I)Ljava/lang/String;
+   #77 = InterfaceMethodref #298.#299     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+   #78 = String             #300          // ReadErrors
+   #79 = String             #301          // SampleRate
+   #80 = Methodref          #253.#302     // java/lang/String.valueOf:(D)Ljava/lang/String;
+   #81 = Methodref          #291.#303     // java/io/InputStream.read:()I
+   #82 = Methodref          #36.#304      // ActigraphReader.isPayload:(III)Z
+   #83 = Methodref          #36.#305      // ActigraphReader.isAccelScale:([B)Z
+   #84 = Methodref          #36.#306      // ActigraphReader.decodePara:(I)D
+   #85 = Methodref          #36.#307      // ActigraphReader.processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
+   #86 = Methodref          #36.#308      // ActigraphReader.processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
+   #87 = Methodref          #36.#309      // ActigraphReader.checkChecksum:(IIIIJII)V
+   #88 = Methodref          #36.#310      // ActigraphReader.readAccelPair:([BD)[D
    #89 = Double             1000.0d
-   #91 = Methodref          #301.#302     // java/lang/Math.round:(D)J
-   #92 = Methodref          #36.#303      // ActigraphReader.getTrueUnixTime:(JLjava/lang/String;)J
-   #93 = Methodref          #36.#304      // ActigraphReader.toItems:(JDDD)Ljava/util/Map;
-   #94 = Methodref          #7.#305       // NpyWriter.write:(Ljava/util/Map;)V
-   #95 = String             #306          // Line write error:
-   #96 = Methodref          #69.#238      // java/lang/Exception.toString:()Ljava/lang/String;
+   #91 = Methodref          #311.#312     // java/lang/Math.round:(D)J
+   #92 = Methodref          #36.#313      // ActigraphReader.getTrueUnixTime:(JLjava/lang/String;)J
+   #93 = Methodref          #36.#314      // ActigraphReader.toItems:(JDDD)Ljava/util/Map;
+   #94 = Methodref          #7.#315       // NpyWriter.write:(Ljava/util/Map;)V
+   #95 = String             #316          // Line write error:
+   #96 = Methodref          #69.#244      // java/lang/Exception.toString:()Ljava/lang/String;
    #97 = Integer            61440
    #98 = Long               1000l
-  #100 = String             #307          // error when reading activity at byte
-  #101 = Methodref          #16.#308      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-  #102 = Methodref          #232.#309     // java/lang/System.exit:(I)V
-  #103 = Methodref          #176.#310     // java/lang/String.charAt:(I)C
-  #104 = Methodref          #176.#311     // java/lang/String.substring:(I)Ljava/lang/String;
-  #105 = Methodref          #312.#313     // java/time/LocalTime.parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #106 = Methodref          #312.#314     // java/time/LocalTime.getHour:()I
-  #107 = Methodref          #312.#315     // java/time/LocalTime.getMinute:()I
+  #100 = String             #317          // error when reading activity at byte
+  #101 = Methodref          #16.#318      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+  #102 = Methodref          #238.#319     // java/lang/System.exit:(I)V
+  #103 = Methodref          #253.#320     // java/lang/String.charAt:(I)C
+  #104 = Methodref          #253.#321     // java/lang/String.substring:(I)Ljava/lang/String;
+  #105 = Methodref          #322.#323     // java/time/LocalTime.parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #106 = Methodref          #322.#324     // java/time/LocalTime.getHour:()I
+  #107 = Methodref          #322.#325     // java/time/LocalTime.getMinute:()I
   #108 = Long               255l
   #110 = Double             341.0d
   #112 = Double             256.0d
-  #114 = String             #316          // NEO
-  #115 = Methodref          #176.#317     // java/lang/String.startsWith:(Ljava/lang/String;)Z
-  #116 = String             #318          // CLE
-  #117 = String             #319          // MOS
+  #114 = String             #326          // NEO
+  #115 = Methodref          #253.#327     // java/lang/String.startsWith:(Ljava/lang/String;)Z
+  #116 = String             #328          // CLE
+  #117 = String             #329          // MOS
   #118 = Integer            8388607
-  #119 = Class              #320          // java/lang/Integer
+  #119 = Class              #330          // java/lang/Integer
   #120 = Double             2.147483647E9d
   #122 = Double             -2.147483647E9d
   #124 = Integer            -16777216
   #125 = Integer            16777215
   #126 = Integer            8388608
   #127 = Double             8388608.0d
   #129 = Double             2.0d
-  #131 = Methodref          #301.#321     // java/lang/Math.pow:(DD)D
-  #132 = Class              #322          // java/util/Date
+  #131 = Methodref          #311.#331     // java/lang/Math.pow:(DD)D
+  #132 = Class              #332          // java/util/Date
   #133 = Long               621355968000000000l
   #135 = Long               10000l
-  #137 = Methodref          #132.#323     // java/util/Date."<init>":(J)V
-  #138 = Methodref          #132.#324     // java/util/Date.getTime:()J
-  #139 = String             #325          // lux.bin
-  #140 = String             #326          // time
-  #141 = Methodref          #265.#327     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-  #142 = String             #328          // x
-  #143 = Methodref          #329.#330     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
-  #144 = String             #331          // y
-  #145 = String             #332          // z
-  #146 = Methodref          #36.#333      // ActigraphReader.toItems:(JFFF)Ljava/util/Map;
-  #147 = Class              #334          // java/util/LinkedHashMap
-  #148 = Methodref          #147.#221     // java/util/LinkedHashMap."<init>":()V
-  #149 = String             #335          // Long
-  #150 = String             #336          // Float
-  #151 = Methodref          #337.#338     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-  #152 = Class              #339          // java/lang/Object
+  #137 = Methodref          #132.#333     // java/util/Date."<init>":(J)V
+  #138 = Methodref          #132.#334     // java/util/Date.getTime:()J
+  #139 = String             #335          // lux.bin
+  #140 = String             #336          // time
+  #141 = Methodref          #273.#337     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+  #142 = String             #338          // x
+  #143 = Methodref          #339.#340     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
+  #144 = String             #341          // y
+  #145 = String             #342          // z
+  #146 = Methodref          #36.#343      // ActigraphReader.toItems:(JFFF)Ljava/util/Map;
+  #147 = Class              #344          // java/util/LinkedHashMap
+  #148 = Methodref          #147.#227     // java/util/LinkedHashMap."<init>":()V
+  #149 = String             #345          // Long
+  #150 = String             #346          // Float
+  #151 = Methodref          #347.#348     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+  #152 = Class              #349          // java/lang/Object
   #153 = Utf8               INVALID_GT3_FILE
   #154 = Utf8               I
   #155 = Utf8               ConstantValue
   #156 = Integer            0
   #157 = Utf8               VALID_GT3_V1_FILE
   #158 = Integer            1
   #159 = Utf8               VALID_GT3_V2_FILE
@@ -166,260 +166,270 @@
   #169 = Utf8               Code
   #170 = Utf8               LineNumberTable
   #171 = Utf8               read
   #172 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map;
   #173 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
   #174 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
   #175 = Utf8               StackMapTable
-  #176 = Class              #340          // java/lang/String
-  #177 = Class              #341          // java/util/Map
-  #178 = Class              #342          // java/io/InputStream
-  #179 = Class              #343          // java/util/Enumeration
-  #180 = Class              #344          // "[Ljava/lang/String;"
-  #181 = Class              #345          // java/lang/Throwable
-  #182 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-  #183 = Utf8               readG3TXv2
-  #184 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
-  #185 = Class              #346          // "[B"
-  #186 = Utf8               readG3TXv1Pairs
-  #187 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
-  #188 = Class              #347          // "[D"
-  #189 = Utf8               processActivity
-  #190 = Utf8               (Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
-  #191 = Utf8               getTrueUnixTime
-  #192 = Utf8               (JLjava/lang/String;)J
-  #193 = Utf8               processActivity2
-  #194 = Utf8               readAccelPair
-  #195 = Utf8               ([BD)[D
-  #196 = Utf8               checkChecksum
-  #197 = Utf8               (IIIIJII)V
-  #198 = Utf8               setAccelerationScale
-  #199 = Utf8               (Ljava/lang/String;)D
-  #200 = Utf8               setSampleDelta
-  #201 = Utf8               (D)D
-  #202 = Utf8               isPayload
-  #203 = Utf8               (III)Z
-  #204 = Utf8               decodePara
-  #205 = Utf8               (I)D
-  #206 = Utf8               isAccelScale
-  #207 = Utf8               ([B)Z
-  #208 = Utf8               GT3XfromTickToMillisecond
-  #209 = Utf8               (J)J
-  #210 = Utf8               getGT3XVersion
-  #211 = Utf8               (Ljava/util/zip/ZipFile;)I
-  #212 = Utf8               Exceptions
-  #213 = Utf8               toItems
-  #214 = Utf8               (JFFF)Ljava/util/Map;
-  #215 = Utf8               (JFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #216 = Utf8               (JDDD)Ljava/util/Map;
-  #217 = Utf8               (JDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #218 = Utf8               <clinit>
-  #219 = Utf8               SourceFile
-  #220 = Utf8               ActigraphReader.java
-  #221 = NameAndType        #167:#168     // "<init>":()V
-  #222 = NameAndType        #171:#174     // read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
-  #223 = Utf8               java/util/HashMap
-  #224 = Utf8               NpyWriter
-  #225 = NameAndType        #163:#164     // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-  #226 = NameAndType        #167:#348     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
-  #227 = Utf8               java/util/zip/ZipFile
-  #228 = Utf8               java/io/File
-  #229 = NameAndType        #167:#349     // "<init>":(Ljava/lang/String;)V
-  #230 = NameAndType        #167:#350     // "<init>":(Ljava/io/File;I)V
-  #231 = NameAndType        #210:#211     // getGT3XVersion:(Ljava/util/zip/ZipFile;)I
-  #232 = Class              #351          // java/lang/System
-  #233 = NameAndType        #352:#353     // err:Ljava/io/PrintStream;
-  #234 = Utf8               java/lang/StringBuilder
-  #235 = Utf8               file
-  #236 = NameAndType        #354:#355     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #237 = Utf8                is not a valid V1 or V2 g3tx file
-  #238 = NameAndType        #356:#357     // toString:()Ljava/lang/String;
-  #239 = Class              #358          // java/io/PrintStream
-  #240 = NameAndType        #359:#349     // println:(Ljava/lang/String;)V
-  #241 = NameAndType        #360:#361     // entries:()Ljava/util/Enumeration;
-  #242 = NameAndType        #362:#363     // hasMoreElements:()Z
-  #243 = NameAndType        #364:#365     // nextElement:()Ljava/lang/Object;
-  #244 = Utf8               java/util/zip/ZipEntry
-  #245 = Utf8               info.txt
-  #246 = NameAndType        #366:#367     // equals:(Ljava/lang/Object;)Z
-  #247 = Utf8               java/io/BufferedReader
-  #248 = Utf8               java/io/InputStreamReader
-  #249 = NameAndType        #368:#369     // getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-  #250 = NameAndType        #167:#370     // "<init>":(Ljava/io/InputStream;)V
-  #251 = NameAndType        #167:#371     // "<init>":(Ljava/io/Reader;)V
-  #252 = Utf8               activity.bin
-  #253 = Utf8               ActigraphReader
-  #254 = Utf8               log.bin
-  #255 = Utf8
-  #256 = Utf8               00:00:00
-  #257 = NameAndType        #372:#363     // ready:()Z
-  #258 = NameAndType        #373:#357     // readLine:()Ljava/lang/String;
-  #259 = Utf8               :
-  #260 = NameAndType        #374:#375     // split:(Ljava/lang/String;)[Ljava/lang/String;
-  #261 = NameAndType        #376:#357     // trim:()Ljava/lang/String;
-  #262 = Utf8               Sample Rate
-  #263 = NameAndType        #377:#378     // parseInt:(Ljava/lang/String;)I
-  #264 = Utf8               Start Date
-  #265 = Class              #379          // java/lang/Long
-  #266 = NameAndType        #380:#381     // parseLong:(Ljava/lang/String;)J
-  #267 = NameAndType        #208:#209     // GT3XfromTickToMillisecond:(J)J
-  #268 = Utf8               Acceleration Scale
-  #269 = Class              #382          // java/lang/Double
-  #270 = NameAndType        #383:#199     // parseDouble:(Ljava/lang/String;)D
-  #271 = Utf8               Acceleration Min
-  #272 = Utf8               Acceleration Max
-  #273 = Utf8               Stop Date
-  #274 = Utf8               Serial Number
-  #275 = Utf8               TimeZone
-  #276 = NameAndType        #198:#199     // setAccelerationScale:(Ljava/lang/String;)D
-  #277 = Utf8               Error parsing
-  #278 = Utf8               , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
-  #279 = NameAndType        #200:#201     // setSampleDelta:(D)D
-  #280 = NameAndType        #186:#187     // readG3TXv1Pairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
-  #281 = NameAndType        #183:#184     // readG3TXv2:(Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
-  #282 = NameAndType        #384:#168     // close:()V
-  #283 = Utf8               java/lang/Exception
-  #284 = NameAndType        #385:#386     // printStackTrace:(Ljava/io/PrintStream;)V
-  #285 = Utf8               java/io/IOException
-  #286 = Utf8               Error reading/writing file
-  #287 = Utf8               ReadOK
-  #288 = NameAndType        #387:#388     // valueOf:(I)Ljava/lang/String;
-  #289 = NameAndType        #389:#390     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #290 = Utf8               ReadErrors
-  #291 = Utf8               SampleRate
-  #292 = NameAndType        #387:#391     // valueOf:(D)Ljava/lang/String;
-  #293 = NameAndType        #171:#392     // read:()I
-  #294 = NameAndType        #202:#203     // isPayload:(III)Z
-  #295 = NameAndType        #206:#207     // isAccelScale:([B)Z
-  #296 = NameAndType        #204:#205     // decodePara:(I)D
-  #297 = NameAndType        #189:#190     // processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
-  #298 = NameAndType        #193:#190     // processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
-  #299 = NameAndType        #196:#197     // checkChecksum:(IIIIJII)V
-  #300 = NameAndType        #194:#195     // readAccelPair:([BD)[D
-  #301 = Class              #393          // java/lang/Math
-  #302 = NameAndType        #394:#395     // round:(D)J
-  #303 = NameAndType        #191:#192     // getTrueUnixTime:(JLjava/lang/String;)J
-  #304 = NameAndType        #213:#216     // toItems:(JDDD)Ljava/util/Map;
-  #305 = NameAndType        #396:#397     // write:(Ljava/util/Map;)V
-  #306 = Utf8               Line write error:
-  #307 = Utf8               error when reading activity at byte
-  #308 = NameAndType        #354:#398     // append:(I)Ljava/lang/StringBuilder;
-  #309 = NameAndType        #399:#400     // exit:(I)V
-  #310 = NameAndType        #401:#402     // charAt:(I)C
-  #311 = NameAndType        #403:#388     // substring:(I)Ljava/lang/String;
-  #312 = Class              #404          // java/time/LocalTime
-  #313 = NameAndType        #405:#406     // parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #314 = NameAndType        #407:#392     // getHour:()I
-  #315 = NameAndType        #408:#392     // getMinute:()I
-  #316 = Utf8               NEO
-  #317 = NameAndType        #409:#410     // startsWith:(Ljava/lang/String;)Z
-  #318 = Utf8               CLE
-  #319 = Utf8               MOS
-  #320 = Utf8               java/lang/Integer
-  #321 = NameAndType        #411:#412     // pow:(DD)D
-  #322 = Utf8               java/util/Date
-  #323 = NameAndType        #167:#413     // "<init>":(J)V
-  #324 = NameAndType        #414:#415     // getTime:()J
-  #325 = Utf8               lux.bin
-  #326 = Utf8               time
-  #327 = NameAndType        #387:#416     // valueOf:(J)Ljava/lang/Long;
-  #328 = Utf8               x
-  #329 = Class              #417          // java/lang/Float
-  #330 = NameAndType        #387:#418     // valueOf:(F)Ljava/lang/Float;
-  #331 = Utf8               y
-  #332 = Utf8               z
-  #333 = NameAndType        #213:#214     // toItems:(JFFF)Ljava/util/Map;
-  #334 = Utf8               java/util/LinkedHashMap
-  #335 = Utf8               Long
-  #336 = Utf8               Float
-  #337 = Class              #419          // java/util/Collections
-  #338 = NameAndType        #420:#421     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-  #339 = Utf8               java/lang/Object
-  #340 = Utf8               java/lang/String
-  #341 = Utf8               java/util/Map
-  #342 = Utf8               java/io/InputStream
-  #343 = Utf8               java/util/Enumeration
-  #344 = Utf8               [Ljava/lang/String;
-  #345 = Utf8               java/lang/Throwable
-  #346 = Utf8               [B
-  #347 = Utf8               [D
-  #348 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
-  #349 = Utf8               (Ljava/lang/String;)V
-  #350 = Utf8               (Ljava/io/File;I)V
-  #351 = Utf8               java/lang/System
-  #352 = Utf8               err
-  #353 = Utf8               Ljava/io/PrintStream;
-  #354 = Utf8               append
-  #355 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #356 = Utf8               toString
-  #357 = Utf8               ()Ljava/lang/String;
-  #358 = Utf8               java/io/PrintStream
-  #359 = Utf8               println
-  #360 = Utf8               entries
-  #361 = Utf8               ()Ljava/util/Enumeration;
-  #362 = Utf8               hasMoreElements
-  #363 = Utf8               ()Z
-  #364 = Utf8               nextElement
-  #365 = Utf8               ()Ljava/lang/Object;
-  #366 = Utf8               equals
-  #367 = Utf8               (Ljava/lang/Object;)Z
-  #368 = Utf8               getInputStream
-  #369 = Utf8               (Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-  #370 = Utf8               (Ljava/io/InputStream;)V
-  #371 = Utf8               (Ljava/io/Reader;)V
-  #372 = Utf8               ready
-  #373 = Utf8               readLine
-  #374 = Utf8               split
-  #375 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #376 = Utf8               trim
-  #377 = Utf8               parseInt
-  #378 = Utf8               (Ljava/lang/String;)I
-  #379 = Utf8               java/lang/Long
-  #380 = Utf8               parseLong
-  #381 = Utf8               (Ljava/lang/String;)J
-  #382 = Utf8               java/lang/Double
-  #383 = Utf8               parseDouble
-  #384 = Utf8               close
-  #385 = Utf8               printStackTrace
-  #386 = Utf8               (Ljava/io/PrintStream;)V
-  #387 = Utf8               valueOf
-  #388 = Utf8               (I)Ljava/lang/String;
-  #389 = Utf8               put
-  #390 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #391 = Utf8               (D)Ljava/lang/String;
-  #392 = Utf8               ()I
-  #393 = Utf8               java/lang/Math
-  #394 = Utf8               round
-  #395 = Utf8               (D)J
-  #396 = Utf8               write
-  #397 = Utf8               (Ljava/util/Map;)V
-  #398 = Utf8               (I)Ljava/lang/StringBuilder;
-  #399 = Utf8               exit
-  #400 = Utf8               (I)V
-  #401 = Utf8               charAt
-  #402 = Utf8               (I)C
-  #403 = Utf8               substring
-  #404 = Utf8               java/time/LocalTime
-  #405 = Utf8               parse
-  #406 = Utf8               (Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #407 = Utf8               getHour
-  #408 = Utf8               getMinute
-  #409 = Utf8               startsWith
-  #410 = Utf8               (Ljava/lang/String;)Z
-  #411 = Utf8               pow
-  #412 = Utf8               (DD)D
-  #413 = Utf8               (J)V
-  #414 = Utf8               getTime
-  #415 = Utf8               ()J
-  #416 = Utf8               (J)Ljava/lang/Long;
-  #417 = Utf8               java/lang/Float
-  #418 = Utf8               (F)Ljava/lang/Float;
-  #419 = Utf8               java/util/Collections
-  #420 = Utf8               unmodifiableMap
-  #421 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
+  #176 = Class              #350          // java/lang/String
+  #177 = Class              #351          // java/util/Map
+  #178 = Class              #233          // java/util/zip/ZipFile
+  #179 = Class              #255          // java/io/BufferedReader
+  #180 = Class              #352          // java/io/InputStream
+  #181 = Class              #230          // NpyWriter
+  #182 = Class              #353          // java/util/Enumeration
+  #183 = Class              #251          // java/util/zip/ZipEntry
+  #184 = Class              #354          // "[Ljava/lang/String;"
+  #185 = Class              #292          // java/lang/Exception
+  #186 = Class              #294          // java/io/IOException
+  #187 = Class              #355          // java/lang/Throwable
+  #188 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+  #189 = Utf8               readG3TXv2
+  #190 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
+  #191 = Class              #356          // "[B"
+  #192 = Utf8               readG3TXv1Pairs
+  #193 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
+  #194 = Class              #357          // "[D"
+  #195 = Utf8               processActivity
+  #196 = Utf8               (Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
+  #197 = Utf8               getTrueUnixTime
+  #198 = Utf8               (JLjava/lang/String;)J
+  #199 = Utf8               processActivity2
+  #200 = Utf8               readAccelPair
+  #201 = Utf8               ([BD)[D
+  #202 = Utf8               checkChecksum
+  #203 = Utf8               (IIIIJII)V
+  #204 = Utf8               setAccelerationScale
+  #205 = Utf8               (Ljava/lang/String;)D
+  #206 = Utf8               setSampleDelta
+  #207 = Utf8               (D)D
+  #208 = Utf8               isPayload
+  #209 = Utf8               (III)Z
+  #210 = Utf8               decodePara
+  #211 = Utf8               (I)D
+  #212 = Utf8               isAccelScale
+  #213 = Utf8               ([B)Z
+  #214 = Utf8               GT3XfromTickToMillisecond
+  #215 = Utf8               (J)J
+  #216 = Utf8               getGT3XVersion
+  #217 = Utf8               (Ljava/util/zip/ZipFile;)I
+  #218 = Utf8               Exceptions
+  #219 = Utf8               toItems
+  #220 = Utf8               (JFFF)Ljava/util/Map;
+  #221 = Utf8               (JFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #222 = Utf8               (JDDD)Ljava/util/Map;
+  #223 = Utf8               (JDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #224 = Utf8               <clinit>
+  #225 = Utf8               SourceFile
+  #226 = Utf8               ActigraphReader.java
+  #227 = NameAndType        #167:#168     // "<init>":()V
+  #228 = NameAndType        #171:#174     // read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
+  #229 = Utf8               java/util/HashMap
+  #230 = Utf8               NpyWriter
+  #231 = NameAndType        #163:#164     // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+  #232 = NameAndType        #167:#358     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
+  #233 = Utf8               java/util/zip/ZipFile
+  #234 = Utf8               java/io/File
+  #235 = NameAndType        #167:#359     // "<init>":(Ljava/lang/String;)V
+  #236 = NameAndType        #167:#360     // "<init>":(Ljava/io/File;I)V
+  #237 = NameAndType        #216:#217     // getGT3XVersion:(Ljava/util/zip/ZipFile;)I
+  #238 = Class              #361          // java/lang/System
+  #239 = NameAndType        #362:#363     // err:Ljava/io/PrintStream;
+  #240 = Utf8               java/lang/StringBuilder
+  #241 = Utf8               file
+  #242 = NameAndType        #364:#365     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #243 = Utf8                is not a valid V1 or V2 g3tx file
+  #244 = NameAndType        #366:#367     // toString:()Ljava/lang/String;
+  #245 = Class              #368          // java/io/PrintStream
+  #246 = NameAndType        #369:#359     // println:(Ljava/lang/String;)V
+  #247 = NameAndType        #370:#371     // entries:()Ljava/util/Enumeration;
+  #248 = Class              #353          // java/util/Enumeration
+  #249 = NameAndType        #372:#373     // hasMoreElements:()Z
+  #250 = NameAndType        #374:#375     // nextElement:()Ljava/lang/Object;
+  #251 = Utf8               java/util/zip/ZipEntry
+  #252 = Utf8               info.txt
+  #253 = Class              #350          // java/lang/String
+  #254 = NameAndType        #376:#377     // equals:(Ljava/lang/Object;)Z
+  #255 = Utf8               java/io/BufferedReader
+  #256 = Utf8               java/io/InputStreamReader
+  #257 = NameAndType        #378:#379     // getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+  #258 = NameAndType        #167:#380     // "<init>":(Ljava/io/InputStream;)V
+  #259 = NameAndType        #167:#381     // "<init>":(Ljava/io/Reader;)V
+  #260 = Utf8               activity.bin
+  #261 = Utf8               ActigraphReader
+  #262 = Utf8               log.bin
+  #263 = Utf8
+  #264 = Utf8               00:00:00
+  #265 = NameAndType        #382:#373     // ready:()Z
+  #266 = NameAndType        #383:#367     // readLine:()Ljava/lang/String;
+  #267 = Utf8               :
+  #268 = NameAndType        #384:#385     // split:(Ljava/lang/String;)[Ljava/lang/String;
+  #269 = NameAndType        #386:#367     // trim:()Ljava/lang/String;
+  #270 = Utf8               Sample Rate
+  #271 = NameAndType        #387:#388     // parseInt:(Ljava/lang/String;)I
+  #272 = Utf8               Start Date
+  #273 = Class              #389          // java/lang/Long
+  #274 = NameAndType        #390:#391     // parseLong:(Ljava/lang/String;)J
+  #275 = NameAndType        #214:#215     // GT3XfromTickToMillisecond:(J)J
+  #276 = Utf8               Acceleration Scale
+  #277 = Class              #392          // java/lang/Double
+  #278 = NameAndType        #393:#205     // parseDouble:(Ljava/lang/String;)D
+  #279 = Utf8               Acceleration Min
+  #280 = Utf8               Acceleration Max
+  #281 = Utf8               Stop Date
+  #282 = Utf8               Serial Number
+  #283 = Utf8               TimeZone
+  #284 = NameAndType        #204:#205     // setAccelerationScale:(Ljava/lang/String;)D
+  #285 = Utf8               Error parsing
+  #286 = Utf8               , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
+  #287 = NameAndType        #206:#207     // setSampleDelta:(D)D
+  #288 = NameAndType        #192:#193     // readG3TXv1Pairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLNpyWriter;)V
+  #289 = NameAndType        #189:#190     // readG3TXv2:(Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
+  #290 = NameAndType        #394:#168     // close:()V
+  #291 = Class              #352          // java/io/InputStream
+  #292 = Utf8               java/lang/Exception
+  #293 = NameAndType        #395:#396     // printStackTrace:(Ljava/io/PrintStream;)V
+  #294 = Utf8               java/io/IOException
+  #295 = Utf8               Error reading/writing file
+  #296 = Utf8               ReadOK
+  #297 = NameAndType        #397:#398     // valueOf:(I)Ljava/lang/String;
+  #298 = Class              #351          // java/util/Map
+  #299 = NameAndType        #399:#400     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #300 = Utf8               ReadErrors
+  #301 = Utf8               SampleRate
+  #302 = NameAndType        #397:#401     // valueOf:(D)Ljava/lang/String;
+  #303 = NameAndType        #171:#402     // read:()I
+  #304 = NameAndType        #208:#209     // isPayload:(III)Z
+  #305 = NameAndType        #212:#213     // isAccelScale:([B)Z
+  #306 = NameAndType        #210:#211     // decodePara:(I)D
+  #307 = NameAndType        #195:#196     // processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
+  #308 = NameAndType        #199:#196     // processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LNpyWriter;)[I
+  #309 = NameAndType        #202:#203     // checkChecksum:(IIIIJII)V
+  #310 = NameAndType        #200:#201     // readAccelPair:([BD)[D
+  #311 = Class              #403          // java/lang/Math
+  #312 = NameAndType        #404:#405     // round:(D)J
+  #313 = NameAndType        #197:#198     // getTrueUnixTime:(JLjava/lang/String;)J
+  #314 = NameAndType        #219:#222     // toItems:(JDDD)Ljava/util/Map;
+  #315 = NameAndType        #406:#407     // write:(Ljava/util/Map;)V
+  #316 = Utf8               Line write error:
+  #317 = Utf8               error when reading activity at byte
+  #318 = NameAndType        #364:#408     // append:(I)Ljava/lang/StringBuilder;
+  #319 = NameAndType        #409:#410     // exit:(I)V
+  #320 = NameAndType        #411:#412     // charAt:(I)C
+  #321 = NameAndType        #413:#398     // substring:(I)Ljava/lang/String;
+  #322 = Class              #414          // java/time/LocalTime
+  #323 = NameAndType        #415:#416     // parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #324 = NameAndType        #417:#402     // getHour:()I
+  #325 = NameAndType        #418:#402     // getMinute:()I
+  #326 = Utf8               NEO
+  #327 = NameAndType        #419:#420     // startsWith:(Ljava/lang/String;)Z
+  #328 = Utf8               CLE
+  #329 = Utf8               MOS
+  #330 = Utf8               java/lang/Integer
+  #331 = NameAndType        #421:#422     // pow:(DD)D
+  #332 = Utf8               java/util/Date
+  #333 = NameAndType        #167:#423     // "<init>":(J)V
+  #334 = NameAndType        #424:#425     // getTime:()J
+  #335 = Utf8               lux.bin
+  #336 = Utf8               time
+  #337 = NameAndType        #397:#426     // valueOf:(J)Ljava/lang/Long;
+  #338 = Utf8               x
+  #339 = Class              #427          // java/lang/Float
+  #340 = NameAndType        #397:#428     // valueOf:(F)Ljava/lang/Float;
+  #341 = Utf8               y
+  #342 = Utf8               z
+  #343 = NameAndType        #219:#220     // toItems:(JFFF)Ljava/util/Map;
+  #344 = Utf8               java/util/LinkedHashMap
+  #345 = Utf8               Long
+  #346 = Utf8               Float
+  #347 = Class              #429          // java/util/Collections
+  #348 = NameAndType        #430:#431     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+  #349 = Utf8               java/lang/Object
+  #350 = Utf8               java/lang/String
+  #351 = Utf8               java/util/Map
+  #352 = Utf8               java/io/InputStream
+  #353 = Utf8               java/util/Enumeration
+  #354 = Utf8               [Ljava/lang/String;
+  #355 = Utf8               java/lang/Throwable
+  #356 = Utf8               [B
+  #357 = Utf8               [D
+  #358 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
+  #359 = Utf8               (Ljava/lang/String;)V
+  #360 = Utf8               (Ljava/io/File;I)V
+  #361 = Utf8               java/lang/System
+  #362 = Utf8               err
+  #363 = Utf8               Ljava/io/PrintStream;
+  #364 = Utf8               append
+  #365 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #366 = Utf8               toString
+  #367 = Utf8               ()Ljava/lang/String;
+  #368 = Utf8               java/io/PrintStream
+  #369 = Utf8               println
+  #370 = Utf8               entries
+  #371 = Utf8               ()Ljava/util/Enumeration;
+  #372 = Utf8               hasMoreElements
+  #373 = Utf8               ()Z
+  #374 = Utf8               nextElement
+  #375 = Utf8               ()Ljava/lang/Object;
+  #376 = Utf8               equals
+  #377 = Utf8               (Ljava/lang/Object;)Z
+  #378 = Utf8               getInputStream
+  #379 = Utf8               (Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+  #380 = Utf8               (Ljava/io/InputStream;)V
+  #381 = Utf8               (Ljava/io/Reader;)V
+  #382 = Utf8               ready
+  #383 = Utf8               readLine
+  #384 = Utf8               split
+  #385 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #386 = Utf8               trim
+  #387 = Utf8               parseInt
+  #388 = Utf8               (Ljava/lang/String;)I
+  #389 = Utf8               java/lang/Long
+  #390 = Utf8               parseLong
+  #391 = Utf8               (Ljava/lang/String;)J
+  #392 = Utf8               java/lang/Double
+  #393 = Utf8               parseDouble
+  #394 = Utf8               close
+  #395 = Utf8               printStackTrace
+  #396 = Utf8               (Ljava/io/PrintStream;)V
+  #397 = Utf8               valueOf
+  #398 = Utf8               (I)Ljava/lang/String;
+  #399 = Utf8               put
+  #400 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #401 = Utf8               (D)Ljava/lang/String;
+  #402 = Utf8               ()I
+  #403 = Utf8               java/lang/Math
+  #404 = Utf8               round
+  #405 = Utf8               (D)J
+  #406 = Utf8               write
+  #407 = Utf8               (Ljava/util/Map;)V
+  #408 = Utf8               (I)Ljava/lang/StringBuilder;
+  #409 = Utf8               exit
+  #410 = Utf8               (I)V
+  #411 = Utf8               charAt
+  #412 = Utf8               (I)C
+  #413 = Utf8               substring
+  #414 = Utf8               java/time/LocalTime
+  #415 = Utf8               parse
+  #416 = Utf8               (Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #417 = Utf8               getHour
+  #418 = Utf8               getMinute
+  #419 = Utf8               startsWith
+  #420 = Utf8               (Ljava/lang/String;)Z
+  #421 = Utf8               pow
+  #422 = Utf8               (DD)D
+  #423 = Utf8               (J)V
+  #424 = Utf8               getTime
+  #425 = Utf8               ()J
+  #426 = Utf8               (J)Ljava/lang/Long;
+  #427 = Utf8               java/lang/Float
+  #428 = Utf8               (F)Ljava/lang/Float;
+  #429 = Utf8               java/util/Collections
+  #430 = Utf8               unmodifiableMap
+  #431 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
 {
   private static final int INVALID_GT3_FILE = 0;
     descriptor: I
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
     ConstantValue: int 0
 
   private static final int VALID_GT3_V1_FILE = 1;
@@ -1013,15 +1023,15 @@
           locals = [ class java/lang/String, class java/lang/String, int, class java/util/Map, int, double, int, class java/util/zip/ZipFile, class java/io/BufferedReader, class java/io/InputStream, class NpyWriter, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Exception ]
         frame_type = 9 /* same */
         frame_type = 255 /* full_frame */
           offset_delta = 2
           locals = [ class java/lang/String, class java/lang/String, int, class java/util/Map, int, double, int, class java/util/zip/ZipFile, class java/io/BufferedReader, class java/io/InputStream, class NpyWriter ]
           stack = []
-    Signature: #182                         // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #188                         // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   private static void readG3TXv2(java.io.InputStream, java.lang.String, double, double, double, NpyWriter);
     descriptor: (Ljava/io/InputStream;Ljava/lang/String;DDDLNpyWriter;)V
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=14, locals=28, args_size=6
          0: iconst_0
@@ -2879,15 +2889,15 @@
       LineNumberTable:
         line 787: 0
         line 788: 9
         line 789: 23
         line 790: 37
         line 791: 51
         line 794: 66
-    Signature: #215                         // (JFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #221                         // (JFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   private static java.util.Map<java.lang.String, java.lang.Object> toItems(long, double, double, double);
     descriptor: (JDDD)Ljava/util/Map;
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=6, locals=8, args_size=4
          0: lload_0
@@ -2897,15 +2907,15 @@
          5: d2f
          6: dload         6
          8: d2f
          9: invokestatic  #146                // Method toItems:(JFFF)Ljava/util/Map;
         12: areturn
       LineNumberTable:
         line 798: 0
-    Signature: #217                         // (JDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #223                         // (JDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   static {};
     descriptor: ()V
     flags: (0x0008) ACC_STATIC
     Code:
       stack=3, locals=1, args_size=0
          0: new           #147                // class java/util/LinkedHashMap
```

### Comparing `actipy-2.0.3/actipy/ActigraphReader.java` & `actipy-2.0.3.post0/src/actipy/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/actipy/AxivityReader.class` & `actipy-2.0.3.post0/src/actipy/AxivityReader.class`

 * *Files 17% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,116 +1,116 @@
-  SHA-256 checksum 897357d183b007430911d90b052716927183f9f6b7f2d772e48d7444d6134cac
+  SHA-256 checksum 8e68ef4e9c3cc580def071ea480803b5f79136061c7af5c465417f1aa48cf757
   Compiled from "AxivityReader.java"
 public class AxivityReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #18                         // AxivityReader
   super_class: #107                       // java/lang/Object
   interfaces: 0, fields: 11, methods: 16, attributes: 1
 Constant pool:
-    #1 = Methodref          #107.#172     // java/lang/Object."<init>":()V
-    #2 = Fieldref           #18.#173      // AxivityReader.sessionStart:Ljava/time/LocalDateTime;
-    #3 = Fieldref           #18.#174      // AxivityReader.statusOK:I
+    #1 = Methodref          #107.#176     // java/lang/Object."<init>":()V
+    #2 = Fieldref           #18.#177      // AxivityReader.sessionStart:Ljava/time/LocalDateTime;
+    #3 = Fieldref           #18.#178      // AxivityReader.statusOK:I
     #4 = Float              -1.0f
-    #5 = Fieldref           #18.#175      // AxivityReader.sampleRate:F
-    #6 = Fieldref           #18.#176      // AxivityReader.errCounter:I
-    #7 = Fieldref           #18.#177      // AxivityReader.lastBlockTime:D
-    #8 = Fieldref           #18.#178      // AxivityReader.accFile:Ljava/lang/String;
-    #9 = Fieldref           #18.#179      // AxivityReader.outFile:Ljava/lang/String;
-   #10 = Fieldref           #18.#180      // AxivityReader.verbose:Z
-   #11 = Class              #181          // java/util/HashMap
-   #12 = Methodref          #11.#172      // java/util/HashMap."<init>":()V
-   #13 = Class              #182          // java/io/FileInputStream
-   #14 = Methodref          #13.#183      // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
-   #15 = Methodref          #13.#184      // java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
-   #16 = Methodref          #18.#185      // AxivityReader.setupWriter:()V
-   #17 = Methodref          #139.#186     // java/nio/channels/FileChannel.size:()J
-   #18 = Class              #187          // AxivityReader
+    #5 = Fieldref           #18.#179      // AxivityReader.sampleRate:F
+    #6 = Fieldref           #18.#180      // AxivityReader.errCounter:I
+    #7 = Fieldref           #18.#181      // AxivityReader.lastBlockTime:D
+    #8 = Fieldref           #18.#182      // AxivityReader.accFile:Ljava/lang/String;
+    #9 = Fieldref           #18.#183      // AxivityReader.outFile:Ljava/lang/String;
+   #10 = Fieldref           #18.#184      // AxivityReader.verbose:Z
+   #11 = Class              #185          // java/util/HashMap
+   #12 = Methodref          #11.#176      // java/util/HashMap."<init>":()V
+   #13 = Class              #186          // java/io/FileInputStream
+   #14 = Methodref          #13.#187      // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
+   #15 = Methodref          #13.#188      // java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
+   #16 = Methodref          #18.#189      // AxivityReader.setupWriter:()V
+   #17 = Methodref          #190.#191     // java/nio/channels/FileChannel.size:()J
+   #18 = Class              #192          // AxivityReader
    #19 = Long               512l
-   #21 = Methodref          #140.#188     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
-   #22 = Methodref          #139.#189     // java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
-   #23 = Methodref          #18.#190      // AxivityReader.parseCwaBlock:(Ljava/nio/ByteBuffer;)V
-   #24 = Methodref          #140.#191     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-   #25 = Fieldref           #192.#193     // java/lang/System.out:Ljava/io/PrintStream;
-   #26 = Class              #194          // java/lang/StringBuilder
-   #27 = Methodref          #26.#172      // java/lang/StringBuilder."<init>":()V
-   #28 = String             #195          // Reading file...
-   #29 = Methodref          #26.#196      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #30 = Methodref          #26.#197      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-   #31 = String             #198          // %\r
-   #32 = Methodref          #26.#199      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #33 = Methodref          #200.#201     // java/io/PrintStream.print:(Ljava/lang/String;)V
-   #34 = Methodref          #139.#202     // java/nio/channels/FileChannel.close:()V
-   #35 = Class              #203          // java/lang/Throwable
-   #36 = Methodref          #35.#204      // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-   #37 = Methodref          #13.#202      // java/io/FileInputStream.close:()V
-   #38 = Methodref          #18.#205      // AxivityReader.closeWriter:()V
-   #39 = Class              #206          // java/lang/Exception
-   #40 = Methodref          #39.#207      // java/lang/Exception.printStackTrace:()V
-   #41 = String             #208          // ReadOK
-   #42 = Methodref          #148.#209     // java/lang/String.valueOf:(I)Ljava/lang/String;
-   #43 = InterfaceMethodref #138.#210     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-   #44 = String             #211          // ReadErrors
-   #45 = String             #212          // SampleRate
-   #46 = Methodref          #148.#213     // java/lang/String.valueOf:(F)Ljava/lang/String;
-   #47 = Methodref          #18.#214      // AxivityReader."<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
-   #48 = Methodref          #18.#215      // AxivityReader.read:()Ljava/util/Map;
-   #49 = Methodref          #140.#216     // java/nio/ByteBuffer.flip:()Ljava/nio/Buffer;
-   #50 = Fieldref           #217.#218     // java/nio/ByteOrder.LITTLE_ENDIAN:Ljava/nio/ByteOrder;
-   #51 = Methodref          #140.#219     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-   #52 = Methodref          #140.#220     // java/nio/ByteBuffer.get:()B
-   #53 = Methodref          #26.#221      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
-   #54 = String             #222          //
-   #55 = String             #223          // MD
-   #56 = Methodref          #148.#224     // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #57 = String             #225          // AX
-   #58 = Methodref          #18.#226      // AxivityReader.getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
-   #59 = Methodref          #18.#227      // AxivityReader.getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
+   #21 = Methodref          #193.#194     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
+   #22 = Methodref          #190.#195     // java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
+   #23 = Methodref          #18.#196      // AxivityReader.parseCwaBlock:(Ljava/nio/ByteBuffer;)V
+   #24 = Methodref          #193.#197     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+   #25 = Fieldref           #198.#199     // java/lang/System.out:Ljava/io/PrintStream;
+   #26 = Class              #200          // java/lang/StringBuilder
+   #27 = Methodref          #26.#176      // java/lang/StringBuilder."<init>":()V
+   #28 = String             #201          // Reading file...
+   #29 = Methodref          #26.#202      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #30 = Methodref          #26.#203      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+   #31 = String             #204          // %\r
+   #32 = Methodref          #26.#205      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #33 = Methodref          #206.#207     // java/io/PrintStream.print:(Ljava/lang/String;)V
+   #34 = Methodref          #190.#208     // java/nio/channels/FileChannel.close:()V
+   #35 = Class              #209          // java/lang/Throwable
+   #36 = Methodref          #35.#210      // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+   #37 = Methodref          #13.#208      // java/io/FileInputStream.close:()V
+   #38 = Methodref          #18.#211      // AxivityReader.closeWriter:()V
+   #39 = Class              #212          // java/lang/Exception
+   #40 = Methodref          #39.#213      // java/lang/Exception.printStackTrace:()V
+   #41 = String             #214          // ReadOK
+   #42 = Methodref          #215.#216     // java/lang/String.valueOf:(I)Ljava/lang/String;
+   #43 = InterfaceMethodref #217.#218     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+   #44 = String             #219          // ReadErrors
+   #45 = String             #220          // SampleRate
+   #46 = Methodref          #215.#221     // java/lang/String.valueOf:(F)Ljava/lang/String;
+   #47 = Methodref          #18.#222      // AxivityReader."<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
+   #48 = Methodref          #18.#223      // AxivityReader.read:()Ljava/util/Map;
+   #49 = Methodref          #193.#224     // java/nio/ByteBuffer.flip:()Ljava/nio/Buffer;
+   #50 = Fieldref           #225.#226     // java/nio/ByteOrder.LITTLE_ENDIAN:Ljava/nio/ByteOrder;
+   #51 = Methodref          #193.#227     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+   #52 = Methodref          #193.#228     // java/nio/ByteBuffer.get:()B
+   #53 = Methodref          #26.#229      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
+   #54 = String             #230          //
+   #55 = String             #231          // MD
+   #56 = Methodref          #215.#232     // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #57 = String             #233          // AX
+   #58 = Methodref          #18.#234      // AxivityReader.getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
+   #59 = Methodref          #18.#235      // AxivityReader.getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
    #60 = Double             150.0d
    #62 = Double             20500.0d
    #64 = Double             1000.0d
-   #66 = Methodref          #140.#228     // java/nio/ByteBuffer.get:(I)B
-   #67 = Methodref          #18.#229      // AxivityReader.getCwaTimestamp:(I)J
-   #68 = Methodref          #140.#230     // java/nio/ByteBuffer.getShort:(I)S
+   #66 = Methodref          #193.#236     // java/nio/ByteBuffer.get:(I)B
+   #67 = Methodref          #18.#237      // AxivityReader.getCwaTimestamp:(I)J
+   #68 = Methodref          #193.#238     // java/nio/ByteBuffer.getShort:(I)S
    #69 = Float              3200.0f
-   #70 = String             #231          // Found checksum error. Skipping data block
-   #71 = Methodref          #39.#183      // java/lang/Exception."<init>":(Ljava/lang/String;)V
-   #72 = Methodref          #232.#233     // java/lang/Math.floor:(D)D
-   #73 = Methodref          #18.#234      // AxivityReader.getCwaLocalDateTime:(I)Ljava/time/LocalDateTime;
+   #70 = String             #239          // Found checksum error. Skipping data block
+   #71 = Methodref          #39.#187      // java/lang/Exception."<init>":(Ljava/lang/String;)V
+   #72 = Methodref          #240.#241     // java/lang/Math.floor:(D)D
+   #73 = Methodref          #18.#242      // AxivityReader.getCwaLocalDateTime:(I)Ljava/time/LocalDateTime;
    #74 = Long               -64l
    #76 = Long               6l
    #78 = Long               3l
    #80 = Float              256.0f
-   #81 = Fieldref           #18.#235      // AxivityReader.writer:LNpyWriter;
-   #82 = Methodref          #18.#236      // AxivityReader.toItems:(JFFFF)Ljava/util/Map;
-   #83 = Methodref          #91.#237      // NpyWriter.write:(Ljava/util/Map;)V
-   #84 = Methodref          #238.#239     // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
-   #85 = Fieldref           #240.#241     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
-   #86 = Methodref          #238.#242     // java/time/LocalDateTime.toEpochSecond:(Ljava/time/ZoneOffset;)J
-   #87 = Methodref          #140.#243     // java/nio/ByteBuffer.getInt:(I)I
+   #81 = Fieldref           #18.#243      // AxivityReader.writer:LNpyWriter;
+   #82 = Methodref          #18.#244      // AxivityReader.toItems:(JFFFF)Ljava/util/Map;
+   #83 = Methodref          #91.#245      // NpyWriter.write:(Ljava/util/Map;)V
+   #84 = Methodref          #246.#247     // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
+   #85 = Fieldref           #248.#249     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
+   #86 = Methodref          #246.#250     // java/time/LocalDateTime.toEpochSecond:(Ljava/time/ZoneOffset;)J
+   #87 = Methodref          #193.#251     // java/nio/ByteBuffer.getInt:(I)I
    #88 = Long               4294967295l
    #90 = Integer            65535
-   #91 = Class              #244          // NpyWriter
-   #92 = Fieldref           #18.#245      // AxivityReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-   #93 = Methodref          #91.#246      // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
-   #94 = Methodref          #91.#202      // NpyWriter.close:()V
-   #95 = String             #247          // time
-   #96 = Methodref          #248.#249     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-   #97 = String             #250          // x
-   #98 = Methodref          #251.#252     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
-   #99 = String             #253          // y
-  #100 = String             #254          // z
-  #101 = String             #255          // temperature
-  #102 = Class              #256          // java/util/LinkedHashMap
-  #103 = Methodref          #102.#172     // java/util/LinkedHashMap."<init>":()V
-  #104 = String             #257          // Long
-  #105 = String             #258          // Float
-  #106 = Methodref          #259.#260     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-  #107 = Class              #261          // java/lang/Object
+   #91 = Class              #252          // NpyWriter
+   #92 = Fieldref           #18.#253      // AxivityReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+   #93 = Methodref          #91.#254      // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
+   #94 = Methodref          #91.#208      // NpyWriter.close:()V
+   #95 = String             #255          // time
+   #96 = Methodref          #256.#257     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+   #97 = String             #258          // x
+   #98 = Methodref          #259.#260     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
+   #99 = String             #261          // y
+  #100 = String             #262          // z
+  #101 = String             #263          // temperature
+  #102 = Class              #264          // java/util/LinkedHashMap
+  #103 = Methodref          #102.#176     // java/util/LinkedHashMap."<init>":()V
+  #104 = String             #265          // Long
+  #105 = String             #266          // Float
+  #106 = Methodref          #267.#268     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+  #107 = Class              #269          // java/lang/Object
   #108 = Utf8               BLOCKSIZE
   #109 = Utf8               I
   #110 = Utf8               ConstantValue
   #111 = Integer            512
   #112 = Utf8               ITEM_NAMES_AND_TYPES
   #113 = Utf8               Ljava/util/Map;
   #114 = Utf8               Signature
@@ -133,207 +133,215 @@
   #131 = Utf8               <init>
   #132 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)V
   #133 = Utf8               Code
   #134 = Utf8               LineNumberTable
   #135 = Utf8               read
   #136 = Utf8               ()Ljava/util/Map;
   #137 = Utf8               StackMapTable
-  #138 = Class              #262          // java/util/Map
-  #139 = Class              #263          // java/nio/channels/FileChannel
-  #140 = Class              #264          // java/nio/ByteBuffer
-  #141 = Utf8               ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-  #142 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
-  #143 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-  #144 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map;
-  #145 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-  #146 = Utf8               parseCwaBlock
-  #147 = Utf8               (Ljava/nio/ByteBuffer;)V
-  #148 = Class              #265          // java/lang/String
-  #149 = Utf8               getCwaLocalDateTime
-  #150 = Utf8               (I)Ljava/time/LocalDateTime;
-  #151 = Utf8               getCwaTimestamp
-  #152 = Utf8               (I)J
-  #153 = Utf8               getCwaHeaderLoggingStartTime
-  #154 = Utf8               (Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
-  #155 = Utf8               getOutFile
-  #156 = Utf8               ()Ljava/lang/String;
-  #157 = Utf8               getUnsignedInt
-  #158 = Utf8               (Ljava/nio/ByteBuffer;I)J
-  #159 = Utf8               getUnsignedShort
-  #160 = Utf8               (Ljava/nio/ByteBuffer;I)I
-  #161 = Utf8               setupWriter
-  #162 = Utf8               ()V
-  #163 = Utf8               closeWriter
-  #164 = Utf8               toItems
-  #165 = Utf8               (JFFFF)Ljava/util/Map;
-  #166 = Utf8               (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #167 = Utf8               (JDDDD)Ljava/util/Map;
-  #168 = Utf8               (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #169 = Utf8               <clinit>
-  #170 = Utf8               SourceFile
-  #171 = Utf8               AxivityReader.java
-  #172 = NameAndType        #131:#162     // "<init>":()V
-  #173 = NameAndType        #121:#122     // sessionStart:Ljava/time/LocalDateTime;
-  #174 = NameAndType        #123:#109     // statusOK:I
-  #175 = NameAndType        #124:#125     // sampleRate:F
-  #176 = NameAndType        #126:#109     // errCounter:I
-  #177 = NameAndType        #127:#128     // lastBlockTime:D
-  #178 = NameAndType        #116:#117     // accFile:Ljava/lang/String;
-  #179 = NameAndType        #118:#117     // outFile:Ljava/lang/String;
-  #180 = NameAndType        #119:#120     // verbose:Z
-  #181 = Utf8               java/util/HashMap
-  #182 = Utf8               java/io/FileInputStream
-  #183 = NameAndType        #131:#266     // "<init>":(Ljava/lang/String;)V
-  #184 = NameAndType        #267:#268     // getChannel:()Ljava/nio/channels/FileChannel;
-  #185 = NameAndType        #161:#162     // setupWriter:()V
-  #186 = NameAndType        #269:#270     // size:()J
-  #187 = Utf8               AxivityReader
-  #188 = NameAndType        #271:#272     // allocate:(I)Ljava/nio/ByteBuffer;
-  #189 = NameAndType        #135:#273     // read:(Ljava/nio/ByteBuffer;)I
-  #190 = NameAndType        #146:#147     // parseCwaBlock:(Ljava/nio/ByteBuffer;)V
-  #191 = NameAndType        #274:#275     // clear:()Ljava/nio/Buffer;
-  #192 = Class              #276          // java/lang/System
-  #193 = NameAndType        #277:#278     // out:Ljava/io/PrintStream;
-  #194 = Utf8               java/lang/StringBuilder
-  #195 = Utf8               Reading file...
-  #196 = NameAndType        #279:#280     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #197 = NameAndType        #279:#281     // append:(J)Ljava/lang/StringBuilder;
-  #198 = Utf8               %\r
-  #199 = NameAndType        #282:#156     // toString:()Ljava/lang/String;
-  #200 = Class              #283          // java/io/PrintStream
-  #201 = NameAndType        #284:#266     // print:(Ljava/lang/String;)V
-  #202 = NameAndType        #285:#162     // close:()V
-  #203 = Utf8               java/lang/Throwable
-  #204 = NameAndType        #286:#287     // addSuppressed:(Ljava/lang/Throwable;)V
-  #205 = NameAndType        #163:#162     // closeWriter:()V
-  #206 = Utf8               java/lang/Exception
-  #207 = NameAndType        #288:#162     // printStackTrace:()V
-  #208 = Utf8               ReadOK
-  #209 = NameAndType        #289:#290     // valueOf:(I)Ljava/lang/String;
-  #210 = NameAndType        #291:#292     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #211 = Utf8               ReadErrors
-  #212 = Utf8               SampleRate
-  #213 = NameAndType        #289:#293     // valueOf:(F)Ljava/lang/String;
-  #214 = NameAndType        #131:#132     // "<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
-  #215 = NameAndType        #135:#136     // read:()Ljava/util/Map;
-  #216 = NameAndType        #294:#275     // flip:()Ljava/nio/Buffer;
-  #217 = Class              #295          // java/nio/ByteOrder
-  #218 = NameAndType        #296:#297     // LITTLE_ENDIAN:Ljava/nio/ByteOrder;
-  #219 = NameAndType        #298:#299     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #220 = NameAndType        #300:#301     // get:()B
-  #221 = NameAndType        #279:#302     // append:(C)Ljava/lang/StringBuilder;
-  #222 = Utf8
-  #223 = Utf8               MD
-  #224 = NameAndType        #303:#304     // equals:(Ljava/lang/Object;)Z
-  #225 = Utf8               AX
-  #226 = NameAndType        #157:#158     // getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
-  #227 = NameAndType        #159:#160     // getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
-  #228 = NameAndType        #300:#305     // get:(I)B
-  #229 = NameAndType        #151:#152     // getCwaTimestamp:(I)J
-  #230 = NameAndType        #306:#307     // getShort:(I)S
-  #231 = Utf8               Found checksum error. Skipping data block
-  #232 = Class              #308          // java/lang/Math
-  #233 = NameAndType        #309:#310     // floor:(D)D
-  #234 = NameAndType        #149:#150     // getCwaLocalDateTime:(I)Ljava/time/LocalDateTime;
-  #235 = NameAndType        #129:#130     // writer:LNpyWriter;
-  #236 = NameAndType        #164:#165     // toItems:(JFFFF)Ljava/util/Map;
-  #237 = NameAndType        #311:#312     // write:(Ljava/util/Map;)V
-  #238 = Class              #313          // java/time/LocalDateTime
-  #239 = NameAndType        #314:#315     // of:(IIIIII)Ljava/time/LocalDateTime;
-  #240 = Class              #316          // java/time/ZoneOffset
-  #241 = NameAndType        #317:#318     // UTC:Ljava/time/ZoneOffset;
-  #242 = NameAndType        #319:#320     // toEpochSecond:(Ljava/time/ZoneOffset;)J
-  #243 = NameAndType        #321:#322     // getInt:(I)I
-  #244 = Utf8               NpyWriter
-  #245 = NameAndType        #112:#113     // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-  #246 = NameAndType        #131:#323     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
-  #247 = Utf8               time
-  #248 = Class              #324          // java/lang/Long
-  #249 = NameAndType        #289:#325     // valueOf:(J)Ljava/lang/Long;
-  #250 = Utf8               x
-  #251 = Class              #326          // java/lang/Float
-  #252 = NameAndType        #289:#327     // valueOf:(F)Ljava/lang/Float;
-  #253 = Utf8               y
-  #254 = Utf8               z
-  #255 = Utf8               temperature
-  #256 = Utf8               java/util/LinkedHashMap
-  #257 = Utf8               Long
-  #258 = Utf8               Float
-  #259 = Class              #328          // java/util/Collections
-  #260 = NameAndType        #329:#330     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-  #261 = Utf8               java/lang/Object
-  #262 = Utf8               java/util/Map
-  #263 = Utf8               java/nio/channels/FileChannel
-  #264 = Utf8               java/nio/ByteBuffer
-  #265 = Utf8               java/lang/String
-  #266 = Utf8               (Ljava/lang/String;)V
-  #267 = Utf8               getChannel
-  #268 = Utf8               ()Ljava/nio/channels/FileChannel;
-  #269 = Utf8               size
-  #270 = Utf8               ()J
-  #271 = Utf8               allocate
-  #272 = Utf8               (I)Ljava/nio/ByteBuffer;
-  #273 = Utf8               (Ljava/nio/ByteBuffer;)I
-  #274 = Utf8               clear
-  #275 = Utf8               ()Ljava/nio/Buffer;
-  #276 = Utf8               java/lang/System
-  #277 = Utf8               out
-  #278 = Utf8               Ljava/io/PrintStream;
-  #279 = Utf8               append
-  #280 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #281 = Utf8               (J)Ljava/lang/StringBuilder;
-  #282 = Utf8               toString
-  #283 = Utf8               java/io/PrintStream
-  #284 = Utf8               print
-  #285 = Utf8               close
-  #286 = Utf8               addSuppressed
-  #287 = Utf8               (Ljava/lang/Throwable;)V
-  #288 = Utf8               printStackTrace
-  #289 = Utf8               valueOf
-  #290 = Utf8               (I)Ljava/lang/String;
-  #291 = Utf8               put
-  #292 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #293 = Utf8               (F)Ljava/lang/String;
-  #294 = Utf8               flip
-  #295 = Utf8               java/nio/ByteOrder
-  #296 = Utf8               LITTLE_ENDIAN
-  #297 = Utf8               Ljava/nio/ByteOrder;
-  #298 = Utf8               order
-  #299 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #300 = Utf8               get
-  #301 = Utf8               ()B
-  #302 = Utf8               (C)Ljava/lang/StringBuilder;
-  #303 = Utf8               equals
-  #304 = Utf8               (Ljava/lang/Object;)Z
-  #305 = Utf8               (I)B
-  #306 = Utf8               getShort
-  #307 = Utf8               (I)S
-  #308 = Utf8               java/lang/Math
-  #309 = Utf8               floor
-  #310 = Utf8               (D)D
-  #311 = Utf8               write
-  #312 = Utf8               (Ljava/util/Map;)V
-  #313 = Utf8               java/time/LocalDateTime
-  #314 = Utf8               of
-  #315 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
-  #316 = Utf8               java/time/ZoneOffset
-  #317 = Utf8               UTC
-  #318 = Utf8               Ljava/time/ZoneOffset;
-  #319 = Utf8               toEpochSecond
-  #320 = Utf8               (Ljava/time/ZoneOffset;)J
-  #321 = Utf8               getInt
-  #322 = Utf8               (I)I
-  #323 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
-  #324 = Utf8               java/lang/Long
-  #325 = Utf8               (J)Ljava/lang/Long;
-  #326 = Utf8               java/lang/Float
-  #327 = Utf8               (F)Ljava/lang/Float;
-  #328 = Utf8               java/util/Collections
-  #329 = Utf8               unmodifiableMap
-  #330 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
+  #138 = Class              #192          // AxivityReader
+  #139 = Class              #270          // java/util/Map
+  #140 = Class              #186          // java/io/FileInputStream
+  #141 = Class              #209          // java/lang/Throwable
+  #142 = Class              #271          // java/nio/channels/FileChannel
+  #143 = Class              #272          // java/nio/ByteBuffer
+  #144 = Class              #212          // java/lang/Exception
+  #145 = Utf8               ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+  #146 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
+  #147 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+  #148 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map;
+  #149 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+  #150 = Utf8               parseCwaBlock
+  #151 = Utf8               (Ljava/nio/ByteBuffer;)V
+  #152 = Class              #273          // java/lang/String
+  #153 = Utf8               getCwaLocalDateTime
+  #154 = Utf8               (I)Ljava/time/LocalDateTime;
+  #155 = Utf8               getCwaTimestamp
+  #156 = Utf8               (I)J
+  #157 = Utf8               getCwaHeaderLoggingStartTime
+  #158 = Utf8               (Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
+  #159 = Utf8               getOutFile
+  #160 = Utf8               ()Ljava/lang/String;
+  #161 = Utf8               getUnsignedInt
+  #162 = Utf8               (Ljava/nio/ByteBuffer;I)J
+  #163 = Utf8               getUnsignedShort
+  #164 = Utf8               (Ljava/nio/ByteBuffer;I)I
+  #165 = Utf8               setupWriter
+  #166 = Utf8               ()V
+  #167 = Utf8               closeWriter
+  #168 = Utf8               toItems
+  #169 = Utf8               (JFFFF)Ljava/util/Map;
+  #170 = Utf8               (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #171 = Utf8               (JDDDD)Ljava/util/Map;
+  #172 = Utf8               (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #173 = Utf8               <clinit>
+  #174 = Utf8               SourceFile
+  #175 = Utf8               AxivityReader.java
+  #176 = NameAndType        #131:#166     // "<init>":()V
+  #177 = NameAndType        #121:#122     // sessionStart:Ljava/time/LocalDateTime;
+  #178 = NameAndType        #123:#109     // statusOK:I
+  #179 = NameAndType        #124:#125     // sampleRate:F
+  #180 = NameAndType        #126:#109     // errCounter:I
+  #181 = NameAndType        #127:#128     // lastBlockTime:D
+  #182 = NameAndType        #116:#117     // accFile:Ljava/lang/String;
+  #183 = NameAndType        #118:#117     // outFile:Ljava/lang/String;
+  #184 = NameAndType        #119:#120     // verbose:Z
+  #185 = Utf8               java/util/HashMap
+  #186 = Utf8               java/io/FileInputStream
+  #187 = NameAndType        #131:#274     // "<init>":(Ljava/lang/String;)V
+  #188 = NameAndType        #275:#276     // getChannel:()Ljava/nio/channels/FileChannel;
+  #189 = NameAndType        #165:#166     // setupWriter:()V
+  #190 = Class              #271          // java/nio/channels/FileChannel
+  #191 = NameAndType        #277:#278     // size:()J
+  #192 = Utf8               AxivityReader
+  #193 = Class              #272          // java/nio/ByteBuffer
+  #194 = NameAndType        #279:#280     // allocate:(I)Ljava/nio/ByteBuffer;
+  #195 = NameAndType        #135:#281     // read:(Ljava/nio/ByteBuffer;)I
+  #196 = NameAndType        #150:#151     // parseCwaBlock:(Ljava/nio/ByteBuffer;)V
+  #197 = NameAndType        #282:#283     // clear:()Ljava/nio/Buffer;
+  #198 = Class              #284          // java/lang/System
+  #199 = NameAndType        #285:#286     // out:Ljava/io/PrintStream;
+  #200 = Utf8               java/lang/StringBuilder
+  #201 = Utf8               Reading file...
+  #202 = NameAndType        #287:#288     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #203 = NameAndType        #287:#289     // append:(J)Ljava/lang/StringBuilder;
+  #204 = Utf8               %\r
+  #205 = NameAndType        #290:#160     // toString:()Ljava/lang/String;
+  #206 = Class              #291          // java/io/PrintStream
+  #207 = NameAndType        #292:#274     // print:(Ljava/lang/String;)V
+  #208 = NameAndType        #293:#166     // close:()V
+  #209 = Utf8               java/lang/Throwable
+  #210 = NameAndType        #294:#295     // addSuppressed:(Ljava/lang/Throwable;)V
+  #211 = NameAndType        #167:#166     // closeWriter:()V
+  #212 = Utf8               java/lang/Exception
+  #213 = NameAndType        #296:#166     // printStackTrace:()V
+  #214 = Utf8               ReadOK
+  #215 = Class              #273          // java/lang/String
+  #216 = NameAndType        #297:#298     // valueOf:(I)Ljava/lang/String;
+  #217 = Class              #270          // java/util/Map
+  #218 = NameAndType        #299:#300     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #219 = Utf8               ReadErrors
+  #220 = Utf8               SampleRate
+  #221 = NameAndType        #297:#301     // valueOf:(F)Ljava/lang/String;
+  #222 = NameAndType        #131:#132     // "<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
+  #223 = NameAndType        #135:#136     // read:()Ljava/util/Map;
+  #224 = NameAndType        #302:#283     // flip:()Ljava/nio/Buffer;
+  #225 = Class              #303          // java/nio/ByteOrder
+  #226 = NameAndType        #304:#305     // LITTLE_ENDIAN:Ljava/nio/ByteOrder;
+  #227 = NameAndType        #306:#307     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #228 = NameAndType        #308:#309     // get:()B
+  #229 = NameAndType        #287:#310     // append:(C)Ljava/lang/StringBuilder;
+  #230 = Utf8
+  #231 = Utf8               MD
+  #232 = NameAndType        #311:#312     // equals:(Ljava/lang/Object;)Z
+  #233 = Utf8               AX
+  #234 = NameAndType        #161:#162     // getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
+  #235 = NameAndType        #163:#164     // getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
+  #236 = NameAndType        #308:#313     // get:(I)B
+  #237 = NameAndType        #155:#156     // getCwaTimestamp:(I)J
+  #238 = NameAndType        #314:#315     // getShort:(I)S
+  #239 = Utf8               Found checksum error. Skipping data block
+  #240 = Class              #316          // java/lang/Math
+  #241 = NameAndType        #317:#318     // floor:(D)D
+  #242 = NameAndType        #153:#154     // getCwaLocalDateTime:(I)Ljava/time/LocalDateTime;
+  #243 = NameAndType        #129:#130     // writer:LNpyWriter;
+  #244 = NameAndType        #168:#169     // toItems:(JFFFF)Ljava/util/Map;
+  #245 = NameAndType        #319:#320     // write:(Ljava/util/Map;)V
+  #246 = Class              #321          // java/time/LocalDateTime
+  #247 = NameAndType        #322:#323     // of:(IIIIII)Ljava/time/LocalDateTime;
+  #248 = Class              #324          // java/time/ZoneOffset
+  #249 = NameAndType        #325:#326     // UTC:Ljava/time/ZoneOffset;
+  #250 = NameAndType        #327:#328     // toEpochSecond:(Ljava/time/ZoneOffset;)J
+  #251 = NameAndType        #329:#330     // getInt:(I)I
+  #252 = Utf8               NpyWriter
+  #253 = NameAndType        #112:#113     // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+  #254 = NameAndType        #131:#331     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
+  #255 = Utf8               time
+  #256 = Class              #332          // java/lang/Long
+  #257 = NameAndType        #297:#333     // valueOf:(J)Ljava/lang/Long;
+  #258 = Utf8               x
+  #259 = Class              #334          // java/lang/Float
+  #260 = NameAndType        #297:#335     // valueOf:(F)Ljava/lang/Float;
+  #261 = Utf8               y
+  #262 = Utf8               z
+  #263 = Utf8               temperature
+  #264 = Utf8               java/util/LinkedHashMap
+  #265 = Utf8               Long
+  #266 = Utf8               Float
+  #267 = Class              #336          // java/util/Collections
+  #268 = NameAndType        #337:#338     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+  #269 = Utf8               java/lang/Object
+  #270 = Utf8               java/util/Map
+  #271 = Utf8               java/nio/channels/FileChannel
+  #272 = Utf8               java/nio/ByteBuffer
+  #273 = Utf8               java/lang/String
+  #274 = Utf8               (Ljava/lang/String;)V
+  #275 = Utf8               getChannel
+  #276 = Utf8               ()Ljava/nio/channels/FileChannel;
+  #277 = Utf8               size
+  #278 = Utf8               ()J
+  #279 = Utf8               allocate
+  #280 = Utf8               (I)Ljava/nio/ByteBuffer;
+  #281 = Utf8               (Ljava/nio/ByteBuffer;)I
+  #282 = Utf8               clear
+  #283 = Utf8               ()Ljava/nio/Buffer;
+  #284 = Utf8               java/lang/System
+  #285 = Utf8               out
+  #286 = Utf8               Ljava/io/PrintStream;
+  #287 = Utf8               append
+  #288 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #289 = Utf8               (J)Ljava/lang/StringBuilder;
+  #290 = Utf8               toString
+  #291 = Utf8               java/io/PrintStream
+  #292 = Utf8               print
+  #293 = Utf8               close
+  #294 = Utf8               addSuppressed
+  #295 = Utf8               (Ljava/lang/Throwable;)V
+  #296 = Utf8               printStackTrace
+  #297 = Utf8               valueOf
+  #298 = Utf8               (I)Ljava/lang/String;
+  #299 = Utf8               put
+  #300 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #301 = Utf8               (F)Ljava/lang/String;
+  #302 = Utf8               flip
+  #303 = Utf8               java/nio/ByteOrder
+  #304 = Utf8               LITTLE_ENDIAN
+  #305 = Utf8               Ljava/nio/ByteOrder;
+  #306 = Utf8               order
+  #307 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #308 = Utf8               get
+  #309 = Utf8               ()B
+  #310 = Utf8               (C)Ljava/lang/StringBuilder;
+  #311 = Utf8               equals
+  #312 = Utf8               (Ljava/lang/Object;)Z
+  #313 = Utf8               (I)B
+  #314 = Utf8               getShort
+  #315 = Utf8               (I)S
+  #316 = Utf8               java/lang/Math
+  #317 = Utf8               floor
+  #318 = Utf8               (D)D
+  #319 = Utf8               write
+  #320 = Utf8               (Ljava/util/Map;)V
+  #321 = Utf8               java/time/LocalDateTime
+  #322 = Utf8               of
+  #323 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
+  #324 = Utf8               java/time/ZoneOffset
+  #325 = Utf8               UTC
+  #326 = Utf8               Ljava/time/ZoneOffset;
+  #327 = Utf8               toEpochSecond
+  #328 = Utf8               (Ljava/time/ZoneOffset;)J
+  #329 = Utf8               getInt
+  #330 = Utf8               (I)I
+  #331 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
+  #332 = Utf8               java/lang/Long
+  #333 = Utf8               (J)Ljava/lang/Long;
+  #334 = Utf8               java/lang/Float
+  #335 = Utf8               (F)Ljava/lang/Float;
+  #336 = Utf8               java/util/Collections
+  #337 = Utf8               unmodifiableMap
+  #338 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
 {
   private static final int BLOCKSIZE = 512;
     descriptor: I
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
     ConstantValue: int 512
 
   private static final java.util.Map<java.lang.String, java.lang.String> ITEM_NAMES_AND_TYPES;
@@ -421,231 +429,303 @@
         line 52: 40
         line 53: 45
 
   public java.util.Map<java.lang.String, java.lang.String> read();
     descriptor: ()Ljava/util/Map;
     flags: (0x0001) ACC_PUBLIC
     Code:
-      stack=6, locals=9, args_size=1
+      stack=6, locals=15, args_size=1
          0: new           #11                 // class java/util/HashMap
          3: dup
          4: invokespecial #12                 // Method java/util/HashMap."<init>":()V
          7: astore_1
          8: new           #13                 // class java/io/FileInputStream
         11: dup
         12: aload_0
         13: getfield      #8                  // Field accFile:Ljava/lang/String;
         16: invokespecial #14                 // Method java/io/FileInputStream."<init>":(Ljava/lang/String;)V
         19: astore_2
-        20: aload_2
-        21: invokevirtual #15                 // Method java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
-        24: astore_3
-        25: aload_0
-        26: invokespecial #16                 // Method setupWriter:()V
-        29: iconst_0
-        30: istore        4
-        32: aload_3
-        33: invokevirtual #17                 // Method java/nio/channels/FileChannel.size:()J
-        36: ldc2_w        #19                 // long 512l
-        39: ldiv
-        40: lstore        5
-        42: sipush        512
-        45: invokestatic  #21                 // Method java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
-        48: astore        7
-        50: aload_3
-        51: aload         7
-        53: invokevirtual #22                 // Method java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
-        56: iconst_m1
-        57: if_icmpeq     141
-        60: aload_0
-        61: aload         7
-        63: invokespecial #23                 // Method parseCwaBlock:(Ljava/nio/ByteBuffer;)V
-        66: aload         7
-        68: invokevirtual #24                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-        71: pop
-        72: iinc          4, 1
-        75: aload_0
-        76: getfield      #10                 // Field verbose:Z
-        79: ifeq          50
-        82: iload         4
-        84: sipush        10000
-        87: irem
-        88: ifeq          100
-        91: iload         4
-        93: i2l
-        94: lload         5
-        96: lcmp
-        97: ifne          50
-       100: getstatic     #25                 // Field java/lang/System.out:Ljava/io/PrintStream;
-       103: new           #26                 // class java/lang/StringBuilder
-       106: dup
-       107: invokespecial #27                 // Method java/lang/StringBuilder."<init>":()V
-       110: ldc           #28                 // String Reading file...
-       112: invokevirtual #29                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       115: iload         4
-       117: bipush        100
-       119: imul
-       120: i2l
-       121: lload         5
-       123: ldiv
-       124: invokevirtual #30                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-       127: ldc           #31                 // String %\r
-       129: invokevirtual #29                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       132: invokevirtual #32                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
-       135: invokevirtual #33                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
-       138: goto          50
-       141: aload_0
-       142: iconst_1
-       143: putfield      #3                  // Field statusOK:I
-       146: aload_3
-       147: ifnull        182
-       150: aload_3
-       151: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
-       154: goto          182
-       157: astore        4
-       159: aload_3
-       160: ifnull        179
-       163: aload_3
-       164: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
-       167: goto          179
-       170: astore        5
-       172: aload         4
+        20: aconst_null
+        21: astore_3
+        22: aload_2
+        23: invokevirtual #15                 // Method java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
+        26: astore        4
+        28: aconst_null
+        29: astore        5
+        31: aload_0
+        32: invokespecial #16                 // Method setupWriter:()V
+        35: iconst_0
+        36: istore        6
+        38: aload         4
+        40: invokevirtual #17                 // Method java/nio/channels/FileChannel.size:()J
+        43: ldc2_w        #19                 // long 512l
+        46: ldiv
+        47: lstore        7
+        49: sipush        512
+        52: invokestatic  #21                 // Method java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
+        55: astore        9
+        57: aload         4
+        59: aload         9
+        61: invokevirtual #22                 // Method java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
+        64: iconst_m1
+        65: if_icmpeq     149
+        68: aload_0
+        69: aload         9
+        71: invokespecial #23                 // Method parseCwaBlock:(Ljava/nio/ByteBuffer;)V
+        74: aload         9
+        76: invokevirtual #24                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+        79: pop
+        80: iinc          6, 1
+        83: aload_0
+        84: getfield      #10                 // Field verbose:Z
+        87: ifeq          57
+        90: iload         6
+        92: sipush        10000
+        95: irem
+        96: ifeq          108
+        99: iload         6
+       101: i2l
+       102: lload         7
+       104: lcmp
+       105: ifne          57
+       108: getstatic     #25                 // Field java/lang/System.out:Ljava/io/PrintStream;
+       111: new           #26                 // class java/lang/StringBuilder
+       114: dup
+       115: invokespecial #27                 // Method java/lang/StringBuilder."<init>":()V
+       118: ldc           #28                 // String Reading file...
+       120: invokevirtual #29                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       123: iload         6
+       125: bipush        100
+       127: imul
+       128: i2l
+       129: lload         7
+       131: ldiv
+       132: invokevirtual #30                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+       135: ldc           #31                 // String %\r
+       137: invokevirtual #29                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       140: invokevirtual #32                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+       143: invokevirtual #33                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
+       146: goto          57
+       149: aload_0
+       150: iconst_1
+       151: putfield      #3                  // Field statusOK:I
+       154: aload         4
+       156: ifnull        241
+       159: aload         5
+       161: ifnull        184
+       164: aload         4
+       166: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
+       169: goto          241
+       172: astore        6
        174: aload         5
-       176: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-       179: aload         4
-       181: athrow
-       182: aload_2
-       183: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
-       186: goto          207
-       189: astore_3
-       190: aload_2
-       191: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
-       194: goto          205
-       197: astore        4
-       199: aload_3
-       200: aload         4
-       202: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-       205: aload_3
-       206: athrow
-       207: aload_0
-       208: invokespecial #38                 // Method closeWriter:()V
-       211: goto          240
-       214: astore_2
-       215: aload_0
-       216: iconst_0
-       217: putfield      #3                  // Field statusOK:I
-       220: aload_2
-       221: invokevirtual #40                 // Method java/lang/Exception.printStackTrace:()V
-       224: aload_0
-       225: invokespecial #38                 // Method closeWriter:()V
-       228: goto          240
-       231: astore        8
-       233: aload_0
-       234: invokespecial #38                 // Method closeWriter:()V
-       237: aload         8
-       239: athrow
-       240: aload_1
-       241: ldc           #41                 // String ReadOK
-       243: aload_0
-       244: getfield      #3                  // Field statusOK:I
-       247: invokestatic  #42                 // Method java/lang/String.valueOf:(I)Ljava/lang/String;
-       250: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-       255: pop
-       256: aload_1
-       257: ldc           #44                 // String ReadErrors
-       259: aload_0
-       260: getfield      #6                  // Field errCounter:I
-       263: invokestatic  #42                 // Method java/lang/String.valueOf:(I)Ljava/lang/String;
-       266: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-       271: pop
-       272: aload_1
-       273: ldc           #45                 // String SampleRate
-       275: aload_0
-       276: getfield      #5                  // Field sampleRate:F
-       279: invokestatic  #46                 // Method java/lang/String.valueOf:(F)Ljava/lang/String;
-       282: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-       287: pop
-       288: aload_1
-       289: areturn
+       176: aload         6
+       178: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       181: goto          241
+       184: aload         4
+       186: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
+       189: goto          241
+       192: astore        6
+       194: aload         6
+       196: astore        5
+       198: aload         6
+       200: athrow
+       201: astore        10
+       203: aload         4
+       205: ifnull        238
+       208: aload         5
+       210: ifnull        233
+       213: aload         4
+       215: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
+       218: goto          238
+       221: astore        11
+       223: aload         5
+       225: aload         11
+       227: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       230: goto          238
+       233: aload         4
+       235: invokevirtual #34                 // Method java/nio/channels/FileChannel.close:()V
+       238: aload         10
+       240: athrow
+       241: aload_2
+       242: ifnull        317
+       245: aload_3
+       246: ifnull        267
+       249: aload_2
+       250: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
+       253: goto          317
+       256: astore        4
+       258: aload_3
+       259: aload         4
+       261: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       264: goto          317
+       267: aload_2
+       268: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
+       271: goto          317
+       274: astore        4
+       276: aload         4
+       278: astore_3
+       279: aload         4
+       281: athrow
+       282: astore        12
+       284: aload_2
+       285: ifnull        314
+       288: aload_3
+       289: ifnull        310
+       292: aload_2
+       293: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
+       296: goto          314
+       299: astore        13
+       301: aload_3
+       302: aload         13
+       304: invokevirtual #36                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       307: goto          314
+       310: aload_2
+       311: invokevirtual #37                 // Method java/io/FileInputStream.close:()V
+       314: aload         12
+       316: athrow
+       317: aload_0
+       318: invokespecial #38                 // Method closeWriter:()V
+       321: goto          350
+       324: astore_2
+       325: aload_0
+       326: iconst_0
+       327: putfield      #3                  // Field statusOK:I
+       330: aload_2
+       331: invokevirtual #40                 // Method java/lang/Exception.printStackTrace:()V
+       334: aload_0
+       335: invokespecial #38                 // Method closeWriter:()V
+       338: goto          350
+       341: astore        14
+       343: aload_0
+       344: invokespecial #38                 // Method closeWriter:()V
+       347: aload         14
+       349: athrow
+       350: aload_1
+       351: ldc           #41                 // String ReadOK
+       353: aload_0
+       354: getfield      #3                  // Field statusOK:I
+       357: invokestatic  #42                 // Method java/lang/String.valueOf:(I)Ljava/lang/String;
+       360: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+       365: pop
+       366: aload_1
+       367: ldc           #44                 // String ReadErrors
+       369: aload_0
+       370: getfield      #6                  // Field errCounter:I
+       373: invokestatic  #42                 // Method java/lang/String.valueOf:(I)Ljava/lang/String;
+       376: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+       381: pop
+       382: aload_1
+       383: ldc           #45                 // String SampleRate
+       385: aload_0
+       386: getfield      #5                  // Field sampleRate:F
+       389: invokestatic  #46                 // Method java/lang/String.valueOf:(F)Ljava/lang/String;
+       392: invokeinterface #43,  3           // InterfaceMethod java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+       397: pop
+       398: aload_1
+       399: areturn
       Exception table:
          from    to  target type
-            25   146   157   Class java/lang/Throwable
-           163   167   170   Class java/lang/Throwable
-            20   182   189   Class java/lang/Throwable
-           190   194   197   Class java/lang/Throwable
-             8   207   214   Class java/lang/Exception
-             8   207   231   any
-           214   224   231   any
-           231   233   231   any
+           164   169   172   Class java/lang/Throwable
+            31   154   192   Class java/lang/Throwable
+            31   154   201   any
+           213   218   221   Class java/lang/Throwable
+           192   203   201   any
+           249   253   256   Class java/lang/Throwable
+            22   241   274   Class java/lang/Throwable
+            22   241   282   any
+           292   296   299   Class java/lang/Throwable
+           274   284   282   any
+             8   317   324   Class java/lang/Exception
+             8   317   341   any
+           324   334   341   any
+           341   343   341   any
       LineNumberTable:
         line 58: 0
         line 60: 8
-        line 61: 20
-        line 63: 25
-        line 65: 29
-        line 66: 32
-        line 67: 42
-        line 69: 50
-        line 71: 60
-        line 72: 66
-        line 75: 72
-        line 76: 75
-        line 77: 82
-        line 78: 100
-        line 85: 141
-        line 87: 146
-        line 60: 157
-        line 87: 182
-        line 60: 189
-        line 92: 207
-        line 93: 211
-        line 87: 214
-        line 88: 215
-        line 89: 220
-        line 92: 224
-        line 93: 228
-        line 92: 231
-        line 93: 237
-        line 95: 240
-        line 96: 256
-        line 97: 272
-        line 99: 288
-      StackMapTable: number_of_entries = 14
+        line 61: 22
+        line 60: 28
+        line 63: 31
+        line 65: 35
+        line 66: 38
+        line 67: 49
+        line 69: 57
+        line 71: 68
+        line 72: 74
+        line 75: 80
+        line 76: 83
+        line 77: 90
+        line 78: 108
+        line 85: 149
+        line 87: 154
+        line 60: 192
+        line 87: 201
+        line 60: 274
+        line 87: 282
+        line 92: 317
+        line 93: 321
+        line 87: 324
+        line 88: 325
+        line 89: 330
+        line 92: 334
+        line 93: 338
+        line 92: 341
+        line 93: 347
+        line 95: 350
+        line 96: 366
+        line 97: 382
+        line 99: 398
+      StackMapTable: number_of_entries = 22
         frame_type = 255 /* full_frame */
-          offset_delta = 50
-          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/nio/channels/FileChannel, int, long, class java/nio/ByteBuffer ]
+          offset_delta = 57
+          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable, class java/nio/channels/FileChannel, class java/lang/Throwable, int, long, class java/nio/ByteBuffer ]
           stack = []
-        frame_type = 49 /* same */
+        frame_type = 50 /* same */
         frame_type = 40 /* same */
         frame_type = 255 /* full_frame */
-          offset_delta = 15
-          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/nio/channels/FileChannel ]
+          offset_delta = 22
+          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable, class java/nio/channels/FileChannel, class java/lang/Throwable ]
+          stack = [ class java/lang/Throwable ]
+        frame_type = 11 /* same */
+        frame_type = 71 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
+        frame_type = 72 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
         frame_type = 255 /* full_frame */
-          offset_delta = 12
-          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/nio/channels/FileChannel, class java/lang/Throwable ]
+          offset_delta = 19
+          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable, class java/nio/channels/FileChannel, class java/lang/Throwable, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Throwable ]
-        frame_type = 8 /* same */
-        frame_type = 249 /* chop */
+        frame_type = 11 /* same */
+        frame_type = 4 /* same */
+        frame_type = 255 /* full_frame */
           offset_delta = 2
+          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable ]
+          stack = []
+        frame_type = 78 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
+        frame_type = 10 /* same */
         frame_type = 70 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
+        frame_type = 71 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
         frame_type = 255 /* full_frame */
-          offset_delta = 7
-          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable ]
+          offset_delta = 16
+          locals = [ class AxivityReader, class java/util/Map, class java/io/FileInputStream, class java/lang/Throwable, top, top, top, top, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Throwable ]
-        frame_type = 7 /* same */
-        frame_type = 249 /* chop */
-          offset_delta = 1
+        frame_type = 10 /* same */
+        frame_type = 3 /* same */
+        frame_type = 255 /* full_frame */
+          offset_delta = 2
+          locals = [ class AxivityReader, class java/util/Map ]
+          stack = []
         frame_type = 70 /* same_locals_1_stack_item */
           stack = [ class java/lang/Exception ]
         frame_type = 80 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
         frame_type = 8 /* same */
-    Signature: #141                         // ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #145                         // ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   public static java.util.Map<java.lang.String, java.lang.String> read(java.lang.String, java.lang.String, boolean);
     descriptor: (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=5, locals=3, args_size=3
          0: new           #18                 // class AxivityReader
@@ -654,15 +734,15 @@
          5: aload_1
          6: iload_2
          7: invokespecial #47                 // Method "<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
         10: invokevirtual #48                 // Method read:()Ljava/util/Map;
         13: areturn
       LineNumberTable:
         line 105: 0
-    Signature: #143                         // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #147                         // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   public static java.util.Map<java.lang.String, java.lang.String> read(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=5, locals=2, args_size=2
          0: new           #18                 // class AxivityReader
@@ -671,15 +751,15 @@
          5: aload_1
          6: iconst_1
          7: invokespecial #47                 // Method "<init>":(Ljava/lang/String;Ljava/lang/String;Z)V
         10: invokevirtual #48                 // Method read:()Ljava/util/Map;
         13: areturn
       LineNumberTable:
         line 110: 0
-    Signature: #145                         // (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #149                         // (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   private void parseCwaBlock(java.nio.ByteBuffer);
     descriptor: (Ljava/nio/ByteBuffer;)V
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=8, locals=29, args_size=2
          0: aload_1
@@ -1449,15 +1529,15 @@
         line 297: 0
         line 298: 9
         line 299: 23
         line 300: 37
         line 301: 51
         line 302: 66
         line 304: 81
-    Signature: #166                         // (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #170                         // (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   private static java.util.Map<java.lang.String, java.lang.Object> toItems(long, double, double, double, double);
     descriptor: (JDDDD)Ljava/util/Map;
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=7, locals=10, args_size=5
          0: lload_0
@@ -1469,15 +1549,15 @@
          8: d2f
          9: dload         8
         11: d2f
         12: invokestatic  #82                 // Method toItems:(JFFFF)Ljava/util/Map;
         15: areturn
       LineNumberTable:
         line 309: 0
-    Signature: #168                         // (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #172                         // (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   static {};
     descriptor: ()V
     flags: (0x0008) ACC_STATIC
     Code:
       stack=3, locals=1, args_size=0
          0: new           #102                // class java/util/LinkedHashMap
```

### Comparing `actipy-2.0.3/actipy/AxivityReader.java` & `actipy-2.0.3.post0/src/actipy/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/actipy/GENEActivReader.class` & `actipy-2.0.3.post0/src/actipy/GENEActivReader.class`

 * *Files 6% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,267 +1,273 @@
-  SHA-256 checksum f784906f65f74f517d7973c4ed711221c7d7fb69b28cb3f94378a93eb962f037
+  SHA-256 checksum 6b803eb767d0299fdb3b95bd8413610c21697c18629fb4bc5b6f91fedc4c2bac
   Compiled from "GENEActivReader.java"
 public class GENEActivReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #73                         // GENEActivReader
   super_class: #74                        // java/lang/Object
   interfaces: 0, fields: 1, methods: 11, attributes: 1
 Constant pool:
-    #1 = Methodref          #74.#113      // java/lang/Object."<init>":()V
-    #2 = Methodref          #73.#114      // GENEActivReader.read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
-    #3 = Class              #115          // java/util/HashMap
-    #4 = Methodref          #3.#113       // java/util/HashMap."<init>":()V
+    #1 = Methodref          #74.#116      // java/lang/Object."<init>":()V
+    #2 = Methodref          #73.#117      // GENEActivReader.read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
+    #3 = Class              #118          // java/util/HashMap
+    #4 = Methodref          #3.#116       // java/util/HashMap."<init>":()V
     #5 = Double             -1.0d
-    #7 = Class              #116          // NpyWriter
-    #8 = Fieldref           #73.#117      // GENEActivReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-    #9 = Methodref          #7.#118       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
-   #10 = Class              #119          // java/io/BufferedReader
-   #11 = Class              #120          // java/io/FileReader
-   #12 = Methodref          #11.#121      // java/io/FileReader."<init>":(Ljava/lang/String;)V
-   #13 = Methodref          #10.#122      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
-   #14 = Methodref          #73.#123      // GENEActivReader.parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
-   #15 = String             #124          // yyyy-MM-dd HH:mm:ss:SSS
-   #16 = Methodref          #92.#125      // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-   #17 = Methodref          #73.#126      // GENEActivReader.readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
-   #18 = String             #127          // Time:
-   #19 = Methodref          #88.#128      // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #20 = Methodref          #129.#130     // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-   #21 = Fieldref           #131.#132     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
-   #22 = Methodref          #129.#133     // java/time/LocalDateTime.toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
-   #23 = Methodref          #134.#135     // java/time/Instant.toEpochMilli:()J
-   #24 = String             #136          // :
-   #25 = Methodref          #137.#138     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #26 = Class              #139          // java/lang/Exception
-   #27 = Methodref          #26.#140      // java/lang/Exception.printStackTrace:()V
-   #28 = Methodref          #88.#141      // java/lang/String.length:()I
-   #29 = Methodref          #73.#142      // GENEActivReader.getSignedIntFromHex:(Ljava/lang/String;II)I
+    #7 = Class              #119          // NpyWriter
+    #8 = Fieldref           #73.#120      // GENEActivReader.ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+    #9 = Methodref          #7.#121       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
+   #10 = Class              #122          // java/io/BufferedReader
+   #11 = Class              #123          // java/io/FileReader
+   #12 = Methodref          #11.#124      // java/io/FileReader."<init>":(Ljava/lang/String;)V
+   #13 = Methodref          #10.#125      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
+   #14 = Methodref          #73.#126      // GENEActivReader.parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
+   #15 = String             #127          // yyyy-MM-dd HH:mm:ss:SSS
+   #16 = Methodref          #128.#129     // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+   #17 = Methodref          #73.#130      // GENEActivReader.readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
+   #18 = String             #131          // Time:
+   #19 = Methodref          #132.#133     // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #20 = Methodref          #134.#135     // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+   #21 = Fieldref           #136.#137     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
+   #22 = Methodref          #134.#138     // java/time/LocalDateTime.toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
+   #23 = Methodref          #139.#140     // java/time/Instant.toEpochMilli:()J
+   #24 = String             #141          // :
+   #25 = Methodref          #142.#143     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #26 = Class              #144          // java/lang/Exception
+   #27 = Methodref          #26.#145      // java/lang/Exception.printStackTrace:()V
+   #28 = Methodref          #132.#146     // java/lang/String.length:()I
+   #29 = Methodref          #73.#147      // GENEActivReader.getSignedIntFromHex:(Ljava/lang/String;II)I
    #30 = Double             100.0d
    #32 = Double             1000.0d
-   #34 = Methodref          #73.#143      // GENEActivReader.toItems:(JDDDD)Ljava/util/Map;
-   #35 = Methodref          #7.#144       // NpyWriter.write:(Ljava/util/Map;)V
-   #36 = Fieldref           #145.#146     // java/lang/System.out:Ljava/io/PrintStream;
-   #37 = Class              #147          // java/lang/StringBuilder
-   #38 = Methodref          #37.#113      // java/lang/StringBuilder."<init>":()V
-   #39 = String             #148          // Reading file...
-   #40 = Methodref          #37.#149      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #41 = Methodref          #37.#150      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #42 = String             #151          // %\r
-   #43 = Methodref          #37.#152      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #44 = Methodref          #153.#154     // java/io/PrintStream.print:(Ljava/lang/String;)V
-   #45 = Methodref          #10.#155      // java/io/BufferedReader.close:()V
-   #46 = Methodref          #7.#155       // NpyWriter.close:()V
-   #47 = String             #156          // ReadOK
-   #48 = Methodref          #88.#157      // java/lang/String.valueOf:(I)Ljava/lang/String;
-   #49 = InterfaceMethodref #89.#158      // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-   #50 = String             #159          // ReadErrors
-   #51 = String             #160          // SampleRate
-   #52 = Methodref          #88.#161      // java/lang/String.valueOf:(D)Ljava/lang/String;
-   #53 = Methodref          #162.#163     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
-   #54 = String             #164          //
-   #55 = Methodref          #10.#165      // java/io/BufferedReader.readLine:()Ljava/lang/String;
-   #56 = Methodref          #88.#166      // java/lang/String.substring:(II)Ljava/lang/String;
-   #57 = Methodref          #162.#167     // java/lang/Integer.parseInt:(Ljava/lang/String;I)I
-   #58 = Fieldref           #168.#169     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
-   #59 = Methodref          #168.#170     // java/util/concurrent/TimeUnit.toNanos:(J)J
-   #60 = String             #171          // time
-   #61 = Methodref          #172.#173     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-   #62 = String             #174          // x
-   #63 = Methodref          #175.#176     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
-   #64 = String             #177          // y
-   #65 = String             #178          // z
-   #66 = String             #179          // temperature
-   #67 = Methodref          #73.#180      // GENEActivReader.toItems:(JFFFF)Ljava/util/Map;
-   #68 = Class              #181          // java/util/LinkedHashMap
-   #69 = Methodref          #68.#113      // java/util/LinkedHashMap."<init>":()V
-   #70 = String             #182          // Long
-   #71 = String             #183          // Float
-   #72 = Methodref          #184.#185     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-   #73 = Class              #186          // GENEActivReader
-   #74 = Class              #187          // java/lang/Object
+   #34 = Methodref          #73.#148      // GENEActivReader.toItems:(JDDDD)Ljava/util/Map;
+   #35 = Methodref          #7.#149       // NpyWriter.write:(Ljava/util/Map;)V
+   #36 = Fieldref           #150.#151     // java/lang/System.out:Ljava/io/PrintStream;
+   #37 = Class              #152          // java/lang/StringBuilder
+   #38 = Methodref          #37.#116      // java/lang/StringBuilder."<init>":()V
+   #39 = String             #153          // Reading file...
+   #40 = Methodref          #37.#154      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #41 = Methodref          #37.#155      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #42 = String             #156          // %\r
+   #43 = Methodref          #37.#157      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #44 = Methodref          #158.#159     // java/io/PrintStream.print:(Ljava/lang/String;)V
+   #45 = Methodref          #10.#160      // java/io/BufferedReader.close:()V
+   #46 = Methodref          #7.#160       // NpyWriter.close:()V
+   #47 = String             #161          // ReadOK
+   #48 = Methodref          #132.#162     // java/lang/String.valueOf:(I)Ljava/lang/String;
+   #49 = InterfaceMethodref #163.#164     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+   #50 = String             #165          // ReadErrors
+   #51 = String             #166          // SampleRate
+   #52 = Methodref          #132.#167     // java/lang/String.valueOf:(D)Ljava/lang/String;
+   #53 = Methodref          #168.#169     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
+   #54 = String             #170          //
+   #55 = Methodref          #10.#171      // java/io/BufferedReader.readLine:()Ljava/lang/String;
+   #56 = Methodref          #132.#172     // java/lang/String.substring:(II)Ljava/lang/String;
+   #57 = Methodref          #168.#173     // java/lang/Integer.parseInt:(Ljava/lang/String;I)I
+   #58 = Fieldref           #174.#175     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
+   #59 = Methodref          #174.#176     // java/util/concurrent/TimeUnit.toNanos:(J)J
+   #60 = String             #177          // time
+   #61 = Methodref          #178.#179     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+   #62 = String             #180          // x
+   #63 = Methodref          #181.#182     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
+   #64 = String             #183          // y
+   #65 = String             #184          // z
+   #66 = String             #185          // temperature
+   #67 = Methodref          #73.#186      // GENEActivReader.toItems:(JFFFF)Ljava/util/Map;
+   #68 = Class              #187          // java/util/LinkedHashMap
+   #69 = Methodref          #68.#116      // java/util/LinkedHashMap."<init>":()V
+   #70 = String             #188          // Long
+   #71 = String             #189          // Float
+   #72 = Methodref          #190.#191     // java/util/Collections.unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+   #73 = Class              #192          // GENEActivReader
+   #74 = Class              #193          // java/lang/Object
    #75 = Utf8               ITEM_NAMES_AND_TYPES
    #76 = Utf8               Ljava/util/Map;
    #77 = Utf8               Signature
    #78 = Utf8               Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
    #79 = Utf8               <init>
    #80 = Utf8               ()V
    #81 = Utf8               Code
    #82 = Utf8               LineNumberTable
    #83 = Utf8               read
    #84 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map;
    #85 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
    #86 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
    #87 = Utf8               StackMapTable
-   #88 = Class              #188          // java/lang/String
-   #89 = Class              #189          // java/util/Map
-   #90 = Class              #190          // "[D"
-   #91 = Class              #191          // "[I"
-   #92 = Class              #192          // java/time/format/DateTimeFormatter
-   #93 = Class              #193          // java/lang/Throwable
-   #94 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-   #95 = Utf8               parseBinFileHeader
-   #96 = Utf8               (Ljava/io/BufferedReader;II[D[I)I
-   #97 = Utf8               readLine
-   #98 = Utf8               (Ljava/io/BufferedReader;)Ljava/lang/String;
-   #99 = Utf8               getSignedIntFromHex
-  #100 = Utf8               (Ljava/lang/String;II)I
-  #101 = Utf8               getEpochMillis
-  #102 = Utf8               (Ljava/time/LocalDateTime;)J
-  #103 = Utf8               secs2Nanos
-  #104 = Utf8               (D)J
-  #105 = Utf8               toItems
-  #106 = Utf8               (JFFFF)Ljava/util/Map;
-  #107 = Utf8               (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #108 = Utf8               (JDDDD)Ljava/util/Map;
-  #109 = Utf8               (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
-  #110 = Utf8               <clinit>
-  #111 = Utf8               SourceFile
-  #112 = Utf8               GENEActivReader.java
-  #113 = NameAndType        #79:#80       // "<init>":()V
-  #114 = NameAndType        #83:#86       // read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
-  #115 = Utf8               java/util/HashMap
-  #116 = Utf8               NpyWriter
-  #117 = NameAndType        #75:#76       // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
-  #118 = NameAndType        #79:#194      // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
-  #119 = Utf8               java/io/BufferedReader
-  #120 = Utf8               java/io/FileReader
-  #121 = NameAndType        #79:#195      // "<init>":(Ljava/lang/String;)V
-  #122 = NameAndType        #79:#196      // "<init>":(Ljava/io/Reader;)V
-  #123 = NameAndType        #95:#96       // parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
-  #124 = Utf8               yyyy-MM-dd HH:mm:ss:SSS
-  #125 = NameAndType        #197:#198     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-  #126 = NameAndType        #97:#98       // readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
-  #127 = Utf8               Time:
-  #128 = NameAndType        #199:#200     // split:(Ljava/lang/String;)[Ljava/lang/String;
-  #129 = Class              #201          // java/time/LocalDateTime
-  #130 = NameAndType        #202:#203     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-  #131 = Class              #204          // java/time/ZoneOffset
-  #132 = NameAndType        #205:#206     // UTC:Ljava/time/ZoneOffset;
-  #133 = NameAndType        #207:#208     // toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
-  #134 = Class              #209          // java/time/Instant
-  #135 = NameAndType        #210:#211     // toEpochMilli:()J
-  #136 = Utf8               :
-  #137 = Class              #212          // java/lang/Double
-  #138 = NameAndType        #213:#214     // parseDouble:(Ljava/lang/String;)D
-  #139 = Utf8               java/lang/Exception
-  #140 = NameAndType        #215:#80      // printStackTrace:()V
-  #141 = NameAndType        #216:#217     // length:()I
-  #142 = NameAndType        #99:#100      // getSignedIntFromHex:(Ljava/lang/String;II)I
-  #143 = NameAndType        #105:#108     // toItems:(JDDDD)Ljava/util/Map;
-  #144 = NameAndType        #218:#219     // write:(Ljava/util/Map;)V
-  #145 = Class              #220          // java/lang/System
-  #146 = NameAndType        #221:#222     // out:Ljava/io/PrintStream;
-  #147 = Utf8               java/lang/StringBuilder
-  #148 = Utf8               Reading file...
-  #149 = NameAndType        #223:#224     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #150 = NameAndType        #223:#225     // append:(I)Ljava/lang/StringBuilder;
-  #151 = Utf8               %\r
-  #152 = NameAndType        #226:#227     // toString:()Ljava/lang/String;
-  #153 = Class              #228          // java/io/PrintStream
-  #154 = NameAndType        #229:#195     // print:(Ljava/lang/String;)V
-  #155 = NameAndType        #230:#80      // close:()V
-  #156 = Utf8               ReadOK
-  #157 = NameAndType        #231:#232     // valueOf:(I)Ljava/lang/String;
-  #158 = NameAndType        #233:#234     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #159 = Utf8               ReadErrors
-  #160 = Utf8               SampleRate
-  #161 = NameAndType        #231:#235     // valueOf:(D)Ljava/lang/String;
-  #162 = Class              #236          // java/lang/Integer
-  #163 = NameAndType        #237:#238     // parseInt:(Ljava/lang/String;)I
-  #164 = Utf8
-  #165 = NameAndType        #97:#227      // readLine:()Ljava/lang/String;
-  #166 = NameAndType        #239:#240     // substring:(II)Ljava/lang/String;
-  #167 = NameAndType        #237:#241     // parseInt:(Ljava/lang/String;I)I
-  #168 = Class              #242          // java/util/concurrent/TimeUnit
-  #169 = NameAndType        #243:#244     // SECONDS:Ljava/util/concurrent/TimeUnit;
-  #170 = NameAndType        #245:#246     // toNanos:(J)J
-  #171 = Utf8               time
-  #172 = Class              #247          // java/lang/Long
-  #173 = NameAndType        #231:#248     // valueOf:(J)Ljava/lang/Long;
-  #174 = Utf8               x
-  #175 = Class              #249          // java/lang/Float
-  #176 = NameAndType        #231:#250     // valueOf:(F)Ljava/lang/Float;
-  #177 = Utf8               y
-  #178 = Utf8               z
-  #179 = Utf8               temperature
-  #180 = NameAndType        #105:#106     // toItems:(JFFFF)Ljava/util/Map;
-  #181 = Utf8               java/util/LinkedHashMap
-  #182 = Utf8               Long
-  #183 = Utf8               Float
-  #184 = Class              #251          // java/util/Collections
-  #185 = NameAndType        #252:#253     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
-  #186 = Utf8               GENEActivReader
-  #187 = Utf8               java/lang/Object
-  #188 = Utf8               java/lang/String
-  #189 = Utf8               java/util/Map
-  #190 = Utf8               [D
-  #191 = Utf8               [I
-  #192 = Utf8               java/time/format/DateTimeFormatter
-  #193 = Utf8               java/lang/Throwable
-  #194 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
-  #195 = Utf8               (Ljava/lang/String;)V
-  #196 = Utf8               (Ljava/io/Reader;)V
-  #197 = Utf8               ofPattern
-  #198 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-  #199 = Utf8               split
-  #200 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #201 = Utf8               java/time/LocalDateTime
-  #202 = Utf8               parse
-  #203 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-  #204 = Utf8               java/time/ZoneOffset
-  #205 = Utf8               UTC
-  #206 = Utf8               Ljava/time/ZoneOffset;
-  #207 = Utf8               toInstant
-  #208 = Utf8               (Ljava/time/ZoneOffset;)Ljava/time/Instant;
-  #209 = Utf8               java/time/Instant
-  #210 = Utf8               toEpochMilli
-  #211 = Utf8               ()J
-  #212 = Utf8               java/lang/Double
-  #213 = Utf8               parseDouble
-  #214 = Utf8               (Ljava/lang/String;)D
-  #215 = Utf8               printStackTrace
-  #216 = Utf8               length
-  #217 = Utf8               ()I
-  #218 = Utf8               write
-  #219 = Utf8               (Ljava/util/Map;)V
-  #220 = Utf8               java/lang/System
-  #221 = Utf8               out
-  #222 = Utf8               Ljava/io/PrintStream;
-  #223 = Utf8               append
-  #224 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #225 = Utf8               (I)Ljava/lang/StringBuilder;
-  #226 = Utf8               toString
-  #227 = Utf8               ()Ljava/lang/String;
-  #228 = Utf8               java/io/PrintStream
-  #229 = Utf8               print
-  #230 = Utf8               close
-  #231 = Utf8               valueOf
-  #232 = Utf8               (I)Ljava/lang/String;
-  #233 = Utf8               put
-  #234 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #235 = Utf8               (D)Ljava/lang/String;
-  #236 = Utf8               java/lang/Integer
-  #237 = Utf8               parseInt
-  #238 = Utf8               (Ljava/lang/String;)I
-  #239 = Utf8               substring
-  #240 = Utf8               (II)Ljava/lang/String;
-  #241 = Utf8               (Ljava/lang/String;I)I
-  #242 = Utf8               java/util/concurrent/TimeUnit
-  #243 = Utf8               SECONDS
-  #244 = Utf8               Ljava/util/concurrent/TimeUnit;
-  #245 = Utf8               toNanos
-  #246 = Utf8               (J)J
-  #247 = Utf8               java/lang/Long
-  #248 = Utf8               (J)Ljava/lang/Long;
-  #249 = Utf8               java/lang/Float
-  #250 = Utf8               (F)Ljava/lang/Float;
-  #251 = Utf8               java/util/Collections
-  #252 = Utf8               unmodifiableMap
-  #253 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
+   #88 = Class              #194          // java/lang/String
+   #89 = Class              #195          // java/util/Map
+   #90 = Class              #119          // NpyWriter
+   #91 = Class              #122          // java/io/BufferedReader
+   #92 = Class              #196          // "[D"
+   #93 = Class              #197          // "[I"
+   #94 = Class              #198          // java/time/format/DateTimeFormatter
+   #95 = Class              #144          // java/lang/Exception
+   #96 = Class              #199          // java/lang/Throwable
+   #97 = Utf8               (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+   #98 = Utf8               parseBinFileHeader
+   #99 = Utf8               (Ljava/io/BufferedReader;II[D[I)I
+  #100 = Utf8               readLine
+  #101 = Utf8               (Ljava/io/BufferedReader;)Ljava/lang/String;
+  #102 = Utf8               getSignedIntFromHex
+  #103 = Utf8               (Ljava/lang/String;II)I
+  #104 = Utf8               getEpochMillis
+  #105 = Utf8               (Ljava/time/LocalDateTime;)J
+  #106 = Utf8               secs2Nanos
+  #107 = Utf8               (D)J
+  #108 = Utf8               toItems
+  #109 = Utf8               (JFFFF)Ljava/util/Map;
+  #110 = Utf8               (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #111 = Utf8               (JDDDD)Ljava/util/Map;
+  #112 = Utf8               (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+  #113 = Utf8               <clinit>
+  #114 = Utf8               SourceFile
+  #115 = Utf8               GENEActivReader.java
+  #116 = NameAndType        #79:#80       // "<init>":()V
+  #117 = NameAndType        #83:#86       // read:(Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map;
+  #118 = Utf8               java/util/HashMap
+  #119 = Utf8               NpyWriter
+  #120 = NameAndType        #75:#76       // ITEM_NAMES_AND_TYPES:Ljava/util/Map;
+  #121 = NameAndType        #79:#200      // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
+  #122 = Utf8               java/io/BufferedReader
+  #123 = Utf8               java/io/FileReader
+  #124 = NameAndType        #79:#201      // "<init>":(Ljava/lang/String;)V
+  #125 = NameAndType        #79:#202      // "<init>":(Ljava/io/Reader;)V
+  #126 = NameAndType        #98:#99       // parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
+  #127 = Utf8               yyyy-MM-dd HH:mm:ss:SSS
+  #128 = Class              #198          // java/time/format/DateTimeFormatter
+  #129 = NameAndType        #203:#204     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+  #130 = NameAndType        #100:#101     // readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
+  #131 = Utf8               Time:
+  #132 = Class              #194          // java/lang/String
+  #133 = NameAndType        #205:#206     // split:(Ljava/lang/String;)[Ljava/lang/String;
+  #134 = Class              #207          // java/time/LocalDateTime
+  #135 = NameAndType        #208:#209     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+  #136 = Class              #210          // java/time/ZoneOffset
+  #137 = NameAndType        #211:#212     // UTC:Ljava/time/ZoneOffset;
+  #138 = NameAndType        #213:#214     // toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
+  #139 = Class              #215          // java/time/Instant
+  #140 = NameAndType        #216:#217     // toEpochMilli:()J
+  #141 = Utf8               :
+  #142 = Class              #218          // java/lang/Double
+  #143 = NameAndType        #219:#220     // parseDouble:(Ljava/lang/String;)D
+  #144 = Utf8               java/lang/Exception
+  #145 = NameAndType        #221:#80      // printStackTrace:()V
+  #146 = NameAndType        #222:#223     // length:()I
+  #147 = NameAndType        #102:#103     // getSignedIntFromHex:(Ljava/lang/String;II)I
+  #148 = NameAndType        #108:#111     // toItems:(JDDDD)Ljava/util/Map;
+  #149 = NameAndType        #224:#225     // write:(Ljava/util/Map;)V
+  #150 = Class              #226          // java/lang/System
+  #151 = NameAndType        #227:#228     // out:Ljava/io/PrintStream;
+  #152 = Utf8               java/lang/StringBuilder
+  #153 = Utf8               Reading file...
+  #154 = NameAndType        #229:#230     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #155 = NameAndType        #229:#231     // append:(I)Ljava/lang/StringBuilder;
+  #156 = Utf8               %\r
+  #157 = NameAndType        #232:#233     // toString:()Ljava/lang/String;
+  #158 = Class              #234          // java/io/PrintStream
+  #159 = NameAndType        #235:#201     // print:(Ljava/lang/String;)V
+  #160 = NameAndType        #236:#80      // close:()V
+  #161 = Utf8               ReadOK
+  #162 = NameAndType        #237:#238     // valueOf:(I)Ljava/lang/String;
+  #163 = Class              #195          // java/util/Map
+  #164 = NameAndType        #239:#240     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #165 = Utf8               ReadErrors
+  #166 = Utf8               SampleRate
+  #167 = NameAndType        #237:#241     // valueOf:(D)Ljava/lang/String;
+  #168 = Class              #242          // java/lang/Integer
+  #169 = NameAndType        #243:#244     // parseInt:(Ljava/lang/String;)I
+  #170 = Utf8
+  #171 = NameAndType        #100:#233     // readLine:()Ljava/lang/String;
+  #172 = NameAndType        #245:#246     // substring:(II)Ljava/lang/String;
+  #173 = NameAndType        #243:#247     // parseInt:(Ljava/lang/String;I)I
+  #174 = Class              #248          // java/util/concurrent/TimeUnit
+  #175 = NameAndType        #249:#250     // SECONDS:Ljava/util/concurrent/TimeUnit;
+  #176 = NameAndType        #251:#252     // toNanos:(J)J
+  #177 = Utf8               time
+  #178 = Class              #253          // java/lang/Long
+  #179 = NameAndType        #237:#254     // valueOf:(J)Ljava/lang/Long;
+  #180 = Utf8               x
+  #181 = Class              #255          // java/lang/Float
+  #182 = NameAndType        #237:#256     // valueOf:(F)Ljava/lang/Float;
+  #183 = Utf8               y
+  #184 = Utf8               z
+  #185 = Utf8               temperature
+  #186 = NameAndType        #108:#109     // toItems:(JFFFF)Ljava/util/Map;
+  #187 = Utf8               java/util/LinkedHashMap
+  #188 = Utf8               Long
+  #189 = Utf8               Float
+  #190 = Class              #257          // java/util/Collections
+  #191 = NameAndType        #258:#259     // unmodifiableMap:(Ljava/util/Map;)Ljava/util/Map;
+  #192 = Utf8               GENEActivReader
+  #193 = Utf8               java/lang/Object
+  #194 = Utf8               java/lang/String
+  #195 = Utf8               java/util/Map
+  #196 = Utf8               [D
+  #197 = Utf8               [I
+  #198 = Utf8               java/time/format/DateTimeFormatter
+  #199 = Utf8               java/lang/Throwable
+  #200 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
+  #201 = Utf8               (Ljava/lang/String;)V
+  #202 = Utf8               (Ljava/io/Reader;)V
+  #203 = Utf8               ofPattern
+  #204 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+  #205 = Utf8               split
+  #206 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #207 = Utf8               java/time/LocalDateTime
+  #208 = Utf8               parse
+  #209 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+  #210 = Utf8               java/time/ZoneOffset
+  #211 = Utf8               UTC
+  #212 = Utf8               Ljava/time/ZoneOffset;
+  #213 = Utf8               toInstant
+  #214 = Utf8               (Ljava/time/ZoneOffset;)Ljava/time/Instant;
+  #215 = Utf8               java/time/Instant
+  #216 = Utf8               toEpochMilli
+  #217 = Utf8               ()J
+  #218 = Utf8               java/lang/Double
+  #219 = Utf8               parseDouble
+  #220 = Utf8               (Ljava/lang/String;)D
+  #221 = Utf8               printStackTrace
+  #222 = Utf8               length
+  #223 = Utf8               ()I
+  #224 = Utf8               write
+  #225 = Utf8               (Ljava/util/Map;)V
+  #226 = Utf8               java/lang/System
+  #227 = Utf8               out
+  #228 = Utf8               Ljava/io/PrintStream;
+  #229 = Utf8               append
+  #230 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #231 = Utf8               (I)Ljava/lang/StringBuilder;
+  #232 = Utf8               toString
+  #233 = Utf8               ()Ljava/lang/String;
+  #234 = Utf8               java/io/PrintStream
+  #235 = Utf8               print
+  #236 = Utf8               close
+  #237 = Utf8               valueOf
+  #238 = Utf8               (I)Ljava/lang/String;
+  #239 = Utf8               put
+  #240 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #241 = Utf8               (D)Ljava/lang/String;
+  #242 = Utf8               java/lang/Integer
+  #243 = Utf8               parseInt
+  #244 = Utf8               (Ljava/lang/String;)I
+  #245 = Utf8               substring
+  #246 = Utf8               (II)Ljava/lang/String;
+  #247 = Utf8               (Ljava/lang/String;I)I
+  #248 = Utf8               java/util/concurrent/TimeUnit
+  #249 = Utf8               SECONDS
+  #250 = Utf8               Ljava/util/concurrent/TimeUnit;
+  #251 = Utf8               toNanos
+  #252 = Utf8               (J)J
+  #253 = Utf8               java/lang/Long
+  #254 = Utf8               (J)Ljava/lang/Long;
+  #255 = Utf8               java/lang/Float
+  #256 = Utf8               (F)Ljava/lang/Float;
+  #257 = Utf8               java/util/Collections
+  #258 = Utf8               unmodifiableMap
+  #259 = Utf8               (Ljava/util/Map;)Ljava/util/Map;
 {
   private static final java.util.Map<java.lang.String, java.lang.String> ITEM_NAMES_AND_TYPES;
     descriptor: Ljava/util/Map;
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
     Signature: #78                          // Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   public GENEActivReader();
@@ -759,15 +765,15 @@
           locals = [ class java/lang/String, class java/lang/String, int, class java/util/Map, int, int, int, int, double, int, class NpyWriter, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Exception ]
         frame_type = 6 /* same */
         frame_type = 255 /* full_frame */
           offset_delta = 2
           locals = [ class java/lang/String, class java/lang/String, int, class java/util/Map, int, int, int, int, double, int, class NpyWriter ]
           stack = []
-    Signature: #94                          // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #97                          // (Ljava/lang/String;Ljava/lang/String;Z)Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   private static int parseBinFileHeader(java.io.BufferedReader, int, int, double[], int[]);
     descriptor: (Ljava/io/BufferedReader;II[D[I)I
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=4, locals=9, args_size=5
          0: iconst_0
@@ -1064,15 +1070,15 @@
         line 247: 0
         line 248: 9
         line 249: 23
         line 250: 37
         line 251: 51
         line 252: 66
         line 253: 81
-    Signature: #107                         // (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #110                         // (JFFFF)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   private static java.util.Map<java.lang.String, java.lang.Object> toItems(long, double, double, double, double);
     descriptor: (JDDDD)Ljava/util/Map;
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=7, locals=10, args_size=5
          0: lload_0
@@ -1084,15 +1090,15 @@
          8: d2f
          9: dload         8
         11: d2f
         12: invokestatic  #67                 // Method toItems:(JFFFF)Ljava/util/Map;
         15: areturn
       LineNumberTable:
         line 258: 0
-    Signature: #109                         // (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
+    Signature: #112                         // (JDDDD)Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
 
   static {};
     descriptor: ()V
     flags: (0x0008) ACC_STATIC
     Code:
       stack=3, locals=1, args_size=0
          0: new           #68                 // class java/util/LinkedHashMap
```

### Comparing `actipy-2.0.3/actipy/GENEActivReader.java` & `actipy-2.0.3.post0/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/actipy/NpyWriter.class` & `actipy-2.0.3.post0/src/actipy/NpyWriter.class`

 * *Files 18% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,156 +1,156 @@
-  SHA-256 checksum e608c6032d56a835b9c5ac014d90f24a39d9154776eb2a9fb2fc76610c1e773d
+  SHA-256 checksum 60e7fab461f42066770900025e39bbe2d51b5b74d8a3a4561f7f5966bd5b34a0
   Compiled from "NpyWriter.java"
 public class NpyWriter
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #1                          // NpyWriter
   super_class: #139                       // java/lang/Object
   interfaces: 0, fields: 15, methods: 18, attributes: 2
 Constant pool:
-    #1 = Class              #214          // NpyWriter
-    #2 = Methodref          #139.#215     // java/lang/Object."<init>":()V
-    #3 = Fieldref           #1.#216       // NpyWriter.linesWritten:I
-    #4 = Fieldref           #1.#217       // NpyWriter.outputFile:Ljava/lang/String;
-    #5 = Fieldref           #1.#218       // NpyWriter.itemNamesAndTypes:Ljava/util/Map;
-    #6 = Methodref          #1.#219       // NpyWriter.getBytesPerLine:(Ljava/util/Map;)I
-    #7 = Methodref          #220.#221     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
-    #8 = Fieldref           #1.#222       // NpyWriter.NATIVE_BYTE_ORDER:Ljava/nio/ByteOrder;
-    #9 = Methodref          #220.#223     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-   #10 = Fieldref           #1.#224       // NpyWriter.buf:Ljava/nio/ByteBuffer;
-   #11 = Class              #225          // java/io/File
-   #12 = Methodref          #11.#226      // java/io/File."<init>":(Ljava/lang/String;)V
-   #13 = Fieldref           #1.#227       // NpyWriter.file:Ljava/io/File;
-   #14 = Class              #228          // java/io/RandomAccessFile
-   #15 = String             #229          // rw
-   #16 = Methodref          #14.#230      // java/io/RandomAccessFile."<init>":(Ljava/io/File;Ljava/lang/String;)V
-   #17 = Fieldref           #1.#231       // NpyWriter.raf:Ljava/io/RandomAccessFile;
-   #18 = Methodref          #14.#232      // java/io/RandomAccessFile.setLength:(J)V
-   #19 = Fieldref           #1.#233       // NpyWriter.NPY_HEADER:[B
-   #20 = Class              #234          // java/lang/StringBuilder
-   #21 = Methodref          #20.#215      // java/lang/StringBuilder."<init>":()V
-   #22 = Class              #235          // java/lang/String
-   #23 = Methodref          #22.#236      // java/lang/String."<init>":([C)V
-   #24 = String             #237          // \u0000
-   #25 = String             #238          //
-   #26 = Methodref          #22.#239      // java/lang/String.replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-   #27 = Methodref          #20.#240      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #28 = String             #241          // \n
-   #29 = Methodref          #20.#242      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #30 = Methodref          #14.#243      // java/io/RandomAccessFile.writeBytes:(Ljava/lang/String;)V
-   #31 = Class              #244          // java/io/IOException
-   #32 = Class              #245          // java/lang/RuntimeException
-   #33 = String             #246          // The .npy file
-   #34 = String             #247          //  could not be created
-   #35 = Methodref          #32.#226      // java/lang/RuntimeException."<init>":(Ljava/lang/String;)V
-   #36 = Methodref          #1.#248       // NpyWriter.getDefaultItemNamesAndTypes:()Ljava/util/Map;
-   #37 = Methodref          #1.#249       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
-   #38 = Methodref          #1.#250       // NpyWriter.putItems:(Ljava/util/Map;)V
-   #39 = Methodref          #220.#251     // java/nio/ByteBuffer.hasRemaining:()Z
-   #40 = Methodref          #220.#252     // java/nio/ByteBuffer.array:()[B
-   #41 = Methodref          #14.#253      // java/io/RandomAccessFile.write:([B)V
-   #42 = Methodref          #220.#254     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-   #43 = InterfaceMethodref #179.#255     // java/util/Map.entrySet:()Ljava/util/Set;
-   #44 = InterfaceMethodref #256.#257     // java/util/Set.iterator:()Ljava/util/Iterator;
-   #45 = InterfaceMethodref #187.#258     // java/util/Iterator.hasNext:()Z
-   #46 = InterfaceMethodref #187.#259     // java/util/Iterator.next:()Ljava/lang/Object;
-   #47 = Class              #260          // java/util/Map$Entry
-   #48 = InterfaceMethodref #47.#263      // java/util/Map$Entry.getKey:()Ljava/lang/Object;
-   #49 = InterfaceMethodref #47.#264      // java/util/Map$Entry.getValue:()Ljava/lang/Object;
-   #50 = InterfaceMethodref #179.#265     // java/util/Map.get:(Ljava/lang/Object;)Ljava/lang/Object;
-   #51 = Methodref          #1.#266       // NpyWriter.putItem:(Ljava/lang/Object;Ljava/lang/String;)V
-   #52 = Methodref          #22.#267      // java/lang/String.hashCode:()I
-   #53 = String             #268          // Integer
-   #54 = Methodref          #22.#269      // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #55 = String             #270          // Short
-   #56 = String             #271          // Long
-   #57 = String             #272          // Float
-   #58 = String             #273          // Double
-   #59 = Class              #274          // java/lang/Integer
-   #60 = Methodref          #59.#275      // java/lang/Integer.intValue:()I
-   #61 = Methodref          #220.#276     // java/nio/ByteBuffer.putInt:(I)Ljava/nio/ByteBuffer;
-   #62 = Class              #277          // java/lang/Short
-   #63 = Methodref          #62.#278      // java/lang/Short.shortValue:()S
-   #64 = Methodref          #220.#279     // java/nio/ByteBuffer.putShort:(S)Ljava/nio/ByteBuffer;
-   #65 = Class              #280          // java/lang/Long
-   #66 = Methodref          #65.#281      // java/lang/Long.longValue:()J
-   #67 = Methodref          #220.#282     // java/nio/ByteBuffer.putLong:(J)Ljava/nio/ByteBuffer;
-   #68 = Class              #283          // java/lang/Float
-   #69 = Methodref          #68.#284      // java/lang/Float.floatValue:()F
-   #70 = Methodref          #220.#285     // java/nio/ByteBuffer.putFloat:(F)Ljava/nio/ByteBuffer;
-   #71 = Class              #286          // java/lang/Double
-   #72 = Methodref          #71.#287      // java/lang/Double.doubleValue:()D
-   #73 = Methodref          #220.#288     // java/nio/ByteBuffer.putDouble:(D)Ljava/nio/ByteBuffer;
-   #74 = Class              #289          // java/lang/IllegalArgumentException
-   #75 = String             #290          // Unrecognized item type:
-   #76 = Methodref          #74.#226      // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
-   #77 = Methodref          #14.#291      // java/io/RandomAccessFile.seek:(J)V
-   #78 = Methodref          #14.#292      // java/io/RandomAccessFile.write:(I)V
-   #79 = String             #293          // { \'descr\': [
-   #80 = String             #294          // (\'
-   #81 = String             #295          // \',\'
-   #82 = Methodref          #1.#296       // NpyWriter.toNpyTypeStr:(Ljava/lang/String;)Ljava/lang/String;
-   #83 = String             #297          // \')
-   #84 = InterfaceMethodref #256.#298     // java/util/Set.size:()I
-   #85 = String             #299          // ,
-   #86 = String             #300          // ], \'fortran_order\': False, \'shape\': (
-   #87 = Methodref          #20.#301      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #88 = String             #302          // ,), }
-   #89 = Methodref          #22.#303      // java/lang/String.length:()I
-   #90 = String             #304          // header is too big to be written.
-   #91 = Methodref          #20.#305      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
-   #92 = Methodref          #1.#306       // NpyWriter.writeLEShort:(Ljava/io/RandomAccessFile;S)V
-   #93 = Methodref          #14.#307      // java/io/RandomAccessFile.length:()J
-   #94 = Methodref          #31.#308      // java/io/IOException.printStackTrace:()V
-   #95 = String             #309          // The .npy file could not write a header created
-   #96 = Methodref          #1.#310       // NpyWriter.finalFlush:()V
-   #97 = Class              #311          // java/util/zip/GZIPOutputStream
-   #98 = Class              #312          // java/io/FileOutputStream
-   #99 = Methodref          #98.#313      // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
-  #100 = Methodref          #97.#314      // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
-  #101 = Methodref          #14.#315      // java/io/RandomAccessFile.read:([B)I
-  #102 = Methodref          #97.#316      // java/util/zip/GZIPOutputStream.write:([BII)V
-  #103 = Methodref          #97.#317      // java/util/zip/GZIPOutputStream.close:()V
-  #104 = Class              #318          // java/lang/Throwable
-  #105 = Methodref          #104.#319     // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-  #106 = String             #320          // .gz
-  #107 = Methodref          #1.#321       // NpyWriter.compress:(Ljava/lang/String;)V
-  #108 = Methodref          #1.#322       // NpyWriter.writeHeader:()V
-  #109 = Methodref          #14.#317      // java/io/RandomAccessFile.close:()V
-  #110 = Methodref          #1.#317       // NpyWriter.close:()V
-  #111 = Methodref          #11.#323      // java/io/File.delete:()Z
+    #1 = Class              #220          // NpyWriter
+    #2 = Methodref          #139.#221     // java/lang/Object."<init>":()V
+    #3 = Fieldref           #1.#222       // NpyWriter.linesWritten:I
+    #4 = Fieldref           #1.#223       // NpyWriter.outputFile:Ljava/lang/String;
+    #5 = Fieldref           #1.#224       // NpyWriter.itemNamesAndTypes:Ljava/util/Map;
+    #6 = Methodref          #1.#225       // NpyWriter.getBytesPerLine:(Ljava/util/Map;)I
+    #7 = Methodref          #226.#227     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
+    #8 = Fieldref           #1.#228       // NpyWriter.NATIVE_BYTE_ORDER:Ljava/nio/ByteOrder;
+    #9 = Methodref          #226.#229     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+   #10 = Fieldref           #1.#230       // NpyWriter.buf:Ljava/nio/ByteBuffer;
+   #11 = Class              #231          // java/io/File
+   #12 = Methodref          #11.#232      // java/io/File."<init>":(Ljava/lang/String;)V
+   #13 = Fieldref           #1.#233       // NpyWriter.file:Ljava/io/File;
+   #14 = Class              #234          // java/io/RandomAccessFile
+   #15 = String             #235          // rw
+   #16 = Methodref          #14.#236      // java/io/RandomAccessFile."<init>":(Ljava/io/File;Ljava/lang/String;)V
+   #17 = Fieldref           #1.#237       // NpyWriter.raf:Ljava/io/RandomAccessFile;
+   #18 = Methodref          #14.#238      // java/io/RandomAccessFile.setLength:(J)V
+   #19 = Fieldref           #1.#239       // NpyWriter.NPY_HEADER:[B
+   #20 = Class              #240          // java/lang/StringBuilder
+   #21 = Methodref          #20.#221      // java/lang/StringBuilder."<init>":()V
+   #22 = Class              #241          // java/lang/String
+   #23 = Methodref          #22.#242      // java/lang/String."<init>":([C)V
+   #24 = String             #243          // \u0000
+   #25 = String             #244          //
+   #26 = Methodref          #22.#245      // java/lang/String.replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+   #27 = Methodref          #20.#246      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #28 = String             #247          // \n
+   #29 = Methodref          #20.#248      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #30 = Methodref          #14.#249      // java/io/RandomAccessFile.writeBytes:(Ljava/lang/String;)V
+   #31 = Class              #250          // java/io/IOException
+   #32 = Class              #251          // java/lang/RuntimeException
+   #33 = String             #252          // The .npy file
+   #34 = String             #253          //  could not be created
+   #35 = Methodref          #32.#232      // java/lang/RuntimeException."<init>":(Ljava/lang/String;)V
+   #36 = Methodref          #1.#254       // NpyWriter.getDefaultItemNamesAndTypes:()Ljava/util/Map;
+   #37 = Methodref          #1.#255       // NpyWriter."<init>":(Ljava/lang/String;Ljava/util/Map;)V
+   #38 = Methodref          #1.#256       // NpyWriter.putItems:(Ljava/util/Map;)V
+   #39 = Methodref          #226.#257     // java/nio/ByteBuffer.hasRemaining:()Z
+   #40 = Methodref          #226.#258     // java/nio/ByteBuffer.array:()[B
+   #41 = Methodref          #14.#259      // java/io/RandomAccessFile.write:([B)V
+   #42 = Methodref          #226.#260     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+   #43 = InterfaceMethodref #261.#262     // java/util/Map.entrySet:()Ljava/util/Set;
+   #44 = InterfaceMethodref #263.#264     // java/util/Set.iterator:()Ljava/util/Iterator;
+   #45 = InterfaceMethodref #265.#266     // java/util/Iterator.hasNext:()Z
+   #46 = InterfaceMethodref #265.#267     // java/util/Iterator.next:()Ljava/lang/Object;
+   #47 = Class              #268          // java/util/Map$Entry
+   #48 = InterfaceMethodref #47.#271      // java/util/Map$Entry.getKey:()Ljava/lang/Object;
+   #49 = InterfaceMethodref #47.#272      // java/util/Map$Entry.getValue:()Ljava/lang/Object;
+   #50 = InterfaceMethodref #261.#273     // java/util/Map.get:(Ljava/lang/Object;)Ljava/lang/Object;
+   #51 = Methodref          #1.#274       // NpyWriter.putItem:(Ljava/lang/Object;Ljava/lang/String;)V
+   #52 = Methodref          #22.#275      // java/lang/String.hashCode:()I
+   #53 = String             #276          // Integer
+   #54 = Methodref          #22.#277      // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #55 = String             #278          // Short
+   #56 = String             #279          // Long
+   #57 = String             #280          // Float
+   #58 = String             #281          // Double
+   #59 = Class              #282          // java/lang/Integer
+   #60 = Methodref          #59.#283      // java/lang/Integer.intValue:()I
+   #61 = Methodref          #226.#284     // java/nio/ByteBuffer.putInt:(I)Ljava/nio/ByteBuffer;
+   #62 = Class              #285          // java/lang/Short
+   #63 = Methodref          #62.#286      // java/lang/Short.shortValue:()S
+   #64 = Methodref          #226.#287     // java/nio/ByteBuffer.putShort:(S)Ljava/nio/ByteBuffer;
+   #65 = Class              #288          // java/lang/Long
+   #66 = Methodref          #65.#289      // java/lang/Long.longValue:()J
+   #67 = Methodref          #226.#290     // java/nio/ByteBuffer.putLong:(J)Ljava/nio/ByteBuffer;
+   #68 = Class              #291          // java/lang/Float
+   #69 = Methodref          #68.#292      // java/lang/Float.floatValue:()F
+   #70 = Methodref          #226.#293     // java/nio/ByteBuffer.putFloat:(F)Ljava/nio/ByteBuffer;
+   #71 = Class              #294          // java/lang/Double
+   #72 = Methodref          #71.#295      // java/lang/Double.doubleValue:()D
+   #73 = Methodref          #226.#296     // java/nio/ByteBuffer.putDouble:(D)Ljava/nio/ByteBuffer;
+   #74 = Class              #297          // java/lang/IllegalArgumentException
+   #75 = String             #298          // Unrecognized item type:
+   #76 = Methodref          #74.#232      // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
+   #77 = Methodref          #14.#299      // java/io/RandomAccessFile.seek:(J)V
+   #78 = Methodref          #14.#300      // java/io/RandomAccessFile.write:(I)V
+   #79 = String             #301          // { \'descr\': [
+   #80 = String             #302          // (\'
+   #81 = String             #303          // \',\'
+   #82 = Methodref          #1.#304       // NpyWriter.toNpyTypeStr:(Ljava/lang/String;)Ljava/lang/String;
+   #83 = String             #305          // \')
+   #84 = InterfaceMethodref #263.#306     // java/util/Set.size:()I
+   #85 = String             #307          // ,
+   #86 = String             #308          // ], \'fortran_order\': False, \'shape\': (
+   #87 = Methodref          #20.#309      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #88 = String             #310          // ,), }
+   #89 = Methodref          #22.#311      // java/lang/String.length:()I
+   #90 = String             #312          // header is too big to be written.
+   #91 = Methodref          #20.#313      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
+   #92 = Methodref          #1.#314       // NpyWriter.writeLEShort:(Ljava/io/RandomAccessFile;S)V
+   #93 = Methodref          #14.#315      // java/io/RandomAccessFile.length:()J
+   #94 = Methodref          #31.#316      // java/io/IOException.printStackTrace:()V
+   #95 = String             #317          // The .npy file could not write a header created
+   #96 = Methodref          #1.#318       // NpyWriter.finalFlush:()V
+   #97 = Class              #319          // java/util/zip/GZIPOutputStream
+   #98 = Class              #320          // java/io/FileOutputStream
+   #99 = Methodref          #98.#321      // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
+  #100 = Methodref          #97.#322      // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
+  #101 = Methodref          #14.#323      // java/io/RandomAccessFile.read:([B)I
+  #102 = Methodref          #97.#324      // java/util/zip/GZIPOutputStream.write:([BII)V
+  #103 = Methodref          #97.#325      // java/util/zip/GZIPOutputStream.close:()V
+  #104 = Class              #326          // java/lang/Throwable
+  #105 = Methodref          #104.#327     // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+  #106 = String             #328          // .gz
+  #107 = Methodref          #1.#329       // NpyWriter.compress:(Ljava/lang/String;)V
+  #108 = Methodref          #1.#330       // NpyWriter.writeHeader:()V
+  #109 = Methodref          #14.#325      // java/io/RandomAccessFile.close:()V
+  #110 = Methodref          #1.#325       // NpyWriter.close:()V
+  #111 = Methodref          #11.#331      // java/io/File.delete:()Z
   #112 = Integer            65280
-  #113 = Methodref          #14.#324      // java/io/RandomAccessFile.writeShort:(I)V
-  #114 = Fieldref           #325.#326     // java/lang/System.out:Ljava/io/PrintStream;
-  #115 = String             #327          // writing:
-  #116 = Methodref          #328.#329     // java/io/PrintStream.println:(Ljava/lang/String;)V
-  #117 = Methodref          #14.#330      // java/io/RandomAccessFile.writeByte:(I)V
-  #118 = Class              #331          // java/util/LinkedHashMap
-  #119 = Methodref          #118.#215     // java/util/LinkedHashMap."<init>":()V
-  #120 = String             #332          // time
-  #121 = InterfaceMethodref #179.#333     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #122 = String             #334          // x
-  #123 = String             #335          // y
-  #124 = String             #336          // z
-  #125 = InterfaceMethodref #179.#337     // java/util/Map.values:()Ljava/util/Collection;
-  #126 = InterfaceMethodref #338.#257     // java/util/Collection.iterator:()Ljava/util/Iterator;
-  #127 = Methodref          #1.#339       // NpyWriter.getBytesPerType:(Ljava/lang/String;)I
-  #128 = Fieldref           #1.#340       // NpyWriter.NUMPY_BYTE_ORDER:C
-  #129 = String             #341          // i4
-  #130 = String             #342          // i2
-  #131 = String             #343          // i8
-  #132 = String             #344          // f4
-  #133 = String             #345          // f8
-  #134 = Methodref          #346.#347     // java/nio/ByteOrder.nativeOrder:()Ljava/nio/ByteOrder;
-  #135 = Fieldref           #346.#348     // java/nio/ByteOrder.BIG_ENDIAN:Ljava/nio/ByteOrder;
-  #136 = String             #349          // XNUMPY
-  #137 = Fieldref           #350.#351     // java/nio/charset/StandardCharsets.US_ASCII:Ljava/nio/charset/Charset;
-  #138 = Methodref          #22.#352      // java/lang/String.getBytes:(Ljava/nio/charset/Charset;)[B
-  #139 = Class              #353          // java/lang/Object
+  #113 = Methodref          #14.#332      // java/io/RandomAccessFile.writeShort:(I)V
+  #114 = Fieldref           #333.#334     // java/lang/System.out:Ljava/io/PrintStream;
+  #115 = String             #335          // writing:
+  #116 = Methodref          #336.#337     // java/io/PrintStream.println:(Ljava/lang/String;)V
+  #117 = Methodref          #14.#338      // java/io/RandomAccessFile.writeByte:(I)V
+  #118 = Class              #339          // java/util/LinkedHashMap
+  #119 = Methodref          #118.#221     // java/util/LinkedHashMap."<init>":()V
+  #120 = String             #340          // time
+  #121 = InterfaceMethodref #261.#341     // java/util/Map.put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #122 = String             #342          // x
+  #123 = String             #343          // y
+  #124 = String             #344          // z
+  #125 = InterfaceMethodref #261.#345     // java/util/Map.values:()Ljava/util/Collection;
+  #126 = InterfaceMethodref #346.#264     // java/util/Collection.iterator:()Ljava/util/Iterator;
+  #127 = Methodref          #1.#347       // NpyWriter.getBytesPerType:(Ljava/lang/String;)I
+  #128 = Fieldref           #1.#348       // NpyWriter.NUMPY_BYTE_ORDER:C
+  #129 = String             #349          // i4
+  #130 = String             #350          // i2
+  #131 = String             #351          // i8
+  #132 = String             #352          // f4
+  #133 = String             #353          // f8
+  #134 = Methodref          #354.#355     // java/nio/ByteOrder.nativeOrder:()Ljava/nio/ByteOrder;
+  #135 = Fieldref           #354.#356     // java/nio/ByteOrder.BIG_ENDIAN:Ljava/nio/ByteOrder;
+  #136 = String             #357          // XNUMPY
+  #137 = Fieldref           #358.#359     // java/nio/charset/StandardCharsets.US_ASCII:Ljava/nio/charset/Charset;
+  #138 = Methodref          #22.#360      // java/lang/String.getBytes:(Ljava/nio/charset/Charset;)[B
+  #139 = Class              #361          // java/lang/Object
   #140 = Utf8               BUFSIZE
   #141 = Utf8               I
   #142 = Utf8               ConstantValue
   #143 = Integer            8192
   #144 = Utf8               NATIVE_BYTE_ORDER
   #145 = Utf8               Ljava/nio/ByteOrder;
   #146 = Utf8               NUMPY_BYTE_ORDER
@@ -182,284 +182,292 @@
   #172 = Utf8               Ljava/io/RandomAccessFile;
   #173 = Utf8               linesWritten
   #174 = Utf8               <init>
   #175 = Utf8               (Ljava/lang/String;Ljava/util/Map;)V
   #176 = Utf8               Code
   #177 = Utf8               LineNumberTable
   #178 = Utf8               StackMapTable
-  #179 = Class              #354          // java/util/Map
-  #180 = Utf8               (Ljava/lang/String;Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)V
-  #181 = Utf8               (Ljava/lang/String;)V
-  #182 = Utf8               write
-  #183 = Utf8               (Ljava/util/Map;)V
-  #184 = Utf8               Exceptions
-  #185 = Utf8               (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
-  #186 = Utf8               putItems
-  #187 = Class              #355          // java/util/Iterator
-  #188 = Utf8               putItem
-  #189 = Utf8               (Ljava/lang/Object;Ljava/lang/String;)V
-  #190 = Utf8               writeHeader
-  #191 = Utf8               ()V
-  #192 = Utf8               compress
-  #193 = Class              #160          // "[B"
-  #194 = Utf8               finalFlush
-  #195 = Utf8               close
-  #196 = Utf8               closeAndDelete
-  #197 = Utf8               writeLEShort
-  #198 = Utf8               (Ljava/io/RandomAccessFile;S)V
-  #199 = Utf8               writeLEInt
-  #200 = Utf8               (Ljava/io/RandomAccessFile;I)V
-  #201 = Utf8               getDefaultItemNamesAndTypes
-  #202 = Utf8               ()Ljava/util/Map;
-  #203 = Utf8               ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
-  #204 = Utf8               getBytesPerLine
-  #205 = Utf8               (Ljava/util/Map;)I
-  #206 = Utf8               (Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)I
-  #207 = Utf8               getBytesPerType
-  #208 = Utf8               (Ljava/lang/String;)I
-  #209 = Utf8               toNpyTypeStr
-  #210 = Utf8               (Ljava/lang/String;)Ljava/lang/String;
-  #211 = Utf8               <clinit>
-  #212 = Utf8               SourceFile
-  #213 = Utf8               NpyWriter.java
-  #214 = Utf8               NpyWriter
-  #215 = NameAndType        #174:#191     // "<init>":()V
-  #216 = NameAndType        #173:#141     // linesWritten:I
-  #217 = NameAndType        #161:#162     // outputFile:Ljava/lang/String;
-  #218 = NameAndType        #163:#164     // itemNamesAndTypes:Ljava/util/Map;
-  #219 = NameAndType        #204:#205     // getBytesPerLine:(Ljava/util/Map;)I
-  #220 = Class              #356          // java/nio/ByteBuffer
-  #221 = NameAndType        #357:#358     // allocate:(I)Ljava/nio/ByteBuffer;
-  #222 = NameAndType        #144:#145     // NATIVE_BYTE_ORDER:Ljava/nio/ByteOrder;
-  #223 = NameAndType        #359:#360     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #224 = NameAndType        #167:#168     // buf:Ljava/nio/ByteBuffer;
-  #225 = Utf8               java/io/File
-  #226 = NameAndType        #174:#181     // "<init>":(Ljava/lang/String;)V
-  #227 = NameAndType        #169:#170     // file:Ljava/io/File;
-  #228 = Utf8               java/io/RandomAccessFile
-  #229 = Utf8               rw
-  #230 = NameAndType        #174:#361     // "<init>":(Ljava/io/File;Ljava/lang/String;)V
-  #231 = NameAndType        #171:#172     // raf:Ljava/io/RandomAccessFile;
-  #232 = NameAndType        #362:#363     // setLength:(J)V
-  #233 = NameAndType        #159:#160     // NPY_HEADER:[B
-  #234 = Utf8               java/lang/StringBuilder
-  #235 = Utf8               java/lang/String
-  #236 = NameAndType        #174:#364     // "<init>":([C)V
-  #237 = Utf8               \u0000
-  #238 = Utf8
-  #239 = NameAndType        #365:#366     // replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-  #240 = NameAndType        #367:#368     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #241 = Utf8               \n
-  #242 = NameAndType        #369:#370     // toString:()Ljava/lang/String;
-  #243 = NameAndType        #371:#181     // writeBytes:(Ljava/lang/String;)V
-  #244 = Utf8               java/io/IOException
-  #245 = Utf8               java/lang/RuntimeException
-  #246 = Utf8               The .npy file
-  #247 = Utf8                could not be created
-  #248 = NameAndType        #201:#202     // getDefaultItemNamesAndTypes:()Ljava/util/Map;
-  #249 = NameAndType        #174:#175     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
-  #250 = NameAndType        #186:#183     // putItems:(Ljava/util/Map;)V
-  #251 = NameAndType        #372:#373     // hasRemaining:()Z
-  #252 = NameAndType        #374:#375     // array:()[B
-  #253 = NameAndType        #182:#376     // write:([B)V
-  #254 = NameAndType        #377:#378     // clear:()Ljava/nio/Buffer;
-  #255 = NameAndType        #379:#380     // entrySet:()Ljava/util/Set;
-  #256 = Class              #381          // java/util/Set
-  #257 = NameAndType        #382:#383     // iterator:()Ljava/util/Iterator;
-  #258 = NameAndType        #384:#373     // hasNext:()Z
-  #259 = NameAndType        #385:#386     // next:()Ljava/lang/Object;
-  #260 = Utf8               java/util/Map$Entry
-  #261 = Utf8               Entry
-  #262 = Utf8               InnerClasses
-  #263 = NameAndType        #387:#386     // getKey:()Ljava/lang/Object;
-  #264 = NameAndType        #388:#386     // getValue:()Ljava/lang/Object;
-  #265 = NameAndType        #389:#390     // get:(Ljava/lang/Object;)Ljava/lang/Object;
-  #266 = NameAndType        #188:#189     // putItem:(Ljava/lang/Object;Ljava/lang/String;)V
-  #267 = NameAndType        #391:#392     // hashCode:()I
-  #268 = Utf8               Integer
-  #269 = NameAndType        #393:#394     // equals:(Ljava/lang/Object;)Z
-  #270 = Utf8               Short
-  #271 = Utf8               Long
-  #272 = Utf8               Float
-  #273 = Utf8               Double
-  #274 = Utf8               java/lang/Integer
-  #275 = NameAndType        #395:#392     // intValue:()I
-  #276 = NameAndType        #396:#358     // putInt:(I)Ljava/nio/ByteBuffer;
-  #277 = Utf8               java/lang/Short
-  #278 = NameAndType        #397:#398     // shortValue:()S
-  #279 = NameAndType        #399:#400     // putShort:(S)Ljava/nio/ByteBuffer;
-  #280 = Utf8               java/lang/Long
-  #281 = NameAndType        #401:#402     // longValue:()J
-  #282 = NameAndType        #403:#404     // putLong:(J)Ljava/nio/ByteBuffer;
-  #283 = Utf8               java/lang/Float
-  #284 = NameAndType        #405:#406     // floatValue:()F
-  #285 = NameAndType        #407:#408     // putFloat:(F)Ljava/nio/ByteBuffer;
-  #286 = Utf8               java/lang/Double
-  #287 = NameAndType        #409:#410     // doubleValue:()D
-  #288 = NameAndType        #411:#412     // putDouble:(D)Ljava/nio/ByteBuffer;
-  #289 = Utf8               java/lang/IllegalArgumentException
-  #290 = Utf8               Unrecognized item type:
-  #291 = NameAndType        #413:#363     // seek:(J)V
-  #292 = NameAndType        #182:#414     // write:(I)V
-  #293 = Utf8               { \'descr\': [
-  #294 = Utf8               (\'
-  #295 = Utf8               \',\'
-  #296 = NameAndType        #209:#210     // toNpyTypeStr:(Ljava/lang/String;)Ljava/lang/String;
-  #297 = Utf8               \')
-  #298 = NameAndType        #415:#392     // size:()I
-  #299 = Utf8               ,
-  #300 = Utf8               ], \'fortran_order\': False, \'shape\': (
-  #301 = NameAndType        #367:#416     // append:(I)Ljava/lang/StringBuilder;
-  #302 = Utf8               ,), }
-  #303 = NameAndType        #417:#392     // length:()I
-  #304 = Utf8               header is too big to be written.
-  #305 = NameAndType        #367:#418     // append:(C)Ljava/lang/StringBuilder;
-  #306 = NameAndType        #197:#198     // writeLEShort:(Ljava/io/RandomAccessFile;S)V
-  #307 = NameAndType        #417:#402     // length:()J
-  #308 = NameAndType        #419:#191     // printStackTrace:()V
-  #309 = Utf8               The .npy file could not write a header created
-  #310 = NameAndType        #194:#191     // finalFlush:()V
-  #311 = Utf8               java/util/zip/GZIPOutputStream
-  #312 = Utf8               java/io/FileOutputStream
-  #313 = NameAndType        #174:#420     // "<init>":(Ljava/io/File;)V
-  #314 = NameAndType        #174:#421     // "<init>":(Ljava/io/OutputStream;)V
-  #315 = NameAndType        #422:#423     // read:([B)I
-  #316 = NameAndType        #182:#424     // write:([BII)V
-  #317 = NameAndType        #195:#191     // close:()V
-  #318 = Utf8               java/lang/Throwable
-  #319 = NameAndType        #425:#426     // addSuppressed:(Ljava/lang/Throwable;)V
-  #320 = Utf8               .gz
-  #321 = NameAndType        #192:#181     // compress:(Ljava/lang/String;)V
-  #322 = NameAndType        #190:#191     // writeHeader:()V
-  #323 = NameAndType        #427:#373     // delete:()Z
-  #324 = NameAndType        #428:#414     // writeShort:(I)V
-  #325 = Class              #429          // java/lang/System
-  #326 = NameAndType        #430:#431     // out:Ljava/io/PrintStream;
-  #327 = Utf8               writing:
-  #328 = Class              #432          // java/io/PrintStream
-  #329 = NameAndType        #433:#181     // println:(Ljava/lang/String;)V
-  #330 = NameAndType        #434:#414     // writeByte:(I)V
-  #331 = Utf8               java/util/LinkedHashMap
-  #332 = Utf8               time
-  #333 = NameAndType        #435:#436     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #334 = Utf8               x
-  #335 = Utf8               y
-  #336 = Utf8               z
-  #337 = NameAndType        #437:#438     // values:()Ljava/util/Collection;
-  #338 = Class              #439          // java/util/Collection
-  #339 = NameAndType        #207:#208     // getBytesPerType:(Ljava/lang/String;)I
-  #340 = NameAndType        #146:#147     // NUMPY_BYTE_ORDER:C
-  #341 = Utf8               i4
-  #342 = Utf8               i2
-  #343 = Utf8               i8
-  #344 = Utf8               f4
-  #345 = Utf8               f8
-  #346 = Class              #440          // java/nio/ByteOrder
-  #347 = NameAndType        #441:#442     // nativeOrder:()Ljava/nio/ByteOrder;
-  #348 = NameAndType        #443:#145     // BIG_ENDIAN:Ljava/nio/ByteOrder;
-  #349 = Utf8               XNUMPY
-  #350 = Class              #444          // java/nio/charset/StandardCharsets
-  #351 = NameAndType        #445:#446     // US_ASCII:Ljava/nio/charset/Charset;
-  #352 = NameAndType        #447:#448     // getBytes:(Ljava/nio/charset/Charset;)[B
-  #353 = Utf8               java/lang/Object
-  #354 = Utf8               java/util/Map
-  #355 = Utf8               java/util/Iterator
-  #356 = Utf8               java/nio/ByteBuffer
-  #357 = Utf8               allocate
-  #358 = Utf8               (I)Ljava/nio/ByteBuffer;
-  #359 = Utf8               order
-  #360 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #361 = Utf8               (Ljava/io/File;Ljava/lang/String;)V
-  #362 = Utf8               setLength
-  #363 = Utf8               (J)V
-  #364 = Utf8               ([C)V
-  #365 = Utf8               replace
-  #366 = Utf8               (Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-  #367 = Utf8               append
-  #368 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #369 = Utf8               toString
-  #370 = Utf8               ()Ljava/lang/String;
-  #371 = Utf8               writeBytes
-  #372 = Utf8               hasRemaining
-  #373 = Utf8               ()Z
-  #374 = Utf8               array
-  #375 = Utf8               ()[B
-  #376 = Utf8               ([B)V
-  #377 = Utf8               clear
-  #378 = Utf8               ()Ljava/nio/Buffer;
-  #379 = Utf8               entrySet
-  #380 = Utf8               ()Ljava/util/Set;
-  #381 = Utf8               java/util/Set
-  #382 = Utf8               iterator
-  #383 = Utf8               ()Ljava/util/Iterator;
-  #384 = Utf8               hasNext
-  #385 = Utf8               next
-  #386 = Utf8               ()Ljava/lang/Object;
-  #387 = Utf8               getKey
-  #388 = Utf8               getValue
-  #389 = Utf8               get
-  #390 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
-  #391 = Utf8               hashCode
-  #392 = Utf8               ()I
-  #393 = Utf8               equals
-  #394 = Utf8               (Ljava/lang/Object;)Z
-  #395 = Utf8               intValue
-  #396 = Utf8               putInt
-  #397 = Utf8               shortValue
-  #398 = Utf8               ()S
-  #399 = Utf8               putShort
-  #400 = Utf8               (S)Ljava/nio/ByteBuffer;
-  #401 = Utf8               longValue
-  #402 = Utf8               ()J
-  #403 = Utf8               putLong
-  #404 = Utf8               (J)Ljava/nio/ByteBuffer;
-  #405 = Utf8               floatValue
-  #406 = Utf8               ()F
-  #407 = Utf8               putFloat
-  #408 = Utf8               (F)Ljava/nio/ByteBuffer;
-  #409 = Utf8               doubleValue
-  #410 = Utf8               ()D
-  #411 = Utf8               putDouble
-  #412 = Utf8               (D)Ljava/nio/ByteBuffer;
-  #413 = Utf8               seek
-  #414 = Utf8               (I)V
-  #415 = Utf8               size
-  #416 = Utf8               (I)Ljava/lang/StringBuilder;
-  #417 = Utf8               length
-  #418 = Utf8               (C)Ljava/lang/StringBuilder;
-  #419 = Utf8               printStackTrace
-  #420 = Utf8               (Ljava/io/File;)V
-  #421 = Utf8               (Ljava/io/OutputStream;)V
-  #422 = Utf8               read
-  #423 = Utf8               ([B)I
-  #424 = Utf8               ([BII)V
-  #425 = Utf8               addSuppressed
-  #426 = Utf8               (Ljava/lang/Throwable;)V
-  #427 = Utf8               delete
-  #428 = Utf8               writeShort
-  #429 = Utf8               java/lang/System
-  #430 = Utf8               out
-  #431 = Utf8               Ljava/io/PrintStream;
-  #432 = Utf8               java/io/PrintStream
-  #433 = Utf8               println
-  #434 = Utf8               writeByte
-  #435 = Utf8               put
-  #436 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
-  #437 = Utf8               values
-  #438 = Utf8               ()Ljava/util/Collection;
-  #439 = Utf8               java/util/Collection
-  #440 = Utf8               java/nio/ByteOrder
-  #441 = Utf8               nativeOrder
-  #442 = Utf8               ()Ljava/nio/ByteOrder;
-  #443 = Utf8               BIG_ENDIAN
-  #444 = Utf8               java/nio/charset/StandardCharsets
-  #445 = Utf8               US_ASCII
-  #446 = Utf8               Ljava/nio/charset/Charset;
-  #447 = Utf8               getBytes
-  #448 = Utf8               (Ljava/nio/charset/Charset;)[B
+  #179 = Class              #220          // NpyWriter
+  #180 = Class              #241          // java/lang/String
+  #181 = Class              #362          // java/util/Map
+  #182 = Class              #250          // java/io/IOException
+  #183 = Utf8               (Ljava/lang/String;Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)V
+  #184 = Utf8               (Ljava/lang/String;)V
+  #185 = Utf8               write
+  #186 = Utf8               (Ljava/util/Map;)V
+  #187 = Utf8               Exceptions
+  #188 = Utf8               (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
+  #189 = Utf8               putItems
+  #190 = Class              #363          // java/util/Iterator
+  #191 = Utf8               putItem
+  #192 = Utf8               (Ljava/lang/Object;Ljava/lang/String;)V
+  #193 = Utf8               writeHeader
+  #194 = Utf8               ()V
+  #195 = Class              #268          // java/util/Map$Entry
+  #196 = Utf8               compress
+  #197 = Class              #319          // java/util/zip/GZIPOutputStream
+  #198 = Class              #326          // java/lang/Throwable
+  #199 = Class              #160          // "[B"
+  #200 = Utf8               finalFlush
+  #201 = Utf8               close
+  #202 = Utf8               closeAndDelete
+  #203 = Utf8               writeLEShort
+  #204 = Utf8               (Ljava/io/RandomAccessFile;S)V
+  #205 = Utf8               writeLEInt
+  #206 = Utf8               (Ljava/io/RandomAccessFile;I)V
+  #207 = Utf8               getDefaultItemNamesAndTypes
+  #208 = Utf8               ()Ljava/util/Map;
+  #209 = Utf8               ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+  #210 = Utf8               getBytesPerLine
+  #211 = Utf8               (Ljava/util/Map;)I
+  #212 = Utf8               (Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)I
+  #213 = Utf8               getBytesPerType
+  #214 = Utf8               (Ljava/lang/String;)I
+  #215 = Utf8               toNpyTypeStr
+  #216 = Utf8               (Ljava/lang/String;)Ljava/lang/String;
+  #217 = Utf8               <clinit>
+  #218 = Utf8               SourceFile
+  #219 = Utf8               NpyWriter.java
+  #220 = Utf8               NpyWriter
+  #221 = NameAndType        #174:#194     // "<init>":()V
+  #222 = NameAndType        #173:#141     // linesWritten:I
+  #223 = NameAndType        #161:#162     // outputFile:Ljava/lang/String;
+  #224 = NameAndType        #163:#164     // itemNamesAndTypes:Ljava/util/Map;
+  #225 = NameAndType        #210:#211     // getBytesPerLine:(Ljava/util/Map;)I
+  #226 = Class              #364          // java/nio/ByteBuffer
+  #227 = NameAndType        #365:#366     // allocate:(I)Ljava/nio/ByteBuffer;
+  #228 = NameAndType        #144:#145     // NATIVE_BYTE_ORDER:Ljava/nio/ByteOrder;
+  #229 = NameAndType        #367:#368     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #230 = NameAndType        #167:#168     // buf:Ljava/nio/ByteBuffer;
+  #231 = Utf8               java/io/File
+  #232 = NameAndType        #174:#184     // "<init>":(Ljava/lang/String;)V
+  #233 = NameAndType        #169:#170     // file:Ljava/io/File;
+  #234 = Utf8               java/io/RandomAccessFile
+  #235 = Utf8               rw
+  #236 = NameAndType        #174:#369     // "<init>":(Ljava/io/File;Ljava/lang/String;)V
+  #237 = NameAndType        #171:#172     // raf:Ljava/io/RandomAccessFile;
+  #238 = NameAndType        #370:#371     // setLength:(J)V
+  #239 = NameAndType        #159:#160     // NPY_HEADER:[B
+  #240 = Utf8               java/lang/StringBuilder
+  #241 = Utf8               java/lang/String
+  #242 = NameAndType        #174:#372     // "<init>":([C)V
+  #243 = Utf8               \u0000
+  #244 = Utf8
+  #245 = NameAndType        #373:#374     // replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+  #246 = NameAndType        #375:#376     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #247 = Utf8               \n
+  #248 = NameAndType        #377:#378     // toString:()Ljava/lang/String;
+  #249 = NameAndType        #379:#184     // writeBytes:(Ljava/lang/String;)V
+  #250 = Utf8               java/io/IOException
+  #251 = Utf8               java/lang/RuntimeException
+  #252 = Utf8               The .npy file
+  #253 = Utf8                could not be created
+  #254 = NameAndType        #207:#208     // getDefaultItemNamesAndTypes:()Ljava/util/Map;
+  #255 = NameAndType        #174:#175     // "<init>":(Ljava/lang/String;Ljava/util/Map;)V
+  #256 = NameAndType        #189:#186     // putItems:(Ljava/util/Map;)V
+  #257 = NameAndType        #380:#381     // hasRemaining:()Z
+  #258 = NameAndType        #382:#383     // array:()[B
+  #259 = NameAndType        #185:#384     // write:([B)V
+  #260 = NameAndType        #385:#386     // clear:()Ljava/nio/Buffer;
+  #261 = Class              #362          // java/util/Map
+  #262 = NameAndType        #387:#388     // entrySet:()Ljava/util/Set;
+  #263 = Class              #389          // java/util/Set
+  #264 = NameAndType        #390:#391     // iterator:()Ljava/util/Iterator;
+  #265 = Class              #363          // java/util/Iterator
+  #266 = NameAndType        #392:#381     // hasNext:()Z
+  #267 = NameAndType        #393:#394     // next:()Ljava/lang/Object;
+  #268 = Utf8               java/util/Map$Entry
+  #269 = Utf8               Entry
+  #270 = Utf8               InnerClasses
+  #271 = NameAndType        #395:#394     // getKey:()Ljava/lang/Object;
+  #272 = NameAndType        #396:#394     // getValue:()Ljava/lang/Object;
+  #273 = NameAndType        #397:#398     // get:(Ljava/lang/Object;)Ljava/lang/Object;
+  #274 = NameAndType        #191:#192     // putItem:(Ljava/lang/Object;Ljava/lang/String;)V
+  #275 = NameAndType        #399:#400     // hashCode:()I
+  #276 = Utf8               Integer
+  #277 = NameAndType        #401:#402     // equals:(Ljava/lang/Object;)Z
+  #278 = Utf8               Short
+  #279 = Utf8               Long
+  #280 = Utf8               Float
+  #281 = Utf8               Double
+  #282 = Utf8               java/lang/Integer
+  #283 = NameAndType        #403:#400     // intValue:()I
+  #284 = NameAndType        #404:#366     // putInt:(I)Ljava/nio/ByteBuffer;
+  #285 = Utf8               java/lang/Short
+  #286 = NameAndType        #405:#406     // shortValue:()S
+  #287 = NameAndType        #407:#408     // putShort:(S)Ljava/nio/ByteBuffer;
+  #288 = Utf8               java/lang/Long
+  #289 = NameAndType        #409:#410     // longValue:()J
+  #290 = NameAndType        #411:#412     // putLong:(J)Ljava/nio/ByteBuffer;
+  #291 = Utf8               java/lang/Float
+  #292 = NameAndType        #413:#414     // floatValue:()F
+  #293 = NameAndType        #415:#416     // putFloat:(F)Ljava/nio/ByteBuffer;
+  #294 = Utf8               java/lang/Double
+  #295 = NameAndType        #417:#418     // doubleValue:()D
+  #296 = NameAndType        #419:#420     // putDouble:(D)Ljava/nio/ByteBuffer;
+  #297 = Utf8               java/lang/IllegalArgumentException
+  #298 = Utf8               Unrecognized item type:
+  #299 = NameAndType        #421:#371     // seek:(J)V
+  #300 = NameAndType        #185:#422     // write:(I)V
+  #301 = Utf8               { \'descr\': [
+  #302 = Utf8               (\'
+  #303 = Utf8               \',\'
+  #304 = NameAndType        #215:#216     // toNpyTypeStr:(Ljava/lang/String;)Ljava/lang/String;
+  #305 = Utf8               \')
+  #306 = NameAndType        #423:#400     // size:()I
+  #307 = Utf8               ,
+  #308 = Utf8               ], \'fortran_order\': False, \'shape\': (
+  #309 = NameAndType        #375:#424     // append:(I)Ljava/lang/StringBuilder;
+  #310 = Utf8               ,), }
+  #311 = NameAndType        #425:#400     // length:()I
+  #312 = Utf8               header is too big to be written.
+  #313 = NameAndType        #375:#426     // append:(C)Ljava/lang/StringBuilder;
+  #314 = NameAndType        #203:#204     // writeLEShort:(Ljava/io/RandomAccessFile;S)V
+  #315 = NameAndType        #425:#410     // length:()J
+  #316 = NameAndType        #427:#194     // printStackTrace:()V
+  #317 = Utf8               The .npy file could not write a header created
+  #318 = NameAndType        #200:#194     // finalFlush:()V
+  #319 = Utf8               java/util/zip/GZIPOutputStream
+  #320 = Utf8               java/io/FileOutputStream
+  #321 = NameAndType        #174:#428     // "<init>":(Ljava/io/File;)V
+  #322 = NameAndType        #174:#429     // "<init>":(Ljava/io/OutputStream;)V
+  #323 = NameAndType        #430:#431     // read:([B)I
+  #324 = NameAndType        #185:#432     // write:([BII)V
+  #325 = NameAndType        #201:#194     // close:()V
+  #326 = Utf8               java/lang/Throwable
+  #327 = NameAndType        #433:#434     // addSuppressed:(Ljava/lang/Throwable;)V
+  #328 = Utf8               .gz
+  #329 = NameAndType        #196:#184     // compress:(Ljava/lang/String;)V
+  #330 = NameAndType        #193:#194     // writeHeader:()V
+  #331 = NameAndType        #435:#381     // delete:()Z
+  #332 = NameAndType        #436:#422     // writeShort:(I)V
+  #333 = Class              #437          // java/lang/System
+  #334 = NameAndType        #438:#439     // out:Ljava/io/PrintStream;
+  #335 = Utf8               writing:
+  #336 = Class              #440          // java/io/PrintStream
+  #337 = NameAndType        #441:#184     // println:(Ljava/lang/String;)V
+  #338 = NameAndType        #442:#422     // writeByte:(I)V
+  #339 = Utf8               java/util/LinkedHashMap
+  #340 = Utf8               time
+  #341 = NameAndType        #443:#444     // put:(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #342 = Utf8               x
+  #343 = Utf8               y
+  #344 = Utf8               z
+  #345 = NameAndType        #445:#446     // values:()Ljava/util/Collection;
+  #346 = Class              #447          // java/util/Collection
+  #347 = NameAndType        #213:#214     // getBytesPerType:(Ljava/lang/String;)I
+  #348 = NameAndType        #146:#147     // NUMPY_BYTE_ORDER:C
+  #349 = Utf8               i4
+  #350 = Utf8               i2
+  #351 = Utf8               i8
+  #352 = Utf8               f4
+  #353 = Utf8               f8
+  #354 = Class              #448          // java/nio/ByteOrder
+  #355 = NameAndType        #449:#450     // nativeOrder:()Ljava/nio/ByteOrder;
+  #356 = NameAndType        #451:#145     // BIG_ENDIAN:Ljava/nio/ByteOrder;
+  #357 = Utf8               XNUMPY
+  #358 = Class              #452          // java/nio/charset/StandardCharsets
+  #359 = NameAndType        #453:#454     // US_ASCII:Ljava/nio/charset/Charset;
+  #360 = NameAndType        #455:#456     // getBytes:(Ljava/nio/charset/Charset;)[B
+  #361 = Utf8               java/lang/Object
+  #362 = Utf8               java/util/Map
+  #363 = Utf8               java/util/Iterator
+  #364 = Utf8               java/nio/ByteBuffer
+  #365 = Utf8               allocate
+  #366 = Utf8               (I)Ljava/nio/ByteBuffer;
+  #367 = Utf8               order
+  #368 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #369 = Utf8               (Ljava/io/File;Ljava/lang/String;)V
+  #370 = Utf8               setLength
+  #371 = Utf8               (J)V
+  #372 = Utf8               ([C)V
+  #373 = Utf8               replace
+  #374 = Utf8               (Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+  #375 = Utf8               append
+  #376 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #377 = Utf8               toString
+  #378 = Utf8               ()Ljava/lang/String;
+  #379 = Utf8               writeBytes
+  #380 = Utf8               hasRemaining
+  #381 = Utf8               ()Z
+  #382 = Utf8               array
+  #383 = Utf8               ()[B
+  #384 = Utf8               ([B)V
+  #385 = Utf8               clear
+  #386 = Utf8               ()Ljava/nio/Buffer;
+  #387 = Utf8               entrySet
+  #388 = Utf8               ()Ljava/util/Set;
+  #389 = Utf8               java/util/Set
+  #390 = Utf8               iterator
+  #391 = Utf8               ()Ljava/util/Iterator;
+  #392 = Utf8               hasNext
+  #393 = Utf8               next
+  #394 = Utf8               ()Ljava/lang/Object;
+  #395 = Utf8               getKey
+  #396 = Utf8               getValue
+  #397 = Utf8               get
+  #398 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
+  #399 = Utf8               hashCode
+  #400 = Utf8               ()I
+  #401 = Utf8               equals
+  #402 = Utf8               (Ljava/lang/Object;)Z
+  #403 = Utf8               intValue
+  #404 = Utf8               putInt
+  #405 = Utf8               shortValue
+  #406 = Utf8               ()S
+  #407 = Utf8               putShort
+  #408 = Utf8               (S)Ljava/nio/ByteBuffer;
+  #409 = Utf8               longValue
+  #410 = Utf8               ()J
+  #411 = Utf8               putLong
+  #412 = Utf8               (J)Ljava/nio/ByteBuffer;
+  #413 = Utf8               floatValue
+  #414 = Utf8               ()F
+  #415 = Utf8               putFloat
+  #416 = Utf8               (F)Ljava/nio/ByteBuffer;
+  #417 = Utf8               doubleValue
+  #418 = Utf8               ()D
+  #419 = Utf8               putDouble
+  #420 = Utf8               (D)Ljava/nio/ByteBuffer;
+  #421 = Utf8               seek
+  #422 = Utf8               (I)V
+  #423 = Utf8               size
+  #424 = Utf8               (I)Ljava/lang/StringBuilder;
+  #425 = Utf8               length
+  #426 = Utf8               (C)Ljava/lang/StringBuilder;
+  #427 = Utf8               printStackTrace
+  #428 = Utf8               (Ljava/io/File;)V
+  #429 = Utf8               (Ljava/io/OutputStream;)V
+  #430 = Utf8               read
+  #431 = Utf8               ([B)I
+  #432 = Utf8               ([BII)V
+  #433 = Utf8               addSuppressed
+  #434 = Utf8               (Ljava/lang/Throwable;)V
+  #435 = Utf8               delete
+  #436 = Utf8               writeShort
+  #437 = Utf8               java/lang/System
+  #438 = Utf8               out
+  #439 = Utf8               Ljava/io/PrintStream;
+  #440 = Utf8               java/io/PrintStream
+  #441 = Utf8               println
+  #442 = Utf8               writeByte
+  #443 = Utf8               put
+  #444 = Utf8               (Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object;
+  #445 = Utf8               values
+  #446 = Utf8               ()Ljava/util/Collection;
+  #447 = Utf8               java/util/Collection
+  #448 = Utf8               java/nio/ByteOrder
+  #449 = Utf8               nativeOrder
+  #450 = Utf8               ()Ljava/nio/ByteOrder;
+  #451 = Utf8               BIG_ENDIAN
+  #452 = Utf8               java/nio/charset/StandardCharsets
+  #453 = Utf8               US_ASCII
+  #454 = Utf8               Ljava/nio/charset/Charset;
+  #455 = Utf8               getBytes
+  #456 = Utf8               (Ljava/nio/charset/Charset;)[B
 {
   private static final int BUFSIZE = 8192;
     descriptor: I
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
     ConstantValue: int 8192
 
   private static final java.nio.ByteOrder NATIVE_BYTE_ORDER;
@@ -632,15 +640,15 @@
         line 57: 170
       StackMapTable: number_of_entries = 2
         frame_type = 255 /* full_frame */
           offset_delta = 137
           locals = [ class NpyWriter, class java/lang/String, class java/util/Map ]
           stack = [ class java/io/IOException ]
         frame_type = 32 /* same */
-    Signature: #180                         // (Ljava/lang/String;Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)V
+    Signature: #183                         // (Ljava/lang/String;Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)V
 
   public NpyWriter(java.lang.String);
     descriptor: (Ljava/lang/String;)V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=3, locals=2, args_size=2
          0: aload_0
@@ -688,15 +696,15 @@
         line 70: 29
         line 73: 37
         line 74: 47
       StackMapTable: number_of_entries = 1
         frame_type = 37 /* same */
     Exceptions:
       throws java.io.IOException
-    Signature: #185                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
+    Signature: #188                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
 
   private void putItems(java.util.Map<java.lang.String, java.lang.Object>);
     descriptor: (Ljava/util/Map;)V
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=3, locals=7, args_size=2
          0: aload_0
@@ -739,15 +747,15 @@
         line 84: 77
       StackMapTable: number_of_entries = 2
         frame_type = 252 /* append */
           offset_delta = 15
           locals = [ class java/util/Iterator ]
         frame_type = 250 /* chop */
           offset_delta = 61
-    Signature: #185                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
+    Signature: #188                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)V
 
   private void putItem(java.lang.Object, java.lang.String);
     descriptor: (Ljava/lang/Object;Ljava/lang/String;)V
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=4, locals=5, args_size=3
          0: aload_2
@@ -1090,100 +1098,138 @@
           stack = [ class java/io/IOException ]
         frame_type = 14 /* same */
 
   public void compress(java.lang.String);
     descriptor: (Ljava/lang/String;)V
     flags: (0x0001) ACC_PUBLIC
     Code:
-      stack=7, locals=5, args_size=2
+      stack=7, locals=8, args_size=2
          0: aload_0
          1: invokespecial #96                 // Method finalFlush:()V
          4: new           #97                 // class java/util/zip/GZIPOutputStream
          7: dup
          8: new           #98                 // class java/io/FileOutputStream
         11: dup
         12: new           #11                 // class java/io/File
         15: dup
         16: aload_1
         17: invokespecial #12                 // Method java/io/File."<init>":(Ljava/lang/String;)V
         20: invokespecial #99                 // Method java/io/FileOutputStream."<init>":(Ljava/io/File;)V
         23: invokespecial #100                // Method java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
         26: astore_2
-        27: sipush        1024
-        30: newarray       byte
-        32: astore_3
-        33: aload_0
-        34: getfield      #17                 // Field raf:Ljava/io/RandomAccessFile;
-        37: lconst_0
-        38: invokevirtual #77                 // Method java/io/RandomAccessFile.seek:(J)V
-        41: aload_0
-        42: getfield      #17                 // Field raf:Ljava/io/RandomAccessFile;
-        45: aload_3
-        46: invokevirtual #101                // Method java/io/RandomAccessFile.read:([B)I
-        49: dup
-        50: istore        4
-        52: iconst_m1
-        53: if_icmpeq     67
-        56: aload_2
-        57: aload_3
-        58: iconst_0
-        59: iload         4
-        61: invokevirtual #102                // Method java/util/zip/GZIPOutputStream.write:([BII)V
-        64: goto          41
-        67: aload_2
-        68: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
-        71: goto          92
-        74: astore_3
-        75: aload_2
-        76: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
-        79: goto          90
-        82: astore        4
-        84: aload_3
-        85: aload         4
-        87: invokevirtual #105                // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-        90: aload_3
-        91: athrow
-        92: goto          100
-        95: astore_2
-        96: aload_2
-        97: invokevirtual #94                 // Method java/io/IOException.printStackTrace:()V
-       100: return
+        27: aconst_null
+        28: astore_3
+        29: sipush        1024
+        32: newarray       byte
+        34: astore        4
+        36: aload_0
+        37: getfield      #17                 // Field raf:Ljava/io/RandomAccessFile;
+        40: lconst_0
+        41: invokevirtual #77                 // Method java/io/RandomAccessFile.seek:(J)V
+        44: aload_0
+        45: getfield      #17                 // Field raf:Ljava/io/RandomAccessFile;
+        48: aload         4
+        50: invokevirtual #101                // Method java/io/RandomAccessFile.read:([B)I
+        53: dup
+        54: istore        5
+        56: iconst_m1
+        57: if_icmpeq     72
+        60: aload_2
+        61: aload         4
+        63: iconst_0
+        64: iload         5
+        66: invokevirtual #102                // Method java/util/zip/GZIPOutputStream.write:([BII)V
+        69: goto          44
+        72: aload_2
+        73: ifnull        148
+        76: aload_3
+        77: ifnull        98
+        80: aload_2
+        81: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
+        84: goto          148
+        87: astore        4
+        89: aload_3
+        90: aload         4
+        92: invokevirtual #105                // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+        95: goto          148
+        98: aload_2
+        99: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
+       102: goto          148
+       105: astore        4
+       107: aload         4
+       109: astore_3
+       110: aload         4
+       112: athrow
+       113: astore        6
+       115: aload_2
+       116: ifnull        145
+       119: aload_3
+       120: ifnull        141
+       123: aload_2
+       124: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
+       127: goto          145
+       130: astore        7
+       132: aload_3
+       133: aload         7
+       135: invokevirtual #105                // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       138: goto          145
+       141: aload_2
+       142: invokevirtual #103                // Method java/util/zip/GZIPOutputStream.close:()V
+       145: aload         6
+       147: athrow
+       148: goto          156
+       151: astore_2
+       152: aload_2
+       153: invokevirtual #94                 // Method java/io/IOException.printStackTrace:()V
+       156: return
       Exception table:
          from    to  target type
-            27    67    74   Class java/lang/Throwable
-            75    79    82   Class java/lang/Throwable
-             4    92    95   Class java/io/IOException
+            80    84    87   Class java/lang/Throwable
+            29    72   105   Class java/lang/Throwable
+            29    72   113   any
+           123   127   130   Class java/lang/Throwable
+           105   115   113   any
+             4   148   151   Class java/io/IOException
       LineNumberTable:
         line 169: 0
         line 171: 4
-        line 172: 27
-        line 174: 33
-        line 175: 41
-        line 176: 56
-        line 178: 67
-        line 171: 74
-        line 180: 92
-        line 178: 95
-        line 179: 96
-        line 181: 100
-      StackMapTable: number_of_entries = 8
-        frame_type = 253 /* append */
-          offset_delta = 41
-          locals = [ class java/util/zip/GZIPOutputStream, class "[B" ]
+        line 172: 29
+        line 174: 36
+        line 175: 44
+        line 176: 60
+        line 178: 72
+        line 171: 105
+        line 178: 113
+        line 180: 148
+        line 178: 151
+        line 179: 152
+        line 181: 156
+      StackMapTable: number_of_entries = 12
+        frame_type = 254 /* append */
+          offset_delta = 44
+          locals = [ class java/util/zip/GZIPOutputStream, class java/lang/Throwable, class "[B" ]
         frame_type = 250 /* chop */
-          offset_delta = 25
+          offset_delta = 27
+        frame_type = 78 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
+        frame_type = 10 /* same */
         frame_type = 70 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
+        frame_type = 71 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
         frame_type = 255 /* full_frame */
-          offset_delta = 7
-          locals = [ class NpyWriter, class java/lang/String, class java/util/zip/GZIPOutputStream, class java/lang/Throwable ]
+          offset_delta = 16
+          locals = [ class NpyWriter, class java/lang/String, class java/util/zip/GZIPOutputStream, class java/lang/Throwable, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Throwable ]
-        frame_type = 7 /* same */
-        frame_type = 249 /* chop */
-          offset_delta = 1
+        frame_type = 10 /* same */
+        frame_type = 3 /* same */
+        frame_type = 255 /* full_frame */
+          offset_delta = 2
+          locals = [ class NpyWriter, class java/lang/String ]
+          stack = []
         frame_type = 66 /* same_locals_1_stack_item */
           stack = [ class java/io/IOException ]
         frame_type = 4 /* same */
 
   public void compress();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
@@ -1404,15 +1450,15 @@
       LineNumberTable:
         line 253: 0
         line 254: 8
         line 255: 19
         line 256: 30
         line 257: 41
         line 258: 52
-    Signature: #203                         // ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
+    Signature: #209                         // ()Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
 
   private static int getBytesPerLine(java.util.Map<java.lang.String, java.lang.String>);
     descriptor: (Ljava/util/Map;)I
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=2, locals=4, args_size=1
          0: iconst_0
@@ -1444,15 +1490,15 @@
         line 267: 43
       StackMapTable: number_of_entries = 2
         frame_type = 253 /* append */
           offset_delta = 14
           locals = [ int, class java/util/Iterator ]
         frame_type = 250 /* chop */
           offset_delta = 28
-    Signature: #206                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)I
+    Signature: #212                         // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;)I
 
   private static int getBytesPerType(java.lang.String);
     descriptor: (Ljava/lang/String;)I
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=4, locals=3, args_size=1
          0: aload_0
@@ -1736,8 +1782,8 @@
       StackMapTable: number_of_entries = 2
         frame_type = 20 /* same */
         frame_type = 65 /* same_locals_1_stack_item */
           stack = [ int ]
 }
 SourceFile: "NpyWriter.java"
 InnerClasses:
-  public static #261= #47 of #179;        // Entry=class java/util/Map$Entry of class java/util/Map
+  public static #269= #47 of #261;        // Entry=class java/util/Map$Entry of class java/util/Map
```

### Comparing `actipy-2.0.3/actipy/NpyWriter.java` & `actipy-2.0.3.post0/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/actipy/processing.py` & `actipy-2.0.3.post0/src/actipy/processing.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/actipy/reader.py` & `actipy-2.0.3.post0/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3/setup.py` & `actipy-2.0.3.post0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,58 @@
+import sys
+import os.path
+# https://github.com/python-versioneer/python-versioneer/issues/193
+sys.path.insert(0, os.path.dirname(__file__))
+
 import setuptools
 import codecs
-import os.path
+
+import versioneer
 
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
-def get_string(string, rel_path="actipy/__init__.py"):
+def get_string(string, rel_path="src/actipy/__init__.py"):
     for line in read(rel_path).splitlines():
         if line.startswith(string):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="actipy",
     python_requires=">=3.8",
-    version=get_string("__version__"),
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     description="Python package to process wearable accelerometer data",
+    keywords="wearable accelerometer data processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/activityMonitoring/actipy",
+    url="https://github.com/OxWearables/actipy",
+    download_url="https://github.com/OxWearables/actipy",
     author=get_string("__author__"),
-    author_email=get_string("__email__"),
+    maintainer=get_string("__maintainer__"),
+    maintainer_email=get_string("__maintainer_email__"),
     license=get_string("__license__"),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Unix",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Medical Science Apps.",
     ],
-    packages=setuptools.find_packages(exclude=("test", "tests")),
+    packages=setuptools.find_packages(where="src", exclude=("test", "tests")),
+    package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         "numpy>=1.22",
         "scipy>=1.7",
         "pandas>=1.3",
         "statsmodels>=0.13",
         "Jpype1>=1.3",
```

