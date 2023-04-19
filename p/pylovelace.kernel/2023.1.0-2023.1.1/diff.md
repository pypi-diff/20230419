# Comparing `tmp/pylovelace.kernel-2023.1.0-py3-none-any.whl.zip` & `tmp/pylovelace.kernel-2023.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 197223 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-19 05:54 pylovelace/kernel/__init__.py
--rw-rw-rw-  2.0 fat   471040 b- defN 23-Apr-19 05:51 pylovelace/kernel/lovelace.pyd
--rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-19 05:54 pylovelace.kernel-2023.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:54 pylovelace.kernel-2023.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 05:54 pylovelace.kernel-2023.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      523 b- defN 23-Apr-19 05:54 pylovelace.kernel-2023.1.0.dist-info/RECORD
-6 files, 472096 bytes uncompressed, 196267 bytes compressed:  58.4%
+Zip file size: 196367 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-19 06:21 pylovelace/kernel/__init__.py
+-rw-rw-rw-  2.0 fat   469504 b- defN 23-Apr-19 06:20 pylovelace/kernel/lovelace.pyd
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-19 06:21 pylovelace.kernel-2023.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 06:21 pylovelace.kernel-2023.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 06:21 pylovelace.kernel-2023.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      523 b- defN 23-Apr-19 06:21 pylovelace.kernel-2023.1.1.dist-info/RECORD
+6 files, 470560 bytes uncompressed, 195411 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylovelace/kernel/__init__.py
 Comment: 
 
 Filename: pylovelace/kernel/lovelace.pyd
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.0.dist-info/METADATA
+Filename: pylovelace.kernel-2023.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.0.dist-info/WHEEL
+Filename: pylovelace.kernel-2023.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.0.dist-info/top_level.txt
+Filename: pylovelace.kernel-2023.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.0.dist-info/RECORD
+Filename: pylovelace.kernel-2023.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/kernel/__init__.py

```diff
@@ -5,9 +5,9 @@
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 from .lovelace import PyLovelace, get_runtime_module, protect_code, compile_module, finalize, validate
 
-__version__ = '2023.1.0'
+__version__ = '2023.1.1'
 __description__ = 'PyLovelace Kernel'
```

## Comparing `pylovelace.kernel-2023.1.0.dist-info/RECORD` & `pylovelace.kernel-2023.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-pylovelace/kernel/__init__.py,sha256=nPDb2sJpn2Pt5yjs_6hgjrLK7n9cQ5GoeqLlrtY-C7M,317
-pylovelace/kernel/lovelace.pyd,sha256=QSmH3c9cbnCNES0xLREfgsfOb1q0PkOSKGaDgQJ8TKo,471040
-pylovelace.kernel-2023.1.0.dist-info/METADATA,sha256=Igxt3Huyvoon4Kg8TYjyl57UduqVJTXAIkMBHEkXI3w,113
-pylovelace.kernel-2023.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pylovelace.kernel-2023.1.0.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
-pylovelace.kernel-2023.1.0.dist-info/RECORD,,
+pylovelace/kernel/__init__.py,sha256=099a_j27kln8C1ZTLNjSJV1QVZ6LJbRRZE9QsIjcmjE,317
+pylovelace/kernel/lovelace.pyd,sha256=kcKFfKU-AMXaZFYL-sXvBif2WoY3W05Ics7oGdDblKc,469504
+pylovelace.kernel-2023.1.1.dist-info/METADATA,sha256=NoYrkHlOVaGdISG24F-K44vkvBuHhDViJM2lMBKikjg,113
+pylovelace.kernel-2023.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pylovelace.kernel-2023.1.1.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
+pylovelace.kernel-2023.1.1.dist-info/RECORD,,
```

