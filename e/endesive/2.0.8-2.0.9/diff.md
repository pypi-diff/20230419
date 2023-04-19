# Comparing `tmp/endesive-2.0.8-py3-none-any.whl.zip` & `tmp/endesive-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 340833 bytes, number of entries: 68
--rw-rw-r--  2.0 unx      159 b- defN 22-Jan-15 23:53 endesive/__init__.py
+Zip file size: 340825 bytes, number of entries: 68
+-rw-rw-r--  2.0 unx      159 b- defN 22-Mar-28 16:35 endesive/__init__.py
 -rw-rw-r--  2.0 unx    13201 b- defN 20-Jul-12 17:19 endesive/hsm.py
 -rw-rw-r--  2.0 unx     9208 b- defN 22-Jan-07 23:44 endesive/signer.py
--rw-rw-r--  2.0 unx     4587 b- defN 21-Feb-05 15:58 endesive/verifier.py
+-rw-rw-r--  2.0 unx     4587 b- defN 22-Mar-26 18:08 endesive/verifier.py
 -rw-rw-r--  2.0 unx      132 b- defN 20-Jul-12 17:19 endesive/email/__init__.py
 -rw-rw-r--  2.0 unx     3301 b- defN 20-Jul-12 17:19 endesive/email/decrypt.py
 -rw-rw-r--  2.0 unx     4593 b- defN 20-Jul-12 17:19 endesive/email/encrypt.py
 -rw-rw-r--  2.0 unx     1429 b- defN 20-Jul-12 17:19 endesive/email/sign.py
 -rw-rw-r--  2.0 unx      816 b- defN 20-Jul-12 17:19 endesive/email/verify.py
 -rw-rw-r--  2.0 unx       63 b- defN 20-Jul-12 17:19 endesive/pdf/__init__.py
 -rw-rw-r--  2.0 unx    39890 b- defN 22-Mar-01 10:49 endesive/pdf/cms.py
@@ -55,16 +55,16 @@
 -rw-rw-r--  2.0 unx     9282 b- defN 20-Jul-12 17:19 endesive/pdf/fpdf/template.py
 -rw-rw-r--  2.0 unx    39345 b- defN 20-Jul-12 17:19 endesive/pdf/fpdf/ttfonts.py
 -rw-rw-r--  2.0 unx       50 b- defN 20-Jul-12 17:19 endesive/plain/__init__.py
 -rw-rw-r--  2.0 unx      203 b- defN 20-Jul-12 17:19 endesive/plain/sign.py
 -rw-rw-r--  2.0 unx      137 b- defN 20-Jul-12 17:19 endesive/plain/verify.py
 -rw-rw-r--  2.0 unx       21 b- defN 20-Jul-12 17:19 endesive/xades/__init__.py
 -rw-rw-r--  2.0 unx    20307 b- defN 20-Nov-24 02:34 endesive/xades/bes.py
--rw-rw-r--  2.0 unx     1076 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1073 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/LICENSE.pdf-annotate
--rw-rw-r--  2.0 unx     7632 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/LICENSE.pyfpdf
--rw-rw-r--  2.0 unx     1605 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/LICENSE.pypdf2
--rw-rw-r--  2.0 unx     5660 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6128 b- defN 22-Mar-15 23:49 endesive-2.0.8.dist-info/RECORD
-68 files, 967551 bytes uncompressed, 331003 bytes compressed:  65.8%
+-rw-rw-r--  2.0 unx     1076 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/LICENSE.pdf-annotate
+-rw-rw-r--  2.0 unx     7632 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/LICENSE.pyfpdf
+-rw-rw-r--  2.0 unx     1605 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/LICENSE.pypdf2
+-rw-rw-r--  2.0 unx     5660 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6128 b- defN 22-Mar-28 16:38 endesive-2.0.9.dist-info/RECORD
+68 files, 967551 bytes uncompressed, 330995 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -174,32 +174,32 @@
 
 Filename: endesive/xades/__init__.py
 Comment: 
 
 Filename: endesive/xades/bes.py
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/LICENSE
+Filename: endesive-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/LICENSE.pdf-annotate
+Filename: endesive-2.0.9.dist-info/LICENSE.pdf-annotate
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/LICENSE.pyfpdf
+Filename: endesive-2.0.9.dist-info/LICENSE.pyfpdf
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/LICENSE.pypdf2
+Filename: endesive-2.0.9.dist-info/LICENSE.pypdf2
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/METADATA
+Filename: endesive-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/WHEEL
+Filename: endesive-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/top_level.txt
+Filename: endesive-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: endesive-2.0.8.dist-info/RECORD
+Filename: endesive-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## endesive/__init__.py

```diff
@@ -1,7 +1,7 @@
 """Python ENDESIVE library."""
 
 __author__ = 'Grzegorz Makarewicz'
 __license__ = 'MIT'
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 __all__ = [__author__, __license__, __version__]
```

## endesive/verifier.py

```diff
@@ -38,15 +38,15 @@
                 _, _, cert_bytes = pem.unarmor(cert_bytes)
             return x509.Certificate.load(cert_bytes)
 
     def verify(self, datas, datau):
         signed_data = cms.ContentInfo.load(datas)['content']
         # signed_data.debug()
 
-        signature = signed_data['signer_infos'][0].native['signature']
+        signature = signed_data['signer_infos'][0]['signature'].native
         algo = signed_data['digest_algorithms'][0]['algorithm'].native
         attrs = signed_data['signer_infos'][0]['signed_attrs']
         mdData = getattr(hashlib, algo)(datau).digest()
         if attrs is not None and not isinstance(attrs, core.Void):
             mdSigned = None
             for attr in attrs:
                 if attr['type'].native == 'message_digest':
```

## Comparing `endesive-2.0.8.dist-info/LICENSE` & `endesive-2.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `endesive-2.0.8.dist-info/LICENSE.pdf-annotate` & `endesive-2.0.9.dist-info/LICENSE.pdf-annotate`

 * *Files identical despite different names*

## Comparing `endesive-2.0.8.dist-info/LICENSE.pyfpdf` & `endesive-2.0.9.dist-info/LICENSE.pyfpdf`

 * *Files identical despite different names*

## Comparing `endesive-2.0.8.dist-info/LICENSE.pypdf2` & `endesive-2.0.9.dist-info/LICENSE.pypdf2`

 * *Files identical despite different names*

## Comparing `endesive-2.0.8.dist-info/METADATA` & `endesive-2.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endesive
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library for digital signing and verification of digital signatures in mail, PDF and XML documents.
 Home-page: https://github.com/m32/endesive
 Author: Grzegorz Makarewicz
 Author-email: mak@trisoft.com.pl
 License: MIT
 Keywords: cryptography pki x509 smime email pdf pkcs11 asn1 xades
 Platform: all
```

## Comparing `endesive-2.0.8.dist-info/RECORD` & `endesive-2.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-endesive/__init__.py,sha256=xQlnuYQlZLvwTpU6u1cye4tjzsLXjuAf2otPPIjAdhM,159
+endesive/__init__.py,sha256=GzGLfaiZZoYeRW7-XPr_-DouZulmq2aH5NMNkE_lG94,159
 endesive/hsm.py,sha256=hIrkt3bfJytMuVkA2CACryEq0KEHiPfGnxC7cVda-eI,13201
 endesive/signer.py,sha256=DTYxcCBJTH5G1zYsHI7to_GDtA32Da6ZzMEs3XVL2mg,9208
-endesive/verifier.py,sha256=-lnc0mcegOxrfU4k-ZsKdWyhrUlhVGPofgEeiiqPJvg,4587
+endesive/verifier.py,sha256=DGjk_U-Va9FW-nM3hMPvgDvKsIKawZoRwSFP4JebK_c,4587
 endesive/email/__init__.py,sha256=lCeGLDR0S8MkEHBT6aKrjYYQXHnipnVGu0-M7jpzXpA,132
 endesive/email/decrypt.py,sha256=zNhRaJvRTnwiyvrJofUiBNjKlP6hL3jfRoHgj3DDKyQ,3301
 endesive/email/encrypt.py,sha256=Vqi2EFZmBc8i9Gdhqo2DR_vB-Ewhb62eCvT224fg74g,4593
 endesive/email/sign.py,sha256=wAJaz3fj-fbUVOSaPzLGhlAeik1ZW29GajVjbaAMqHA,1429
 endesive/email/verify.py,sha256=ePGsAWVBWpW7wPANtrUtYlTCYnWEnVQVCvxH8Z63vns,816
 endesive/pdf/__init__.py,sha256=j3ukEpzd35jQHSJk8pk0smsGC-pb6YAfnrZZN8dMfKE,63
 endesive/pdf/cms.py,sha256=wDtBGNLZQv1QrcOlEdd8xws-5vWpf6VqiboVBLtgVCA,39890
@@ -54,15 +54,15 @@
 endesive/pdf/fpdf/template.py,sha256=8AJ_-oYLBh2ZaIOXQrFtMp9sWyZajgpjSBJDWxqkL2U,9282
 endesive/pdf/fpdf/ttfonts.py,sha256=ekuwPDsbH8msrKaZt0saRedDKbAcQPc0-TtUh-svWnw,39345
 endesive/plain/__init__.py,sha256=6cywlFN6nG3mhEjkJZkbkLAHWMrVJoowFp7568jPlbc,50
 endesive/plain/sign.py,sha256=rlDL5RNZuks8zlx26CZH0mKHM9jqOtQjtRME-dkRaI8,203
 endesive/plain/verify.py,sha256=Wsm81crUW3H1SBl3SCqnBj7g_kfN6YvzRNsKm1f0muc,137
 endesive/xades/__init__.py,sha256=85bxEaA9DJdfKRuoAfmMj4E58NAJQo7mMqc-bxFKIa8,21
 endesive/xades/bes.py,sha256=rWSiFF4H9D55fHf_rEAfZtaJMPQ4Gx9LVjtexSJSgrk,20307
-endesive-2.0.8.dist-info/LICENSE,sha256=ybveZh1lwiEhaP0MHYzyHZcC9AU2hPqytPImQh_U_D8,1076
-endesive-2.0.8.dist-info/LICENSE.pdf-annotate,sha256=q6S3sjJq3CAVgjelqrIlBFuoc7Dik0bdhMvbi4LWdDg,1073
-endesive-2.0.8.dist-info/LICENSE.pyfpdf,sha256=-XvEu5t66KZTlBBzZ4tcd3Xo3kSgHDvMIefNwUi5DmE,7632
-endesive-2.0.8.dist-info/LICENSE.pypdf2,sha256=qXrCMOXzPvEKU2eoUOsB-R8aCwZONHQsd5TSKUVX9SQ,1605
-endesive-2.0.8.dist-info/METADATA,sha256=gSG62Sy-n6ZxnfNmNLrdmbl3qAZLXBhjSyg0SBBg1TE,5660
-endesive-2.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-endesive-2.0.8.dist-info/top_level.txt,sha256=OSartL5MHflKHQIFPWEmG1FFXHEcLiJ0M2kGTbddrBM,9
-endesive-2.0.8.dist-info/RECORD,,
+endesive-2.0.9.dist-info/LICENSE,sha256=ybveZh1lwiEhaP0MHYzyHZcC9AU2hPqytPImQh_U_D8,1076
+endesive-2.0.9.dist-info/LICENSE.pdf-annotate,sha256=q6S3sjJq3CAVgjelqrIlBFuoc7Dik0bdhMvbi4LWdDg,1073
+endesive-2.0.9.dist-info/LICENSE.pyfpdf,sha256=-XvEu5t66KZTlBBzZ4tcd3Xo3kSgHDvMIefNwUi5DmE,7632
+endesive-2.0.9.dist-info/LICENSE.pypdf2,sha256=qXrCMOXzPvEKU2eoUOsB-R8aCwZONHQsd5TSKUVX9SQ,1605
+endesive-2.0.9.dist-info/METADATA,sha256=uXaKEewQYNhm2M2IS2UphEVu-H3FtnZyhGSzfIPmcNw,5660
+endesive-2.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+endesive-2.0.9.dist-info/top_level.txt,sha256=OSartL5MHflKHQIFPWEmG1FFXHEcLiJ0M2kGTbddrBM,9
+endesive-2.0.9.dist-info/RECORD,,
```

