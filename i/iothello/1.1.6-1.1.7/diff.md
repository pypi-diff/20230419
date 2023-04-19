# Comparing `tmp/iothello-1.1.6-py3-none-any.whl.zip` & `tmp/iothello-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 66990 bytes, number of entries: 41
+Zip file size: 66992 bytes, number of entries: 41
 -rw-rw-rw-  2.0 fat       31 b- defN 22-Jun-25 17:46 iothello/__init__.py
 -rw-rw-rw-  2.0 fat     6636 b- defN 22-Jun-26 18:21 iothello/backend_gui.py
 -rw-rw-rw-  2.0 fat    60852 b- defN 22-Jun-11 11:35 iothello/font.otf
--rw-rw-rw-  2.0 fat     5666 b- defN 22-Jun-26 18:39 iothello/gui.py
+-rw-rw-rw-  2.0 fat     5668 b- defN 22-Jul-01 10:22 iothello/gui.py
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/0_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/10_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/11_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/12_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/13_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/14_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/15_ridge.sav
@@ -31,13 +31,13 @@
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/3_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/4_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/5_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/6_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/7_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/8_ridge.sav
 -rw-rw-rw-  2.0 fat      770 b- defN 22-Jun-11 11:35 iothello/models/9_ridge.sav
--rw-rw-rw-  2.0 fat     1093 b- defN 22-Jun-28 07:37 iothello-1.1.6.dist-info/LICENCE.txt
--rw-rw-rw-  2.0 fat      426 b- defN 22-Jun-28 07:37 iothello-1.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-28 07:37 iothello-1.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Jun-28 07:37 iothello-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3373 b- defN 22-Jun-28 07:37 iothello-1.1.6.dist-info/RECORD
-41 files, 102949 bytes uncompressed, 61594 bytes compressed:  40.2%
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-19 09:23 iothello-1.1.7.dist-info/LICENCE.txt
+-rw-rw-rw-  2.0 fat      443 b- defN 23-Apr-19 09:23 iothello-1.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 09:23 iothello-1.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-19 09:23 iothello-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3373 b- defN 23-Apr-19 09:23 iothello-1.1.7.dist-info/RECORD
+41 files, 102968 bytes uncompressed, 61596 bytes compressed:  40.2%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: iothello/models/8_ridge.sav
 Comment: 
 
 Filename: iothello/models/9_ridge.sav
 Comment: 
 
-Filename: iothello-1.1.6.dist-info/LICENCE.txt
+Filename: iothello-1.1.7.dist-info/LICENCE.txt
 Comment: 
 
-Filename: iothello-1.1.6.dist-info/METADATA
+Filename: iothello-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: iothello-1.1.6.dist-info/WHEEL
+Filename: iothello-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: iothello-1.1.6.dist-info/top_level.txt
+Filename: iothello-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: iothello-1.1.6.dist-info/RECORD
+Filename: iothello-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iothello/gui.py

 * *Ordering differences only*

```diff
@@ -148,8 +148,8 @@
 
             move_count += 1
             self.draw_piece()
             player = -player
 
 
 def play():
-    Gui().main_menu()
+    Gui().main_menu()
```

## Comparing `iothello-1.1.6.dist-info/LICENCE.txt` & `iothello-1.1.7.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `iothello-1.1.6.dist-info/RECORD` & `iothello-1.1.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 iothello/__init__.py,sha256=269649Gm6LZoz2l3CVVrVEn8Sd7CCAlCy81e1Vb5pts,31
 iothello/backend_gui.py,sha256=m6BMdDjCSUePHSB-rMDoclEhZ9ApDTIW44txNcOCMCU,6636
 iothello/font.otf,sha256=fGuef6yhkDKglJ24t2jUyEGpx8jgMjW-Uuj0jWUAEAs,60852
-iothello/gui.py,sha256=6R1oJTO6tGSnfJEfjm1ZURCbRT4xvR8QE6rBuSr-un0,5666
+iothello/gui.py,sha256=uZAp-AR69N7QoUcgIEbJzBhJ90fp8xVTUqgKyl-rxVU,5668
 iothello/models/0_ridge.sav,sha256=b3yjueBq_FuWAkbtmjIF9qwKVy786_7rt-5czjUg9mM,770
 iothello/models/10_ridge.sav,sha256=cAePdo62fiK2hQISMidwKgW75qGxv4fjaVF2r__XUCY,770
 iothello/models/11_ridge.sav,sha256=Fcqe830PonPlsrHup2BF5BFtO23B4_db30top5U4ss4,770
 iothello/models/12_ridge.sav,sha256=ryCj76dNWi3CSO7rYP_r3MJmwTFkwyB65uhQyA8W_hw,770
 iothello/models/13_ridge.sav,sha256=XwBBrKXZstO2hnNlmfvr0d2qjAneztGGG3oJVVor2kQ,770
 iothello/models/14_ridge.sav,sha256=5yTPR1Avcx5ABBKLNYna4WfdYk3lSMkLNd_oMDg4NxQ,770
 iothello/models/15_ridge.sav,sha256=wrUVRUfKuAyY-x-BMzsvGyo091gjZ5WYzCjY7UpwRvg,770
@@ -30,12 +30,12 @@
 iothello/models/3_ridge.sav,sha256=9Ni_4UrnHVqnNcetf5igdlJdKGKMeWhjGaSjVC1uRac,770
 iothello/models/4_ridge.sav,sha256=9iTH8W9cZL3qMIuy-rNhO03mSaxx9bL3R6RVWeCx_nY,770
 iothello/models/5_ridge.sav,sha256=uZvEt9sxLf2C8lHO88p1yCVPHljtIfTXjDB-4DtY3mc,770
 iothello/models/6_ridge.sav,sha256=a8fNC3FkdaQJW86lixu7-1vvo53j_gihengcGHbuO7M,770
 iothello/models/7_ridge.sav,sha256=zCkKQW52F7lXrnebTJM7kwGtUPXREh5AZuFw5OEmQCA,770
 iothello/models/8_ridge.sav,sha256=3OhrEH2BAzKGbMxEVSqPbg2xSZoddkDSyP21asGT3QY,770
 iothello/models/9_ridge.sav,sha256=JN4_k03gPuI2x8bbEV1ScB_vwXCfGGvgU9kXYuHY_pI,770
-iothello-1.1.6.dist-info/LICENCE.txt,sha256=1Hg-a1yebiVDAXsKsZVseaaNbI8Wc9bCQydVKhpr3rs,1093
-iothello-1.1.6.dist-info/METADATA,sha256=apy7e0qTuPFpj_H6uf6s5F2Cb7feQ2ujHVZ9VnSzxu0,426
-iothello-1.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-iothello-1.1.6.dist-info/top_level.txt,sha256=VppwlCnRUJca2_10ebkL6QTXhPb49dKa3Gke--3eGw8,9
-iothello-1.1.6.dist-info/RECORD,,
+iothello-1.1.7.dist-info/LICENCE.txt,sha256=1Hg-a1yebiVDAXsKsZVseaaNbI8Wc9bCQydVKhpr3rs,1093
+iothello-1.1.7.dist-info/METADATA,sha256=L8mAQngyNg4In_CA6shxNV6g5B0uowYI_fCdz7kLnqI,443
+iothello-1.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+iothello-1.1.7.dist-info/top_level.txt,sha256=VppwlCnRUJca2_10ebkL6QTXhPb49dKa3Gke--3eGw8,9
+iothello-1.1.7.dist-info/RECORD,,
```

