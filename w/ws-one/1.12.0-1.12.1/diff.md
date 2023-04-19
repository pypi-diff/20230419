# Comparing `tmp/ws_one-1.12.0-py3-none-any.whl.zip` & `tmp/ws_one-1.12.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13783 bytes, number of entries: 34
+Zip file size: 13778 bytes, number of entries: 34
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/__init__.py
 -rw-rw-rw-  2.0 fat      609 b- defN 22-Mar-29 12:06 ws_one_stable/errors.py
 -rw-rw-rw-  2.0 fat     4144 b- defN 23-Mar-22 08:18 ws_one_stable/main.py
 -rw-rw-rw-  2.0 fat      149 b- defN 21-Nov-29 08:04 ws_one_stable/server_test.py
 -rw-rw-rw-  2.0 fat      492 b- defN 21-Sep-30 05:48 ws_one_stable/settings.py
 -rw-rw-rw-  2.0 fat     1117 b- defN 21-Nov-29 08:04 ws_one_stable/support_functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/terminals/__init__.py
@@ -24,13 +24,13 @@
 -rw-rw-rw-  2.0 fat      590 b- defN 22-Nov-14 05:04 ws_one_stable/terminals/Uvzo/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 12:59 ws_one_stable/terminals/middle_mi010/__init__.py
 -rw-rw-rw-  2.0 fat      431 b- defN 23-Apr-19 13:01 ws_one_stable/terminals/middle_mi010/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/tests/__init__.py
 -rw-rw-rw-  2.0 fat      145 b- defN 21-Sep-30 05:48 ws_one_stable/tests/client_test.py
 -rw-rw-rw-  2.0 fat       68 b- defN 21-Sep-30 05:48 ws_one_stable/tests/settings_test.py
 -rw-rw-rw-  2.0 fat      651 b- defN 21-Sep-30 05:48 ws_one_stable/tests/support_functions_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-19 13:05 ws_one-1.12.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1063 b- defN 23-Apr-19 13:05 ws_one-1.12.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 13:05 ws_one-1.12.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-19 13:05 ws_one-1.12.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3084 b- defN 23-Apr-19 13:05 ws_one-1.12.0.dist-info/RECORD
-34 files, 17878 bytes uncompressed, 8665 bytes compressed:  51.5%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-19 13:20 ws_one-1.12.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1063 b- defN 23-Apr-19 13:20 ws_one-1.12.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 13:20 ws_one-1.12.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-19 13:20 ws_one-1.12.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3084 b- defN 23-Apr-19 13:20 ws_one-1.12.1.dist-info/RECORD
+34 files, 17878 bytes uncompressed, 8660 bytes compressed:  51.6%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: ws_one_stable/tests/settings_test.py
 Comment: 
 
 Filename: ws_one_stable/tests/support_functions_tests.py
 Comment: 
 
-Filename: ws_one-1.12.0.dist-info/LICENSE
+Filename: ws_one-1.12.1.dist-info/LICENSE
 Comment: 
 
-Filename: ws_one-1.12.0.dist-info/METADATA
+Filename: ws_one-1.12.1.dist-info/METADATA
 Comment: 
 
-Filename: ws_one-1.12.0.dist-info/WHEEL
+Filename: ws_one-1.12.1.dist-info/WHEEL
 Comment: 
 
-Filename: ws_one-1.12.0.dist-info/top_level.txt
+Filename: ws_one-1.12.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ws_one-1.12.0.dist-info/RECORD
+Filename: ws_one-1.12.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ws_one-1.12.0.dist-info/LICENSE` & `ws_one-1.12.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ws_one-1.12.0.dist-info/METADATA` & `ws_one-1.12.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ws-one
-Version: 1.12.0
+Version: 1.12.1
 Author: PunchyArchy
 Author-email: ksmdrmvscthny@gmail.com
 License-File: LICENSE
 Requires-Dist: pyserial
-Requires-Dist: pds-one (==1.3.2)
+Requires-Dist: pds-one (==1.4.0)
 
 PDS (Port Data Splitter) - это программный разветлитель данных, реализованный в виде TCP сервера,
 прослушивающего некоторый порт (USB, COM) и рассылающего эти данные своим клиентам (subscribers).
 
 Пример использования (Рассыльщик данных с USB на порту 2290 на Linux):
 pds = PortDataSplitter('0.0.0.0', 2290, port_name='/dev/ttyUSB0', debug=False, device_name='USB listener')
```

## Comparing `ws_one-1.12.0.dist-info/RECORD` & `ws_one-1.12.1.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 ws_one_stable/terminals/Uvzo/functions.py,sha256=IKBj2mvpcVXQDwLqw2Uua99Z8bCIiE22TVwP2R-7RtA,590
 ws_one_stable/terminals/middle_mi010/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/terminals/middle_mi010/functions.py,sha256=o7PtlHQ3hLRDwCo41OD46IyNdUv7PzUJjAg7OS8H1xg,431
 ws_one_stable/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/tests/client_test.py,sha256=2xT9G4dOB66pYp7pQ4pjiRdihGioz3gUo9k-TcWcbaw,145
 ws_one_stable/tests/settings_test.py,sha256=uhQjp-fDlMZW3_Q0uDFRBg_bjujcUNSnk8tGqXEjgo4,68
 ws_one_stable/tests/support_functions_tests.py,sha256=u_7UqjhrUqjUlFQi8x4gVQ2ERqe54NMVXRdZmI57cqw,651
-ws_one-1.12.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ws_one-1.12.0.dist-info/METADATA,sha256=JGmLxfYD0yJywetcpb9N-ey4ICQ4MkvLFxzaU5QKA0o,1063
-ws_one-1.12.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ws_one-1.12.0.dist-info/top_level.txt,sha256=VucC9pCRaAyG119eEE7EoLBql-CDOLFUfKGqOxGIA8Q,14
-ws_one-1.12.0.dist-info/RECORD,,
+ws_one-1.12.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ws_one-1.12.1.dist-info/METADATA,sha256=uz93fC17iP7Fup_vrsRI2pnJbVrf98CB6sklIl-S7Eo,1063
+ws_one-1.12.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ws_one-1.12.1.dist-info/top_level.txt,sha256=VucC9pCRaAyG119eEE7EoLBql-CDOLFUfKGqOxGIA8Q,14
+ws_one-1.12.1.dist-info/RECORD,,
```

