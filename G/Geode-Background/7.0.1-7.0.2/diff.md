# Comparing `tmp/Geode_Background-7.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.0.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 2391760 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-19 16:12 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-19 16:12 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-Apr-19 16:12 geode_background/surface.py
--rw-rw-rw-  2.0 fat    61440 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_common.dll
--rw-rw-rw-  2.0 fat  2379776 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_solid.dll
--rw-rw-rw-  2.0 fat  2171392 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_surface.dll
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1102 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1279 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/RECORD
-13 files, 4991915 bytes uncompressed, 2389578 bytes compressed:  52.1%
+Zip file size: 2391765 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-19 17:30 geode_background/__init__.py
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-19 17:30 geode_background/solid.py
+-rw-rw-rw-  2.0 fat      203 b- defN 23-Apr-19 17:30 geode_background/surface.py
+-rw-rw-rw-  2.0 fat    61440 b- defN 23-Apr-19 17:31 geode_background/bin/Geode-Background_common.dll
+-rw-rw-rw-  2.0 fat  2379776 b- defN 23-Apr-19 17:31 geode_background/bin/Geode-Background_solid.dll
+-rw-rw-rw-  2.0 fat  2171392 b- defN 23-Apr-19 17:31 geode_background/bin/Geode-Background_surface.dll
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 17:31 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 17:31 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 17:31 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1102 b- defN 23-Apr-19 17:31 Geode_Background-7.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-19 17:31 Geode_Background-7.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-19 17:31 Geode_Background-7.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1279 b- defN 23-Apr-19 17:31 Geode_Background-7.0.2.dist-info/RECORD
+13 files, 4991922 bytes uncompressed, 2389583 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Background-7.0.1.dist-info/METADATA
+Filename: Geode_Background-7.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.0.1.dist-info/WHEEL
+Filename: Geode_Background-7.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.0.1.dist-info/top_level.txt
+Filename: Geode_Background-7.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.0.1.dist-info/RECORD
+Filename: Geode_Background-7.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/solid.py

```diff
@@ -2,8 +2,8 @@
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 import geode_common
 
 from .bin.geode_background_py_solid import *
-BackgroundSolid.initialize()
+BackgroundSolidLibrary.initialize()
```

## geode_background/bin/Geode-Background_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000815c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Apr 19 16:12:25 2023
+Time/Date		Wed Apr 19 17:30:42 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000008400
 SizeOfInitializedData	0000000000006e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000815c
@@ -13932,17 +13932,17 @@
    18000a80a:	(bad)
    18000a80b:	(bad)
    18000a80c:	(bad)
    18000a80d:	(bad)
    18000a80e:	(bad)
    18000a80f:	incl   (%rax)
    18000a811:	add    %al,(%rax)
-   18000a813:	add    %ch,%cl
-   18000a815:	adc    0x64(%rax),%al
-   18000a818:	add    %al,(%rax)
+   18000a813:	add    %al,0x25(%rdx)
+   18000a816:	rex
+   18000a817:	add    %al,%fs:(%rax)
    18000a81a:	add    %al,(%rax)
    18000a81c:	or     $0xa4000000,%eax
    18000a821:	add    (%rax),%al
    18000a823:	add    %dh,%ah
    18000a825:	mov    $0x0,%ah
    18000a827:	add    %dh,%ah
    18000a829:	pushf
```

## geode_background/bin/Geode-Background_solid.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018019b928
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Apr 19 16:13:11 2023
+Time/Date		Wed Apr 19 17:31:27 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000001a0400
 SizeOfInitializedData	00000000000a8400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000019b928
@@ -699389,17 +699389,16 @@
    18020a530:	(bad)
    18020a535:	insb   (%dx),%es:(%rdi)
    18020a536:	insb   (%dx),%es:(%rdi)
    18020a537:	outsl  %ds:(%rsi),(%dx)
    18020a538:	movsxd 0x74(%rcx),%esp
    18020a53b:	imul   $0x0,0x6e(%rdi),%ebp
    18020a542:	add    %al,(%rax)
-   18020a544:	(bad)
-   18020a545:	adc    0x64(%rax),%eax
-   18020a548:	add    %al,(%rax)
+   18020a544:	outsl  %ds:(%rsi),(%dx)
+   18020a545:	and    $0x6440,%eax
    18020a54a:	add    %al,(%rax)
    18020a54c:	or     $0x88000000,%eax
    18020a551:	add    (%rax),%eax
    18020a553:	add    %al,-0x7fffdf2e(%rax)
    18020a559:	mov    $0x20,%edx
    18020a55e:	add    %al,(%rax)
    18020a560:	cmp    %al,(%rcx)
```

## geode_background/bin/Geode-Background_surface.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180174da8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Apr 19 16:12:47 2023
+Time/Date		Wed Apr 19 17:31:07 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000176e00
 SizeOfInitializedData	000000000009ea00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000174da8
@@ -645722,17 +645722,16 @@
    1801df9f0:	(bad)
    1801df9f5:	insb   (%dx),%es:(%rdi)
    1801df9f6:	insb   (%dx),%es:(%rdi)
    1801df9f7:	outsl  %ds:(%rsi),(%dx)
    1801df9f8:	movsxd 0x74(%rcx),%esp
    1801df9fb:	imul   $0x0,0x6e(%rdi),%ebp
    1801dfa02:	add    %al,(%rax)
-   1801dfa04:	call   *(%rdx)
-   1801dfa06:	rex
-   1801dfa07:	add    %al,%fs:(%rax)
+   1801dfa04:	pop    %rbx
+   1801dfa05:	and    $0x6440,%eax
    1801dfa0a:	add    %al,(%rax)
    1801dfa0c:	or     $0x88000000,%eax
    1801dfa11:	add    (%rax),%eax
    1801dfa13:	add    %cl,(%rax)
    1801dfa15:	and    (%rsi),%ebx
    1801dfa17:	add    %cl,(%rax)
    1801dfa19:	adc    $0x1e,%eax
```

## Comparing `Geode_Background-7.0.1.dist-info/METADATA` & `Geode_Background-7.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Background
-Version: 7.0.1
+Version: 7.0.2
 Summary: Geode-solutions OpenGeode module for building background meshes
 Home-page: https://github.com/Geode-solutions/Geode-Background
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `Geode_Background-7.0.1.dist-info/RECORD` & `Geode_Background-7.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 geode_background/__init__.py,sha256=CTtrrNi0y001nV0307I5erAdfuvWGTSLY3cqK7SLCQo,94
-geode_background/solid.py,sha256=Q-M2Q2M9TWQeGp9AU77C6mhjPqlsQqERjSjUFwNnvGI,192
+geode_background/solid.py,sha256=DMeE_kcPihrhANbHWVJLkRmXJNV60SmALzozbU9AsXY,199
 geode_background/surface.py,sha256=KNExP1n53P95lYbgU7GJXKaZqKakt1kUzkCj3LDs4mw,203
-geode_background/bin/Geode-Background_common.dll,sha256=U1ABdxSN-eNQj47-QtZr2eu_jtRWkA3tc0pIslCy2Ys,61440
-geode_background/bin/Geode-Background_solid.dll,sha256=iDiQlEs4yQ3VGRFAmYnPeINKyuwg72gwmgpm3tdTWac,2379776
-geode_background/bin/Geode-Background_surface.dll,sha256=VAwZjKt9m2LvSU-0O6bB7XgyXWZubrVKt-CveNHc2R4,2171392
-geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd,sha256=tAjWc9rUiWvBql0f720N9gIQX4vfzqRSeiFdZDomQkQ,125440
-geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd,sha256=OH1TpbmsZNPyOLSrxW1LZPi62khvoVGPeSR5iL0dV70,125440
-geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd,sha256=kcq6crlqiQW-iA-CYVN44uRGSC6boLpjADXK4BhoURw,125440
-Geode_Background-7.0.1.dist-info/METADATA,sha256=0oUoIPn16zDapXBooxgPnxviNHPg49JDs4H4AAp-F_M,1102
-Geode_Background-7.0.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Background-7.0.1.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
-Geode_Background-7.0.1.dist-info/RECORD,,
+geode_background/bin/Geode-Background_common.dll,sha256=lJSUUnwehhkdRmbNRzjVE88hZhtijzWo1xOgg5VrD3A,61440
+geode_background/bin/Geode-Background_solid.dll,sha256=6-otNVzDgGrtbA2vqX5yGCZGDWfmjJ24iPDGHHbakVg,2379776
+geode_background/bin/Geode-Background_surface.dll,sha256=CYwqiK3Bs-XgSMO-zppKLRr05B0NdLQzn_3BnIx6UtA,2171392
+geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd,sha256=uvN_hpsVwVANOXlrU6bsMbFXKNn6ZqMk0d4G7DeoYmI,125440
+geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd,sha256=SMXVLvRAPmt-e1FUlJLR9ubtNnjGa5NSQXRpoqsiELk,125440
+geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd,sha256=GuI-wpU4uV3kLOqHa94Yew2nH_9ziW1gbxBfb46eIiE,125440
+Geode_Background-7.0.2.dist-info/METADATA,sha256=dIPgPFrNYzeKwFqwmO4QO0h_bcfRPZsXRFlCdJmP0IA,1102
+Geode_Background-7.0.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Background-7.0.2.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
+Geode_Background-7.0.2.dist-info/RECORD,,
```

