# Comparing `tmp/pycvc-1.2.3-py3-none-any.whl.zip` & `tmp/pycvc-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 22029 bytes, number of entries: 16
--rw-r--r--  2.0 unx       34 b- defN 22-Aug-19 10:13 cvc/__init__.py
--rw-r--r--  2.0 unx      770 b- defN 23-Apr-18 06:52 cvc/_version.py
--rw-r--r--  2.0 unx     3507 b- defN 23-Mar-08 21:04 cvc/asn1.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Apr-18 06:46 cvc/certificates.py
--rw-r--r--  2.0 unx    15209 b- defN 22-Aug-22 13:32 cvc/ec_curves.py
--rw-r--r--  2.0 unx     8006 b- defN 22-Aug-23 11:50 cvc/oid.py
--rw-r--r--  2.0 unx     2508 b- defN 23-Apr-18 06:51 cvc/terminal.py
--rw-r--r--  2.0 unx     2639 b- defN 22-Aug-19 11:35 cvc/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-17 12:41 cvc/tools/__init__.py
--rw-r--r--  2.0 unx    12838 b- defN 23-Apr-18 06:48 cvc/tools/cvc_create.py
--rw-r--r--  2.0 unx     4829 b- defN 23-Apr-17 12:42 cvc/tools/cvc_print.py
--rw-r--r--  2.0 unx     5600 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1185 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/RECORD
-16 files, 66584 bytes uncompressed, 20117 bytes compressed:  69.8%
+Zip file size: 22266 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Apr-19 06:06 cvc/__init__.py
+-rw-rw-rw-  2.0 fat      791 b- defN 23-Apr-19 06:37 cvc/_version.py
+-rw-rw-rw-  2.0 fat     3626 b- defN 23-Apr-19 06:06 cvc/asn1.py
+-rw-rw-rw-  2.0 fat     9544 b- defN 23-Apr-19 06:23 cvc/certificates.py
+-rw-rw-rw-  2.0 fat    15373 b- defN 23-Apr-19 06:06 cvc/ec_curves.py
+-rw-rw-rw-  2.0 fat     8204 b- defN 23-Apr-19 06:06 cvc/oid.py
+-rw-rw-rw-  2.0 fat     2574 b- defN 23-Apr-19 06:06 cvc/terminal.py
+-rw-rw-rw-  2.0 fat     2699 b- defN 23-Apr-19 06:06 cvc/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 06:06 cvc/tools/__init__.py
+-rw-rw-rw-  2.0 fat    13073 b- defN 23-Apr-19 06:06 cvc/tools/cvc_create.py
+-rw-rw-rw-  2.0 fat     4957 b- defN 23-Apr-19 06:06 cvc/tools/cvc_print.py
+-rw-rw-rw-  2.0 fat     7197 b- defN 23-Apr-19 06:46 pycvc-1.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 06:46 pycvc-1.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 06:46 pycvc-1.2.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-19 06:46 pycvc-1.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1185 b- defN 23-Apr-19 06:46 pycvc-1.2.4.dist-info/RECORD
+16 files, 69456 bytes uncompressed, 20354 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: cvc/tools/cvc_create.py
 Comment: 
 
 Filename: cvc/tools/cvc_print.py
 Comment: 
 
-Filename: pycvc-1.2.3.dist-info/METADATA
+Filename: pycvc-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: pycvc-1.2.3.dist-info/WHEEL
+Filename: pycvc-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: pycvc-1.2.3.dist-info/entry_points.txt
+Filename: pycvc-1.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: pycvc-1.2.3.dist-info/top_level.txt
+Filename: pycvc-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pycvc-1.2.3.dist-info/RECORD
+Filename: pycvc-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cvc/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from ._version import __version__
+from ._version import __version__
```

## cvc/_version.py

```diff
@@ -1,21 +1,21 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-__version__ = "1.2.3"
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+__version__ = "1.2.4"
```

## cvc/asn1.py

 * *Ordering differences only*

```diff
@@ -1,119 +1,119 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-from cvc.utils import to_bytes
-
-class ASN1:
-    DER = 1
-
-    _TAG_OID = 0x6
-    _TAG_CONTEXT = 0x80
-
-    def __init__(self):
-        self._buffer = b''
-        self._context_counter = 0
-
-    def calculate_len(size):
-        if (size <= 0x7f):
-            return bytearray([size])
-        b = to_bytes(size)
-        return bytearray([0x80+len(b)]) + b
-
-    def make_tag(tag, b):
-        return to_bytes(tag) + ASN1.calculate_len(len(b)) + bytearray(b)
-
-    def make_context(tag, n):
-        return ASN1.make_tag(tag, to_bytes(n))
-
-    def make_oid(oid):
-        return ASN1.make_tag(ASN1._TAG_OID, oid)
-
-    def _append_buffer(self, b):
-        self._buffer = self._buffer + b
-
-    def add_tag(self, tag, b):
-        self._append_buffer(ASN1.make_tag(tag, b))
-        return self
-
-    def add_context(self, b, idx=None):
-        if (idx is None):
-            self._context_counter = self._context_counter + 1
-            idx = self._context_counter
-        if (b != None):
-            return self.add_tag(ASN1._TAG_CONTEXT + idx, b)
-        return self
-
-    def add_oid(self, b):
-        return self.add_tag(ASN1._TAG_OID, b)
-
-    def add_object(self, tag, oid, ctxs):
-        ta = ASN1().add_oid(oid)
-        for idx, c in ctxs.items() if isinstance(ctxs, dict) else enumerate(ctxs):
-            ta.add_context(c, idx)
-        self.add_tag(tag, ta.encode())
-        return self
-
-    def encode(self, encoding_type = DER):
-        return self._buffer
-
-    def decode(self, data, encoding_type = DER):
-        self._buffer = bytearray(data)
-        return self
-
-    def all(self):
-        p = 0
-        while p < len(self._buffer):
-            tag = self._buffer[p]
-            p += 1
-            if ((tag & 0x1f) == 0x1f):
-                tag = (tag << 8) | self._buffer[p]
-                p += 1
-            if ((self._buffer[p] & 0x80) == 0x80):
-                n = self._buffer[p] & 0x7f
-                p += 1
-                l = 0
-                for i in range(n):
-                    l = l | (self._buffer[p+i] << 8*(n-i-1))
-                p += n
-            else:
-                l = self._buffer[p]
-                p += 1
-            d = self._buffer[p:p+l]
-            p += l
-            yield (tag, d)
-
-    def find(self, tag, pos=0):
-        pos_counter = 0
-        for t, d in self.all():
-            if (tag == t):
-                if (pos_counter == pos):
-                    self._buffer = d
-                    self._current_tag = tag
-                    return self
-                pos_counter += 1
-        return None
-
-    def data(self, return_tag=False):
-        if (return_tag is True):
-            return ASN1.make_tag(self._current_tag, self._buffer)
-        return self._buffer
-
-    def oid(self):
-        return self.find(0x6).data()
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+from cvc.utils import to_bytes
+
+class ASN1:
+    DER = 1
+
+    _TAG_OID = 0x6
+    _TAG_CONTEXT = 0x80
+
+    def __init__(self):
+        self._buffer = b''
+        self._context_counter = 0
+
+    def calculate_len(size):
+        if (size <= 0x7f):
+            return bytearray([size])
+        b = to_bytes(size)
+        return bytearray([0x80+len(b)]) + b
+
+    def make_tag(tag, b):
+        return to_bytes(tag) + ASN1.calculate_len(len(b)) + bytearray(b)
+
+    def make_context(tag, n):
+        return ASN1.make_tag(tag, to_bytes(n))
+
+    def make_oid(oid):
+        return ASN1.make_tag(ASN1._TAG_OID, oid)
+
+    def _append_buffer(self, b):
+        self._buffer = self._buffer + b
+
+    def add_tag(self, tag, b):
+        self._append_buffer(ASN1.make_tag(tag, b))
+        return self
+
+    def add_context(self, b, idx=None):
+        if (idx is None):
+            self._context_counter = self._context_counter + 1
+            idx = self._context_counter
+        if (b != None):
+            return self.add_tag(ASN1._TAG_CONTEXT + idx, b)
+        return self
+
+    def add_oid(self, b):
+        return self.add_tag(ASN1._TAG_OID, b)
+
+    def add_object(self, tag, oid, ctxs):
+        ta = ASN1().add_oid(oid)
+        for idx, c in ctxs.items() if isinstance(ctxs, dict) else enumerate(ctxs):
+            ta.add_context(c, idx)
+        self.add_tag(tag, ta.encode())
+        return self
+
+    def encode(self, encoding_type = DER):
+        return self._buffer
+
+    def decode(self, data, encoding_type = DER):
+        self._buffer = bytearray(data)
+        return self
+
+    def all(self):
+        p = 0
+        while p < len(self._buffer):
+            tag = self._buffer[p]
+            p += 1
+            if ((tag & 0x1f) == 0x1f):
+                tag = (tag << 8) | self._buffer[p]
+                p += 1
+            if ((self._buffer[p] & 0x80) == 0x80):
+                n = self._buffer[p] & 0x7f
+                p += 1
+                l = 0
+                for i in range(n):
+                    l = l | (self._buffer[p+i] << 8*(n-i-1))
+                p += n
+            else:
+                l = self._buffer[p]
+                p += 1
+            d = self._buffer[p:p+l]
+            p += l
+            yield (tag, d)
+
+    def find(self, tag, pos=0):
+        pos_counter = 0
+        for t, d in self.all():
+            if (tag == t):
+                if (pos_counter == pos):
+                    self._buffer = d
+                    self._current_tag = tag
+                    return self
+                pos_counter += 1
+        return None
+
+    def data(self, return_tag=False):
+        if (return_tag is True):
+            return ASN1.make_tag(self._current_tag, self._buffer)
+        return self._buffer
+
+    def oid(self):
+        return self.find(0x6).data()
```

## cvc/certificates.py

```diff
@@ -1,223 +1,223 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-from binascii import hexlify
-from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
-from cryptography.hazmat.primitives.asymmetric import ec, rsa, utils
-from cryptography.exceptions import InvalidSignature
-import datetime
-from cvc.utils import to_bytes, bcd, get_hash_padding, scheme_rsa
-from cvc.ec_curves import ec_domain, find_curve
-from cvc.asn1 import ASN1
-import os
-
-class CVC:
-    __data=None
-    def __init__(self):
-        self.__a = ASN1()
-
-    def decode(self, data):
-        self.__data = data
-        self.__a = ASN1().decode(self.__data)
-        return self
-
-    def body(self, pubkey=None, scheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
-        if (self.__data != None):
-            return self.cert().find(0x7f4e)
-        self.__a = ASN1().add_tag(0x7f4e, self.cpi().car(car).pubkey(pubkey, scheme, req).chr(chr).role(role).valid(valid, since).extensions(extensions).encode())
-        return self
-
-    def extensions(self, extensions=None):
-        if (self.__data != None):
-            return self.body().find(0x65)
-        if (extensions != None):
-            data = b''
-            for ext in extensions:
-                data += ASN1().add_object(tag=ext['tag'], oid=ext['oid'], ctxs=ext['contexts']).encode()
-            self.__a = self.__a.add_tag(0x65, data)
-        return self
-
-    def car(self, car=None):
-        if (self.__data != None):
-            return self.body().find(0x42).data()
-        self.__a = self.__a.add_tag(0x42, car)
-        return self
-
-    def outer_car(self):
-        if (self.req().find(0x42)):
-            return self.req().find(0x42).data()
-        return None
-
-    def chr(self, chr=None):
-        if (self.__data != None):
-            return self.body().find(0x5f20).data()
-        self.__a = self.__a.add_tag(0x5f20, chr)
-        return self
-
-    def cpi(self, val = 0):
-        if (self.__data != None):
-            return self.body().find(0x5f29).data()
-        self.__a = self.__a.add_tag(0x5f29, to_bytes(val))
-        return self
-
-    def pubkey(self, pubkey=None, scheme=None, full=None):
-        if (self.__data != None):
-            return self.body().find(0x7f49)
-        if (isinstance(pubkey, rsa.RSAPublicKey)):
-            pubctx = {1: to_bytes(pubkey.public_numbers().n), 2: to_bytes(pubkey.public_numbers().e)}
-        elif (isinstance(pubkey, ec.EllipticCurvePublicKey)):
-            dom = ec_domain(pubkey.public_numbers().curve)
-            Y = pubkey.public_bytes(Encoding.X962, PublicFormat.UncompressedPoint)
-            if (full):
-                pubctx = {1: dom.P, 2: dom.A, 3: dom.B, 4: dom.G, 5: dom.O, 6: Y, 7: dom.F}
-            else:
-                pubctx = {6: Y}
-        self.__a = self.__a.add_object(0x7f49, scheme, pubctx)
-        return self
-
-    def role(self, role=None):
-        if (self.__data != None):
-            return self.body().find(0x7f4c)
-        if (role != None):
-            self.__a = self.__a.add_tag(0x7f4c, ASN1().add_oid(role.OID).add_tag(0x53, role.to_bytes()).encode())
-        return self
-
-    def valid(self, valid=None, since=None):
-        if (self.__data != None):
-            return self.body().find(0x5f25).data()
-        if (valid != None):
-            if (since == None):
-                since = datetime.datetime.now().strftime("%y%m%d")
-            until = (datetime.datetime.strptime(since, "%y%m%d") + datetime.timedelta(days = int(valid))).strftime("%y%m%d")
-            self.__a = self.__a.add_tag(0x5f25, bcd(since)).add_tag(0x5f24, bcd(until))
-        return self
-
-    def expires(self):
-        return self.body().find(0x5f24).data()
-
-    def signature(self):
-        if (self.__data != None):
-            return self.cert().find(0x5f37).data()
-
-    def outer_signature(self):
-        if (self.req().find(0x5f37)):
-            return self.req().find(0x5f37).data()
-
-    def sign(self, key, scheme):
-        h,p = get_hash_padding(scheme)
-        if (isinstance(key, ec.EllipticCurvePrivateKey)):
-            signature = key.sign(self.__a.encode(), ec.ECDSA(h))
-            r,s = utils.decode_dss_signature(signature)
-            signature = to_bytes(r) + to_bytes(s)
-        elif (isinstance(key, rsa.RSAPrivateKey)):
-            signature = key.sign(self.__a.encode(), p, h)
-        self.__a = self.__a.add_tag(0x5f37, bytearray(signature))
-        return self
-
-    def cert(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
-        if (self.__data != None):
-            return self.req().find(0x7f21)
-        self.__a = ASN1().add_tag(0x7f21, self.body(pubkey, scheme, car, chr, role, valid, since, extensions, req or chr==car).sign(signkey, signscheme).encode())
-        return self
-
-    def req(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, outercar=None, outerkey=None, outerscheme=None, extensions=None):
-        if (self.__data != None):
-            aut = ASN1().decode(self.__data).find(0x67)
-            if (aut):
-                return aut
-            return ASN1().decode(self.__data)
-        cert = self.cert(pubkey, scheme, signkey, signscheme, car, chr, role=None, valid=None, since=None, extensions=extensions, req=True)
-        if (outercar != None and outerkey != None and outerscheme != None):
-            self.__a = ASN1().add_tag(0x67, cert.car(outercar).sign(outerkey, outerscheme).encode())
-        return self
-
-    def is_req(self):
-        if (self.__data != None):
-            b = self.__a
-            ret = self.__a.find(0x67) != None or self.body().find(0x5f25) == None
-            self.__a = b
-            return ret
-        return False
-
-    def encode(self):
-        return self.__a.encode()
-
-    def verify(self, outer=False, cert_dir=None, curve=None, dica=None):
-        chr = self.chr()
-        if (outer is True):
-            car = self.outer_car()
-            signature = self.outer_signature()
-            body = self.cert().data()
-            body = ASN1().add_tag(0x7f21, body).add_tag(0x42, car).encode()
-        else:
-            car = self.car()
-            signature = self.signature()
-            body = self.body().data(return_tag=True)
-        if ((car != chr or outer is True) and dica is None):
-            try:
-                with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
-                    dica = f.read()
-            except FileNotFoundError:
-                print(f'[Warning: File {car.decode()} not found]')
-                return False
-        if (dica is None):
-            puk = self.pubkey().data()
-        else:
-            puk = CVC().decode(dica).pubkey().data()
-        scheme = ASN1().decode(puk).oid()
-        h,p = get_hash_padding(scheme)
-        try:
-            if (scheme_rsa(scheme)):
-                pubkey = rsa.RSAPublicNumbers(ASN1().decode(puk).find(0x82).data(), ASN1().decode(puk).find(0x81).data()).public_key()
-                pubkey.verify(signature, body, p, h)
-            else:
-                if (not curve):
-                    curve = self.find_domain(cert_dir, outer)
-                Q = ASN1().decode(puk).find(0x86).data()
-                if (curve and Q):
-                    pubkey = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
-                    pubkey.verify(utils.encode_dss_signature(int.from_bytes(signature[:len(signature)//2],'big'), int.from_bytes(signature[len(signature)//2:],'big')), body, ec.ECDSA(h))
-                else:
-                    return False
-        except InvalidSignature:
-            return False
-        return True
-
-    def find_domain(self, cert_dir='', outer=False):
-        adata = self.encode()
-        try:
-            P = CVC().decode(adata).pubkey().find(0x81) if outer is False else None
-            if (P):
-                return find_curve(P.data())
-            depth = 10
-            while (P == None and depth > 0):
-                car = CVC().decode(adata).outer_car()
-                if (not car or outer is False):
-                    car = CVC().decode(adata).car()
-                chr = CVC().decode(adata).chr()
-                with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
-                    adata = f.read()
-                    P = CVC().decode(adata).pubkey().find(0x81)
-                if (P):
-                    return find_curve(P.data())
-                depth -= 1
-        except FileNotFoundError:
-            print(f'[Warning: File {car.decode()} not found]')
-        return None
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+from binascii import hexlify
+from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
+from cryptography.hazmat.primitives.asymmetric import ec, rsa, utils
+from cryptography.exceptions import InvalidSignature
+import datetime
+from cvc.utils import to_bytes, bcd, get_hash_padding, scheme_rsa
+from cvc.ec_curves import ec_domain, find_curve
+from cvc.asn1 import ASN1
+import os
+
+class CVC:
+    __data=None
+    def __init__(self):
+        self.__a = ASN1()
+
+    def decode(self, data):
+        self.__data = data
+        self.__a = ASN1().decode(self.__data)
+        return self
+
+    def body(self, pubkey=None, scheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
+        if (self.__data != None):
+            return self.cert().find(0x7f4e)
+        self.__a = ASN1().add_tag(0x7f4e, self.cpi().car(car).pubkey(pubkey, scheme, req).chr(chr).role(role).valid(valid, since).extensions(extensions).encode())
+        return self
+
+    def extensions(self, extensions=None):
+        if (self.__data != None):
+            return self.body().find(0x65)
+        if (extensions != None):
+            data = b''
+            for ext in extensions:
+                data += ASN1().add_object(tag=ext['tag'], oid=ext['oid'], ctxs=ext['contexts']).encode()
+            self.__a = self.__a.add_tag(0x65, data)
+        return self
+
+    def car(self, car=None):
+        if (self.__data != None):
+            return self.body().find(0x42).data()
+        self.__a = self.__a.add_tag(0x42, car)
+        return self
+
+    def outer_car(self):
+        if (self.req().find(0x42)):
+            return self.req().find(0x42).data()
+        return None
+
+    def chr(self, chr=None):
+        if (self.__data != None):
+            return self.body().find(0x5f20).data()
+        self.__a = self.__a.add_tag(0x5f20, chr)
+        return self
+
+    def cpi(self, val = 0):
+        if (self.__data != None):
+            return self.body().find(0x5f29).data()
+        self.__a = self.__a.add_tag(0x5f29, to_bytes(val))
+        return self
+
+    def pubkey(self, pubkey=None, scheme=None, full=None):
+        if (self.__data != None):
+            return self.body().find(0x7f49)
+        if (isinstance(pubkey, rsa.RSAPublicKey)):
+            pubctx = {1: to_bytes(pubkey.public_numbers().n), 2: to_bytes(pubkey.public_numbers().e)}
+        elif (isinstance(pubkey, ec.EllipticCurvePublicKey)):
+            dom = ec_domain(pubkey.public_numbers().curve)
+            Y = pubkey.public_bytes(Encoding.X962, PublicFormat.UncompressedPoint)
+            if (full):
+                pubctx = {1: dom.P, 2: dom.A, 3: dom.B, 4: dom.G, 5: dom.O, 6: Y, 7: dom.F}
+            else:
+                pubctx = {6: Y}
+        self.__a = self.__a.add_object(0x7f49, scheme, pubctx)
+        return self
+
+    def role(self, role=None):
+        if (self.__data != None):
+            return self.body().find(0x7f4c)
+        if (role != None):
+            self.__a = self.__a.add_tag(0x7f4c, ASN1().add_oid(role.OID).add_tag(0x53, role.to_bytes()).encode())
+        return self
+
+    def valid(self, valid=None, since=None):
+        if (self.__data != None):
+            return self.body().find(0x5f25).data()
+        if (valid != None):
+            if (since == None):
+                since = datetime.datetime.now().strftime("%y%m%d")
+            until = (datetime.datetime.strptime(since, "%y%m%d") + datetime.timedelta(days = int(valid))).strftime("%y%m%d")
+            self.__a = self.__a.add_tag(0x5f25, bcd(since)).add_tag(0x5f24, bcd(until))
+        return self
+
+    def expires(self):
+        return self.body().find(0x5f24).data()
+
+    def signature(self):
+        if (self.__data != None):
+            return self.cert().find(0x5f37).data()
+
+    def outer_signature(self):
+        if (self.req().find(0x5f37)):
+            return self.req().find(0x5f37).data()
+
+    def sign(self, key, scheme):
+        h,p = get_hash_padding(scheme)
+        if (isinstance(key, ec.EllipticCurvePrivateKey)):
+            signature = key.sign(self.__a.encode(), ec.ECDSA(h))
+            r,s = utils.decode_dss_signature(signature)
+            signature = to_bytes(r) + to_bytes(s)
+        elif (isinstance(key, rsa.RSAPrivateKey)):
+            signature = key.sign(self.__a.encode(), p, h)
+        self.__a = self.__a.add_tag(0x5f37, bytearray(signature))
+        return self
+
+    def cert(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
+        if (self.__data != None):
+            return self.req().find(0x7f21)
+        self.__a = ASN1().add_tag(0x7f21, self.body(pubkey, scheme, car, chr, role, valid, since, extensions, req or chr==car).sign(signkey, signscheme).encode())
+        return self
+
+    def req(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, outercar=None, outerkey=None, outerscheme=None, extensions=None):
+        if (self.__data != None):
+            aut = ASN1().decode(self.__data).find(0x67)
+            if (aut):
+                return aut
+            return ASN1().decode(self.__data)
+        cert = self.cert(pubkey, scheme, signkey, signscheme, car, chr, role=None, valid=None, since=None, extensions=extensions, req=True)
+        if (outercar != None and outerkey != None and outerscheme != None):
+            self.__a = ASN1().add_tag(0x67, cert.car(outercar).sign(outerkey, outerscheme).encode())
+        return self
+
+    def is_req(self):
+        if (self.__data != None):
+            b = self.__a
+            ret = self.__a.find(0x67) != None or self.body().find(0x5f25) == None
+            self.__a = b
+            return ret
+        return False
+
+    def encode(self):
+        return self.__a.encode()
+
+    def verify(self, outer=False, cert_dir=None, curve=None, dica=None):
+        chr = self.chr()
+        if (outer is True):
+            car = self.outer_car()
+            signature = self.outer_signature()
+            body = self.cert().data()
+            body = ASN1().add_tag(0x7f21, body).add_tag(0x42, car).encode()
+        else:
+            car = self.car()
+            signature = self.signature()
+            body = self.body().data(return_tag=True)
+        if ((car != chr or outer is True) and dica is None):
+            try:
+                with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
+                    dica = f.read()
+            except FileNotFoundError:
+                print(f'[Warning: File {car.decode()} not found]')
+                return False
+        if (dica is None):
+            puk = self.pubkey().data()
+        else:
+            puk = CVC().decode(dica).pubkey().data()
+        scheme = ASN1().decode(puk).oid()
+        h,p = get_hash_padding(scheme)
+        try:
+            if (scheme_rsa(scheme)):
+                pubkey = rsa.RSAPublicNumbers(int.from_bytes(ASN1().decode(puk).find(0x82).data(), 'big'), int.from_bytes(ASN1().decode(puk).find(0x81).data(), 'big')).public_key()
+                pubkey.verify(bytes(signature), bytes(body), p, h)
+            else:
+                if (not curve):
+                    curve = self.find_domain(cert_dir, outer)
+                Q = ASN1().decode(puk).find(0x86).data()
+                if (curve and Q):
+                    pubkey = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
+                    pubkey.verify(utils.encode_dss_signature(int.from_bytes(signature[:len(signature)//2],'big'), int.from_bytes(signature[len(signature)//2:],'big')), body, ec.ECDSA(h))
+                else:
+                    return False
+        except InvalidSignature:
+            return False
+        return True
+
+    def find_domain(self, cert_dir='', outer=False):
+        adata = self.encode()
+        try:
+            P = CVC().decode(adata).pubkey().find(0x81) if outer is False else None
+            if (P):
+                return find_curve(P.data())
+            depth = 10
+            while (P == None and depth > 0):
+                car = CVC().decode(adata).outer_car()
+                if (not car or outer is False):
+                    car = CVC().decode(adata).car()
+                chr = CVC().decode(adata).chr()
+                with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
+                    adata = f.read()
+                    P = CVC().decode(adata).pubkey().find(0x81)
+                if (P):
+                    return find_curve(P.data())
+                depth -= 1
+        except FileNotFoundError:
+            print(f'[Warning: File {car.decode()} not found]')
+        return None
```

## cvc/ec_curves.py

 * *Ordering differences only*

```diff
@@ -1,165 +1,165 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-from cryptography.hazmat.primitives.asymmetric import ec
-
-class SECP192R1:
-    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
-    A = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
-    B = bytearray(b"\x64\x21\x05\x19\xE5\x9C\x80\xE7\x0F\xA7\xE9\xAB\x72\x24\x30\x49\xFE\xB8\xDE\xEC\xC1\x46\xB9\xB1")
-    G = bytearray(b"\x04\x18\x8D\xA8\x0E\xB0\x30\x90\xF6\x7C\xBF\x20\xEB\x43\xA1\x88\x00\xF4\xFF\x0A\xFD\x82\xFF\x10\x12\x07\x19\x2B\x95\xFF\xC8\xDA\x78\x63\x10\x11\xED\x6B\x24\xCD\xD5\x73\xF9\x77\xA1\x1E\x79\x48\x11")
-    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\x99\xDE\xF8\x36\x14\x6B\xC9\xB1\xB4\xD2\x28\x31")
-    F = bytearray(b"\x01")
-
-class SECP256R1:
-    P = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
-    A = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
-    B = bytearray(b"\x5A\xC6\x35\xD8\xAA\x3A\x93\xE7\xB3\xEB\xBD\x55\x76\x98\x86\xBC\x65\x1D\x06\xB0\xCC\x53\xB0\xF6\x3B\xCE\x3C\x3E\x27\xD2\x60\x4B")
-    G = bytearray(b"\x04\x6B\x17\xD1\xF2\xE1\x2C\x42\x47\xF8\xBC\xE6\xE5\x63\xA4\x40\xF2\x77\x03\x7D\x81\x2D\xEB\x33\xA0\xF4\xA1\x39\x45\xD8\x98\xC2\x96\x4F\xE3\x42\xE2\xFE\x1A\x7F\x9B\x8E\xE7\xEB\x4A\x7C\x0F\x9E\x16\x2B\xCE\x33\x57\x6B\x31\x5E\xCE\xCB\xB6\x40\x68\x37\xBF\x51\xF5")
-    O = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xBC\xE6\xFA\xAD\xA7\x17\x9E\x84\xF3\xB9\xCA\xC2\xFC\x63\x25\x51")
-    F = bytearray(b"\x01")
-
-class SECP384R1:
-    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF")
-    A = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFC")
-    B = bytearray(b"\xB3\x31\x2F\xA7\xE2\x3E\xE7\xE4\x98\x8E\x05\x6B\xE3\xF8\x2D\x19\x18\x1D\x9C\x6E\xFE\x81\x41\x12\x03\x14\x08\x8F\x50\x13\x87\x5A\xC6\x56\x39\x8D\x8A\x2E\xD1\x9D\x2A\x85\xC8\xED\xD3\xEC\x2A\xEF")
-    G = bytearray(b"\x04\xAA\x87\xCA\x22\xBE\x8B\x05\x37\x8E\xB1\xC7\x1E\xF3\x20\xAD\x74\x6E\x1D\x3B\x62\x8B\xA7\x9B\x98\x59\xF7\x41\xE0\x82\x54\x2A\x38\x55\x02\xF2\x5D\xBF\x55\x29\x6C\x3A\x54\x5E\x38\x72\x76\x0A\xB7\x36\x17\xDE\x4A\x96\x26\x2C\x6F\x5D\x9E\x98\xBF\x92\x92\xDC\x29\xF8\xF4\x1D\xBD\x28\x9A\x14\x7C\xE9\xDA\x31\x13\xB5\xF0\xB8\xC0\x0A\x60\xB1\xCE\x1D\x7E\x81\x9D\x7A\x43\x1D\x7C\x90\xEA\x0E\x5F")
-    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xC7\x63\x4D\x81\xF4\x37\x2D\xDF\x58\x1A\x0D\xB2\x48\xB0\xA7\x7A\xEC\xEC\x19\x6A\xCC\xC5\x29\x73")
-    F = bytearray(b"\x01")
-
-class SECP521R1:
-    P = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
-    A = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
-    B = bytearray(b"\x00\x51\x95\x3E\xB9\x61\x8E\x1C\x9A\x1F\x92\x9A\x21\xA0\xB6\x85\x40\xEE\xA2\xDA\x72\x5B\x99\xB3\x15\xF3\xB8\xB4\x89\x91\x8E\xF1\x09\xE1\x56\x19\x39\x51\xEC\x7E\x93\x7B\x16\x52\xC0\xBD\x3B\xB1\xBF\x07\x35\x73\xDF\x88\x3D\x2C\x34\xF1\xEF\x45\x1F\xD4\x6B\x50\x3F\x00")
-    G = bytearray(b"\x04\x00\xC6\x85\x8E\x06\xB7\x04\x04\xE9\xCD\x9E\x3E\xCB\x66\x23\x95\xB4\x42\x9C\x64\x81\x39\x05\x3F\xB5\x21\xF8\x28\xAF\x60\x6B\x4D\x3D\xBA\xA1\x4B\x5E\x77\xEF\xE7\x59\x28\xFE\x1D\xC1\x27\xA2\xFF\xA8\xDE\x33\x48\xB3\xC1\x85\x6A\x42\x9B\xF9\x7E\x7E\x31\xC2\xE5\xBD\x66\x01\x18\x39\x29\x6A\x78\x9A\x3B\xC0\x04\x5C\x8A\x5F\xB4\x2C\x7D\x1B\xD9\x98\xF5\x44\x49\x57\x9B\x44\x68\x17\xAF\xBD\x17\x27\x3E\x66\x2C\x97\xEE\x72\x99\x5E\xF4\x26\x40\xC5\x50\xB9\x01\x3F\xAD\x07\x61\x35\x3C\x70\x86\xA2\x72\xC2\x40\x88\xBE\x94\x76\x9F\xD1\x66\x50")
-    O = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFA\x51\x86\x87\x83\xBF\x2F\x96\x6B\x7F\xCC\x01\x48\xF7\x09\xA5\xD0\x3B\xB5\xC9\xB8\x89\x9C\x47\xAE\xBB\x6F\xB7\x1E\x91\x38\x64\x09")
-    F = bytearray(b"\x01")
-
-
-class BP192R1:
-    P = bytearray(b"\xC3\x02\xF4\x1D\x93\x2A\x36\xCD\xA7\xA3\x46\x30\x93\xD1\x8D\xB7\x8F\xCE\x47\x6D\xE1\xA8\x62\x97")
-    A = bytearray(b"\x6A\x91\x17\x40\x76\xB1\xE0\xE1\x9C\x39\xC0\x31\xFE\x86\x85\xC1\xCA\xE0\x40\xE5\xC6\x9A\x28\xEF")
-    B = bytearray(b"\x46\x9A\x28\xEF\x7C\x28\xCC\xA3\xDC\x72\x1D\x04\x4F\x44\x96\xBC\xCA\x7E\xF4\x14\x6F\xBF\x25\xC9")
-    G = bytearray(b"\x04\xC0\xA0\x64\x7E\xAA\xB6\xA4\x87\x53\xB0\x33\xC5\x6C\xB0\xF0\x90\x0A\x2F\x5C\x48\x53\x37\x5F\xD6\x14\xB6\x90\x86\x6A\xBD\x5B\xB8\x8B\x5F\x48\x28\xC1\x49\x00\x02\xE6\x77\x3F\xA2\xFA\x29\x9B\x8F")
-    O = bytearray(b"\xC3\x02\xF4\x1D\x93\x2A\x36\xCD\xA7\xA3\x46\x2F\x9E\x9E\x91\x6B\x5B\xE8\xF1\x02\x9A\xC4\xAC\xC1")
-    F = bytearray(b"\x01")
-
-class BP224R1:
-    P = bytearray(b"\xD7\xC1\x34\xAA\x26\x43\x66\x86\x2A\x18\x30\x25\x75\xD1\xD7\x87\xB0\x9F\x07\x57\x97\xDA\x89\xF5\x7E\xC8\xC0\xFF")
-    A = bytearray(b"\x68\xA5\xE6\x2C\xA9\xCE\x6C\x1C\x29\x98\x03\xA6\xC1\x53\x0B\x51\x4E\x18\x2A\xD8\xB0\x04\x2A\x59\xCA\xD2\x9F\x43")
-    B = bytearray(b"\x25\x80\xF6\x3C\xCF\xE4\x41\x38\x87\x07\x13\xB1\xA9\x23\x69\xE3\x3E\x21\x35\xD2\x66\xDB\xB3\x72\x38\x6C\x40\x0B")
-    G = bytearray(b"\x04\x0D\x90\x29\xAD\x2C\x7E\x5C\xF4\x34\x08\x23\xB2\xA8\x7D\xC6\x8C\x9E\x4C\xE3\x17\x4C\x1E\x6E\xFD\xEE\x12\xC0\x7D\x58\xAA\x56\xF7\x72\xC0\x72\x6F\x24\xC6\xB8\x9E\x4E\xCD\xAC\x24\x35\x4B\x9E\x99\xCA\xA3\xF6\xD3\x76\x14\x02\xCD")
-    O = bytearray(b"\xD7\xC1\x34\xAA\x26\x43\x66\x86\x2A\x18\x30\x25\x75\xD0\xFB\x98\xD1\x16\xBC\x4B\x6D\xDE\xBC\xA3\xA5\xA7\x93\x9F")
-    F = bytearray(b"\x01")
-
-class BP256R1:
-    P = bytearray(b"\xA9\xFB\x57\xDB\xA1\xEE\xA9\xBC\x3E\x66\x0A\x90\x9D\x83\x8D\x72\x6E\x3B\xF6\x23\xD5\x26\x20\x28\x20\x13\x48\x1D\x1F\x6E\x53\x77")
-    A = bytearray(b"\x7D\x5A\x09\x75\xFC\x2C\x30\x57\xEE\xF6\x75\x30\x41\x7A\xFF\xE7\xFB\x80\x55\xC1\x26\xDC\x5C\x6C\xE9\x4A\x4B\x44\xF3\x30\xB5\xD9")
-    B = bytearray(b"\x26\xDC\x5C\x6C\xE9\x4A\x4B\x44\xF3\x30\xB5\xD9\xBB\xD7\x7C\xBF\x95\x84\x16\x29\x5C\xF7\xE1\xCE\x6B\xCC\xDC\x18\xFF\x8C\x07\xB6")
-    G = bytearray(b"\x04\x8B\xD2\xAE\xB9\xCB\x7E\x57\xCB\x2C\x4B\x48\x2F\xFC\x81\xB7\xAF\xB9\xDE\x27\xE1\xE3\xBD\x23\xC2\x3A\x44\x53\xBD\x9A\xCE\x32\x62\x54\x7E\xF8\x35\xC3\xDA\xC4\xFD\x97\xF8\x46\x1A\x14\x61\x1D\xC9\xC2\x77\x45\x13\x2D\xED\x8E\x54\x5C\x1D\x54\xC7\x2F\x04\x69\x97")
-    O = bytearray(b"\xA9\xFB\x57\xDB\xA1\xEE\xA9\xBC\x3E\x66\x0A\x90\x9D\x83\x8D\x71\x8C\x39\x7A\xA3\xB5\x61\xA6\xF7\x90\x1E\x0E\x82\x97\x48\x56\xA7")
-    F = bytearray(b"\x01")
-
-class BP320R1:
-    P = bytearray(b"\xD3\x5E\x47\x20\x36\xBC\x4F\xB7\xE1\x3C\x78\x5E\xD2\x01\xE0\x65\xF9\x8F\xCF\xA6\xF6\xF4\x0D\xEF\x4F\x92\xB9\xEC\x78\x93\xEC\x28\xFC\xD4\x12\xB1\xF1\xB3\x2E\x27")
-    A = bytearray(b"\x3E\xE3\x0B\x56\x8F\xBA\xB0\xF8\x83\xCC\xEB\xD4\x6D\x3F\x3B\xB8\xA2\xA7\x35\x13\xF5\xEB\x79\xDA\x66\x19\x0E\xB0\x85\xFF\xA9\xF4\x92\xF3\x75\xA9\x7D\x86\x0E\xB4")
-    B = bytearray(b"\x52\x08\x83\x94\x9D\xFD\xBC\x42\xD3\xAD\x19\x86\x40\x68\x8A\x6F\xE1\x3F\x41\x34\x95\x54\xB4\x9A\xCC\x31\xDC\xCD\x88\x45\x39\x81\x6F\x5E\xB4\xAC\x8F\xB1\xF1\xA6")
-    G = bytearray(b"\x04\x43\xBD\x7E\x9A\xFB\x53\xD8\xB8\x52\x89\xBC\xC4\x8E\xE5\xBF\xE6\xF2\x01\x37\xD1\x0A\x08\x7E\xB6\xE7\x87\x1E\x2A\x10\xA5\x99\xC7\x10\xAF\x8D\x0D\x39\xE2\x06\x11\x14\xFD\xD0\x55\x45\xEC\x1C\xC8\xAB\x40\x93\x24\x7F\x77\x27\x5E\x07\x43\xFF\xED\x11\x71\x82\xEA\xA9\xC7\x78\x77\xAA\xAC\x6A\xC7\xD3\x52\x45\xD1\x69\x2E\x8E\xE1")
-    O = bytearray(b"\xD3\x5E\x47\x20\x36\xBC\x4F\xB7\xE1\x3C\x78\x5E\xD2\x01\xE0\x65\xF9\x8F\xCF\xA5\xB6\x8F\x12\xA3\x2D\x48\x2E\xC7\xEE\x86\x58\xE9\x86\x91\x55\x5B\x44\xC5\x93\x11")
-    F = bytearray(b"\0x1")
-
-class BP384R1:
-    P = bytearray(b"\x8C\xB9\x1E\x82\xA3\x38\x6D\x28\x0F\x5D\x6F\x7E\x50\xE6\x41\xDF\x15\x2F\x71\x09\xED\x54\x56\xB4\x12\xB1\xDA\x19\x7F\xB7\x11\x23\xAC\xD3\xA7\x29\x90\x1D\x1A\x71\x87\x47\x00\x13\x31\x07\xEC\x53")
-    A = bytearray(b"\x7B\xC3\x82\xC6\x3D\x8C\x15\x0C\x3C\x72\x08\x0A\xCE\x05\xAF\xA0\xC2\xBE\xA2\x8E\x4F\xB2\x27\x87\x13\x91\x65\xEF\xBA\x91\xF9\x0F\x8A\xA5\x81\x4A\x50\x3A\xD4\xEB\x04\xA8\xC7\xDD\x22\xCE\x28\x26")
-    B = bytearray(b"\x04\xA8\xC7\xDD\x22\xCE\x28\x26\x8B\x39\xB5\x54\x16\xF0\x44\x7C\x2F\xB7\x7D\xE1\x07\xDC\xD2\xA6\x2E\x88\x0E\xA5\x3E\xEB\x62\xD5\x7C\xB4\x39\x02\x95\xDB\xC9\x94\x3A\xB7\x86\x96\xFA\x50\x4C\x11")
-    G = bytearray(b"\x04\x1D\x1C\x64\xF0\x68\xCF\x45\xFF\xA2\xA6\x3A\x81\xB7\xC1\x3F\x6B\x88\x47\xA3\xE7\x7E\xF1\x4F\xE3\xDB\x7F\xCA\xFE\x0C\xBD\x10\xE8\xE8\x26\xE0\x34\x36\xD6\x46\xAA\xEF\x87\xB2\xE2\x47\xD4\xAF\x1E\x8A\xBE\x1D\x75\x20\xF9\xC2\xA4\x5C\xB1\xEB\x8E\x95\xCF\xD5\x52\x62\xB7\x0B\x29\xFE\xEC\x58\x64\xE1\x9C\x05\x4F\xF9\x91\x29\x28\x0E\x46\x46\x21\x77\x91\x81\x11\x42\x82\x03\x41\x26\x3C\x53\x15")
-    O = bytearray(b"\x8C\xB9\x1E\x82\xA3\x38\x6D\x28\x0F\x5D\x6F\x7E\x50\xE6\x41\xDF\x15\x2F\x71\x09\xED\x54\x56\xB3\x1F\x16\x6E\x6C\xAC\x04\x25\xA7\xCF\x3A\xB6\xAF\x6B\x7F\xC3\x10\x3B\x88\x32\x02\xE9\x04\x65\x65")
-    F = bytearray(b"\x01")
-
-class BP512R1:
-    P = bytearray(b"\xAA\xDD\x9D\xB8\xDB\xE9\xC4\x8B\x3F\xD4\xE6\xAE\x33\xC9\xFC\x07\xCB\x30\x8D\xB3\xB3\xC9\xD2\x0E\xD6\x63\x9C\xCA\x70\x33\x08\x71\x7D\x4D\x9B\x00\x9B\xC6\x68\x42\xAE\xCD\xA1\x2A\xE6\xA3\x80\xE6\x28\x81\xFF\x2F\x2D\x82\xC6\x85\x28\xAA\x60\x56\x58\x3A\x48\xF3")
-    A = bytearray(b"\x78\x30\xA3\x31\x8B\x60\x3B\x89\xE2\x32\x71\x45\xAC\x23\x4C\xC5\x94\xCB\xDD\x8D\x3D\xF9\x16\x10\xA8\x34\x41\xCA\xEA\x98\x63\xBC\x2D\xED\x5D\x5A\xA8\x25\x3A\xA1\x0A\x2E\xF1\xC9\x8B\x9A\xC8\xB5\x7F\x11\x17\xA7\x2B\xF2\xC7\xB9\xE7\xC1\xAC\x4D\x77\xFC\x94\xCA")
-    B = bytearray(b"\x3D\xF9\x16\x10\xA8\x34\x41\xCA\xEA\x98\x63\xBC\x2D\xED\x5D\x5A\xA8\x25\x3A\xA1\x0A\x2E\xF1\xC9\x8B\x9A\xC8\xB5\x7F\x11\x17\xA7\x2B\xF2\xC7\xB9\xE7\xC1\xAC\x4D\x77\xFC\x94\xCA\xDC\x08\x3E\x67\x98\x40\x50\xB7\x5E\xBA\xE5\xDD\x28\x09\xBD\x63\x80\x16\xF7\x23")
-    G = bytearray(b"\x04\x81\xAE\xE4\xBD\xD8\x2E\xD9\x64\x5A\x21\x32\x2E\x9C\x4C\x6A\x93\x85\xED\x9F\x70\xB5\xD9\x16\xC1\xB4\x3B\x62\xEE\xF4\xD0\x09\x8E\xFF\x3B\x1F\x78\xE2\xD0\xD4\x8D\x50\xD1\x68\x7B\x93\xB9\x7D\x5F\x7C\x6D\x50\x47\x40\x6A\x5E\x68\x8B\x35\x22\x09\xBC\xB9\xF8\x22\x7D\xDE\x38\x5D\x56\x63\x32\xEC\xC0\xEA\xBF\xA9\xCF\x78\x22\xFD\xF2\x09\xF7\x00\x24\xA5\x7B\x1A\xA0\x00\xC5\x5B\x88\x1F\x81\x11\xB2\xDC\xDE\x49\x4A\x5F\x48\x5E\x5B\xCA\x4B\xD8\x8A\x27\x63\xAE\xD1\xCA\x2B\x2F\xA8\xF0\x54\x06\x78\xCD\x1E\x0F\x3A\xD8\x08\x92")
-    O = bytearray(b"\xAA\xDD\x9D\xB8\xDB\xE9\xC4\x8B\x3F\xD4\xE6\xAE\x33\xC9\xFC\x07\xCB\x30\x8D\xB3\xB3\xC9\xD2\x0E\xD6\x63\x9C\xCA\x70\x33\x08\x70\x55\x3E\x5C\x41\x4C\xA9\x26\x19\x41\x86\x61\x19\x7F\xAC\x10\x47\x1D\xB1\xD3\x81\x08\x5D\xDA\xDD\xB5\x87\x96\x82\x9C\xA9\x00\x69")
-    F = bytearray(b"\x01")
-
-class SECP192K1:
-    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xEE\x37")
-    A = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
-    B = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x03")
-    G = bytearray(b"\x04\xDB\x4F\xF1\x0E\xC0\x57\xE9\xAE\x26\xB0\x7D\x02\x80\xB7\xF4\x34\x1D\xA5\xD1\xB1\xEA\xE0\x6C\x7D\x9B\x2F\x2F\x6D\x9C\x56\x28\xA7\x84\x41\x63\xD0\x15\xBE\x86\x34\x40\x82\xAA\x88\xD9\x5E\x2F\x9D")
-    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\x26\xF2\xFC\x17\x0F\x69\x46\x6A\x74\xDE\xFD\x8D")
-    F = bytearray(b"\x01")
-
-class SECP256K1:
-    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFC\x2F")
-    A = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
-    B = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x07")
-    G = bytearray(b"\x04\x79\xBE\x66\x7E\xF9\xDC\xBB\xAC\x55\xA0\x62\x95\xCE\x87\x0B\x07\x02\x9B\xFC\xDB\x2D\xCE\x28\xD9\x59\xF2\x81\x5B\x16\xF8\x17\x98\x48\x3A\xDA\x77\x26\xA3\xC4\x65\x5D\xA4\xFB\xFC\x0E\x11\x08\xA8\xFD\x17\xB4\x48\xA6\x85\x54\x19\x9C\x47\xD0\x8F\xFB\x10\xD4\xB8")
-    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xBA\xAE\xDC\xE6\xAF\x48\xA0\x3B\xBF\xD2\x5E\x8C\xD0\x36\x41\x41")
-    F = bytearray(b"\x01")
-
-
-def ec_domain(curve):
-    if (curve.name == 'secp192r1'):
-        return SECP192R1()
-    elif (curve.name == 'secp256r1'):
-        return SECP256R1()
-    elif (curve.name == 'secp384r1'):
-        return SECP384R1()
-    elif (curve.name == 'secp521r1'):
-        return SECP521R1()
-    elif (curve.name == 'brainpoolP192r1'):
-        return BP192R1()
-    elif (curve.name == 'brainpoolP224r1'):
-        return BP224R1()
-    elif (curve.name == 'brainpoolP256r1'):
-        return BP256R1()
-    elif (curve.name == 'brainpoolP320r1'):
-        return BP320R1()
-    elif (curve.name == 'brainpoolP384r1'):
-        return BP384R1()
-    elif (curve.name == 'brainpoolP512r1'):
-        return BP512R1()
-    elif (curve.name == 'secp192k1'):
-        return SECP192K1()
-    elif (curve.name == 'secp256k1'):
-        return SECP256K1()
-    return None
-
-def find_curve(P):
-    if (SECP192R1.P == P):
-        return ec.SECP192R1()
-    elif (SECP256K1.P == P):
-        return ec.SECP256K1()
-    elif (SECP256R1.P == P):
-        return ec.SECP256R1()
-    elif (SECP384R1.P == P):
-        return ec.SECP384R1()
-    elif (SECP521R1.P == P):
-        return ec.SECP521R1()
-    elif (BP256R1.P == P):
-        return ec.BrainpoolP256R1()
-    elif (BP384R1.P == P):
-        return ec.BrainpoolP384R1()
-    elif (BP512R1.P == P):
-        return ec.BrainpoolP512R1()
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+from cryptography.hazmat.primitives.asymmetric import ec
+
+class SECP192R1:
+    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
+    A = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
+    B = bytearray(b"\x64\x21\x05\x19\xE5\x9C\x80\xE7\x0F\xA7\xE9\xAB\x72\x24\x30\x49\xFE\xB8\xDE\xEC\xC1\x46\xB9\xB1")
+    G = bytearray(b"\x04\x18\x8D\xA8\x0E\xB0\x30\x90\xF6\x7C\xBF\x20\xEB\x43\xA1\x88\x00\xF4\xFF\x0A\xFD\x82\xFF\x10\x12\x07\x19\x2B\x95\xFF\xC8\xDA\x78\x63\x10\x11\xED\x6B\x24\xCD\xD5\x73\xF9\x77\xA1\x1E\x79\x48\x11")
+    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\x99\xDE\xF8\x36\x14\x6B\xC9\xB1\xB4\xD2\x28\x31")
+    F = bytearray(b"\x01")
+
+class SECP256R1:
+    P = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
+    A = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
+    B = bytearray(b"\x5A\xC6\x35\xD8\xAA\x3A\x93\xE7\xB3\xEB\xBD\x55\x76\x98\x86\xBC\x65\x1D\x06\xB0\xCC\x53\xB0\xF6\x3B\xCE\x3C\x3E\x27\xD2\x60\x4B")
+    G = bytearray(b"\x04\x6B\x17\xD1\xF2\xE1\x2C\x42\x47\xF8\xBC\xE6\xE5\x63\xA4\x40\xF2\x77\x03\x7D\x81\x2D\xEB\x33\xA0\xF4\xA1\x39\x45\xD8\x98\xC2\x96\x4F\xE3\x42\xE2\xFE\x1A\x7F\x9B\x8E\xE7\xEB\x4A\x7C\x0F\x9E\x16\x2B\xCE\x33\x57\x6B\x31\x5E\xCE\xCB\xB6\x40\x68\x37\xBF\x51\xF5")
+    O = bytearray(b"\xFF\xFF\xFF\xFF\x00\x00\x00\x00\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xBC\xE6\xFA\xAD\xA7\x17\x9E\x84\xF3\xB9\xCA\xC2\xFC\x63\x25\x51")
+    F = bytearray(b"\x01")
+
+class SECP384R1:
+    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFF")
+    A = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFF\xFF\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF\xFF\xFC")
+    B = bytearray(b"\xB3\x31\x2F\xA7\xE2\x3E\xE7\xE4\x98\x8E\x05\x6B\xE3\xF8\x2D\x19\x18\x1D\x9C\x6E\xFE\x81\x41\x12\x03\x14\x08\x8F\x50\x13\x87\x5A\xC6\x56\x39\x8D\x8A\x2E\xD1\x9D\x2A\x85\xC8\xED\xD3\xEC\x2A\xEF")
+    G = bytearray(b"\x04\xAA\x87\xCA\x22\xBE\x8B\x05\x37\x8E\xB1\xC7\x1E\xF3\x20\xAD\x74\x6E\x1D\x3B\x62\x8B\xA7\x9B\x98\x59\xF7\x41\xE0\x82\x54\x2A\x38\x55\x02\xF2\x5D\xBF\x55\x29\x6C\x3A\x54\x5E\x38\x72\x76\x0A\xB7\x36\x17\xDE\x4A\x96\x26\x2C\x6F\x5D\x9E\x98\xBF\x92\x92\xDC\x29\xF8\xF4\x1D\xBD\x28\x9A\x14\x7C\xE9\xDA\x31\x13\xB5\xF0\xB8\xC0\x0A\x60\xB1\xCE\x1D\x7E\x81\x9D\x7A\x43\x1D\x7C\x90\xEA\x0E\x5F")
+    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xC7\x63\x4D\x81\xF4\x37\x2D\xDF\x58\x1A\x0D\xB2\x48\xB0\xA7\x7A\xEC\xEC\x19\x6A\xCC\xC5\x29\x73")
+    F = bytearray(b"\x01")
+
+class SECP521R1:
+    P = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF")
+    A = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFC")
+    B = bytearray(b"\x00\x51\x95\x3E\xB9\x61\x8E\x1C\x9A\x1F\x92\x9A\x21\xA0\xB6\x85\x40\xEE\xA2\xDA\x72\x5B\x99\xB3\x15\xF3\xB8\xB4\x89\x91\x8E\xF1\x09\xE1\x56\x19\x39\x51\xEC\x7E\x93\x7B\x16\x52\xC0\xBD\x3B\xB1\xBF\x07\x35\x73\xDF\x88\x3D\x2C\x34\xF1\xEF\x45\x1F\xD4\x6B\x50\x3F\x00")
+    G = bytearray(b"\x04\x00\xC6\x85\x8E\x06\xB7\x04\x04\xE9\xCD\x9E\x3E\xCB\x66\x23\x95\xB4\x42\x9C\x64\x81\x39\x05\x3F\xB5\x21\xF8\x28\xAF\x60\x6B\x4D\x3D\xBA\xA1\x4B\x5E\x77\xEF\xE7\x59\x28\xFE\x1D\xC1\x27\xA2\xFF\xA8\xDE\x33\x48\xB3\xC1\x85\x6A\x42\x9B\xF9\x7E\x7E\x31\xC2\xE5\xBD\x66\x01\x18\x39\x29\x6A\x78\x9A\x3B\xC0\x04\x5C\x8A\x5F\xB4\x2C\x7D\x1B\xD9\x98\xF5\x44\x49\x57\x9B\x44\x68\x17\xAF\xBD\x17\x27\x3E\x66\x2C\x97\xEE\x72\x99\x5E\xF4\x26\x40\xC5\x50\xB9\x01\x3F\xAD\x07\x61\x35\x3C\x70\x86\xA2\x72\xC2\x40\x88\xBE\x94\x76\x9F\xD1\x66\x50")
+    O = bytearray(b"\x01\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFA\x51\x86\x87\x83\xBF\x2F\x96\x6B\x7F\xCC\x01\x48\xF7\x09\xA5\xD0\x3B\xB5\xC9\xB8\x89\x9C\x47\xAE\xBB\x6F\xB7\x1E\x91\x38\x64\x09")
+    F = bytearray(b"\x01")
+
+
+class BP192R1:
+    P = bytearray(b"\xC3\x02\xF4\x1D\x93\x2A\x36\xCD\xA7\xA3\x46\x30\x93\xD1\x8D\xB7\x8F\xCE\x47\x6D\xE1\xA8\x62\x97")
+    A = bytearray(b"\x6A\x91\x17\x40\x76\xB1\xE0\xE1\x9C\x39\xC0\x31\xFE\x86\x85\xC1\xCA\xE0\x40\xE5\xC6\x9A\x28\xEF")
+    B = bytearray(b"\x46\x9A\x28\xEF\x7C\x28\xCC\xA3\xDC\x72\x1D\x04\x4F\x44\x96\xBC\xCA\x7E\xF4\x14\x6F\xBF\x25\xC9")
+    G = bytearray(b"\x04\xC0\xA0\x64\x7E\xAA\xB6\xA4\x87\x53\xB0\x33\xC5\x6C\xB0\xF0\x90\x0A\x2F\x5C\x48\x53\x37\x5F\xD6\x14\xB6\x90\x86\x6A\xBD\x5B\xB8\x8B\x5F\x48\x28\xC1\x49\x00\x02\xE6\x77\x3F\xA2\xFA\x29\x9B\x8F")
+    O = bytearray(b"\xC3\x02\xF4\x1D\x93\x2A\x36\xCD\xA7\xA3\x46\x2F\x9E\x9E\x91\x6B\x5B\xE8\xF1\x02\x9A\xC4\xAC\xC1")
+    F = bytearray(b"\x01")
+
+class BP224R1:
+    P = bytearray(b"\xD7\xC1\x34\xAA\x26\x43\x66\x86\x2A\x18\x30\x25\x75\xD1\xD7\x87\xB0\x9F\x07\x57\x97\xDA\x89\xF5\x7E\xC8\xC0\xFF")
+    A = bytearray(b"\x68\xA5\xE6\x2C\xA9\xCE\x6C\x1C\x29\x98\x03\xA6\xC1\x53\x0B\x51\x4E\x18\x2A\xD8\xB0\x04\x2A\x59\xCA\xD2\x9F\x43")
+    B = bytearray(b"\x25\x80\xF6\x3C\xCF\xE4\x41\x38\x87\x07\x13\xB1\xA9\x23\x69\xE3\x3E\x21\x35\xD2\x66\xDB\xB3\x72\x38\x6C\x40\x0B")
+    G = bytearray(b"\x04\x0D\x90\x29\xAD\x2C\x7E\x5C\xF4\x34\x08\x23\xB2\xA8\x7D\xC6\x8C\x9E\x4C\xE3\x17\x4C\x1E\x6E\xFD\xEE\x12\xC0\x7D\x58\xAA\x56\xF7\x72\xC0\x72\x6F\x24\xC6\xB8\x9E\x4E\xCD\xAC\x24\x35\x4B\x9E\x99\xCA\xA3\xF6\xD3\x76\x14\x02\xCD")
+    O = bytearray(b"\xD7\xC1\x34\xAA\x26\x43\x66\x86\x2A\x18\x30\x25\x75\xD0\xFB\x98\xD1\x16\xBC\x4B\x6D\xDE\xBC\xA3\xA5\xA7\x93\x9F")
+    F = bytearray(b"\x01")
+
+class BP256R1:
+    P = bytearray(b"\xA9\xFB\x57\xDB\xA1\xEE\xA9\xBC\x3E\x66\x0A\x90\x9D\x83\x8D\x72\x6E\x3B\xF6\x23\xD5\x26\x20\x28\x20\x13\x48\x1D\x1F\x6E\x53\x77")
+    A = bytearray(b"\x7D\x5A\x09\x75\xFC\x2C\x30\x57\xEE\xF6\x75\x30\x41\x7A\xFF\xE7\xFB\x80\x55\xC1\x26\xDC\x5C\x6C\xE9\x4A\x4B\x44\xF3\x30\xB5\xD9")
+    B = bytearray(b"\x26\xDC\x5C\x6C\xE9\x4A\x4B\x44\xF3\x30\xB5\xD9\xBB\xD7\x7C\xBF\x95\x84\x16\x29\x5C\xF7\xE1\xCE\x6B\xCC\xDC\x18\xFF\x8C\x07\xB6")
+    G = bytearray(b"\x04\x8B\xD2\xAE\xB9\xCB\x7E\x57\xCB\x2C\x4B\x48\x2F\xFC\x81\xB7\xAF\xB9\xDE\x27\xE1\xE3\xBD\x23\xC2\x3A\x44\x53\xBD\x9A\xCE\x32\x62\x54\x7E\xF8\x35\xC3\xDA\xC4\xFD\x97\xF8\x46\x1A\x14\x61\x1D\xC9\xC2\x77\x45\x13\x2D\xED\x8E\x54\x5C\x1D\x54\xC7\x2F\x04\x69\x97")
+    O = bytearray(b"\xA9\xFB\x57\xDB\xA1\xEE\xA9\xBC\x3E\x66\x0A\x90\x9D\x83\x8D\x71\x8C\x39\x7A\xA3\xB5\x61\xA6\xF7\x90\x1E\x0E\x82\x97\x48\x56\xA7")
+    F = bytearray(b"\x01")
+
+class BP320R1:
+    P = bytearray(b"\xD3\x5E\x47\x20\x36\xBC\x4F\xB7\xE1\x3C\x78\x5E\xD2\x01\xE0\x65\xF9\x8F\xCF\xA6\xF6\xF4\x0D\xEF\x4F\x92\xB9\xEC\x78\x93\xEC\x28\xFC\xD4\x12\xB1\xF1\xB3\x2E\x27")
+    A = bytearray(b"\x3E\xE3\x0B\x56\x8F\xBA\xB0\xF8\x83\xCC\xEB\xD4\x6D\x3F\x3B\xB8\xA2\xA7\x35\x13\xF5\xEB\x79\xDA\x66\x19\x0E\xB0\x85\xFF\xA9\xF4\x92\xF3\x75\xA9\x7D\x86\x0E\xB4")
+    B = bytearray(b"\x52\x08\x83\x94\x9D\xFD\xBC\x42\xD3\xAD\x19\x86\x40\x68\x8A\x6F\xE1\x3F\x41\x34\x95\x54\xB4\x9A\xCC\x31\xDC\xCD\x88\x45\x39\x81\x6F\x5E\xB4\xAC\x8F\xB1\xF1\xA6")
+    G = bytearray(b"\x04\x43\xBD\x7E\x9A\xFB\x53\xD8\xB8\x52\x89\xBC\xC4\x8E\xE5\xBF\xE6\xF2\x01\x37\xD1\x0A\x08\x7E\xB6\xE7\x87\x1E\x2A\x10\xA5\x99\xC7\x10\xAF\x8D\x0D\x39\xE2\x06\x11\x14\xFD\xD0\x55\x45\xEC\x1C\xC8\xAB\x40\x93\x24\x7F\x77\x27\x5E\x07\x43\xFF\xED\x11\x71\x82\xEA\xA9\xC7\x78\x77\xAA\xAC\x6A\xC7\xD3\x52\x45\xD1\x69\x2E\x8E\xE1")
+    O = bytearray(b"\xD3\x5E\x47\x20\x36\xBC\x4F\xB7\xE1\x3C\x78\x5E\xD2\x01\xE0\x65\xF9\x8F\xCF\xA5\xB6\x8F\x12\xA3\x2D\x48\x2E\xC7\xEE\x86\x58\xE9\x86\x91\x55\x5B\x44\xC5\x93\x11")
+    F = bytearray(b"\0x1")
+
+class BP384R1:
+    P = bytearray(b"\x8C\xB9\x1E\x82\xA3\x38\x6D\x28\x0F\x5D\x6F\x7E\x50\xE6\x41\xDF\x15\x2F\x71\x09\xED\x54\x56\xB4\x12\xB1\xDA\x19\x7F\xB7\x11\x23\xAC\xD3\xA7\x29\x90\x1D\x1A\x71\x87\x47\x00\x13\x31\x07\xEC\x53")
+    A = bytearray(b"\x7B\xC3\x82\xC6\x3D\x8C\x15\x0C\x3C\x72\x08\x0A\xCE\x05\xAF\xA0\xC2\xBE\xA2\x8E\x4F\xB2\x27\x87\x13\x91\x65\xEF\xBA\x91\xF9\x0F\x8A\xA5\x81\x4A\x50\x3A\xD4\xEB\x04\xA8\xC7\xDD\x22\xCE\x28\x26")
+    B = bytearray(b"\x04\xA8\xC7\xDD\x22\xCE\x28\x26\x8B\x39\xB5\x54\x16\xF0\x44\x7C\x2F\xB7\x7D\xE1\x07\xDC\xD2\xA6\x2E\x88\x0E\xA5\x3E\xEB\x62\xD5\x7C\xB4\x39\x02\x95\xDB\xC9\x94\x3A\xB7\x86\x96\xFA\x50\x4C\x11")
+    G = bytearray(b"\x04\x1D\x1C\x64\xF0\x68\xCF\x45\xFF\xA2\xA6\x3A\x81\xB7\xC1\x3F\x6B\x88\x47\xA3\xE7\x7E\xF1\x4F\xE3\xDB\x7F\xCA\xFE\x0C\xBD\x10\xE8\xE8\x26\xE0\x34\x36\xD6\x46\xAA\xEF\x87\xB2\xE2\x47\xD4\xAF\x1E\x8A\xBE\x1D\x75\x20\xF9\xC2\xA4\x5C\xB1\xEB\x8E\x95\xCF\xD5\x52\x62\xB7\x0B\x29\xFE\xEC\x58\x64\xE1\x9C\x05\x4F\xF9\x91\x29\x28\x0E\x46\x46\x21\x77\x91\x81\x11\x42\x82\x03\x41\x26\x3C\x53\x15")
+    O = bytearray(b"\x8C\xB9\x1E\x82\xA3\x38\x6D\x28\x0F\x5D\x6F\x7E\x50\xE6\x41\xDF\x15\x2F\x71\x09\xED\x54\x56\xB3\x1F\x16\x6E\x6C\xAC\x04\x25\xA7\xCF\x3A\xB6\xAF\x6B\x7F\xC3\x10\x3B\x88\x32\x02\xE9\x04\x65\x65")
+    F = bytearray(b"\x01")
+
+class BP512R1:
+    P = bytearray(b"\xAA\xDD\x9D\xB8\xDB\xE9\xC4\x8B\x3F\xD4\xE6\xAE\x33\xC9\xFC\x07\xCB\x30\x8D\xB3\xB3\xC9\xD2\x0E\xD6\x63\x9C\xCA\x70\x33\x08\x71\x7D\x4D\x9B\x00\x9B\xC6\x68\x42\xAE\xCD\xA1\x2A\xE6\xA3\x80\xE6\x28\x81\xFF\x2F\x2D\x82\xC6\x85\x28\xAA\x60\x56\x58\x3A\x48\xF3")
+    A = bytearray(b"\x78\x30\xA3\x31\x8B\x60\x3B\x89\xE2\x32\x71\x45\xAC\x23\x4C\xC5\x94\xCB\xDD\x8D\x3D\xF9\x16\x10\xA8\x34\x41\xCA\xEA\x98\x63\xBC\x2D\xED\x5D\x5A\xA8\x25\x3A\xA1\x0A\x2E\xF1\xC9\x8B\x9A\xC8\xB5\x7F\x11\x17\xA7\x2B\xF2\xC7\xB9\xE7\xC1\xAC\x4D\x77\xFC\x94\xCA")
+    B = bytearray(b"\x3D\xF9\x16\x10\xA8\x34\x41\xCA\xEA\x98\x63\xBC\x2D\xED\x5D\x5A\xA8\x25\x3A\xA1\x0A\x2E\xF1\xC9\x8B\x9A\xC8\xB5\x7F\x11\x17\xA7\x2B\xF2\xC7\xB9\xE7\xC1\xAC\x4D\x77\xFC\x94\xCA\xDC\x08\x3E\x67\x98\x40\x50\xB7\x5E\xBA\xE5\xDD\x28\x09\xBD\x63\x80\x16\xF7\x23")
+    G = bytearray(b"\x04\x81\xAE\xE4\xBD\xD8\x2E\xD9\x64\x5A\x21\x32\x2E\x9C\x4C\x6A\x93\x85\xED\x9F\x70\xB5\xD9\x16\xC1\xB4\x3B\x62\xEE\xF4\xD0\x09\x8E\xFF\x3B\x1F\x78\xE2\xD0\xD4\x8D\x50\xD1\x68\x7B\x93\xB9\x7D\x5F\x7C\x6D\x50\x47\x40\x6A\x5E\x68\x8B\x35\x22\x09\xBC\xB9\xF8\x22\x7D\xDE\x38\x5D\x56\x63\x32\xEC\xC0\xEA\xBF\xA9\xCF\x78\x22\xFD\xF2\x09\xF7\x00\x24\xA5\x7B\x1A\xA0\x00\xC5\x5B\x88\x1F\x81\x11\xB2\xDC\xDE\x49\x4A\x5F\x48\x5E\x5B\xCA\x4B\xD8\x8A\x27\x63\xAE\xD1\xCA\x2B\x2F\xA8\xF0\x54\x06\x78\xCD\x1E\x0F\x3A\xD8\x08\x92")
+    O = bytearray(b"\xAA\xDD\x9D\xB8\xDB\xE9\xC4\x8B\x3F\xD4\xE6\xAE\x33\xC9\xFC\x07\xCB\x30\x8D\xB3\xB3\xC9\xD2\x0E\xD6\x63\x9C\xCA\x70\x33\x08\x70\x55\x3E\x5C\x41\x4C\xA9\x26\x19\x41\x86\x61\x19\x7F\xAC\x10\x47\x1D\xB1\xD3\x81\x08\x5D\xDA\xDD\xB5\x87\x96\x82\x9C\xA9\x00\x69")
+    F = bytearray(b"\x01")
+
+class SECP192K1:
+    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xEE\x37")
+    A = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
+    B = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x03")
+    G = bytearray(b"\x04\xDB\x4F\xF1\x0E\xC0\x57\xE9\xAE\x26\xB0\x7D\x02\x80\xB7\xF4\x34\x1D\xA5\xD1\xB1\xEA\xE0\x6C\x7D\x9B\x2F\x2F\x6D\x9C\x56\x28\xA7\x84\x41\x63\xD0\x15\xBE\x86\x34\x40\x82\xAA\x88\xD9\x5E\x2F\x9D")
+    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\x26\xF2\xFC\x17\x0F\x69\x46\x6A\x74\xDE\xFD\x8D")
+    F = bytearray(b"\x01")
+
+class SECP256K1:
+    P = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xFF\xFF\xFC\x2F")
+    A = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
+    B = bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x07")
+    G = bytearray(b"\x04\x79\xBE\x66\x7E\xF9\xDC\xBB\xAC\x55\xA0\x62\x95\xCE\x87\x0B\x07\x02\x9B\xFC\xDB\x2D\xCE\x28\xD9\x59\xF2\x81\x5B\x16\xF8\x17\x98\x48\x3A\xDA\x77\x26\xA3\xC4\x65\x5D\xA4\xFB\xFC\x0E\x11\x08\xA8\xFD\x17\xB4\x48\xA6\x85\x54\x19\x9C\x47\xD0\x8F\xFB\x10\xD4\xB8")
+    O = bytearray(b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFE\xBA\xAE\xDC\xE6\xAF\x48\xA0\x3B\xBF\xD2\x5E\x8C\xD0\x36\x41\x41")
+    F = bytearray(b"\x01")
+
+
+def ec_domain(curve):
+    if (curve.name == 'secp192r1'):
+        return SECP192R1()
+    elif (curve.name == 'secp256r1'):
+        return SECP256R1()
+    elif (curve.name == 'secp384r1'):
+        return SECP384R1()
+    elif (curve.name == 'secp521r1'):
+        return SECP521R1()
+    elif (curve.name == 'brainpoolP192r1'):
+        return BP192R1()
+    elif (curve.name == 'brainpoolP224r1'):
+        return BP224R1()
+    elif (curve.name == 'brainpoolP256r1'):
+        return BP256R1()
+    elif (curve.name == 'brainpoolP320r1'):
+        return BP320R1()
+    elif (curve.name == 'brainpoolP384r1'):
+        return BP384R1()
+    elif (curve.name == 'brainpoolP512r1'):
+        return BP512R1()
+    elif (curve.name == 'secp192k1'):
+        return SECP192K1()
+    elif (curve.name == 'secp256k1'):
+        return SECP256K1()
+    return None
+
+def find_curve(P):
+    if (SECP192R1.P == P):
+        return ec.SECP192R1()
+    elif (SECP256K1.P == P):
+        return ec.SECP256K1()
+    elif (SECP256R1.P == P):
+        return ec.SECP256R1()
+    elif (SECP384R1.P == P):
+        return ec.SECP384R1()
+    elif (SECP521R1.P == P):
+        return ec.SECP521R1()
+    elif (BP256R1.P == P):
+        return ec.BrainpoolP256R1()
+    elif (BP384R1.P == P):
+        return ec.BrainpoolP384R1()
+    elif (BP512R1.P == P):
+        return ec.BrainpoolP512R1()
     return None
```

## cvc/oid.py

 * *Ordering differences only*

```diff
@@ -1,198 +1,198 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-BSI_DE                      = b"\x04\x00\x7F\x00\x07"
-
-ID_ECPSPUBLICKEY            = BSI_DE + b"\x01\x01\x02\x03"
-
-ID_STANDARDIZED_DOMAIN_PARAMETERS = BSI_DE + b"\x01\x02"
-
-ID_PK                       = BSI_DE + b"\x02\x02\x01"
-ID_PK_DH                    = ID_PK + b"\x01"
-ID_PK_ECDH                  = ID_PK + b"\x02"
-ID_PS_PK                    = ID_PK + b"\x03"
-ID_PS_PK_ECSCHNORR          = ID_PS_PK + b"\x02"
-
-ID_TA                       = BSI_DE + b"\x02\x02\x02"
-
-ID_TA_RSA                   = ID_TA + b"\x01"
-
-ID_TA_RSA_V1_5_SHA_1        = ID_TA_RSA + b"\x01"
-ID_TA_RSA_V1_5_SHA_256      = ID_TA_RSA + b"\x02"
-ID_TA_RSA_PSS_SHA_1         = ID_TA_RSA + b"\x03"
-ID_TA_RSA_PSS_SHA_256       = ID_TA_RSA + b"\x04"
-ID_TA_RSA_V1_5_SHA_512      = ID_TA_RSA + b"\x05"
-ID_TA_RSA_PSS_SHA_512       = ID_TA_RSA + b"\x06"
-
-ID_TA_ECDSA                 = ID_TA + b"\x02"
-
-ID_TA_ECDSA_SHA_1           = ID_TA_ECDSA + b"\x01"
-ID_TA_ECDSA_SHA_224         = ID_TA_ECDSA + b"\x02"
-ID_TA_ECDSA_SHA_256         = ID_TA_ECDSA + b"\x03"
-ID_TA_ECDSA_SHA_384         = ID_TA_ECDSA + b"\x04"
-ID_TA_ECDSA_SHA_512         = ID_TA_ECDSA + b"\x05"
-
-ID_CA                       = BSI_DE + b"\x02\x02\x03"
-
-ID_CA_DH                    = ID_CA + b"\x01"
-ID_CA_DH_3DES_CBC_CBC       = ID_CA_DH + b"\x01"
-ID_CA_DH_AES_CBC_CMAC_128   = ID_CA_DH + b"\x02"
-ID_CA_DH_AES_CBC_CMAC_192   = ID_CA_DH + b"\x03"
-ID_CA_DH_AES_CBC_CMAC_256   = ID_CA_DH + b"\x04"
-
-ID_CA_ECDH                  = ID_CA + b"\x02"
-ID_CA_ECDH_3DES_CBC_CBC     = ID_CA_ECDH + b"\x01"
-ID_CA_ECDH_AES_CBC_CMAC_128 = ID_CA_ECDH + b"\x02"
-ID_CA_ECDH_AES_CBC_CMAC_192 = ID_CA_ECDH + b"\x03"
-ID_CA_ECDH_AES_CBC_CMAC_256 = ID_CA_ECDH + b"\x04"
-
-ID_PACE                     = BSI_DE + b"\x02\x02\x04"
-
-ID_PACE_DH_GM               = ID_PACE + b"\x01"
-ID_PACE_DH_GM_3DES_CBC_CBC  = ID_PACE_DH_GM + b"\x01"
-ID_PACE_DH_GM_AES_CBC_CMAC_128  = ID_PACE_DH_GM + b"\x02"
-ID_PACE_DH_GM_AES_CBC_CMAC_192  = ID_PACE_DH_GM + b"\x03"
-ID_PACE_DH_GM_AES_CBC_CMAC_256  = ID_PACE_DH_GM + b"\x04"
-
-ID_PACE_ECDH_GM               = ID_PACE + b"\x02"
-ID_PACE_ECDH_GM_3DES_CBC_CBC  = ID_PACE_ECDH_GM + b"\x01"
-ID_PACE_ECDH_GM_AES_CBC_CMAC_128  = ID_PACE_ECDH_GM + b"\x02"
-ID_PACE_ECDH_GM_AES_CBC_CMAC_192  = ID_PACE_ECDH_GM + b"\x03"
-ID_PACE_ECDH_GM_AES_CBC_CMAC_256  = ID_PACE_ECDH_GM + b"\x04"
-
-ID_PACE_DH_IM               = ID_PACE + b"\x03"
-ID_PACE_DH_IM_3DES_CBC_CBC  = ID_PACE_DH_IM + b"\x01"
-ID_PACE_DH_IM_AES_CBC_CMAC_128  = ID_PACE_DH_IM + b"\x02"
-ID_PACE_DH_IM_AES_CBC_CMAC_192  = ID_PACE_DH_IM + b"\x03"
-ID_PACE_DH_IM_AES_CBC_CMAC_256  = ID_PACE_DH_IM + b"\x04"
-
-ID_PACE_ECDH_IM               = ID_PACE + b"\x04"
-ID_PACE_ECDH_IM_3DES_CBC_CBC  = ID_PACE_ECDH_IM + b"\x01"
-ID_PACE_ECDH_IM_AES_CBC_CMAC_128  = ID_PACE_ECDH_IM + b"\x02"
-ID_PACE_ECDH_IM_AES_CBC_CMAC_192  = ID_PACE_ECDH_IM + b"\x03"
-ID_PACE_ECDH_IM_AES_CBC_CMAC_256  = ID_PACE_ECDH_IM + b"\x04"
-
-ID_RI                       = BSI_DE + b"\x02\x02\x05"
-
-ID_RI_DH                    = ID_RI + b"\x01"
-
-ID_RI_DH_SHA_1              = ID_RI_DH + b"\x01"
-ID_RI_DH_SHA_224            = ID_RI_DH + b"\x02"
-ID_RI_DH_SHA_256            = ID_RI_DH + b"\x03"
-ID_RI_DH_SHA_384            = ID_RI_DH + b"\x04"
-ID_RI_DH_SHA_512            = ID_RI_DH + b"\x05"
-
-ID_RI_ECDH                  = ID_RI + b"\x02"
-
-ID_RI_ECDH_SHA_1            = ID_RI_ECDH + b"\x01"
-ID_RI_ECDH_SHA_224          = ID_RI_ECDH + b"\x02"
-ID_RI_ECDH_SHA_256          = ID_RI_ECDH + b"\x03"
-ID_RI_ECDH_SHA_384          = ID_RI_ECDH + b"\x04"
-ID_RI_ECDH_SHA_512          = ID_RI_ECDH + b"\x05"
-
-ID_CI                       = BSI_DE + b"\x02\x02\x06"
-
-ID_EIDSECURITY              = BSI_DE + b"\x02\x02\x07"
-
-ID_PASSWORD_TYPE            = BSI_DE + b"\x02\x02\x08"
-
-ID_PS                       = BSI_DE + b"\x02\x02\x0B"
-ID_PSA                      = ID_PS + b"\x01"
-ID_PSA_ECDH_ECSCHNORR       = ID_PSA + b"\x02"
-ID_PSA_ECDH_ECSCHNORR_SHA256 = ID_PSA_ECDH_ECSCHNORR + b"\x03"
-ID_PSA_ECDH_ECSCHNORR_SHA384 = ID_PSA_ECDH_ECSCHNORR + b"\x04"
-ID_PSA_ECDH_ECSCHNORR_SHA512 = ID_PSA_ECDH_ECSCHNORR + b"\x05"
-
-ID_PASSWORD_TYPE            = BSI_DE + b"\x02\x02\x0C"
-ID_MRZ                      = ID_PASSWORD_TYPE + b"\x01"
-ID_CAN                      = ID_PASSWORD_TYPE + b"\x02"
-ID_PIN                      = ID_PASSWORD_TYPE + b"\x03"
-ID_PUK                      = ID_PASSWORD_TYPE + b"\x04"
-
-ID_ROLES                    = BSI_DE + b"\x03\x01\x02"
-ID_IS                       = ID_ROLES + b"\x01"
-ID_AT                       = ID_ROLES + b"\x02"
-ID_SPECIAL_FUNCTIONS        = ID_AT + b"\x02"
-ID_ST                       = ID_ROLES + b"\x03"
-
-ID_EXTENSIONS               = BSI_DE + b"\x03\x01\x03"
-ID_DESCRIPTION              = ID_EXTENSIONS + b"\x01"
-ID_PLAINFORMAT              = ID_DESCRIPTION + b"\x01"
-ID_HTMLFORMAT               = ID_DESCRIPTION + b"\x02"
-ID_PDFFORMAT                = ID_DESCRIPTION + b"\x03"
-ID_SECTOR                   = ID_EXTENSIONS + b"\x02"
-ID_PS_SECTOR                = ID_EXTENSIONS + b"\x03"
-
-ID_AUXILIARY_TYPE           = BSI_DE + b"\x03\x01\x04"
-ID_DATEOFBIRTH              = ID_AUXILIARY_TYPE + b"\x01"
-ID_DATEOFEXPIRY             = ID_AUXILIARY_TYPE + b"\x02"
-ID_MUNICIPALITYID           = ID_AUXILIARY_TYPE + b"\x03"
-ID_PSM_MESSAGE              = ID_AUXILIARY_TYPE + b"\x04"
-ID_DGCONTENT                = ID_AUXILIARY_TYPE + b"\x05"
-ID_DGCONTENT_DG1            = ID_DGCONTENT + b"\x01"
-ID_DGCONTENT_DG2            = ID_DGCONTENT + b"\x02"
-ID_DGCONTENT_DG3            = ID_DGCONTENT + b"\x03"
-ID_DGCONTENT_DG4            = ID_DGCONTENT + b"\x04"
-ID_DGCONTENT_DG5            = ID_DGCONTENT + b"\x05"
-ID_DGCONTENT_DG6            = ID_DGCONTENT + b"\x06"
-ID_DGCONTENT_DG7            = ID_DGCONTENT + b"\x07"
-ID_DGCONTENT_DG8            = ID_DGCONTENT + b"\x08"
-ID_DGCONTENT_DG9            = ID_DGCONTENT + b"\x09"
-ID_DGCONTENT_DG10           = ID_DGCONTENT + b"\x0A"
-ID_DGCONTENT_DG11           = ID_DGCONTENT + b"\x0B"
-ID_DGCONTENT_DG12           = ID_DGCONTENT + b"\x0C"
-ID_DGCONTENT_DG13           = ID_DGCONTENT + b"\x0D"
-ID_DGCONTENT_DG14           = ID_DGCONTENT + b"\x0E"
-ID_DGCONTENT_DG15           = ID_DGCONTENT + b"\x0F"
-ID_DGCONTENT_DG16           = ID_DGCONTENT + b"\x10"
-ID_DGCONTENT_DG17           = ID_DGCONTENT + b"\x11"
-ID_DGCONTENT_DG18           = ID_DGCONTENT + b"\x12"
-ID_DGCONTENT_DG19           = ID_DGCONTENT + b"\x13"
-ID_DGCONTENT_DG20           = ID_DGCONTENT + b"\x14"
-ID_DGCONTENT_DG21           = ID_DGCONTENT + b"\x15"
-ID_DGCONTENT_DG22           = ID_DGCONTENT + b"\x16"
-
-ID_SECURITY_OBJECT          = BSI_DE + b"\x03\x02\x01"
-
-schemes = [
-    ('ECDSA_SHA_1', ID_TA_ECDSA_SHA_1),
-    ('ECDSA_SHA_224', ID_TA_ECDSA_SHA_224),
-    ('ECDSA_SHA_256', ID_TA_ECDSA_SHA_256),
-    ('ECDSA_SHA_384', ID_TA_ECDSA_SHA_384),
-    ('ECDSA_SHA_512', ID_TA_ECDSA_SHA_512),
-    ('RSA_v1_5_SHA_1', ID_TA_RSA_V1_5_SHA_1),
-    ('RSA_v1_5_SHA_256', ID_TA_RSA_V1_5_SHA_256),
-    ('RSA_v1_5_SHA_512', ID_TA_RSA_V1_5_SHA_512),
-    ('RSA_PSS_SHA_1', ID_TA_RSA_PSS_SHA_1),
-    ('RSA_PSS_SHA_256', ID_TA_RSA_PSS_SHA_256),
-    ('RSA_PSS_SHA_512', ID_TA_RSA_PSS_SHA_512),
-    ]
-
-def scheme2oid(scheme):
-    for s,o in schemes:
-        if (s == scheme):
-            return o
-    return None
-
-def oid2scheme(oid):
-    for s,o in schemes:
-        if (o == oid):
-            return s
-    return None
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+BSI_DE                      = b"\x04\x00\x7F\x00\x07"
+
+ID_ECPSPUBLICKEY            = BSI_DE + b"\x01\x01\x02\x03"
+
+ID_STANDARDIZED_DOMAIN_PARAMETERS = BSI_DE + b"\x01\x02"
+
+ID_PK                       = BSI_DE + b"\x02\x02\x01"
+ID_PK_DH                    = ID_PK + b"\x01"
+ID_PK_ECDH                  = ID_PK + b"\x02"
+ID_PS_PK                    = ID_PK + b"\x03"
+ID_PS_PK_ECSCHNORR          = ID_PS_PK + b"\x02"
+
+ID_TA                       = BSI_DE + b"\x02\x02\x02"
+
+ID_TA_RSA                   = ID_TA + b"\x01"
+
+ID_TA_RSA_V1_5_SHA_1        = ID_TA_RSA + b"\x01"
+ID_TA_RSA_V1_5_SHA_256      = ID_TA_RSA + b"\x02"
+ID_TA_RSA_PSS_SHA_1         = ID_TA_RSA + b"\x03"
+ID_TA_RSA_PSS_SHA_256       = ID_TA_RSA + b"\x04"
+ID_TA_RSA_V1_5_SHA_512      = ID_TA_RSA + b"\x05"
+ID_TA_RSA_PSS_SHA_512       = ID_TA_RSA + b"\x06"
+
+ID_TA_ECDSA                 = ID_TA + b"\x02"
+
+ID_TA_ECDSA_SHA_1           = ID_TA_ECDSA + b"\x01"
+ID_TA_ECDSA_SHA_224         = ID_TA_ECDSA + b"\x02"
+ID_TA_ECDSA_SHA_256         = ID_TA_ECDSA + b"\x03"
+ID_TA_ECDSA_SHA_384         = ID_TA_ECDSA + b"\x04"
+ID_TA_ECDSA_SHA_512         = ID_TA_ECDSA + b"\x05"
+
+ID_CA                       = BSI_DE + b"\x02\x02\x03"
+
+ID_CA_DH                    = ID_CA + b"\x01"
+ID_CA_DH_3DES_CBC_CBC       = ID_CA_DH + b"\x01"
+ID_CA_DH_AES_CBC_CMAC_128   = ID_CA_DH + b"\x02"
+ID_CA_DH_AES_CBC_CMAC_192   = ID_CA_DH + b"\x03"
+ID_CA_DH_AES_CBC_CMAC_256   = ID_CA_DH + b"\x04"
+
+ID_CA_ECDH                  = ID_CA + b"\x02"
+ID_CA_ECDH_3DES_CBC_CBC     = ID_CA_ECDH + b"\x01"
+ID_CA_ECDH_AES_CBC_CMAC_128 = ID_CA_ECDH + b"\x02"
+ID_CA_ECDH_AES_CBC_CMAC_192 = ID_CA_ECDH + b"\x03"
+ID_CA_ECDH_AES_CBC_CMAC_256 = ID_CA_ECDH + b"\x04"
+
+ID_PACE                     = BSI_DE + b"\x02\x02\x04"
+
+ID_PACE_DH_GM               = ID_PACE + b"\x01"
+ID_PACE_DH_GM_3DES_CBC_CBC  = ID_PACE_DH_GM + b"\x01"
+ID_PACE_DH_GM_AES_CBC_CMAC_128  = ID_PACE_DH_GM + b"\x02"
+ID_PACE_DH_GM_AES_CBC_CMAC_192  = ID_PACE_DH_GM + b"\x03"
+ID_PACE_DH_GM_AES_CBC_CMAC_256  = ID_PACE_DH_GM + b"\x04"
+
+ID_PACE_ECDH_GM               = ID_PACE + b"\x02"
+ID_PACE_ECDH_GM_3DES_CBC_CBC  = ID_PACE_ECDH_GM + b"\x01"
+ID_PACE_ECDH_GM_AES_CBC_CMAC_128  = ID_PACE_ECDH_GM + b"\x02"
+ID_PACE_ECDH_GM_AES_CBC_CMAC_192  = ID_PACE_ECDH_GM + b"\x03"
+ID_PACE_ECDH_GM_AES_CBC_CMAC_256  = ID_PACE_ECDH_GM + b"\x04"
+
+ID_PACE_DH_IM               = ID_PACE + b"\x03"
+ID_PACE_DH_IM_3DES_CBC_CBC  = ID_PACE_DH_IM + b"\x01"
+ID_PACE_DH_IM_AES_CBC_CMAC_128  = ID_PACE_DH_IM + b"\x02"
+ID_PACE_DH_IM_AES_CBC_CMAC_192  = ID_PACE_DH_IM + b"\x03"
+ID_PACE_DH_IM_AES_CBC_CMAC_256  = ID_PACE_DH_IM + b"\x04"
+
+ID_PACE_ECDH_IM               = ID_PACE + b"\x04"
+ID_PACE_ECDH_IM_3DES_CBC_CBC  = ID_PACE_ECDH_IM + b"\x01"
+ID_PACE_ECDH_IM_AES_CBC_CMAC_128  = ID_PACE_ECDH_IM + b"\x02"
+ID_PACE_ECDH_IM_AES_CBC_CMAC_192  = ID_PACE_ECDH_IM + b"\x03"
+ID_PACE_ECDH_IM_AES_CBC_CMAC_256  = ID_PACE_ECDH_IM + b"\x04"
+
+ID_RI                       = BSI_DE + b"\x02\x02\x05"
+
+ID_RI_DH                    = ID_RI + b"\x01"
+
+ID_RI_DH_SHA_1              = ID_RI_DH + b"\x01"
+ID_RI_DH_SHA_224            = ID_RI_DH + b"\x02"
+ID_RI_DH_SHA_256            = ID_RI_DH + b"\x03"
+ID_RI_DH_SHA_384            = ID_RI_DH + b"\x04"
+ID_RI_DH_SHA_512            = ID_RI_DH + b"\x05"
+
+ID_RI_ECDH                  = ID_RI + b"\x02"
+
+ID_RI_ECDH_SHA_1            = ID_RI_ECDH + b"\x01"
+ID_RI_ECDH_SHA_224          = ID_RI_ECDH + b"\x02"
+ID_RI_ECDH_SHA_256          = ID_RI_ECDH + b"\x03"
+ID_RI_ECDH_SHA_384          = ID_RI_ECDH + b"\x04"
+ID_RI_ECDH_SHA_512          = ID_RI_ECDH + b"\x05"
+
+ID_CI                       = BSI_DE + b"\x02\x02\x06"
+
+ID_EIDSECURITY              = BSI_DE + b"\x02\x02\x07"
+
+ID_PASSWORD_TYPE            = BSI_DE + b"\x02\x02\x08"
+
+ID_PS                       = BSI_DE + b"\x02\x02\x0B"
+ID_PSA                      = ID_PS + b"\x01"
+ID_PSA_ECDH_ECSCHNORR       = ID_PSA + b"\x02"
+ID_PSA_ECDH_ECSCHNORR_SHA256 = ID_PSA_ECDH_ECSCHNORR + b"\x03"
+ID_PSA_ECDH_ECSCHNORR_SHA384 = ID_PSA_ECDH_ECSCHNORR + b"\x04"
+ID_PSA_ECDH_ECSCHNORR_SHA512 = ID_PSA_ECDH_ECSCHNORR + b"\x05"
+
+ID_PASSWORD_TYPE            = BSI_DE + b"\x02\x02\x0C"
+ID_MRZ                      = ID_PASSWORD_TYPE + b"\x01"
+ID_CAN                      = ID_PASSWORD_TYPE + b"\x02"
+ID_PIN                      = ID_PASSWORD_TYPE + b"\x03"
+ID_PUK                      = ID_PASSWORD_TYPE + b"\x04"
+
+ID_ROLES                    = BSI_DE + b"\x03\x01\x02"
+ID_IS                       = ID_ROLES + b"\x01"
+ID_AT                       = ID_ROLES + b"\x02"
+ID_SPECIAL_FUNCTIONS        = ID_AT + b"\x02"
+ID_ST                       = ID_ROLES + b"\x03"
+
+ID_EXTENSIONS               = BSI_DE + b"\x03\x01\x03"
+ID_DESCRIPTION              = ID_EXTENSIONS + b"\x01"
+ID_PLAINFORMAT              = ID_DESCRIPTION + b"\x01"
+ID_HTMLFORMAT               = ID_DESCRIPTION + b"\x02"
+ID_PDFFORMAT                = ID_DESCRIPTION + b"\x03"
+ID_SECTOR                   = ID_EXTENSIONS + b"\x02"
+ID_PS_SECTOR                = ID_EXTENSIONS + b"\x03"
+
+ID_AUXILIARY_TYPE           = BSI_DE + b"\x03\x01\x04"
+ID_DATEOFBIRTH              = ID_AUXILIARY_TYPE + b"\x01"
+ID_DATEOFEXPIRY             = ID_AUXILIARY_TYPE + b"\x02"
+ID_MUNICIPALITYID           = ID_AUXILIARY_TYPE + b"\x03"
+ID_PSM_MESSAGE              = ID_AUXILIARY_TYPE + b"\x04"
+ID_DGCONTENT                = ID_AUXILIARY_TYPE + b"\x05"
+ID_DGCONTENT_DG1            = ID_DGCONTENT + b"\x01"
+ID_DGCONTENT_DG2            = ID_DGCONTENT + b"\x02"
+ID_DGCONTENT_DG3            = ID_DGCONTENT + b"\x03"
+ID_DGCONTENT_DG4            = ID_DGCONTENT + b"\x04"
+ID_DGCONTENT_DG5            = ID_DGCONTENT + b"\x05"
+ID_DGCONTENT_DG6            = ID_DGCONTENT + b"\x06"
+ID_DGCONTENT_DG7            = ID_DGCONTENT + b"\x07"
+ID_DGCONTENT_DG8            = ID_DGCONTENT + b"\x08"
+ID_DGCONTENT_DG9            = ID_DGCONTENT + b"\x09"
+ID_DGCONTENT_DG10           = ID_DGCONTENT + b"\x0A"
+ID_DGCONTENT_DG11           = ID_DGCONTENT + b"\x0B"
+ID_DGCONTENT_DG12           = ID_DGCONTENT + b"\x0C"
+ID_DGCONTENT_DG13           = ID_DGCONTENT + b"\x0D"
+ID_DGCONTENT_DG14           = ID_DGCONTENT + b"\x0E"
+ID_DGCONTENT_DG15           = ID_DGCONTENT + b"\x0F"
+ID_DGCONTENT_DG16           = ID_DGCONTENT + b"\x10"
+ID_DGCONTENT_DG17           = ID_DGCONTENT + b"\x11"
+ID_DGCONTENT_DG18           = ID_DGCONTENT + b"\x12"
+ID_DGCONTENT_DG19           = ID_DGCONTENT + b"\x13"
+ID_DGCONTENT_DG20           = ID_DGCONTENT + b"\x14"
+ID_DGCONTENT_DG21           = ID_DGCONTENT + b"\x15"
+ID_DGCONTENT_DG22           = ID_DGCONTENT + b"\x16"
+
+ID_SECURITY_OBJECT          = BSI_DE + b"\x03\x02\x01"
+
+schemes = [
+    ('ECDSA_SHA_1', ID_TA_ECDSA_SHA_1),
+    ('ECDSA_SHA_224', ID_TA_ECDSA_SHA_224),
+    ('ECDSA_SHA_256', ID_TA_ECDSA_SHA_256),
+    ('ECDSA_SHA_384', ID_TA_ECDSA_SHA_384),
+    ('ECDSA_SHA_512', ID_TA_ECDSA_SHA_512),
+    ('RSA_v1_5_SHA_1', ID_TA_RSA_V1_5_SHA_1),
+    ('RSA_v1_5_SHA_256', ID_TA_RSA_V1_5_SHA_256),
+    ('RSA_v1_5_SHA_512', ID_TA_RSA_V1_5_SHA_512),
+    ('RSA_PSS_SHA_1', ID_TA_RSA_PSS_SHA_1),
+    ('RSA_PSS_SHA_256', ID_TA_RSA_PSS_SHA_256),
+    ('RSA_PSS_SHA_512', ID_TA_RSA_PSS_SHA_512),
+    ]
+
+def scheme2oid(scheme):
+    for s,o in schemes:
+        if (s == scheme):
+            return o
+    return None
+
+def oid2scheme(oid):
+    for s,o in schemes:
+        if (o == oid):
+            return s
+    return None
```

## cvc/terminal.py

 * *Ordering differences only*

```diff
@@ -1,66 +1,66 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-from cvc.utils import to_bytes
-from cvc import oid
-
-class Type:
-    CVCA = 3
-    DV_domestic = 2
-    DV_foreign = 1
-    Terminal = 0
-
-    def __init__(self, role):
-        self.role = role
-
-    def to_bytes(self):
-        x = 0
-        total = len(self._args)
-        for ix, attr in enumerate(self._args):
-            x = x + 2**(total-ix-1) * getattr(self, attr, 0)
-        x = x + self.role * 2**(total)
-        return x.to_bytes((total + 7) // 8, 'big')
-
-class TypeIS(Type):
-    OID = oid.ID_IS
-    name = 'TypeIS'
-    _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'iris', 'finger')
-    def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
-
-class TypeAT(Type):
-    OID = oid.ID_AT
-    name = 'TypeAT'
-    _args = ('write_dg17', 'write_dg18', 'write_dg19', 'write_dg20', 'write_dg21', 'write_dg22', 'rfu31', 'psa', 'read_dg22', 'read_dg21', 'read_dg20', 'read_dg19', 'read_dg18', 'read_dg17', 'read_dg16', 'read_dg15', 'read_dg14', 'read_dg13', 'read_dg12', 'read_dg11', 'read_dg10', 'read_dg9', 'read_dg8', 'read_dg7', 'read_dg6', 'read_dg5', 'read_dg4', 'read_dg3', 'read_dg2', 'read_dg1', 'install_qual_cert', 'install_cert', 'pin_management', 'can_allowed', 'privileged', 'rid', 'verify_community', 'verify_age')
-    def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
-
-class TypeST(Type):
-    OID = oid.ID_ST
-    name = 'TypeST'
-    _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'gen_qualified', 'gen_sig')
-    def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+from cvc.utils import to_bytes
+from cvc import oid
+
+class Type:
+    CVCA = 3
+    DV_domestic = 2
+    DV_foreign = 1
+    Terminal = 0
+
+    def __init__(self, role):
+        self.role = role
+
+    def to_bytes(self):
+        x = 0
+        total = len(self._args)
+        for ix, attr in enumerate(self._args):
+            x = x + 2**(total-ix-1) * getattr(self, attr, 0)
+        x = x + self.role * 2**(total)
+        return x.to_bytes((total + 7) // 8, 'big')
+
+class TypeIS(Type):
+    OID = oid.ID_IS
+    name = 'TypeIS'
+    _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'iris', 'finger')
+    def __init__(self, role, **kwargs):
+        for attr in self._args:
+            setattr(self, attr, kwargs.get(attr, 0))
+        super().__init__(role)
+
+class TypeAT(Type):
+    OID = oid.ID_AT
+    name = 'TypeAT'
+    _args = ('write_dg17', 'write_dg18', 'write_dg19', 'write_dg20', 'write_dg21', 'write_dg22', 'rfu31', 'psa', 'read_dg22', 'read_dg21', 'read_dg20', 'read_dg19', 'read_dg18', 'read_dg17', 'read_dg16', 'read_dg15', 'read_dg14', 'read_dg13', 'read_dg12', 'read_dg11', 'read_dg10', 'read_dg9', 'read_dg8', 'read_dg7', 'read_dg6', 'read_dg5', 'read_dg4', 'read_dg3', 'read_dg2', 'read_dg1', 'install_qual_cert', 'install_cert', 'pin_management', 'can_allowed', 'privileged', 'rid', 'verify_community', 'verify_age')
+    def __init__(self, role, **kwargs):
+        for attr in self._args:
+            setattr(self, attr, kwargs.get(attr, 0))
+        super().__init__(role)
+
+class TypeST(Type):
+    OID = oid.ID_ST
+    name = 'TypeST'
+    _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'gen_qualified', 'gen_sig')
+    def __init__(self, role, **kwargs):
+        for attr in self._args:
+            setattr(self, attr, kwargs.get(attr, 0))
+        super().__init__(role)
```

## cvc/utils.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-from cvc import oid
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import padding
-
-def to_bytes(n):
-    if (n == 0):
-        return bytearray([0])
-    if (isinstance(n, int)):
-        return bytearray(n.to_bytes((n.bit_length() + 7) // 8, 'big'))
-    return n #Assume is already
-
-def bcd(s):
-    return bytearray([int(c) for c in s])
-
-def scheme_rsa(o):
-    return (o == oid.ID_TA_RSA_V1_5_SHA_1 or o == oid.ID_TA_RSA_V1_5_SHA_256 or o == oid.ID_TA_RSA_V1_5_SHA_512 or o == oid.ID_TA_RSA_PSS_SHA_1 or o == oid.ID_TA_RSA_PSS_SHA_256 or o == oid.ID_TA_RSA_PSS_SHA_512)
-
-def scheme_ecdsa(o):
-    return (o == oid.ID_TA_ECDSA_SHA_1 or o == oid.ID_TA_ECDSA_SHA_224 or o == oid.ID_TA_ECDSA_SHA_256 or o == oid.ID_TA_ECDSA_SHA_384 or o == oid.ID_TA_ECDSA_SHA_512)
-
-def from_bcd(c):
-    return ''.join([str(s) for s in c])
-
-def get_hash_padding(scheme):
-    h,p = (None,None)
-    if (scheme == oid.ID_TA_ECDSA_SHA_1 or scheme == oid.ID_TA_RSA_PSS_SHA_1 or scheme == oid.ID_TA_RSA_V1_5_SHA_1):
-        h = hashes.SHA1()
-    elif (scheme == oid.ID_TA_ECDSA_SHA_224):
-        h = hashes.SHA224()
-    elif (scheme == oid.ID_TA_ECDSA_SHA_256 or scheme == oid.ID_TA_RSA_PSS_SHA_256 or scheme == oid.ID_TA_RSA_V1_5_SHA_256):
-        h = hashes.SHA256()
-    elif (scheme == oid.ID_TA_ECDSA_SHA_384):
-        h = hashes.SHA384()
-    elif (scheme == oid.ID_TA_ECDSA_SHA_512 or scheme == oid.ID_TA_RSA_PSS_SHA_512 or scheme == oid.ID_TA_RSA_V1_5_SHA_512):
-        h = hashes.SHA512()
-
-    if (scheme == oid.ID_TA_RSA_V1_5_SHA_1 or scheme == oid.ID_TA_RSA_V1_5_SHA_256 or scheme == oid.ID_TA_RSA_V1_5_SHA_512):
-        p = padding.PKCS1v15()
-    elif (scheme == oid.ID_TA_RSA_PSS_SHA_1 or scheme == oid.ID_TA_RSA_PSS_SHA_256 or scheme == oid.ID_TA_RSA_PSS_SHA_512):
-        p = padding.PSS(mgf=padding.MGF1(h), salt_length=padding.PSS.MAX_LENGTH)
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+from cvc import oid
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.asymmetric import padding
+
+def to_bytes(n):
+    if (n == 0):
+        return bytearray([0])
+    if (isinstance(n, int)):
+        return bytearray(n.to_bytes((n.bit_length() + 7) // 8, 'big'))
+    return n #Assume is already
+
+def bcd(s):
+    return bytearray([int(c) for c in s])
+
+def scheme_rsa(o):
+    return (o == oid.ID_TA_RSA_V1_5_SHA_1 or o == oid.ID_TA_RSA_V1_5_SHA_256 or o == oid.ID_TA_RSA_V1_5_SHA_512 or o == oid.ID_TA_RSA_PSS_SHA_1 or o == oid.ID_TA_RSA_PSS_SHA_256 or o == oid.ID_TA_RSA_PSS_SHA_512)
+
+def scheme_ecdsa(o):
+    return (o == oid.ID_TA_ECDSA_SHA_1 or o == oid.ID_TA_ECDSA_SHA_224 or o == oid.ID_TA_ECDSA_SHA_256 or o == oid.ID_TA_ECDSA_SHA_384 or o == oid.ID_TA_ECDSA_SHA_512)
+
+def from_bcd(c):
+    return ''.join([str(s) for s in c])
+
+def get_hash_padding(scheme):
+    h,p = (None,None)
+    if (scheme == oid.ID_TA_ECDSA_SHA_1 or scheme == oid.ID_TA_RSA_PSS_SHA_1 or scheme == oid.ID_TA_RSA_V1_5_SHA_1):
+        h = hashes.SHA1()
+    elif (scheme == oid.ID_TA_ECDSA_SHA_224):
+        h = hashes.SHA224()
+    elif (scheme == oid.ID_TA_ECDSA_SHA_256 or scheme == oid.ID_TA_RSA_PSS_SHA_256 or scheme == oid.ID_TA_RSA_V1_5_SHA_256):
+        h = hashes.SHA256()
+    elif (scheme == oid.ID_TA_ECDSA_SHA_384):
+        h = hashes.SHA384()
+    elif (scheme == oid.ID_TA_ECDSA_SHA_512 or scheme == oid.ID_TA_RSA_PSS_SHA_512 or scheme == oid.ID_TA_RSA_V1_5_SHA_512):
+        h = hashes.SHA512()
+
+    if (scheme == oid.ID_TA_RSA_V1_5_SHA_1 or scheme == oid.ID_TA_RSA_V1_5_SHA_256 or scheme == oid.ID_TA_RSA_V1_5_SHA_512):
+        p = padding.PKCS1v15()
+    elif (scheme == oid.ID_TA_RSA_PSS_SHA_1 or scheme == oid.ID_TA_RSA_PSS_SHA_256 or scheme == oid.ID_TA_RSA_PSS_SHA_512):
+        p = padding.PSS(mgf=padding.MGF1(h), salt_length=padding.PSS.MAX_LENGTH)
     return h,p
```

## cvc/tools/cvc_create.py

 * *Ordering differences only*

```diff
@@ -1,236 +1,236 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-import argparse, logging, sys
-from cryptography.hazmat.primitives.asymmetric import ec, rsa
-from cryptography.hazmat.primitives import serialization
-from cvc.terminal import Type, TypeIS, TypeAT, TypeST
-from cvc.certificates import CVC
-from cvc.utils import scheme_rsa
-from cvc import __version__, oid
-
-logger = logging.getLogger(__name__)
-
-def parse_args():
-    parser = argparse.ArgumentParser(description='Generate a Card Verifiable Certificate')
-    parser.add_argument('--version', help='Displays the current version', action='store_true')
-    parser.add_argument('-o','--out-cert', help='Generated certificate file', metavar='FILENAME')
-    parser.add_argument('-r','--role', help='The role of entity', choices=['cvca','dv_domestic','dv_foreign','terminal'])
-    parser.add_argument('-t','--type', help='The type of terminal. If not provided, it creates a certificate request', choices=['at','is','st'])
-    parser.add_argument('--valid', help='Days of validity since today or date provided by --since', default=90)
-    parser.add_argument('-k','--sign-key', help='Private key to sign the certificate.', required=True, metavar='FILENAME')
-    parser.add_argument('--sign-as', help='CV certificate of signing entity. If not provided, the certificate is self-signed [generates a certificate]', metavar='FILENAME')
-    parser.add_argument('--outer-as', help='Outer certificate for CV request', metavar='FILENAME')
-    parser.add_argument('--outer-key', help='Private key for outer signature of CV request', metavar='FILENAME')
-    parser.add_argument('-p','--public-key', help='The public key contained in the certificate. If not provided, it is derived from the sign-key', metavar='FILENAME')
-    parser.add_argument('-q','--request', help='Generates a certificate based on a request', metavar='FILENAME')
-    parser.add_argument('--out-key', help='File to store the generated private key [default CHR.pkcs8]', metavar='FILENAME')
-    parser.add_argument('-s','--scheme', help='Signature scheme', choices=["ECDSA_SHA_1",
-                               "ECDSA_SHA_224", "ECDSA_SHA_256",
-                               "ECDSA_SHA_384", "ECDSA_SHA_512",
-                               "RSA_v1_5_SHA_1", "RSA_v1_5_SHA_256",
-                               "RSA_v1_5_SHA_512", "RSA_PSS_SHA_1",
-                               "RSA_PSS_SHA_256", "RSA_PSS_SHA_512"])
-    parser.add_argument('-c','--chr', help='Certificate Holder Reference')
-    parser.add_argument('-a','--req-car', help='Certificate Authority Reference expected for CV request [generates a request]')
-    parser.add_argument('--write-dg17', help='Allow writing DG 17 (Normal Place of Residence)', action='store_true')
-    parser.add_argument('--write-dg18', help='Allow writing DG 18 (Community ID)', action='store_true')
-    parser.add_argument('--write-dg19', help='Allow writing DG 19 (Residence Permit I)', action='store_true')
-    parser.add_argument('--write-dg20', help='Allow writing DG 20 (Residence Permit II)', action='store_true')
-    parser.add_argument('--write-dg21', help='Allow writing DG 21 (Optional Data)', action='store_true')
-    parser.add_argument('--write-dg22', help='Allow writing DG 22 (Email address)', action='store_true')
-    parser.add_argument('--rfu31', help='Allow RFU R/W Access bit 31', action='store_true')
-    parser.add_argument('--psa', help='Allow PSA', action='store_true')
-    parser.add_argument('--read-dg1', help='Allow reading DG 1   (Document Type)', action='store_true')
-    parser.add_argument('--read-dg2', help='Allow reading DG 2   (Issuing State)', action='store_true')
-    parser.add_argument('--read-dg3', help='Allow reading DG 3   (Date of Expiry)', action='store_true')
-    parser.add_argument('--read-dg4', help='Allow reading DG 4   (Given Names)', action='store_true')
-    parser.add_argument('--read-dg5', help='Allow reading DG 5   (Family Names)', action='store_true')
-    parser.add_argument('--read-dg6', help='Allow reading DG 6   (Religious/Artistic Name)', action='store_true')
-    parser.add_argument('--read-dg7', help='Allow reading DG 7   (Academic Title)', action='store_true')
-    parser.add_argument('--read-dg8', help='Allow reading DG 8   (Date of Birth)', action='store_true')
-    parser.add_argument('--read-dg9', help='Allow reading DG 9   (Place of Birth)', action='store_true')
-    parser.add_argument('--read-dg10', help='Allow reading DG 10  (Nationality)', action='store_true')
-    parser.add_argument('--read-dg11', help='Allow reading DG 11  (Sex)', action='store_true')
-    parser.add_argument('--read-dg12', help='Allow reading DG 12  (Optional Data)', action='store_true')
-    parser.add_argument('--read-dg13', help='Allow reading DG 13  (Birth Name)', action='store_true')
-    parser.add_argument('--read-dg14', help='Allow reading DG 14  (Written Signature)', action='store_true')
-    parser.add_argument('--read-dg15', help='Allow reading DG 15  (Date of Issuance)', action='store_true')
-    parser.add_argument('--read-dg16', help='Allow reading DG 16', action='store_true')
-    parser.add_argument('--read-dg17', help='Allow reading DG 17  (Normal Place of Residence)', action='store_true')
-    parser.add_argument('--read-dg18', help='Allow reading DG 18  (Community ID)', action='store_true')
-    parser.add_argument('--read-dg19', help='Allow reading DG 19  (Residence Permit I)', action='store_true')
-    parser.add_argument('--read-dg20', help='Allow reading DG 20  (Residence Permit II)', action='store_true')
-    parser.add_argument('--read-dg21', help='Allow reading DG 21  (Phone Number)', action='store_true')
-    parser.add_argument('--read-dg22', help='Allow reading DG 22  (Email Address)', action='store_true')
-    parser.add_argument('--install-qual-cert', help='Allow installing qualified certificate', action='store_true')
-    parser.add_argument('--install-cert', help='Allow installing certificate', action='store_true')
-    parser.add_argument('--pin-management ', help='Allow PIN management', action='store_true')
-    parser.add_argument('--can-allowed', help='CAN allowed', action='store_true')
-    parser.add_argument('--privileged ', help='Privileged terminal', action='store_true')
-    parser.add_argument('--rid', help='Allow restricted identification', action='store_true')
-    parser.add_argument('--verify-community', help='Allow community ID verification', action='store_true')
-    parser.add_argument('--verify-age', help='Allow age verification', action='store_true')
-
-    parser.add_argument('--rfu5', help='Allow RFU bit 5', action='store_true')
-    parser.add_argument('--rfu4', help='Allow RFU bit 4', action='store_true')
-    parser.add_argument('--rfu3', help='Allow RFU bit 3', action='store_true')
-    parser.add_argument('--rfu2', help='Allow RFU bit 2', action='store_true')
-    parser.add_argument('--gen-qual-sig', help='Allow generated qualified electronic signature', action='store_true')
-    parser.add_argument('--gen-sig', help='Allow generated electronic signature', action='store_true')
-
-    parser.add_argument('--read-iris', help='Read access to ePassport application: DG 4 (Iris)', action='store_true')
-    parser.add_argument('--read-finger', help='Read access to ePassport application: DG 3 (Fingerprint)', action='store_true')
-
-    if ('--version' in sys.argv):
-        print('Card Verifiable Certificate tools for Python')
-        print('Author: Pol Henarejos')
-        print(f'Version {__version__}')
-        print('')
-        print('Report bugs to http://github.com/polhenarejos/pycvc/issues')
-        print('')
-        sys.exit(0)
-
-    args = parser.parse_args()
-    return args
-
-def load_private_key(filename):
-    with open(filename, 'rb') as f:
-        p8data = f.read()
-        try:
-            return serialization.load_der_private_key(p8data,password=None)
-        except ValueError:
-            return serialization.load_pem_private_key(p8data,password=None)
-    return None
-
-def get_role(r):
-    if (r == 'cvca'):
-        return Type.CVCA
-    elif (r== 'dv_domestic'):
-        return Type.DV_domestic
-    elif (r == 'dv_foreign'):
-        return Type.dv_foreign
-    elif (r == 'terminal'):
-        return Type.Terminal
-    return None
-
-def get_type(t, role, args):
-    if (t == 'at'):
-        typ = TypeAT(role)
-    elif (t == 'st'):
-        typ = TypeST(role)
-    elif (t == 'is'):
-        typ = TypeIS(role)
-    else:
-        return None
-
-    for attr in typ._args:
-        setattr(typ, attr, getattr(args, attr, 0))
-
-    return typ
-
-def parse_as(a):
-    with open(a, 'rb') as f:
-        cadata = f.read()
-        chr = CVC().decode(cadata).chr()
-        scheme = CVC().decode(cadata).pubkey().oid()
-        return chr,scheme
-    return None
-
-def main(args):
-    sign_key = load_private_key(args.sign_key)
-    puboid = None
-    chr = None
-    if (args.public_key):
-        with open(args.public_key, 'rb') as f:
-            pubdata = f.read()
-            try:
-                pub_key = serialization.load_der_public_key(pubdata)
-            except ValueError:
-                pub_key = serialization.load_pem_public_key(pubdata)
-    elif (args.request):
-        with open(args.request, 'rb') as f:
-            data = f.read()
-            puboid = CVC().decode(data).pubkey().oid()
-            chr = CVC().decode(data).chr()
-            if (scheme_rsa(puboid)):
-                pub_key = rsa.RSAPublicNumbers(int.from_bytes(CVC().decode(data).pubkey().find(0x82).data(), 'big'), int.from_bytes(CVC().decode(data).pubkey().find(0x81).data(), 'big')).public_key()
-            else:
-                curve = CVC().decode(data).find_domain()
-                Q = CVC().decode(data).pubkey().find(0x86).data()
-                pub_key = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
-    else:
-        if (args.sign_as and args.type and not args.outer_as and not args.outer_key):
-            if (isinstance(sign_key, rsa.RSAPrivateKey)):
-                priv_key = rsa.generate_private_key(key_size=sign_key.key_size, public_exponent=65537)
-            elif (isinstance(sign_key, ec.EllipticCurvePrivateKey)):
-                priv_key = ec.generate_private_key(sign_key.curve)
-            pub_key = priv_key.public_key()
-            with open(args.out_key if args.out_key != None else args.chr+'.pkcs8','wb') as f:
-                der = priv_key.private_bytes(encoding=serialization.Encoding.DER, format=serialization.PrivateFormat.PKCS8, encryption_algorithm=serialization.NoEncryption())
-                f.write(der)
-        else:
-            pub_key = sign_key.public_key()
-
-    role = get_role(args.role)
-
-    typ = get_type(args.type, role, args)
-
-    if (not puboid):
-        puboid = oid.scheme2oid(args.scheme)
-    if (not puboid):
-        if (isinstance(pub_key, rsa.RSAPublicKey)):
-            puboid = oid.ID_TA_RSA_PSS_SHA256
-        elif (isinstance(pub_key, ec.EllipticCurvePublicKey)):
-            puboid = oid.ID_TA_ECDSA_SHA_256
-
-    if (args.sign_as and typ and not args.outer_as and not args.outer_key): # Cert
-        car, signscheme = parse_as(args.sign_as)
-    else: # Req
-        if (args.req_car):
-            car = args.req_car.encode()
-        else:
-            car = args.chr.encode()
-        signscheme = puboid
-
-    if (not chr):
-        chr = args.chr.encode()
-    if (args.req_car or (args.outer_as and args.outer_key)):
-        if (args.outer_as and args.outer_key):
-            outercar, outerscheme = parse_as(args.outer_as)
-            outerkey = load_private_key(args.outer_key)
-        else:
-            outercar,outerscheme,outerkey = None,None,None
-        cert = CVC().req(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, outercar=outercar, outerkey=outerkey, outerscheme=outerscheme)
-        ext = 'cvreq'
-    else:
-        cert = CVC().cert(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, role=typ, valid=args.valid if typ else None)
-        ext = 'cvcert'
-
-    with open(args.out_cert if args.out_cert != None else chr.decode()+'.'+ext,'wb') as f:
-        f.write(cert.encode())
-
-def run():
-    args = parse_args()
-    main(args)
-
-if __name__ == "__main__":
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+import argparse, logging, sys
+from cryptography.hazmat.primitives.asymmetric import ec, rsa
+from cryptography.hazmat.primitives import serialization
+from cvc.terminal import Type, TypeIS, TypeAT, TypeST
+from cvc.certificates import CVC
+from cvc.utils import scheme_rsa
+from cvc import __version__, oid
+
+logger = logging.getLogger(__name__)
+
+def parse_args():
+    parser = argparse.ArgumentParser(description='Generate a Card Verifiable Certificate')
+    parser.add_argument('--version', help='Displays the current version', action='store_true')
+    parser.add_argument('-o','--out-cert', help='Generated certificate file', metavar='FILENAME')
+    parser.add_argument('-r','--role', help='The role of entity', choices=['cvca','dv_domestic','dv_foreign','terminal'])
+    parser.add_argument('-t','--type', help='The type of terminal. If not provided, it creates a certificate request', choices=['at','is','st'])
+    parser.add_argument('--valid', help='Days of validity since today or date provided by --since', default=90)
+    parser.add_argument('-k','--sign-key', help='Private key to sign the certificate.', required=True, metavar='FILENAME')
+    parser.add_argument('--sign-as', help='CV certificate of signing entity. If not provided, the certificate is self-signed [generates a certificate]', metavar='FILENAME')
+    parser.add_argument('--outer-as', help='Outer certificate for CV request', metavar='FILENAME')
+    parser.add_argument('--outer-key', help='Private key for outer signature of CV request', metavar='FILENAME')
+    parser.add_argument('-p','--public-key', help='The public key contained in the certificate. If not provided, it is derived from the sign-key', metavar='FILENAME')
+    parser.add_argument('-q','--request', help='Generates a certificate based on a request', metavar='FILENAME')
+    parser.add_argument('--out-key', help='File to store the generated private key [default CHR.pkcs8]', metavar='FILENAME')
+    parser.add_argument('-s','--scheme', help='Signature scheme', choices=["ECDSA_SHA_1",
+                               "ECDSA_SHA_224", "ECDSA_SHA_256",
+                               "ECDSA_SHA_384", "ECDSA_SHA_512",
+                               "RSA_v1_5_SHA_1", "RSA_v1_5_SHA_256",
+                               "RSA_v1_5_SHA_512", "RSA_PSS_SHA_1",
+                               "RSA_PSS_SHA_256", "RSA_PSS_SHA_512"])
+    parser.add_argument('-c','--chr', help='Certificate Holder Reference')
+    parser.add_argument('-a','--req-car', help='Certificate Authority Reference expected for CV request [generates a request]')
+    parser.add_argument('--write-dg17', help='Allow writing DG 17 (Normal Place of Residence)', action='store_true')
+    parser.add_argument('--write-dg18', help='Allow writing DG 18 (Community ID)', action='store_true')
+    parser.add_argument('--write-dg19', help='Allow writing DG 19 (Residence Permit I)', action='store_true')
+    parser.add_argument('--write-dg20', help='Allow writing DG 20 (Residence Permit II)', action='store_true')
+    parser.add_argument('--write-dg21', help='Allow writing DG 21 (Optional Data)', action='store_true')
+    parser.add_argument('--write-dg22', help='Allow writing DG 22 (Email address)', action='store_true')
+    parser.add_argument('--rfu31', help='Allow RFU R/W Access bit 31', action='store_true')
+    parser.add_argument('--psa', help='Allow PSA', action='store_true')
+    parser.add_argument('--read-dg1', help='Allow reading DG 1   (Document Type)', action='store_true')
+    parser.add_argument('--read-dg2', help='Allow reading DG 2   (Issuing State)', action='store_true')
+    parser.add_argument('--read-dg3', help='Allow reading DG 3   (Date of Expiry)', action='store_true')
+    parser.add_argument('--read-dg4', help='Allow reading DG 4   (Given Names)', action='store_true')
+    parser.add_argument('--read-dg5', help='Allow reading DG 5   (Family Names)', action='store_true')
+    parser.add_argument('--read-dg6', help='Allow reading DG 6   (Religious/Artistic Name)', action='store_true')
+    parser.add_argument('--read-dg7', help='Allow reading DG 7   (Academic Title)', action='store_true')
+    parser.add_argument('--read-dg8', help='Allow reading DG 8   (Date of Birth)', action='store_true')
+    parser.add_argument('--read-dg9', help='Allow reading DG 9   (Place of Birth)', action='store_true')
+    parser.add_argument('--read-dg10', help='Allow reading DG 10  (Nationality)', action='store_true')
+    parser.add_argument('--read-dg11', help='Allow reading DG 11  (Sex)', action='store_true')
+    parser.add_argument('--read-dg12', help='Allow reading DG 12  (Optional Data)', action='store_true')
+    parser.add_argument('--read-dg13', help='Allow reading DG 13  (Birth Name)', action='store_true')
+    parser.add_argument('--read-dg14', help='Allow reading DG 14  (Written Signature)', action='store_true')
+    parser.add_argument('--read-dg15', help='Allow reading DG 15  (Date of Issuance)', action='store_true')
+    parser.add_argument('--read-dg16', help='Allow reading DG 16', action='store_true')
+    parser.add_argument('--read-dg17', help='Allow reading DG 17  (Normal Place of Residence)', action='store_true')
+    parser.add_argument('--read-dg18', help='Allow reading DG 18  (Community ID)', action='store_true')
+    parser.add_argument('--read-dg19', help='Allow reading DG 19  (Residence Permit I)', action='store_true')
+    parser.add_argument('--read-dg20', help='Allow reading DG 20  (Residence Permit II)', action='store_true')
+    parser.add_argument('--read-dg21', help='Allow reading DG 21  (Phone Number)', action='store_true')
+    parser.add_argument('--read-dg22', help='Allow reading DG 22  (Email Address)', action='store_true')
+    parser.add_argument('--install-qual-cert', help='Allow installing qualified certificate', action='store_true')
+    parser.add_argument('--install-cert', help='Allow installing certificate', action='store_true')
+    parser.add_argument('--pin-management ', help='Allow PIN management', action='store_true')
+    parser.add_argument('--can-allowed', help='CAN allowed', action='store_true')
+    parser.add_argument('--privileged ', help='Privileged terminal', action='store_true')
+    parser.add_argument('--rid', help='Allow restricted identification', action='store_true')
+    parser.add_argument('--verify-community', help='Allow community ID verification', action='store_true')
+    parser.add_argument('--verify-age', help='Allow age verification', action='store_true')
+
+    parser.add_argument('--rfu5', help='Allow RFU bit 5', action='store_true')
+    parser.add_argument('--rfu4', help='Allow RFU bit 4', action='store_true')
+    parser.add_argument('--rfu3', help='Allow RFU bit 3', action='store_true')
+    parser.add_argument('--rfu2', help='Allow RFU bit 2', action='store_true')
+    parser.add_argument('--gen-qual-sig', help='Allow generated qualified electronic signature', action='store_true')
+    parser.add_argument('--gen-sig', help='Allow generated electronic signature', action='store_true')
+
+    parser.add_argument('--read-iris', help='Read access to ePassport application: DG 4 (Iris)', action='store_true')
+    parser.add_argument('--read-finger', help='Read access to ePassport application: DG 3 (Fingerprint)', action='store_true')
+
+    if ('--version' in sys.argv):
+        print('Card Verifiable Certificate tools for Python')
+        print('Author: Pol Henarejos')
+        print(f'Version {__version__}')
+        print('')
+        print('Report bugs to http://github.com/polhenarejos/pycvc/issues')
+        print('')
+        sys.exit(0)
+
+    args = parser.parse_args()
+    return args
+
+def load_private_key(filename):
+    with open(filename, 'rb') as f:
+        p8data = f.read()
+        try:
+            return serialization.load_der_private_key(p8data,password=None)
+        except ValueError:
+            return serialization.load_pem_private_key(p8data,password=None)
+    return None
+
+def get_role(r):
+    if (r == 'cvca'):
+        return Type.CVCA
+    elif (r== 'dv_domestic'):
+        return Type.DV_domestic
+    elif (r == 'dv_foreign'):
+        return Type.dv_foreign
+    elif (r == 'terminal'):
+        return Type.Terminal
+    return None
+
+def get_type(t, role, args):
+    if (t == 'at'):
+        typ = TypeAT(role)
+    elif (t == 'st'):
+        typ = TypeST(role)
+    elif (t == 'is'):
+        typ = TypeIS(role)
+    else:
+        return None
+
+    for attr in typ._args:
+        setattr(typ, attr, getattr(args, attr, 0))
+
+    return typ
+
+def parse_as(a):
+    with open(a, 'rb') as f:
+        cadata = f.read()
+        chr = CVC().decode(cadata).chr()
+        scheme = CVC().decode(cadata).pubkey().oid()
+        return chr,scheme
+    return None
+
+def main(args):
+    sign_key = load_private_key(args.sign_key)
+    puboid = None
+    chr = None
+    if (args.public_key):
+        with open(args.public_key, 'rb') as f:
+            pubdata = f.read()
+            try:
+                pub_key = serialization.load_der_public_key(pubdata)
+            except ValueError:
+                pub_key = serialization.load_pem_public_key(pubdata)
+    elif (args.request):
+        with open(args.request, 'rb') as f:
+            data = f.read()
+            puboid = CVC().decode(data).pubkey().oid()
+            chr = CVC().decode(data).chr()
+            if (scheme_rsa(puboid)):
+                pub_key = rsa.RSAPublicNumbers(int.from_bytes(CVC().decode(data).pubkey().find(0x82).data(), 'big'), int.from_bytes(CVC().decode(data).pubkey().find(0x81).data(), 'big')).public_key()
+            else:
+                curve = CVC().decode(data).find_domain()
+                Q = CVC().decode(data).pubkey().find(0x86).data()
+                pub_key = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
+    else:
+        if (args.sign_as and args.type and not args.outer_as and not args.outer_key):
+            if (isinstance(sign_key, rsa.RSAPrivateKey)):
+                priv_key = rsa.generate_private_key(key_size=sign_key.key_size, public_exponent=65537)
+            elif (isinstance(sign_key, ec.EllipticCurvePrivateKey)):
+                priv_key = ec.generate_private_key(sign_key.curve)
+            pub_key = priv_key.public_key()
+            with open(args.out_key if args.out_key != None else args.chr+'.pkcs8','wb') as f:
+                der = priv_key.private_bytes(encoding=serialization.Encoding.DER, format=serialization.PrivateFormat.PKCS8, encryption_algorithm=serialization.NoEncryption())
+                f.write(der)
+        else:
+            pub_key = sign_key.public_key()
+
+    role = get_role(args.role)
+
+    typ = get_type(args.type, role, args)
+
+    if (not puboid):
+        puboid = oid.scheme2oid(args.scheme)
+    if (not puboid):
+        if (isinstance(pub_key, rsa.RSAPublicKey)):
+            puboid = oid.ID_TA_RSA_PSS_SHA256
+        elif (isinstance(pub_key, ec.EllipticCurvePublicKey)):
+            puboid = oid.ID_TA_ECDSA_SHA_256
+
+    if (args.sign_as and typ and not args.outer_as and not args.outer_key): # Cert
+        car, signscheme = parse_as(args.sign_as)
+    else: # Req
+        if (args.req_car):
+            car = args.req_car.encode()
+        else:
+            car = args.chr.encode()
+        signscheme = puboid
+
+    if (not chr):
+        chr = args.chr.encode()
+    if (args.req_car or (args.outer_as and args.outer_key)):
+        if (args.outer_as and args.outer_key):
+            outercar, outerscheme = parse_as(args.outer_as)
+            outerkey = load_private_key(args.outer_key)
+        else:
+            outercar,outerscheme,outerkey = None,None,None
+        cert = CVC().req(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, outercar=outercar, outerkey=outerkey, outerscheme=outerscheme)
+        ext = 'cvreq'
+    else:
+        cert = CVC().cert(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, role=typ, valid=args.valid if typ else None)
+        ext = 'cvcert'
+
+    with open(args.out_cert if args.out_cert != None else chr.decode()+'.'+ext,'wb') as f:
+        f.write(cert.encode())
+
+def run():
+    args = parse_args()
+    main(args)
+
+if __name__ == "__main__":
     run()
```

## cvc/tools/cvc_print.py

 * *Ordering differences only*

```diff
@@ -1,128 +1,128 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-/*
- * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
- * Copyright (c) 2022 Pol Henarejos.
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, version 3.
- *
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
- * General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program. If not, see <http://www.gnu.org/licenses/>.
- */
-"""
-
-import argparse, logging, sys
-from cvc.certificates import CVC
-from binascii import hexlify
-from cvc.utils import scheme_rsa
-from cvc.oid import oid2scheme
-from cvc import __version__, oid
-from datetime import date
-import os
-
-logger = logging.getLogger(__name__)
-cert_dir = b''
-
-def parse_args():
-    global cert_dir
-    parser = argparse.ArgumentParser(description='Prints a Card Verifiable Certificate')
-    parser.add_argument('--version', help='Displays the current version', action='store_true')
-    parser.add_argument('file',help='Certificate to print', metavar='FILENAME')
-    parser.add_argument('-d','--directory', help='Directory where chain CV certificates are located', metavar='DIRECTORY')
-    if ('--version' in sys.argv):
-        print('Card Verifiable Certificate tools for Python')
-        print('Author: Pol Henarejos')
-        print(f'Version {__version__}')
-        print('')
-        print('Report bugs to http://github.com/polhenarejos/pycvc/issues')
-        print('')
-        sys.exit(0)
-    args = parser.parse_args()
-    if (args.directory):
-        cert_dir = args.directory.encode()
-    return args
-
-def bcd2date(v):
-    return date(v[0]*10+v[1]+2000, v[2]*10+v[3], v[4]*10+v[5])
-
-def main(args):
-    with open(args.file, 'rb') as f:
-        cdata = f.read()
-
-    print('Certificate:')
-    print(f'  Profile Identifier: {hexlify(CVC().decode(cdata).cpi()).decode()}')
-    print(f'  CAR: {(CVC().decode(cdata).car()).decode()}')
-    print('  Public Key:')
-    puboid = CVC().decode(cdata).pubkey().oid()
-    print(f'    Scheme: {oid2scheme(puboid)}')
-    chr = CVC().decode(cdata).chr()
-    car = CVC().decode(cdata).car()
-    if (scheme_rsa(puboid)):
-        print(f'    Modulus: {hexlify(CVC().decode(cdata).pubkey().find(0x81).data()).decode()}')
-        print(f'    Exponent: {hexlify(CVC().decode(cdata).pubkey().find(0x82).data()).decode()}')
-    else:
-        print(f'    Public Point: {hexlify(CVC().decode(cdata).pubkey().find(0x86).data()).decode()}')
-    print(f'  CHR: {chr.decode()}')
-    role = CVC().decode(cdata).role()
-    if (role):
-        print('  CHAT:')
-        o = role.oid()
-        if (o == oid.ID_IS):
-            print('    Role:  TypeIS')
-        elif (o == oid.ID_AT):
-            print('    Role:  TypeAT')
-        elif (o == oid.ID_ST):
-            print('    Role:  TypeST')
-        print(f'    Bytes: {hexlify(CVC().decode(cdata).role().find(0x53).data()).decode()}')
-        print(f'  Since:   {bcd2date(CVC().decode(cdata).valid()).strftime("%Y-%m-%d")}')
-        print(f'  Expires: {bcd2date(CVC().decode(cdata).expires()).strftime("%Y-%m-%d")}')
-    isreq = CVC().decode(cdata).is_req()
-    if (CVC().decode(cdata).verify(cert_dir=cert_dir, dica=cdata if isreq else None)):
-        print('Inner signature is VALID')
-        ret = True
-    else:
-        print('Inner signature is NOT VALID')
-        ret = False
-    if (car != chr):
-        if (isreq):
-            ret = CVC().decode(cdata).verify(cert_dir=cert_dir, dica=cdata)
-        else:
-            try:
-                while (car != chr):
-                    with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
-                        adata = f.read()
-                        ret = ret and CVC().decode(adata).verify(cert_dir=cert_dir)
-                        chr = CVC().decode(adata).chr()
-                        car = CVC().decode(adata).car()
-            except FileNotFoundError:
-                print(f'[Warning: File {car.decode()} not found]')
-                ret = False
-    else:
-        if (isreq):
-            print(f'Outer CAR: {CVC().decode(cdata).outer_car().decode()}')
-            outret = CVC().decode(cdata).verify(cert_dir=cert_dir, outer=True)
-            if (outret):
-                print('Outer signature is VALID')
-            else:
-                print('Outer signature is NOT VALID')
-            ret = ret and outret
-
-    if (ret):
-        print('Certificate VALID')
-    else:
-        print('Certificate NOT VALID')
-
-def run():
-    args = parse_args()
-    main(args)
-
-if __name__ == "__main__":
-    run()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+/*
+ * This file is part of the pyCVC distribution (https://github.com/polhenarejos/pycvc).
+ * Copyright (c) 2022 Pol Henarejos.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, version 3.
+ *
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program. If not, see <http://www.gnu.org/licenses/>.
+ */
+"""
+
+import argparse, logging, sys
+from cvc.certificates import CVC
+from binascii import hexlify
+from cvc.utils import scheme_rsa
+from cvc.oid import oid2scheme
+from cvc import __version__, oid
+from datetime import date
+import os
+
+logger = logging.getLogger(__name__)
+cert_dir = b''
+
+def parse_args():
+    global cert_dir
+    parser = argparse.ArgumentParser(description='Prints a Card Verifiable Certificate')
+    parser.add_argument('--version', help='Displays the current version', action='store_true')
+    parser.add_argument('file',help='Certificate to print', metavar='FILENAME')
+    parser.add_argument('-d','--directory', help='Directory where chain CV certificates are located', metavar='DIRECTORY')
+    if ('--version' in sys.argv):
+        print('Card Verifiable Certificate tools for Python')
+        print('Author: Pol Henarejos')
+        print(f'Version {__version__}')
+        print('')
+        print('Report bugs to http://github.com/polhenarejos/pycvc/issues')
+        print('')
+        sys.exit(0)
+    args = parser.parse_args()
+    if (args.directory):
+        cert_dir = args.directory.encode()
+    return args
+
+def bcd2date(v):
+    return date(v[0]*10+v[1]+2000, v[2]*10+v[3], v[4]*10+v[5])
+
+def main(args):
+    with open(args.file, 'rb') as f:
+        cdata = f.read()
+
+    print('Certificate:')
+    print(f'  Profile Identifier: {hexlify(CVC().decode(cdata).cpi()).decode()}')
+    print(f'  CAR: {(CVC().decode(cdata).car()).decode()}')
+    print('  Public Key:')
+    puboid = CVC().decode(cdata).pubkey().oid()
+    print(f'    Scheme: {oid2scheme(puboid)}')
+    chr = CVC().decode(cdata).chr()
+    car = CVC().decode(cdata).car()
+    if (scheme_rsa(puboid)):
+        print(f'    Modulus: {hexlify(CVC().decode(cdata).pubkey().find(0x81).data()).decode()}')
+        print(f'    Exponent: {hexlify(CVC().decode(cdata).pubkey().find(0x82).data()).decode()}')
+    else:
+        print(f'    Public Point: {hexlify(CVC().decode(cdata).pubkey().find(0x86).data()).decode()}')
+    print(f'  CHR: {chr.decode()}')
+    role = CVC().decode(cdata).role()
+    if (role):
+        print('  CHAT:')
+        o = role.oid()
+        if (o == oid.ID_IS):
+            print('    Role:  TypeIS')
+        elif (o == oid.ID_AT):
+            print('    Role:  TypeAT')
+        elif (o == oid.ID_ST):
+            print('    Role:  TypeST')
+        print(f'    Bytes: {hexlify(CVC().decode(cdata).role().find(0x53).data()).decode()}')
+        print(f'  Since:   {bcd2date(CVC().decode(cdata).valid()).strftime("%Y-%m-%d")}')
+        print(f'  Expires: {bcd2date(CVC().decode(cdata).expires()).strftime("%Y-%m-%d")}')
+    isreq = CVC().decode(cdata).is_req()
+    if (CVC().decode(cdata).verify(cert_dir=cert_dir, dica=cdata if isreq else None)):
+        print('Inner signature is VALID')
+        ret = True
+    else:
+        print('Inner signature is NOT VALID')
+        ret = False
+    if (car != chr):
+        if (isreq):
+            ret = CVC().decode(cdata).verify(cert_dir=cert_dir, dica=cdata)
+        else:
+            try:
+                while (car != chr):
+                    with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
+                        adata = f.read()
+                        ret = ret and CVC().decode(adata).verify(cert_dir=cert_dir)
+                        chr = CVC().decode(adata).chr()
+                        car = CVC().decode(adata).car()
+            except FileNotFoundError:
+                print(f'[Warning: File {car.decode()} not found]')
+                ret = False
+    else:
+        if (isreq):
+            print(f'Outer CAR: {CVC().decode(cdata).outer_car().decode()}')
+            outret = CVC().decode(cdata).verify(cert_dir=cert_dir, outer=True)
+            if (outret):
+                print('Outer signature is VALID')
+            else:
+                print('Outer signature is NOT VALID')
+            ret = ret and outret
+
+    if (ret):
+        print('Certificate VALID')
+    else:
+        print('Certificate NOT VALID')
+
+def run():
+    args = parse_args()
+    main(args)
+
+if __name__ == "__main__":
+    run()
```

## Comparing `pycvc-1.2.3.dist-info/METADATA` & `pycvc-1.2.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,163 +1,195 @@
-Metadata-Version: 2.1
-Name: pycvc
-Version: 1.2.3
-Summary: Card Verifiable Certificate tools
-Home-page: https://github.com/polhenarejos/pycvc
-Author: Pol Henarejos
-Author-email: pol.henarejos@cttc.es
-License: GPLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Plugins
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Security
-Classifier: Topic :: System :: Installation/Setup
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools
-Requires-Dist: cryptography (>=3.3)
-
-# pycvc
-Card Verifiable Certificates (CVC) tools for Python
-
-## Introduction
-
-Card Verifiable Certificates are an specification of storing electronic certificates, signed by RSA or Elliptic Curves algorithms.
-
-In contrast to X509 certificates, CVC are more compact and are widely used by HSM cards or personal USB tokens.
-
-pycvc implements the specifications of BSI TR 03110 to create CV certificates and requests.
-
-pycvc can be used to make a CV request and deploy a PKI based on CVC.
-
-## Install
-
-```
-pip install pycvc
-```
-
-## Usage
-
-pycvc can be used by importing the package or calling the command line tools `cvc-create`, for CVC generation, and `cvc-print`, for displaying CVC information and verification.
-
-For more information, execute `cvc-create` or `cvc-print` with `--help` flag.
-
-Here some examples.
-
-### Create a PKI
-
-`cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
-
-1- Setup the CA:
-```bash
-openssl ecparam -out ZZATCVCA00001.pem -name prime256v1 -genkey
-openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
-```
-
-2- Setup the DV:
-```bash
-openssl ecparam -out ZZATDVCA00001.pem -name prime256v1 -genkey
-openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
-openssl ec -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
-```
-
-3- Create a certificate request
-```bash
-openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
-openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
-cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
-```
-
-4- Sign a certificate request
-```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
-```
-
-### Validate certificates and requests
-
-`cvc-print` is the tool for certificate validation and verification. Call `cvc-print --help` for a complete list of parameters.
-
-The validation is performed by veryfing all signatures in the certificate chain.
-
-1- Setup trust directory
-```bash
-mkdir certs
-cp ZZATCVCA00001.cvcert certs/ZZATCVCA00001
-cp ZZATDVCA00001.cvcert certs/ZZATDVCA00001
-```
-
-2- Validate certificates
-```bash
-$ cvc-print -d certs ZZATCVCA00001.cvcert
-Certificate:
-  Profile Identifier: 00
-  CAR: ZZATCVCA00001
-  Public Key:
-    Scheme: ECDSA_SHA_256
-    Public Point: 040e5e4d5f20ee36ac920132f7f448da353d826156e9cfd3075f9d877f9c172111a689953b9accd5011248be50ccf47480ab703b42382a7a45484fccdc738a82e7
-  CHR: ZZATCVCA00001
-  CHAT:
-    Role:  TypeAT
-    Bytes: c000000000
-  Since:   2022-08-23
-  Expires: 2023-08-23
-Inner signature is VALID
-Certificate VALID
-
-$ cvc-print -d certs ZZATDVCA00001.cvcert
-Certificate:
-  Profile Identifier: 00
-  CAR: ZZATCVCA00001
-  Public Key:
-    Scheme: ECDSA_SHA_256
-    Public Point: 04b37a6588e55e9db3ea72837f4b4347028a51b1c5964ee54878bf2f856ee4abe06f1465e917c8d9ecf7170dbd61c2bc1fc37a1fa36698a33669daa6fa4c1e7400
-  CHR: ZZATDVCA00001
-  CHAT:
-    Role:  TypeAT
-    Bytes: 8000000000
-  Since:   2022-08-23
-  Expires: 2023-02-19
-Inner signature is VALID
-Certificate VALID
-
-$ cvc-print -d certs ZZATTERM00001.cvreq
-Certificate:
-  Profile Identifier: 00
-  CAR: ZZATTERM00001
-  Public Key:
-    Scheme: ECDSA_SHA_256
-    Public Point: 0406358861bc93173b3931a07595eba2bbcc88b852ed0a7139067047ab8abdba9b28eb07344f4f4e8f375bdc886c86d32060e92541b4d73178f9c9c53d3d98a765
-  CHR: ZZATTERM00001
-Inner signature is VALID
-Certificate VALID
-
-$ cvc-print -d certs ZZATTERM00001.cvcert
-Certificate:
-  Profile Identifier: 00
-  CAR: ZZATDVCA00001
-  Public Key:
-    Scheme: ECDSA_SHA_256
-    Public Point: 0406358861bc93173b3931a07595eba2bbcc88b852ed0a7139067047ab8abdba9b28eb07344f4f4e8f375bdc886c86d32060e92541b4d73178f9c9c53d3d98a765
-  CHR: ZZATTERM00001
-  CHAT:
-    Role:  TypeAT
-    Bytes: 00
-  Since:   2022-08-23
-  Expires: 2022-10-22
-Inner signature is VALID
-Certificate VALID
-```
+Metadata-Version: 2.1
+Name: pycvc
+Version: 1.2.4
+Summary: Card Verifiable Certificate tools
+Home-page: https://github.com/polhenarejos/pycvc
+Author: Pol Henarejos
+Author-email: pol.henarejos@cttc.es
+License: GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Installation/Setup
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools
+Requires-Dist: cryptography (>=3.3)
+Requires-Dist: pywin32
+
+# pycvc
+Card Verifiable Certificates (CVC) tools for Python
+
+## Introduction
+
+Card Verifiable Certificates are an specification of storing electronic certificates, signed by RSA or Elliptic Curves algorithms.
+
+In contrast to X509 certificates, CVC are more compact and are widely used by HSM cards or personal USB tokens.
+
+pycvc implements the specifications of BSI TR 03110 to create CV certificates and requests.
+
+pycvc can be used to make a CV request and deploy a PKI based on CVC.
+
+## Install
+
+```
+pip install pycvc
+```
+
+## Usage
+
+pycvc can be used by importing the package or calling the command line tools `cvc-create`, for CVC generation, and `cvc-print`, for displaying CVC information and verification.
+
+For more information, execute `cvc-create` or `cvc-print` with `--help` flag.
+
+Here some examples.
+
+### Create a PKI with ECC
+
+`cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
+
+1- Setup the CA:
+```bash
+openssl ecparam -out ZZATCVCA00001.pem -name prime256v1 -genkey
+openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
+```
+
+2- Setup the DV:
+```bash
+openssl ecparam -out ZZATDVCA00001.pem -name prime256v1 -genkey
+openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
+openssl ec -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+```
+
+3- Create a certificate request
+```bash
+openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
+openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
+cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
+```
+
+4- Sign a certificate request
+```bash
+cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+```
+
+### Create a PKI with RSA
+
+`cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
+
+1- Setup the CA:
+```bash
+openssl genrsa -out ZZATCVCA00001.pem 3072
+openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
+```
+
+2- Setup the DV:
+```bash
+openssl genrsa -out ZZATDVCA00001.pem 2048
+openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
+openssl rsa -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+```
+
+3- Create a certificate request
+```bash
+openssl genrsa -out ZZATTERM00001.pem 2048
+openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
+cvc-create --chr=ZZATTERM00001 --scheme=RSA_v1_5_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
+```
+
+4- Sign a certificate request
+```bash
+cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+```
+
+### Validate certificates and requests
+
+`cvc-print` is the tool for certificate validation and verification. Call `cvc-print --help` for a complete list of parameters.
+
+The validation is performed by veryfing all signatures in the certificate chain.
+
+1- Setup trust directory
+```bash
+mkdir certs
+cp ZZATCVCA00001.cvcert certs/ZZATCVCA00001
+cp ZZATDVCA00001.cvcert certs/ZZATDVCA00001
+```
+
+2- Validate certificates
+```bash
+$ cvc-print -d certs ZZATCVCA00001.cvcert
+Certificate:
+  Profile Identifier: 00
+  CAR: ZZATCVCA00001
+  Public Key:
+    Scheme: ECDSA_SHA_256
+    Public Point: 040e5e4d5f20ee36ac920132f7f448da353d826156e9cfd3075f9d877f9c172111a689953b9accd5011248be50ccf47480ab703b42382a7a45484fccdc738a82e7
+  CHR: ZZATCVCA00001
+  CHAT:
+    Role:  TypeAT
+    Bytes: c000000000
+  Since:   2022-08-23
+  Expires: 2023-08-23
+Inner signature is VALID
+Certificate VALID
+
+$ cvc-print -d certs ZZATDVCA00001.cvcert
+Certificate:
+  Profile Identifier: 00
+  CAR: ZZATCVCA00001
+  Public Key:
+    Scheme: ECDSA_SHA_256
+    Public Point: 04b37a6588e55e9db3ea72837f4b4347028a51b1c5964ee54878bf2f856ee4abe06f1465e917c8d9ecf7170dbd61c2bc1fc37a1fa36698a33669daa6fa4c1e7400
+  CHR: ZZATDVCA00001
+  CHAT:
+    Role:  TypeAT
+    Bytes: 8000000000
+  Since:   2022-08-23
+  Expires: 2023-02-19
+Inner signature is VALID
+Certificate VALID
+
+$ cvc-print -d certs ZZATTERM00001.cvreq
+Certificate:
+  Profile Identifier: 00
+  CAR: ZZATTERM00001
+  Public Key:
+    Scheme: ECDSA_SHA_256
+    Public Point: 0406358861bc93173b3931a07595eba2bbcc88b852ed0a7139067047ab8abdba9b28eb07344f4f4e8f375bdc886c86d32060e92541b4d73178f9c9c53d3d98a765
+  CHR: ZZATTERM00001
+Inner signature is VALID
+Certificate VALID
+
+$ cvc-print -d certs ZZATTERM00001.cvcert
+Certificate:
+  Profile Identifier: 00
+  CAR: ZZATDVCA00001
+  Public Key:
+    Scheme: ECDSA_SHA_256
+    Public Point: 0406358861bc93173b3931a07595eba2bbcc88b852ed0a7139067047ab8abdba9b28eb07344f4f4e8f375bdc886c86d32060e92541b4d73178f9c9c53d3d98a765
+  CHR: ZZATTERM00001
+  CHAT:
+    Role:  TypeAT
+    Bytes: 00
+  Since:   2022-08-23
+  Expires: 2022-10-22
+Inner signature is VALID
+Certificate VALID
+```
```

