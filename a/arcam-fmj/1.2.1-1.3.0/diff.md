# Comparing `tmp/arcam-fmj-1.2.1.tar.gz` & `tmp/arcam-fmj-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcam-fmj-1.2.1.tar", last modified: Tue Feb 14 19:43:27 2023, max compression
+gzip compressed data, was "arcam-fmj-1.3.0.tar", last modified: Wed Apr 19 19:00:15 2023, max compression
```

## Comparing `arcam-fmj-1.2.1.tar` & `arcam-fmj-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/src/arcam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/src/arcam/fmj/
--rw-r--r--   0 runner    (1001) docker     (123)    35730 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/console.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-02-14 19:43:16.000000 arcam-fmj-1.2.1/src/arcam/fmj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:43:27.093412 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-14 19:43:27.000000 arcam-fmj-1.2.1/src/arcam_fmj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam/fmj/
+-rw-r--r--   0 runner    (1001) docker     (123)    35847 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/top_level.txt
```

### Comparing `arcam-fmj-1.2.1/LICENSE.txt` & `arcam-fmj-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/PKG-INFO` & `arcam-fmj-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.2.1
+Version: 1.3.0
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `arcam-fmj-1.2.1/README.rst` & `arcam-fmj-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/setup.py` & `arcam-fmj-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="arcam-fmj",
-    version="1.2.1",
+    version="1.3.0",
     description="A python library for speaking to Arcam receivers",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     packages=["arcam.fmj"],
     package_dir={"": "src"},
     package_data = {
```

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/__init__.py` & `arcam-fmj-1.3.0/src/arcam/fmj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 
 class InvalidPacket(ArcamException):
     pass
 
 APIVERSION_450_SERIES = {"AVR380", "AVR450", "AVR750"}
 APIVERSION_860_SERIES = {"AV860", "AVR850", "AVR550", "AVR390", "SR250"}
 APIVERSION_SA_SERIES = {"SA10", "SA20", "SA30"}
-APIVERSION_HDA_SERIES = {"AVR5", "AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41"}
-APIVERSION_HDA_PREMIUM_SERIES = {"AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41"}
-APIVERSION_HDA_MULTI_ZONE_SERIES = {"AVR20", "AVR30", "AV40", "AVR21", "ARV31", "AV41"}
+APIVERSION_HDA_SERIES = {"AVR5", "AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
+APIVERSION_HDA_PREMIUM_SERIES = {"AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
+APIVERSION_HDA_MULTI_ZONE_SERIES = {"AVR20", "AVR30", "AV40", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
 APIVERSION_PA_SERIES = {"PA720", "PA240", "PA410"}
 
 APIVERSION_DAB_SERIES = {"AVR450", "AVR750"}
 APIVERSION_DAB_SERIES.update("AV860", "AVR850", "AVR550", "AVR390")
 APIVERSION_DAB_SERIES.update(APIVERSION_HDA_SERIES)
 
 APIVERSION_ZONE2_SERIES = set()
@@ -319,14 +319,16 @@
     DAB = enum.auto()
     NET = enum.auto()
     USB = enum.auto()
     STB = enum.auto()
     GAME = enum.auto()
     PHONO = enum.auto()
     ARC_ERC = enum.auto()
+    UHD = enum.auto()
+    BT = enum.auto()
 
     @classmethod
     def from_bytes(cls, data: bytes, model: ApiModel, zn: int) -> 'SourceCodes':
         try:
             table = SOURCE_CODES[(model, zn)]
         except KeyError:
             raise ValueError("Unknown source map for model {} and zone {}".format(model, zn))
@@ -420,49 +422,57 @@
     SourceCodes.USB: bytes([0x0F]),
     SourceCodes.STB: bytes([0x10]),
     SourceCodes.GAME: bytes([0x11]),
     SourceCodes.PHONO: bytes([0x12]),
     SourceCodes.ARC_ERC: bytes([0x13]),
 }
 
+HDA_SOURCE_MAPPING = {
+    SourceCodes.FOLLOW_ZONE_1: bytes([0x00]),
+    SourceCodes.CD: bytes([0x01]),
+    SourceCodes.BD: bytes([0x02]),
+    SourceCodes.AV: bytes([0x03]),
+    SourceCodes.SAT: bytes([0x04]),
+    SourceCodes.PVR: bytes([0x05]),
+    SourceCodes.UHD: bytes([0x06]),
+    SourceCodes.AUX: bytes([0x08]),
+    SourceCodes.DISPLAY: bytes([0x09]),
+    SourceCodes.FM: bytes([0x0B]),
+    SourceCodes.DAB: bytes([0x0C]),
+    SourceCodes.NET: bytes([0x0E]),
+    SourceCodes.USB: bytes([0x0F]),
+    SourceCodes.STB: bytes([0x10]),
+    SourceCodes.GAME: bytes([0x11]),
+    SourceCodes.BT: bytes([0x12]),
+}
+
+SA_SOURCE_MAPPING = {
+    SourceCodes.PHONO: bytes([0x01]),
+    SourceCodes.AUX: bytes([0x02]),
+    SourceCodes.PVR: bytes([0x03]),
+    SourceCodes.AV: bytes([0x04]),
+    SourceCodes.STB: bytes([0x05]),
+    SourceCodes.CD: bytes([0x06]),
+    SourceCodes.BD: bytes([0x07]),
+    SourceCodes.SAT: bytes([0x08]),
+    SourceCodes.GAME: bytes([0x09]),
+    SourceCodes.NET: bytes([0x0B]),
+    SourceCodes.USB: bytes([0x0B]),
+    SourceCodes.ARC_ERC: bytes([0x0D]),
+}
+
 SOURCE_CODES = {
     (ApiModel.API450_SERIES, 1): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API450_SERIES, 2): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API860_SERIES, 1): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API860_SERIES, 2): DEFAULT_SOURCE_MAPPING,
-    (ApiModel.APIHDA_SERIES, 1): DEFAULT_SOURCE_MAPPING,
-    (ApiModel.APIHDA_SERIES, 2): DEFAULT_SOURCE_MAPPING,
-    (ApiModel.APISA_SERIES, 1): {
-        SourceCodes.PHONO: bytes([0x01]),
-        SourceCodes.AUX: bytes([0x02]),
-        SourceCodes.PVR: bytes([0x03]),
-        SourceCodes.AV: bytes([0x04]),
-        SourceCodes.STB: bytes([0x05]),
-        SourceCodes.CD: bytes([0x06]),
-        SourceCodes.BD: bytes([0x07]),
-        SourceCodes.SAT: bytes([0x08]),
-        SourceCodes.GAME: bytes([0x09]),
-        SourceCodes.NET: bytes([0x0B]),
-        SourceCodes.USB: bytes([0x0B]),
-        SourceCodes.ARC_ERC: bytes([0x0D]),
-    },
-    (ApiModel.APISA_SERIES, 2): {
-        SourceCodes.PHONO: bytes([0x01]),
-        SourceCodes.AUX: bytes([0x02]),
-        SourceCodes.PVR: bytes([0x03]),
-        SourceCodes.AV: bytes([0x04]),
-        SourceCodes.STB: bytes([0x05]),
-        SourceCodes.CD: bytes([0x06]),
-        SourceCodes.BD: bytes([0x07]),
-        SourceCodes.SAT: bytes([0x08]),
-        SourceCodes.GAME: bytes([0x09]),
-        SourceCodes.NET: bytes([0x0B]),
-        SourceCodes.USB: bytes([0x0B]),
-        SourceCodes.ARC_ERC: bytes([0x0D]),
-    },
+    (ApiModel.APIHDA_SERIES, 1): HDA_SOURCE_MAPPING,
+    (ApiModel.APIHDA_SERIES, 2): HDA_SOURCE_MAPPING,
+    (ApiModel.APISA_SERIES, 1): SA_SOURCE_MAPPING,
+    (ApiModel.APISA_SERIES, 2): SA_SOURCE_MAPPING,
 }
 
 RC5CODE_DECODE_MODE_MCH: Dict[Tuple[ApiModel, int], Dict[DecodeModeMCH, bytes]] = {
     (ApiModel.API450_SERIES, 1): {
         DecodeModeMCH.STEREO_DOWNMIX: bytes([16, 107]),
         DecodeModeMCH.MULTI_CHANNEL: bytes([16, 106]),
         DecodeModeMCH.DOLBY_D_EX_OR_DTS_ES: bytes([16, 118]),
@@ -610,40 +620,39 @@
     (ApiModel.APIHDA_SERIES, 1): {
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.AV: bytes([16, 94]),
         SourceCodes.DAB: bytes([16, 72]),
         SourceCodes.FM: bytes([16, 28]),
         SourceCodes.BD: bytes([16, 98]),
         SourceCodes.GAME: bytes([16, 97]),
-        SourceCodes.VCR: bytes([16, 125]), # UHD
+        SourceCodes.UHD: bytes([16, 125]),
         SourceCodes.CD: bytes([16, 118]),
         SourceCodes.AUX: bytes([16, 99]),
         SourceCodes.DISPLAY: bytes([16, 58]),
         SourceCodes.SAT: bytes([16, 27]),
         SourceCodes.PVR: bytes([16, 96]),
-        SourceCodes.USB: bytes([16, 93]), # Not in docs but seems plausible
         SourceCodes.NET: bytes([16, 92]),
-        SourceCodes.PHONO: bytes([16, 122]), # BT
+        SourceCodes.BT: bytes([16, 122]),
     },
     (ApiModel.APIHDA_SERIES, 2): {
         SourceCodes.STB: bytes([23, 8]),
         SourceCodes.AV: bytes([23, 9]),
         SourceCodes.DAB: bytes([23, 16]),
         SourceCodes.FM: bytes([23, 14]),
         SourceCodes.BD: bytes([23, 7]),
         SourceCodes.GAME: bytes([23, 11]),
         SourceCodes.CD: bytes([23, 6]),
         SourceCodes.AUX: bytes([23, 13]),
         SourceCodes.PVR: bytes([23, 15]),
         SourceCodes.USB: bytes([23, 18]),
         SourceCodes.NET: bytes([23, 19]),
         SourceCodes.SAT: bytes([23, 20]),
-        SourceCodes.VCR: bytes([23, 23]), # UHD
-        SourceCodes.PHONO: bytes([23, 22]), # BT
-        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20])
+        SourceCodes.UHD: bytes([23, 23]),
+        SourceCodes.BT: bytes([23, 22]),
+        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20]),
     },
     (ApiModel.APISA_SERIES, 1): {
         SourceCodes.PHONO: bytes([16, 117]),
         SourceCodes.CD: bytes([16, 118]),
         SourceCodes.BD: bytes([16, 98]),
         SourceCodes.SAT: bytes([16, 27]),
         SourceCodes.PVR: bytes([16, 96]),
```

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/client.py` & `arcam-fmj-1.3.0/src/arcam/fmj/client.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/console.py` & `arcam-fmj-1.3.0/src/arcam/fmj/console.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/server.py` & `arcam-fmj-1.3.0/src/arcam/fmj/server.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/state.py` & `arcam-fmj-1.3.0/src/arcam/fmj/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     PresetDetail,
     ResponseException,
     ResponsePacket,
     SourceCodes,
     POWER_WRITE_SUPPORTED,
     MUTE_WRITE_SUPPORTED,
     SOURCE_WRITE_SUPPORTED,
-    SOURCE_CODES,
     RC5CODE_SOURCE,
     RC5CODE_POWER,
     RC5CODE_MUTE,
     RC5CODE_VOLUME,
     RC5CODE_DECODE_MODE_2CH,
     RC5CODE_DECODE_MODE_MCH,
 )
```

### Comparing `arcam-fmj-1.2.1/src/arcam/fmj/utils.py` & `arcam-fmj-1.3.0/src/arcam/fmj/utils.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.2.1/src/arcam_fmj.egg-info/PKG-INFO` & `arcam-fmj-1.3.0/src/arcam_fmj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.2.1
+Version: 1.3.0
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

