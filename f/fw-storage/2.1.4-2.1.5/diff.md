# Comparing `tmp/fw_storage-2.1.4-py3-none-any.whl.zip` & `tmp/fw_storage-2.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 37647 bytes, number of entries: 24
+Zip file size: 37674 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      511 b- defN 80-Jan-01 00:00 fw_storage/__init__.py
--rw-r--r--  2.0 unx    18067 b- defN 80-Jan-01 00:00 fw_storage/config.py
+-rw-r--r--  2.0 unx    18182 b- defN 80-Jan-01 00:00 fw_storage/config.py
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 fw_storage/errors.py
 -rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
 -rw-r--r--  2.0 unx     1016 b- defN 80-Jan-01 00:00 fw_storage/filters.py
 -rw-r--r--  2.0 unx     1013 b- defN 80-Jan-01 00:00 fw_storage/future/__init__.py
 -rw-r--r--  2.0 unx    11541 b- defN 80-Jan-01 00:00 fw_storage/future/base.py
 -rw-r--r--  2.0 unx     4652 b- defN 80-Jan-01 00:00 fw_storage/future/errors.py
 -rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 fw_storage/future/types/__init__.py
@@ -15,12 +15,12 @@
 -rw-r--r--  2.0 unx       28 b- defN 80-Jan-01 00:00 fw_storage/types/__init__.py
 -rw-r--r--  2.0 unx     6844 b- defN 80-Jan-01 00:00 fw_storage/types/az.py
 -rw-r--r--  2.0 unx    13338 b- defN 80-Jan-01 00:00 fw_storage/types/dicom.py
 -rw-r--r--  2.0 unx     7996 b- defN 80-Jan-01 00:00 fw_storage/types/dicomweb.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 fw_storage/types/fs.py
 -rw-r--r--  2.0 unx     4861 b- defN 80-Jan-01 00:00 fw_storage/types/gs.py
 -rw-r--r--  2.0 unx     6374 b- defN 80-Jan-01 00:00 fw_storage/types/s3.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1924 b- defN 16-Jan-01 00:00 fw_storage-2.1.4.dist-info/RECORD
-24 files, 108764 bytes uncompressed, 34563 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1924 b- defN 16-Jan-01 00:00 fw_storage-2.1.5.dist-info/RECORD
+24 files, 108879 bytes uncompressed, 34590 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: fw_storage/types/gs.py
 Comment: 
 
 Filename: fw_storage/types/s3.py
 Comment: 
 
-Filename: fw_storage-2.1.4.dist-info/LICENSE
+Filename: fw_storage-2.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: fw_storage-2.1.4.dist-info/METADATA
+Filename: fw_storage-2.1.5.dist-info/METADATA
 Comment: 
 
-Filename: fw_storage-2.1.4.dist-info/WHEEL
+Filename: fw_storage-2.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: fw_storage-2.1.4.dist-info/RECORD
+Filename: fw_storage-2.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_storage/config.py

```diff
@@ -117,18 +117,21 @@
         """Return safe storage URL without credentials."""
         return format_url(scheme=self.type, host=self.bucket, path=self.prefix)
 
     @property
     def full_url(self) -> str:
         """Return full storage URL with credentials."""
         data = self.dict(secret="val")  # noqa: S106
-        return self.safe_url + qs(
-            access_key_id=data["access_key_id"],
-            secret_access_key=data["secret_access_key"],
-        )
+        qparams = {
+            "access_key_id": data["access_key_id"],
+            "secret_access_key": data["secret_access_key"],
+        }
+        if self.connector_creds:
+            qparams["connector_creds"] = True
+        return self.safe_url + qs(**qparams)
 
     @root_validator(pre=True)
     @classmethod
     def load_creds(cls, values: dict) -> dict:
         """Load creds from the env if enabled."""
         if values.get("connector_creds"):
             # drop creds if passed
```

## Comparing `fw_storage-2.1.4.dist-info/LICENSE` & `fw_storage-2.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_storage-2.1.4.dist-info/METADATA` & `fw_storage-2.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-storage
-Version: 2.1.4
+Version: 2.1.5
 Summary: Unified storage interface.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-storage
 License: MIT
 Keywords: Flywheel,file,object,storage
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_storage-2.1.4.dist-info/RECORD` & `fw_storage-2.1.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 fw_storage/__init__.py,sha256=v36QDeDLZJv7Sj2zXEZ6s0YIxuz42A9OA8boUEFnPvk,511
-fw_storage/config.py,sha256=oXx3c-HaDFtY5U8RhgwFfKF-VaAI7O2JAtn3AmxOQ_w,18067
+fw_storage/config.py,sha256=VNKq8MNQ4dudrJqU6tBmEx8s5kmOdqKhliFvnvncx_s,18182
 fw_storage/errors.py,sha256=HD92V9ebpmsILbhf239XRSmwmO_-WHiOEuYdCUnL1V4,113
 fw_storage/fileinfo.py,sha256=6Xwu3OewGiua6DYFGObNJIAJvF1yiFfdC9sbaJ1nqgc,963
 fw_storage/filters.py,sha256=P3C1oGw1q6UoNEbHiSr-xdi_jumosSKOQgsulZ2GGaA,1016
 fw_storage/future/__init__.py,sha256=TWyZ7CFeCDO4_uiiT6gLJhE-SP8Ie7bNsCB3vUSbv2U,1013
 fw_storage/future/base.py,sha256=XXC7vXnQxWImOfPdj0ez2klhSWKxtMrr8oWo_JcDro4,11541
 fw_storage/future/errors.py,sha256=tE-wb4n_X8-v2zaU5KpoPlQVfDaDhazOpjLmNU45cw0,4652
 fw_storage/future/types/__init__.py,sha256=zOnfjDtMpINsVdYFikGbvjIf_FVnfPpm-DanhqDrLjo,36
@@ -14,11 +14,11 @@
 fw_storage/types/__init__.py,sha256=TT2pfyY-AMuKb4FZduNbVbmWTBRyEC3autb1QbdHE24,28
 fw_storage/types/az.py,sha256=J2KbT9ugvTpLfAZg4BX0lDLK4i2lM8EYisyAnj9tVG4,6844
 fw_storage/types/dicom.py,sha256=XUSFsdSGTyNb8a6-K2H0jvztzj5lT5FmuGHt8pi_SCI,13338
 fw_storage/types/dicomweb.py,sha256=NR9E-csPgznASouwIdokukAxGPKCPRobhz80e4-z_v0,7996
 fw_storage/types/fs.py,sha256=Cz_GGrS_e11m9SvDgdjJkMf-VMI0s5DKUJZp0bWSegM,140
 fw_storage/types/gs.py,sha256=lQRo9qz0EHf3YmPO7LzLBFYEGkwqhmlVtxwF2T9EISI,4861
 fw_storage/types/s3.py,sha256=MMelCfrbaNZbZqGPBj9mt_Cdyhrbeq-ObYmmC4bM1G4,6374
-fw_storage-2.1.4.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_storage-2.1.4.dist-info/METADATA,sha256=XqHzCucuu5CovsSJkh-nasa5ZU1hFmnFv9CXk1Le6tg,4013
-fw_storage-2.1.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_storage-2.1.4.dist-info/RECORD,,
+fw_storage-2.1.5.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_storage-2.1.5.dist-info/METADATA,sha256=prFrwIkmvnhpOXl9UPNjWRyJHA3l18suPvCXm6Si36k,4013
+fw_storage-2.1.5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_storage-2.1.5.dist-info/RECORD,,
```

