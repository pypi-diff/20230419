# Comparing `tmp/pds_one-1.3.2-py3-none-any.whl.zip` & `tmp/pds_one-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7204 bytes, number of entries: 10
+Zip file size: 7226 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Nov-26 12:41 pds_one/__init__.py
 -rw-rw-rw-  2.0 fat     6746 b- defN 22-Apr-18 07:35 pds_one/functions.py
--rw-rw-rw-  2.0 fat     9846 b- defN 23-Mar-24 12:13 pds_one/main.py
+-rw-rw-rw-  2.0 fat     9965 b- defN 23-Apr-19 13:17 pds_one/main.py
 -rw-rw-rw-  2.0 fat      273 b- defN 21-Nov-26 12:41 pds_one/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Nov-26 12:41 pds_one/tests/__init__.py
 -rw-rw-rw-  2.0 fat      260 b- defN 21-Nov-26 12:41 pds_one/tests/server_tests.py
--rw-rw-rw-  2.0 fat     1014 b- defN 23-Mar-24 12:14 pds_one-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-24 12:14 pds_one-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-24 12:14 pds_one-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      758 b- defN 23-Mar-24 12:14 pds_one-1.3.2.dist-info/RECORD
-10 files, 18997 bytes uncompressed, 5912 bytes compressed:  68.9%
+-rw-rw-rw-  2.0 fat     1014 b- defN 23-Apr-19 13:18 pds_one-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 13:18 pds_one-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-19 13:18 pds_one-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      758 b- defN 23-Apr-19 13:18 pds_one-1.4.0.dist-info/RECORD
+10 files, 19116 bytes uncompressed, 5934 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: pds_one/tests/__init__.py
 Comment: 
 
 Filename: pds_one/tests/server_tests.py
 Comment: 
 
-Filename: pds_one-1.3.2.dist-info/METADATA
+Filename: pds_one-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: pds_one-1.3.2.dist-info/WHEEL
+Filename: pds_one-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: pds_one-1.3.2.dist-info/top_level.txt
+Filename: pds_one-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pds_one-1.3.2.dist-info/RECORD
+Filename: pds_one-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pds_one/main.py

```diff
@@ -131,14 +131,16 @@
                 if self.scale_protocol == 'art':
                     data = self.port.read_until(expected=b'\rG')
                 elif self.scale_protocol == 'uzvo':
                     data = self.port.read_until(expected=b"\x03\x02")
                 else:
                     if self.scale_protocol == '6.43':
                         self.port.write([16])
+                    if self.scale_protocol == "middle":
+                        self.port.write(bytes.fromhex("0A"))
                     data = self.port.readline()
             except serial.serialutil.SerialException:
                 data = s.scale_disconnected_code
                 print(format_exc())
             self.show_print('Data from port:', data, debug=True)
             if data:
                 # Если есть данные проверить их и добавить в список отправки data_list
```

## Comparing `pds_one-1.3.2.dist-info/METADATA` & `pds_one-1.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pds-one
-Version: 1.3.2
+Version: 1.4.0
 Author: PunchyArchy
 Author-email: ksmdrmvscthny@gmail.com
 Requires-Dist: pyserial (==3.5)
 
 PDS (Port Data Splitter) - это программный разветлитель данных, реализованный в виде TCP сервера,
 прослушивающего некоторый порт (USB, COM) и рассылающего эти данные своим клиентам (subscribers).
```

## Comparing `pds_one-1.3.2.dist-info/RECORD` & `pds_one-1.4.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pds_one/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pds_one/functions.py,sha256=hO3Plq4MEfoCTTZ9OdLqFaGxmcahMnGJKhC6zmuYG48,6746
-pds_one/main.py,sha256=HYcsPpV3LY20w731FUbYw1rIsBijdxicbNyOFBhhp7g,9846
+pds_one/main.py,sha256=m1fB5tDqveYqYCap1w_rNLADQ6vZ30079IU_eaLzr3Y,9965
 pds_one/settings.py,sha256=0CaDB8C9o969OEK6xXclOKbJKL26Ajix-gEgfZdm6oE,273
 pds_one/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pds_one/tests/server_tests.py,sha256=AeJPWbMq1poMLfTVociCwpkgBRFAHf6Xkkawbx5CwuU,260
-pds_one-1.3.2.dist-info/METADATA,sha256=vSHw4sTjAa2QLSqm9zRG6rqW_UMwNzt5BJCAqe6eirQ,1014
-pds_one-1.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pds_one-1.3.2.dist-info/top_level.txt,sha256=vtcopFCoeEFCN8RTKgCkqmVu07wx8-p-4V7xpz09mrA,8
-pds_one-1.3.2.dist-info/RECORD,,
+pds_one-1.4.0.dist-info/METADATA,sha256=36i-YQJ2ZIdqDMsrz1TGbOhs6Mar5keJPL6bN5Qw6Ls,1014
+pds_one-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pds_one-1.4.0.dist-info/top_level.txt,sha256=vtcopFCoeEFCN8RTKgCkqmVu07wx8-p-4V7xpz09mrA,8
+pds_one-1.4.0.dist-info/RECORD,,
```

