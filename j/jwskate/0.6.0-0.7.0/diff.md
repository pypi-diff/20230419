# Comparing `tmp/jwskate-0.6.0.tar.gz` & `tmp/jwskate-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwskate-0.6.0.tar", max compression
+gzip compressed data, was "jwskate-0.7.0.tar", max compression
```

## Comparing `jwskate-0.6.0.tar` & `jwskate-0.7.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-01-11 14:32:09.691585 jwskate-0.6.0/LICENSE
--rw-r--r--   0        0        0    17961 2023-01-11 14:32:09.691585 jwskate-0.6.0/README.md
--rw-r--r--   0        0        0     3817 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/__init__.py
--rw-r--r--   0        0        0     2356 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/enums.py
--rw-r--r--   0        0        0     2809 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/__init__.py
--rw-r--r--   0        0        0     8992 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/base.py
--rw-r--r--   0        0        0     4567 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/ec.py
--rw-r--r--   0        0        0      323 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/encryption/__init__.py
--rw-r--r--   0        0        0     6245 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/encryption/aescbchmac.py
--rw-r--r--   0        0        0     3322 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/encryption/aesgcm.py
--rw-r--r--   0        0        0     1059 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/__init__.py
--rw-r--r--   0        0        0     2427 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/aesgcmkw.py
--rw-r--r--   0        0        0     2039 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/aeskw.py
--rw-r--r--   0        0        0      740 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/dir.py
--rw-r--r--   0        0        0     9600 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/ecdh.py
--rw-r--r--   0        0        0     3535 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/pbes2.py
--rw-r--r--   0        0        0     3369 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/key_mgmt/rsa.py
--rw-r--r--   0        0        0     4456 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/okp.py
--rw-r--r--   0        0        0      621 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/signature/__init__.py
--rw-r--r--   0        0        0     3536 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/signature/ec.py
--rw-r--r--   0        0        0     2249 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/signature/eddsa.py
--rw-r--r--   0        0        0     1886 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/signature/hmac.py
--rw-r--r--   0        0        0     3751 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwa/signature/rsa.py
--rw-r--r--   0        0        0      214 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwe/__init__.py
--rw-r--r--   0        0        0    12060 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwe/compact.py
--rw-r--r--   0        0        0      754 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/__init__.py
--rw-r--r--   0        0        0     4953 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/alg.py
--rw-r--r--   0        0        0    45088 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/base.py
--rw-r--r--   0        0        0     9380 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/ec.py
--rw-r--r--   0        0        0     7220 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/jwks.py
--rw-r--r--   0        0        0     8208 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/oct.py
--rw-r--r--   0        0        0    12201 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/okp.py
--rw-r--r--   0        0        0    11794 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwk/rsa.py
--rw-r--r--   0        0        0      213 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jws/__init__.py
--rw-r--r--   0        0        0     6127 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jws/compact.py
--rw-r--r--   0        0        0    10695 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jws/json.py
--rw-r--r--   0        0        0     5253 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jws/signature.py
--rw-r--r--   0        0        0      360 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwt/__init__.py
--rw-r--r--   0        0        0     8221 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwt/base.py
--rw-r--r--   0        0        0    11650 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwt/signed.py
--rw-r--r--   0        0        0     4125 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/jwt/signer.py
--rw-r--r--   0        0        0        0 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/py.typed
--rw-r--r--   0        0        0     4986 2023-01-11 14:32:09.695585 jwskate-0.6.0/jwskate/token.py
--rw-r--r--   0        0        0     2488 2023-01-11 14:32:09.695585 jwskate-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/.pydocstyle
--rw-r--r--   0        0        0       37 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2236 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/__init__.py
--rw-r--r--   0        0        0      709 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/test_base.py
--rw-r--r--   0        0        0     2145 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/test_encryption.py
--rw-r--r--   0        0        0     7255 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/test_examples.py
--rw-r--r--   0        0        0     1235 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/test_key_mgmt.py
--rw-r--r--   0        0        0      341 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwa/test_signature.py
--rw-r--r--   0        0        0    31113 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwe.py
--rw-r--r--   0        0        0        0 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwk/__init__.py
--rw-r--r--   0        0        0     3535 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwk/test_alg.py
--rw-r--r--   0        0        0     3168 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwk/test_ec.py
--rw-r--r--   0        0        0     2735 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwk/test_generate.py
--rw-r--r--   0        0        0    17817 2023-01-11 14:32:09.695585 jwskate-0.6.0/tests/test_jwk/test_jwk.py
--rw-r--r--   0        0        0    10374 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jwk/test_jwks.py
--rw-r--r--   0        0        0    10106 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jwk/test_okp.py
--rw-r--r--   0        0        0    11934 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jwk/test_rsa.py
--rw-r--r--   0        0        0     2437 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jwk/test_symmetric.py
--rw-r--r--   0        0        0    21000 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jws.py
--rw-r--r--   0        0        0    18957 2023-01-11 14:32:09.699585 jwskate-0.6.0/tests/test_jwt.py
--rw-r--r--   0        0        0    19426 1970-01-01 00:00:00.000000 jwskate-0.6.0/setup.py
--rw-r--r--   0        0        0    19344 1970-01-01 00:00:00.000000 jwskate-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-19 10:02:25.020868 jwskate-0.7.0/LICENSE
+-rw-r--r--   0        0        0    18475 2023-04-19 10:02:25.020868 jwskate-0.7.0/README.md
+-rw-r--r--   0        0        0     3956 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/__init__.py
+-rw-r--r--   0        0        0     2639 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/enums.py
+-rw-r--r--   0        0        0     2809 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/__init__.py
+-rw-r--r--   0        0        0     9627 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/base.py
+-rw-r--r--   0        0        0     4692 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/ec.py
+-rw-r--r--   0        0        0      323 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/__init__.py
+-rw-r--r--   0        0        0     6245 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/aescbchmac.py
+-rw-r--r--   0        0        0     3322 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/aesgcm.py
+-rw-r--r--   0        0        0     1059 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/aesgcmkw.py
+-rw-r--r--   0        0        0     2221 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/aeskw.py
+-rw-r--r--   0        0        0      740 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/dir.py
+-rw-r--r--   0        0        0     9770 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/ecdh.py
+-rw-r--r--   0        0        0     3551 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/pbes2.py
+-rw-r--r--   0        0        0     3471 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/rsa.py
+-rw-r--r--   0        0        0     4704 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/okp.py
+-rw-r--r--   0        0        0      621 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/__init__.py
+-rw-r--r--   0        0        0     3669 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/ec.py
+-rw-r--r--   0        0        0     2421 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/eddsa.py
+-rw-r--r--   0        0        0     2058 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/hmac.py
+-rw-r--r--   0        0        0     3988 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/rsa.py
+-rw-r--r--   0        0        0      214 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwe/__init__.py
+-rw-r--r--   0        0        0    12736 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwe/compact.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/__init__.py
+-rw-r--r--   0        0        0     6120 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/alg.py
+-rw-r--r--   0        0        0    48771 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/base.py
+-rw-r--r--   0        0        0     8246 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/ec.py
+-rw-r--r--   0        0        0     6989 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/jwks.py
+-rw-r--r--   0        0        0     6714 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/oct.py
+-rw-r--r--   0        0        0    11437 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/okp.py
+-rw-r--r--   0        0        0    10810 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/rsa.py
+-rw-r--r--   0        0        0      265 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/__init__.py
+-rw-r--r--   0        0        0     6111 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/compact.py
+-rw-r--r--   0        0        0    10679 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/json.py
+-rw-r--r--   0        0        0     5252 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/signature.py
+-rw-r--r--   0        0        0      413 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/__init__.py
+-rw-r--r--   0        0        0     8261 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/base.py
+-rw-r--r--   0        0        0    11659 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/signed.py
+-rw-r--r--   0        0        0     6688 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/signer.py
+-rw-r--r--   0        0        0     5035 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/verifier.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/py.typed
+-rw-r--r--   0        0        0     4969 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/token.py
+-rw-r--r--   0        0        0     2433 2023-04-19 10:02:25.024868 jwskate-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/.pydocstyle
+-rw-r--r--   0        0        0       37 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     2236 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/__init__.py
+-rw-r--r--   0        0        0     2276 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_base.py
+-rw-r--r--   0        0        0     2915 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_encryption.py
+-rw-r--r--   0        0        0     7279 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_examples.py
+-rw-r--r--   0        0        0     1601 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwa/test_key_mgmt.py
+-rw-r--r--   0        0        0      316 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwa/test_signature.py
+-rw-r--r--   0        0        0    31132 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwe.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/__init__.py
+-rw-r--r--   0        0        0     3962 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_alg.py
+-rw-r--r--   0        0        0     4401 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_ec.py
+-rw-r--r--   0        0        0     4264 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_generate.py
+-rw-r--r--   0        0        0    21141 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_jwk.py
+-rw-r--r--   0        0        0    10960 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_jwks.py
+-rw-r--r--   0        0        0    11281 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_okp.py
+-rw-r--r--   0        0        0    17351 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_rsa.py
+-rw-r--r--   0        0        0     2437 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_symmetric.py
+-rw-r--r--   0        0        0    22046 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jws.py
+-rw-r--r--   0        0        0    25401 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwt.py
+-rw-r--r--   0        0        0    19746 1970-01-01 00:00:00.000000 jwskate-0.7.0/PKG-INFO
```

### Comparing `jwskate-0.6.0/LICENSE` & `jwskate-0.7.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021, Guillaume Pujol
+Copyright (c) 2023, Guillaume Pujol
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jwskate-0.6.0/README.md` & `jwskate-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,36 @@
 
 A Pythonic implementation of the JOSE set of IETF specifications: [Json Web Signature][rfc7515], [Keys][rfc7517],
 [Algorithms][rfc7518], [Tokens][rfc7519] and [Encryption][rfc7516] (RFC7515 to 7519), and their extensions
 [ECDH Signatures][rfc8037] (RFC8037), [JWK Thumbprints][rfc7638] (RFC7638), and [JWK Thumbprint URI][rfc9278] (RFC9278),
 and with respect to [JWT Best Current Practices][rfc8725].
 
 - Free software: MIT
-- Documentation: <https://guillp.github.io/jwskate/>
+- Documentation: [https://guillp.github.io/jwskate/](https://guillp.github.io/jwskate/)
 
 A quick usage example, generating an RSA private key, signing some data, then validating that signature:
 
 ```python
 from jwskate import Jwk
 
-# let's generate a random private key
-rsa_private_jwk = (
-    Jwk.generate_for_alg(  # generated key will automatically be RSA, based on the required 'alg'
-        alg="RS256", key_size=2048
-    )
-    .with_kid_thumbprint()  # include an RFC7638 thumbprint as key id
-    .with_usage_parameters()  # include the appropriate 'use' and 'key_ops' parameters in the JWK, based on the 'alg'
-)
+# Let's generate a random private key, to use with alg 'RS256'.
+# Based on that alg, jwskate knows it must be an RSA key.
+rsa_private_jwk = Jwk.generate(alg="RS256", key_size=2048)
 
 data = b"Signing is easy!"
 signature = rsa_private_jwk.sign(data)
 
 # extract the public key, and verify the signature with it
 rsa_public_jwk = rsa_private_jwk.public_jwk()
 assert rsa_public_jwk.verify(data, signature)
 
 # let's see what a Jwk looks like:
 assert isinstance(rsa_private_jwk, dict)  # Jwk are dict
 
-print(rsa_private_jwk)
+print(rsa_private_jwk.with_usage_parameters())
 ```
 
 The result of this print will look like this (with the random parts abbreviated to `...` for display purposes only):
 
 ```
 {'kty': 'RSA',
  'n': '...',
@@ -57,44 +52,49 @@
 ```
 
 Now let's sign a JWT containing arbitrary claims, this time using an EC key:
 
 ```python
 from jwskate import Jwk, Jwt
 
-private_jwk = Jwk.generate_for_alg(
-    "ES256", kid="my_key"
-)  # let's specify a kid manually
+# This time let's try an EC key, based on `alg` parameter,
+# and let's specigy an arbitrary Key ID (kid).
+private_jwk = Jwk.generate(alg="ES256", kid="my_key")
+
+# here are claims to sign in a JWT:
 claims = {"sub": "some_sub", "claim1": "value1"}
 
 jwt = Jwt.sign(claims, private_jwk)
 # that's it! we have a signed JWT
+assert isinstance(jwt, Jwt)  # Jwt are objects
 assert jwt.claims == claims  # claims can be accessed as a dict
-assert jwt.sub == "some_sub"  # or individual claims can be accessed as attributes
-assert jwt["claim1"] == "value1"  # or as dict items
+assert jwt.headers == {"alg": "ES256", "kid": "my_key"}  # headers too
+assert jwt.sub == "some_sub"  # individual claims can be accessed as attributes
+assert jwt["claim1"] == "value1"  # or as dict items (with "subscription")
 assert jwt.alg == "ES256"  # alg and kid headers are also accessible as attributes
 assert jwt.kid == private_jwk.kid
+# notice that alg and kid are automatically set with appropriate values
+assert isinstance(jwt.signature, bytes)  # signature is accessible too
+# verifying the jwt signature is as easy as:
 assert jwt.verify_signature(private_jwk.public_jwk())
+# since our jwk contains an 'alg' parameter (here 'ES256'), the signature is automatically verified using that alg
+# you could also specify an alg manually, useful for keys with no "alg" hint:
+assert jwt.verify_signature(private_jwk.public_jwk(), alg="ES256")
 
 print(jwt)
 # eyJhbGciOiJFUzI1NiIsImtpZCI6Im15a2V5In0.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.C1KcDyDT8qXwUqcWzPKkQD7f6xai-gCgaRFMdKPe80Vk7XeYNa8ovuLwvdXgGW4ZZ_lL73QIyncY7tHGXUthag
 # This will output the full JWT compact representation. You can inspect it for example at <https://jwt.io>
-
-print(jwt.headers)
-# {'alg': 'ES256', 'kid': 'my_key'}
 ```
 
-Note above that the JWT headers are automatically generated with the appropriate values.
-
-Or let's sign a JWT with the standardised lifetime, subject, audience and ID claims:
+Or let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
 
 ```python
 from jwskate import Jwk, JwtSigner
 
-private_jwk = Jwk.generate_for_alg("ES256")
+private_jwk = Jwk.generate(alg="ES256")
 signer = JwtSigner(issuer="https://myissuer.com", jwk=private_jwk)
 jwt = signer.sign(
     subject="some_sub",
     audience="some_aud",
     extra_claims={"custom_claim1": "value1", "custom_claim2": "value2"},
 )
 
@@ -115,38 +115,38 @@
 }
 ```
 
 ## Features
 
 - Simple, Clean, Pythonic interface
 - Convenience wrappers around `cryptography` for all algorithms described in JWA
-- Json Web Keys (JWK) loading and generation
+- Json Web Keys (JWK) loading, dumping and generation
 - Arbitrary data signature and verification using Json Web Keys
 - Json Web Signatures (JWS) signing and verification
 - Json Web Encryption (JWE) encryption and decryption
 - Json Web Tokens (JWT) signing, verification and validation
-- 100% type annotated
+- 100% type annotated, verified with `mypy --strict`
 - nearly 100% code coverage
 - Relies on [cryptography](https://cryptography.io) for all cryptographic operations
 - Relies on [BinaPy](https://guillp.github.io/binapy/) for binary data manipulations
 
 ### Supported Token Types
 
-| Token Type                | Support                                                                  |
-|---------------------------|--------------------------------------------------------------------------|
-| Json Web Signature (JWS)  | ☑ Compact <br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |
-| Json Web Encryption (JWE) | ☑ Compact <br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |
-| Json Web Tokens (JWT)     | ☑ Signed <br/> ☑ Signed and Encrypted                        |
+
+| Token Type                | Support                                                  |
+| ------------------------- | -------------------------------------------------------- |
+| Json Web Signature (JWS)  | ☑ Compact<br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |
+| Json Web Encryption (JWE) | ☑ Compact<br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |
+| Json Web Tokens (JWT)     | ☑ Signed<br/> ☑ Signed and Encrypted                   |
 
 ### Supported Signature algorithms
 
-`jwskate` supports the following signature algorithms:
 
 | Signature Alg | Description                                    | Key Type | Reference                          | Note                           |
-|---------------|------------------------------------------------|----------|------------------------------------|--------------------------------|
+| ------------- | ---------------------------------------------- | -------- | ---------------------------------- | ------------------------------ |
 | HS256         | HMAC using SHA-256                             | oct      | [RFC7518, Section 3.2]             |                                |
 | HS384         | HMAC using SHA-384                             | oct      | [RFC7518, Section 3.2]             |                                |
 | HS512         | HMAC using SHA-512                             | oct      | [RFC7518, Section 3.2]             |                                |
 | RS256         | RSASSA-PKCS1-v1_5 using SHA-256                | RSA      | [RFC7518, Section 3.3]             |                                |
 | RS384         | RSASSA-PKCS1-v1_5 using SHA-384                | RSA      | [RFC7518, Section 3.3]             |                                |
 | RS512         | RSASSA-PKCS1-v1_5 using SHA-512                | RSA      | [RFC7518, Section 3.3]             |                                |
 | ES256         | ECDSA using P-256 and SHA-256                  | EC       | [RFC7518, Section 3.4]             |                                |
@@ -159,57 +159,54 @@
 | ES256K        | ECDSA using secp256k1 curve and SHA-256        | EC       | [RFC8812, Section 3.2]             |                                |
 | HS1           | HMAC using SHA-1                               | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
 | RS1           | RSASSA-PKCS1-v1_5 with SHA-1                   | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
 | none          | No digital signature or MAC performed          |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
 
 ### Supported Key Management algorithms
 
-`jwskate` supports the following key management algorithms:
 
-| Signature Alg      | Description                                     | Key Type | Reference                          | Note        |
-|--------------------|-------------------------------------------------|----------|------------------------------------|-------------|
-| RSA1_5             | RSAES-PKCS1-v1_5                                | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |
-| RSA-OAEP           | RSAES OAEP using default parameters             | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256  | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384    | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512    | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| A128KW             | AES Key Wrap using 128-bit key                  | oct      | [RFC7518, Section 4.4]             |             |
-| A192KW             | AES Key Wrap using 192-bit key                  | oct      | [RFC7518, Section 4.4]             |             |
-| A256KW             | AES Key Wrap using 256-bit key                  | oct      | [RFC7518, Section 4.4]             |             |
-| dir                | Direct use of a shared symmetric key            | oct      | [RFC7518, Section 4.5]             |             |
-| ECDH-ES            | ECDH-ES using Concat KDF                        | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |
-| A128GCMKW          | Key wrapping with AES GCM using 128-bit key     | oct      | [RFC7518, Section 4.7]             |             |
-| A192GCMKW          | Key wrapping with AES GCM using 192-bit key     | oct      | [RFC7518, Section 4.7]             |             |
-| A256GCMKW          | Key wrapping with AES GCM using 256-bit key     | oct      | [RFC7518, Section 4.7]             |             |
-| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping   | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping   | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping   | password | [RFC7518, Section 4.8]             |             |
+| Signature Alg      | Description                                    | Key Type | Reference                          | Note        |
+| ------------------ | ---------------------------------------------- | -------- | ---------------------------------- | ----------- |
+| RSA1_5             | RSAES-PKCS1-v1_5                               | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |
+| RSA-OAEP           | RSAES OAEP using default parameters            | RSA      | [RFC7518, Section 4.3]             |             |
+| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 4.3]             |             |
+| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
+| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
+| A128KW             | AES Key Wrap using 128-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| A192KW             | AES Key Wrap using 192-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| A256KW             | AES Key Wrap using 256-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| dir                | Direct use of a shared symmetric key           | oct      | [RFC7518, Section 4.5]             |             |
+| ECDH-ES            | ECDH-ES using Concat KDF                       | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| A128GCMKW          | Key wrapping with AES GCM using 128-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| A192GCMKW          | Key wrapping with AES GCM using 192-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| A256GCMKW          | Key wrapping with AES GCM using 256-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
 
 ### Supported Encryption algorithms
 
-`jwskate` supports the following encryption algorithms:
 
-| Signature Alg  | Description                                                 | Reference                |
-|----------------|-------------------------------------------------------------|--------------------------|
-| A128CBC-HS256  | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
-| A192CBC-HS384  | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
-| A256CBC-HS512  | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
-| A128GCM        | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
-| A192GCM        | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
-| A256GCM        | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
+| Signature Alg | Description                                                 | Reference                |
+| ------------- | ----------------------------------------------------------- | ------------------------ |
+| A128CBC-HS256 | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
+| A192CBC-HS384 | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
+| A256CBC-HS512 | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
+| A128GCM       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
+| A192GCM       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
+| A256GCM       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
 
 ### Supported Elliptic Curves
 
-`jwskate` supports the following Elliptic Curves:
 
 | Curve     | Description                           | Key Type | Usage                 | Reference                  |
-|-----------|---------------------------------------|----------|-----------------------|----------------------------|
+| --------- | ------------------------------------- | -------- | --------------------- | -------------------------- |
 | P-256     | P-256 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
 | P-384     | P-384 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
 | P-521     | P-521 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
 | Ed25519   | Ed25519 signature algorithm key pairs | OKP      | signature             | [RFC8037, Section 3.1]     |
 | Ed448     | Ed448 signature algorithm key pairs   | OKP      | signature             | [RFC8037, Section 3.1]     |
 | X25519    | X25519 function key pairs             | OKP      | encryption            | [RFC8037, Section 3.2]     |
 | X448      | X448 function key pairs               | OKP      | encryption            | [RFC8037, Section 3.2]     |
@@ -231,22 +228,23 @@
 
 ## Design
 
 ### JWK are dicts
 
 JWK are specified as JSON objects, which are parsed as `dict` in Python. The `Jwk` class in `jwskate` is actually a
 `dict` subclass, so you can use it exactly like you would use a dict: you can access its members, dump it back as JSON,
-etc. The same is true for Signed or Encrypted Json Web tokens in JSON format.
+etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. You cannot change the key cryptographic
+material, however, since that would lead to unusable keys.
 
 ### JWA Wrappers
 
 You can use `cryptography` to do the cryptographic operations that are described in
 [JWA](https://www.rfc-editor.org/info/rfc7518), but since `cryptography` is a general purpose library, its usage is not
-straightforward and gives you plenty of options to carefully select and combine, leaving room for errors. It has also a
-quite inconsistent API to handle the different type of keys and algorithms. To work around
+straightforward and gives you plenty of options to carefully select and combine, leaving room for mistakes, errors and
+confusion. It has also a quite inconsistent API to handle the different type of keys and algorithms. To work around
 this, `jwskate` comes with a set of consistent wrappers that implement the exact JWA specifications, with minimum risk
 of mistakes.
 
 ### Safe Signature Verification
 
 As advised in [JWT Best Practices][rfc8725] $3.1:
 
@@ -261,14 +259,22 @@
   algorithms
 - the `alg` parameter from the signature verification `Jwk`, if present. This `alg` is the algorithm intended for use
   with that key.
 
 Note that you cannot use `alg` and `algs` at the same time. If your `Jwk` contains an `alg` parameter, and you provide
 an `alg` or `algs` which does not match that value, a `Warning` will be emitted.
 
+## TODO
+
+- Complete/enhance/proof-read documentation
+- Better exceptions (create dedicated exception classes, better messages, etc.)
+- Support for JWE in JSON format
+- Better tests
+- Support for Selective-Disclosure JWT
+
 ## Credits
 
 All cryptographic operations are handled by [cryptography](https://cryptography.io).
 
 [rfc7515]: https://www.rfc-editor.org/rfc/rfc7515.html
 [rfc7516]: https://www.rfc-editor.org/rfc/rfc7516.html
 [rfc7517]: https://www.rfc-editor.org/rfc/rfc7517.html
```

### Comparing `jwskate-0.6.0/jwskate/__init__.py` & `jwskate-0.7.0/jwskate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 The `jwskate` module implements the various Json Web Crypto-related
 standards: JWA, JWK, JWKS, JWE, JWT. Each standard has its own submodule, but
 for convenience, you can import any class or component directly from the root
 `jwskate` module.
 
 `jwskate` doesn't implement any actual cryptographic operation, it just
 provides a set of convenient wrappers around the `cryptography` module.
+
 """
 
 __author__ = """Guillaume Pujol"""
 __email__ = "guill.p.linux@gmail.com"
 
-from .enums import EncryptionAlgs, KeyManagementAlgs, SignatureAlgs
+from .enums import EncryptionAlgs, KeyManagementAlgs, KeyTypes, SignatureAlgs
 from .jwa import (
     A128CBC_HS256,
     A128GCM,
     A128GCMKW,
     A128KW,
     A192CBC_HS384,
     A192GCM,
@@ -79,33 +80,35 @@
 from .jwe import InvalidJwe, JweCompact
 from .jwk import (
     ECJwk,
     ExpectedAlgRequired,
     InvalidJwk,
     Jwk,
     JwkSet,
+    MismatchingAlg,
     OKPJwk,
     RSAJwk,
     SymmetricJwk,
     UnsupportedAlg,
     UnsupportedEllipticCurve,
     UnsupportedKeyType,
     UnsupportedOKPCurve,
     select_alg_class,
     select_alg_classes,
     to_jwk,
 )
-from .jws import InvalidJws, JwsCompact, JwsJsonFlat, JwsJsonGeneral
+from .jws import InvalidJws, JwsCompact, JwsJsonFlat, JwsJsonGeneral, JwsSignature
 from .jwt import (
     ExpiredJwt,
     InvalidClaim,
     InvalidJwt,
     InvalidSignature,
     Jwt,
     JwtSigner,
+    JwtVerifier,
     SignedJwt,
 )
 
 __all__ = [
     "A128CBC_HS256",
     "A128GCM",
     "A128GCMKW",
@@ -155,17 +158,21 @@
     "InvalidSignature",
     "JweCompact",
     "Jwk",
     "JwkSet",
     "JwsCompact",
     "JwsJsonFlat",
     "JwsJsonGeneral",
+    "JwsSignature",
     "Jwt",
     "JwtSigner",
+    "JwtVerifier",
     "KeyManagementAlgs",
+    "KeyTypes",
+    "MismatchingAlg",
     "MismatchingAuthTag",
     "OKPCurve",
     "OKPJwk",
     "PS256",
     "PS384",
     "PS512",
     "P_256",
```

### Comparing `jwskate-0.6.0/jwskate/enums.py` & `jwskate-0.7.0/jwskate/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,41 +19,44 @@
     PS512 = "PS512"
     EdDSA = "EdDSA"
 
     HS256 = "HS256"
     HS384 = "HS384"
     HS512 = "HS512"
 
-    ALL_SYMMETRIC = [HS256, HS384, HS512]
-    ALL_ASYMMETRIC = [
+    ALL_SYMMETRIC = {HS256, HS384, HS512}
+    ALL_ASYMMETRIC = {
         RS256,
         RS384,
         RS512,
         ES256,
         ES384,
         ES512,
         PS256,
         PS384,
         PS512,
         EdDSA,
-    ]
-    ALL = ALL_ASYMMETRIC + ALL_SYMMETRIC
+    }
+    ALL = ALL_ASYMMETRIC | ALL_SYMMETRIC
 
 
 class EncryptionAlgs:
     """Identifiers for Encryption algorithms."""
 
     A128CBC_HS256 = "A128CBC-HS256"
     A192CBC_HS384 = "A192CBC-HS384"
     A256CBC_HS512 = "A256CBC-HS512"
     A128GCM = "A128GCM"
     A192GCM = "A192GCM"
     A256GCM = "A256GCM"
 
-    ALL = [A128CBC_HS256, A192CBC_HS384, A256CBC_HS512, A128GCM, A192GCM, A256GCM]
+    ALL_AESCBC_HMAC = {A128CBC_HS256, A192CBC_HS384, A256CBC_HS512}
+    ALL_AESGCM = {A128GCM, A192GCM, A256GCM}
+
+    ALL = ALL_AESGCM | ALL_AESCBC_HMAC
 
 
 class KeyManagementAlgs:
     """Identifiers for Key Management algorithms."""
 
     RSA1_5 = "RSA1_5"
     RSA_OAEP = "RSA-OAEP"
@@ -73,34 +76,45 @@
     A256GCMKW = "A256GCMKW"
     dir = "dir"
 
     PBES2_HS256_A128KW = "PBES2-HS256+A128KW"
     PBES2_HS384_A192KW = "PBES2-HS384+A192KW"
     PBES2_HS512_A256KW = "PBES2-HS512+A256KW"
 
-    ALL_SYMMETRIC = [
+    ALL_AES = {A128KW, A192KW, A256KW}
+    ALL_AESGCM = {A128GCMKW, A192GCMKW, A256GCMKW}
+    ALL_SYMMETRIC = {
         A128KW,
         A192KW,
         A256KW,
         A128GCMKW,
         A192GCMKW,
         A256GCMKW,
         dir,
-    ]
-    ALL_ASYMMETRIC = [
+    }
+    ALL_ASYMMETRIC = {
         RSA1_5,
         RSA_OAEP,
         RSA_OAEP_256,
         RSA_OAEP_384,
         RSA_OAEP_512,
         ECDH_ES,
         ECDH_ES_A128KW,
         ECDH_ES_A192KW,
         ECDH_ES_A256KW,
-    ]
-    ALL_PASSWORD_BASED = [
+    }
+    ALL_PASSWORD_BASED = {
         PBES2_HS256_A128KW,
         PBES2_HS384_A192KW,
         PBES2_HS512_A256KW,
-    ]
-    ALL_KEY_BASED = ALL_ASYMMETRIC + ALL_SYMMETRIC
-    ALL = ALL_ASYMMETRIC + ALL_SYMMETRIC + ALL_PASSWORD_BASED
+    }
+    ALL_KEY_BASED = ALL_ASYMMETRIC | ALL_SYMMETRIC
+    ALL = ALL_ASYMMETRIC | ALL_SYMMETRIC | ALL_PASSWORD_BASED
+
+
+class KeyTypes:
+    """Identifier for Key Types (kty)."""
+
+    OCT = "oct"
+    RSA = "RSA"
+    EC = "EC"
+    OKP = "OKP"
```

### Comparing `jwskate-0.6.0/jwskate/jwa/__init__.py` & `jwskate-0.7.0/jwskate/jwa/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/base.py` & `jwskate-0.7.0/jwskate/jwa/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from contextlib import contextmanager
 from typing import Generic, Iterator, SupportsBytes, Tuple, Type, TypeVar, Union
 
 import cryptography.exceptions
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
+from typing_extensions import Self, override
 
 
 class PrivateKeyRequired(AttributeError):
     """Raised when a cryptographic operation requires a private key, and a public key has been provided instead."""
 
 
 class PublicKeyRequired(AttributeError):
@@ -38,14 +39,19 @@
     """For algs that are considered insecure, set to True to allow only signature verification or decryption of existing
     data, but don't allow new signatures or encryption."""
 
     def __repr__(self) -> str:
         """Use the name of the alg as repr."""
         return self.name
 
+    @classmethod
+    def with_random_key(cls) -> Self:
+        """Initialize an instance of this alg with a randomly-generated key."""
+        raise NotImplementedError()
+
 
 class BaseSymmetricAlg(BaseAlg):
     """Base class for Symmetric algorithms (using a raw bytes key).
 
     Args:
         key: the key to use for cryptographic operations
 
@@ -139,30 +145,41 @@
 
         Raises:
             PrivateKeyRequired: if the configured key is not private
 
         """
         if not isinstance(self.key, self.private_key_class):
             raise PrivateKeyRequired()
-        yield self.key  # type: ignore
+        yield self.key  # type: ignore[misc]
 
     @contextmanager
     def public_key_required(self) -> Iterator[Kpub]:
         """Check if this alg is initialised with a public key, as a context manager.
 
         Yields:
             The public key
 
         Raises:
             PublicKeyRequired: if the configured key is private
 
         """
         if not isinstance(self.key, self.public_key_class):
             raise PublicKeyRequired()
-        yield self.key  # type: ignore
+        yield self.key  # type: ignore[misc]
+
+    def public_key(self) -> Kpub:
+        """Return the public key matching the private key."""
+        if hasattr(self.key, "public_key"):
+            return self.key.public_key()  # type: ignore[no-any-return]
+        raise NotImplementedError()
+
+    def public_alg(self) -> Self:
+        """Return an alg instance initialised with the public key."""
+        with self.private_key_required():
+            return self.__class__(self.public_key())
 
 
 class BaseSignatureAlg(BaseAlg):
     """Base class for signature algorithms."""
 
     use = "sig"
     hashing_alg: hashes.HashAlgorithm
@@ -243,32 +260,32 @@
     def encrypt(
         self,
         plaintext: Union[bytes, SupportsBytes],
         *,
         iv: Union[bytes, SupportsBytes],
         aad: Union[bytes, SupportsBytes, None] = None,
     ) -> Tuple[BinaPy, BinaPy]:
-        """Encrypt arbitrary data, with [Authenticated Encryption (with optional Associated Data)][AEAD].
+        """Encrypt arbitrary data, with optional [Authenticated Encryption](https://wikipedia.org/wiki/Authenticated_encryption).
 
         This needs:
+
         - the raw data to encrypt (`plaintext`)
         - a given random Initialisation Vector (`iv`) of the appropriate size
         - optional Additional Authentication Data (`aad`)
+
         And returns a tuple (ciphered_data, authentication_tag).
 
         Args:
           plaintext: the data to encrypt
           iv: the Initialisation Vector to use
           aad: the Additional Authentication Data
 
         Returns:
           a tuple of ciphered data and authentication tag
 
-        [AEAD]: https://wikipedia.org/wiki/Authenticated_encryption
-
         """
         raise NotImplementedError
 
     def decrypt(
         self,
         ciphertext: Union[bytes, SupportsBytes],
         *,
@@ -292,19 +309,20 @@
         Returns:
           the deciphered data
 
         """
         raise NotImplementedError
 
     @classmethod
-    def init_random_key(cls) -> BaseAESEncryptionAlg:
+    @override
+    def with_random_key(cls) -> Self:
         """Initialize this alg with a random key.
 
         Returns:
-            a subclass of BaseAESEncryptionAlg initialized with a randomly generated key
+            a subclass of `BaseAESEncryptionAlg` initialized with a randomly generated key
 
         """
         return cls(cls.generate_key())
 
 
 class BaseKeyManagementAlg(BaseAlg):
     """Base class for Key Management algorithms."""
```

### Comparing `jwskate-0.6.0/jwskate/jwa/ec.py` & `jwskate-0.7.0/jwskate/jwa/ec.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, Tuple, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives.asymmetric import ec
 
+from jwskate import KeyTypes
+
 
 @dataclass
 class EllipticCurve:
     """A descriptive class for Elliptic Curves.
 
     Elliptic Curves have a name, a `cryptography.ec.EllipticCurve`, and a coordinate size.
 
@@ -39,15 +41,15 @@
         """Generate a new EC key on this curve.
 
         Returns:
              a tuple of 4 `int`s: `x` and `y` coordinates (public key) and `d` (private key)
 
         """
         key = ec.generate_private_key(self.cryptography_curve)
-        pn = key.private_numbers()  # type: ignore
+        pn = key.private_numbers()  # type: ignore[attr-defined]
         x = pn.public_numbers.x
         y = pn.public_numbers.y
         d = pn.private_value
         return x, y, d
 
     @classmethod
     def get_curve(
@@ -96,46 +98,46 @@
         public_numbers: ec.EllipticCurvePublicNumbers
         if isinstance(key, ec.EllipticCurvePrivateKey):
             public_numbers = key.public_key().public_numbers()
         elif isinstance(key, ec.EllipticCurvePublicKey):
             public_numbers = key.public_numbers()
         x = BinaPy.from_int(public_numbers.x, crv.coordinate_size).to("b64u").ascii()
         y = BinaPy.from_int(public_numbers.y, crv.coordinate_size).to("b64u").ascii()
-        parameters = {"kty": "EC", "crv": crv.name, "x": x, "y": y}
+        parameters = {"kty": KeyTypes.EC, "crv": crv.name, "x": x, "y": y}
         if isinstance(key, ec.EllipticCurvePrivateKey):
-            pn = key.private_numbers()  # type: ignore
+            pn = key.private_numbers()  # type: ignore[attr-defined]
             d = (
                 BinaPy.from_int(pn.private_value, crv.coordinate_size)
                 .to("b64u")
                 .ascii()
             )
             parameters["d"] = d
         return parameters
 
 
-P_256 = EllipticCurve(
+P_256: EllipticCurve = EllipticCurve(
     name="P-256",
     cryptography_curve=ec.SECP256R1(),
     coordinate_size=32,
 )
 """P-256 curve."""
 
-P_384 = EllipticCurve(
+P_384: EllipticCurve = EllipticCurve(
     name="P-384",
     cryptography_curve=ec.SECP384R1(),
     coordinate_size=48,
 )
 """P-384 curve."""
 
-P_521 = EllipticCurve(
+P_521: EllipticCurve = EllipticCurve(
     name="P-521",
     cryptography_curve=ec.SECP521R1(),
     coordinate_size=66,
 )
 """P-521 curve."""
 
-secp256k1 = EllipticCurve(
+secp256k1: EllipticCurve = EllipticCurve(
     name="secp256k1",
     cryptography_curve=ec.SECP256K1(),
     coordinate_size=32,
 )
 """[secp256k1 curve](https://www.rfc-editor.org/rfc/rfc8812.html)"""
```

### Comparing `jwskate-0.6.0/jwskate/jwa/encryption/aescbchmac.py` & `jwskate-0.7.0/jwskate/jwa/encryption/aescbchmac.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/encryption/aesgcm.py` & `jwskate-0.7.0/jwskate/jwa/encryption/aesgcm.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/__init__.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/aesgcmkw.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/aesgcmkw.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/aeskw.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/aeskw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """This module implements AES based Key Management algorithms."""
 from typing import SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import keywrap
+from typing_extensions import Self, override
 
 from ..base import BaseKeyManagementAlg, BaseSymmetricAlg
 
 
 class BaseAesKeyWrap(BaseKeyManagementAlg, BaseSymmetricAlg):
     """Base class for AES KW algorithms."""
 
     key_size: int
     """Required AES key size in bits."""
 
     @classmethod
+    @override
     def check_key(cls, key: bytes) -> None:
         """Check that a key is valid for usage with this algorithm.
 
         To be valid, a key must be `bytes` and be of appropriate length (128, 192 or 256 bits).
 
         Args:
           key: a key to check
@@ -25,14 +27,19 @@
         Raises:
             ValueError: if the key is not appropriate
 
         """
         if not isinstance(key, bytes) or len(key) * 8 != cls.key_size:
             raise ValueError(f"Key must be {cls.key_size} bits.")
 
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(BinaPy.random_bits(cls.key_size))
+
     def wrap_key(self, plainkey: bytes) -> BinaPy:
         """Wrap a key.
 
         Args:
           plainkey: the key to wrap.
 
         Returns:
```

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/dir.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/dir.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/ecdh.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/ecdh.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Any, SupportsBytes, Type, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec, x448, x25519
 from cryptography.hazmat.primitives.kdf.concatkdf import ConcatKDFHash
+from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseKeyManagementAlg
 from .aeskw import A128KW, A192KW, A256KW, BaseAesKeyWrap
 
 
 class EcdhEs(
     BaseKeyManagementAlg,
@@ -30,14 +31,19 @@
     private_key_class = (
         ec.EllipticCurvePrivateKey,
         x25519.X25519PrivateKey,
         x448.X448PrivateKey,
     )
 
     @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(x25519.X25519PrivateKey.generate())
+
+    @classmethod
     def otherinfo(cls, alg: str, apu: bytes, apv: bytes, key_size: int) -> BinaPy:
         """Build the "otherinfo" parameter for Concat KDF Hash.
 
         Args:
           alg: identifier for the encryption alg
           apu: Agreement PartyUInfo
           apv: Agreement PartyVInfo
```

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/pbes2.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/pbes2.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     def __init__(self, password: Union[SupportsBytes, bytes, str]):
         if isinstance(password, str):
             password = password.encode("utf-8")
         if not isinstance(password, bytes):
             password = bytes(password)
         self.password = password
 
-    def generate_salt(self, size: int = 12) -> BinaPy:
+    @classmethod
+    def generate_salt(cls, size: int = 12) -> BinaPy:
         """Generate a salt that is suitable for use for encryption.
 
         Args:
           size: size of the generated salt, in bytes
 
         Returns:
             the generated salt
```

### Comparing `jwskate-0.6.0/jwskate/jwa/key_mgmt/rsa.py` & `jwskate-0.7.0/jwskate/jwa/key_mgmt/rsa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """This module implements RSA based Key Management algorithms."""
 
 from typing import Any, SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
+from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseKeyManagementAlg
 
 
 class BaseRsaKeyWrap(
     BaseKeyManagementAlg,
     BaseAsymmetricAlg[rsa.RSAPrivateKey, rsa.RSAPublicKey],
 ):
-    """Base class for RSA Key Wrapping algorithms.
-
-    Args:
-        key: the private or public key to use
-
-    """
+    """Base class for RSA Key Wrapping algorithms."""
 
     padding: Any
 
     name: str
     description: str
 
     private_key_class = rsa.RSAPrivateKey
     public_key_class = rsa.RSAPublicKey
 
-    def __init__(self, key: Union[rsa.RSAPublicKey, rsa.RSAPrivateKey]):
-        self.key = key
+    min_key_size: int = 2048
+
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(
+            rsa.generate_private_key(public_exponent=65537, key_size=cls.min_key_size)
+        )
 
     def wrap_key(self, plainkey: bytes) -> BinaPy:
         """Wrap a symmetric key using this algorithm.
 
         Args:
           plainkey: the symmetric key to wrap
```

### Comparing `jwskate-0.6.0/jwskate/jwa/okp.py` & `jwskate-0.7.0/jwskate/jwa/okp.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519, x448, x25519
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
-class PublicKeyProtocol(Protocol):  # noqa
+class PublicKeyProtocol(Protocol):
     """A protocol that each `cryptography` ECDH public key class implements."""
 
     def public_bytes(
         self,
         encoding: serialization.Encoding,
         format: serialization.PublicFormat,
-    ) -> bytes:  # noqa
+    ) -> bytes:  # noqa: D102
         ...
 
 
 @runtime_checkable
-class PrivateKeyProtocol(Protocol):  # noqa
+class PrivateKeyProtocol(Protocol):
     """A protocol that each `cryptography` ECDH private key class implements."""
 
     def private_bytes(
         self,
         encoding: serialization.Encoding,
         format: serialization.PrivateFormat,
         encryption_algorithm: serialization.KeySerializationEncryption,
-    ) -> bytes:  # noqa
+    ) -> bytes:  # noqa: D102
         ...
 
-    def public_key(self) -> PublicKeyProtocol:  # noqa
+    def public_key(self) -> PublicKeyProtocol:  # noqa: D102
         ...
 
     @classmethod
-    def generate(self) -> PrivateKeyProtocol:  # noqa
+    def generate(self) -> PrivateKeyProtocol:  # noqa: D102
         ...
 
 
 @dataclass
 class OKPCurve:
     """Represent an Octet Key Pair (OKP) Curve."""
 
@@ -107,15 +107,23 @@
 
         """
         for c in cls.instances.values():
             if isinstance(
                 key, (c.cryptography_private_key_class, c.cryptography_public_key_class)
             ):
                 return c
-        raise TypeError(f"Unsupported OKP key {type(key)}")
+        raise TypeError(
+            f"""\
+Unsupported key type for OKP: {type(key)}. Supported key types are: "
+{', '.join(
+    name
+    for curve in cls.instances.values()
+    for name in (curve.cryptography_private_key_class.__name__, curve.cryptography_public_key_class.__name__)
+)}"""
+        )
 
 
 Ed25519 = OKPCurve(
     name="Ed25519",
     description="Ed25519 signature algorithm key pairs",
     cryptography_private_key_class=ed25519.Ed25519PrivateKey,
     cryptography_public_key_class=ed25519.Ed25519PublicKey,
```

### Comparing `jwskate-0.6.0/jwskate/jwa/signature/__init__.py` & `jwskate-0.7.0/jwskate/jwa/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/jwskate/jwa/signature/ec.py` & `jwskate-0.7.0/jwskate/jwa/signature/ec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module implement Elliptic Curve signature algorithms."""
 from typing import SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import asymmetric, hashes
 from cryptography.hazmat.primitives.asymmetric import ec
+from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseSignatureAlg
 from ..ec import P_256, P_384, P_521, EllipticCurve, secp256k1
 
 
 class BaseECSignatureAlg(
     BaseAsymmetricAlg[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey],
@@ -25,14 +26,19 @@
         cls, key: Union[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]
     ) -> None:  # noqa: D102
         if key.curve.name != cls.curve.cryptography_curve.name:
             raise ValueError(
                 f"This key is on curve {key.curve.name}. An EC key on curve {cls.curve.name} is expected."
             )
 
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(ec.generate_private_key(cls.curve.cryptography_curve))
+
     def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         with self.private_key_required() as key:
             dss_sig = key.sign(data, ec.ECDSA(self.hashing_alg))
             r, s = asymmetric.utils.decode_dss_signature(dss_sig)
@@ -70,41 +76,41 @@
                     ec.ECDSA(self.hashing_alg),
                 )
                 return True
             except exceptions.InvalidSignature:
                 return False
 
 
-class ES256(BaseECSignatureAlg):  # noqa: D415
+class ES256(BaseECSignatureAlg):
     """ECDSA using P-256 and SHA-256."""
 
     name = "ES256"
     description = __doc__
     curve = P_256
     hashing_alg = hashes.SHA256()
 
 
-class ES384(BaseECSignatureAlg):  # noqa: D415
+class ES384(BaseECSignatureAlg):
     """ECDSA using P-384 and SHA-384."""
 
     name = "ES384"
     description = __doc__
     curve = P_384
     hashing_alg = hashes.SHA384()
 
 
-class ES512(BaseECSignatureAlg):  # noqa: D415
+class ES512(BaseECSignatureAlg):
     """ECDSA using P-521 and SHA-512."""
 
     name = "ES512"
     description = __doc__
     curve = P_521
     hashing_alg = hashes.SHA512()
 
 
-class ES256K(BaseECSignatureAlg):  # noqa: D415
+class ES256K(BaseECSignatureAlg):
     """ECDSA using secp256k1 and SHA-256."""
 
     name = "ES256k"
     description = __doc__
     curve = secp256k1
     hashing_alg = hashes.SHA256()
```

### Comparing `jwskate-0.6.0/jwskate/jwa/signature/eddsa.py` & `jwskate-0.7.0/jwskate/jwa/signature/eddsa.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519
+from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseSignatureAlg
 
 
 class EdDsa(
     BaseAsymmetricAlg[
         Union[ed25519.Ed25519PrivateKey, ed448.Ed448PrivateKey],
@@ -21,14 +22,19 @@
 
     private_key_class = (ed25519.Ed25519PrivateKey, ed448.Ed448PrivateKey)
     public_key_class = (ed25519.Ed25519PublicKey, ed448.Ed448PublicKey)
 
     name = "EdDSA"
     description = __doc__
 
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(ed25519.Ed25519PrivateKey.generate())
+
     def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         with self.private_key_required() as key:
             return BinaPy(key.sign(data))
```

### Comparing `jwskate-0.6.0/jwskate/jwa/signature/hmac.py` & `jwskate-0.7.0/jwskate/jwa/signature/hmac.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """This module implements HMAC based signature algorithms."""
 
 from typing import SupportsBytes, Type, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes, hmac
+from typing_extensions import Self, override
 
 from ..base import BaseSignatureAlg, BaseSymmetricAlg
 
 
 class BaseHMACSigAlg(BaseSymmetricAlg, BaseSignatureAlg):
     """Base class for HMAC signature algorithms."""
 
     mac: Type[hmac.HMAC] = hmac.HMAC
     min_key_size: int
 
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(BinaPy.random_bits(cls.min_key_size))
+
     def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         if self.read_only:
             raise NotImplementedError
         m = self.mac(self.key, self.hashing_alg)
```

### Comparing `jwskate-0.6.0/jwskate/jwa/signature/rsa.py` & `jwskate-0.7.0/jwskate/jwa/signature/rsa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module implements RSA signature algorithms."""
 from typing import SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import asymmetric, hashes
-from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
+from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseSignatureAlg
 
 
 class BaseRSASigAlg(
     BaseAsymmetricAlg[asymmetric.rsa.RSAPrivateKey, asymmetric.rsa.RSAPublicKey],
     BaseSignatureAlg,
@@ -17,14 +18,21 @@
 
     padding_alg: padding.AsymmetricPadding = padding.PKCS1v15()
     min_key_size: int = 2048
 
     private_key_class = asymmetric.rsa.RSAPrivateKey
     public_key_class = asymmetric.rsa.RSAPublicKey
 
+    @classmethod
+    @override
+    def with_random_key(cls) -> Self:
+        return cls(
+            rsa.generate_private_key(public_exponent=65537, key_size=cls.min_key_size)
+        )
+
     def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:
         """Sign arbitrary data.
 
         Args:
           data: the data to sign
 
         Returns:
```

### Comparing `jwskate-0.6.0/jwskate/jwe/compact.py` & `jwskate-0.7.0/jwskate/jwe/compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """This module implements the JWE Compact format."""
 
 import warnings
-from typing import Any, Dict, Mapping, Optional, SupportsBytes, Type, Union
+from functools import cached_property
+from typing import Any, Dict, Iterable, Mapping, Optional, SupportsBytes, Type, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 
 from jwskate.jwa import (
     BasePbes2,
     Pbes2_HS256_A128KW,
     Pbes2_HS384_A192KW,
     Pbes2_HS512_A256KW,
 )
 from jwskate.jwk import Jwk, SymmetricJwk, to_jwk
-from jwskate.jwk.alg import UnsupportedAlg, select_alg_class
+from jwskate.jwk.alg import UnsupportedAlg, select_alg_class, select_alg_classes
 from jwskate.token import BaseCompactToken
 
 
 class InvalidJwe(ValueError):
     """Raised when an invalid JWE token is parsed."""
 
 
 class JweCompact(BaseCompactToken):
     """Represents a Json Web Encryption object, in compact representation, as defined in RFC7516.
 
     Args:
         value: the compact representation for this Jwe
+
     """
 
     def __init__(self, value: Union[bytes, str]):
         super().__init__(value)
 
         if self.value.count(b".") != 4:
             raise InvalidJwe(
@@ -96,14 +97,15 @@
           cek: the raw CEK
           iv: the raw IV
           ciphertext: the raw ciphertext
           tag: the authentication tag
 
         Returns:
             the initialized JweCompact instance
+
         """
         return cls(
             b".".join(
                 (
                     BinaPy.serialize_to("json", headers).to("b64u"),
                     BinaPy(cek).to("b64u"),
                     BinaPy(iv).to("b64u"),
@@ -120,14 +122,15 @@
         The `enc` header contains the identifier of the CEK encryption algorithm.
 
         Returns:
             the enc value
 
         Raises:
             AttributeError: if there is no enc header or it is not a string
+
         """
         return self.get_header("enc")  # type: ignore[no-any-return]
         # header has been checked at init time
 
     @classmethod
     def encrypt(
         cls,
@@ -151,14 +154,15 @@
           extra_headers: additional headers to include in the generated token
           cek: the CEK to force use, for algorithms relying on a random CEK. Leave `None` to have a safe value generated by `jwskate`.
           iv: the IV to force use. Leave `None` to have a safe value generated by `jwskate`.
           epk: the EPK to force use. Leave `None` to have a safe value generated by `jwskate`.
 
         Returns:
             the generated JweCompact instance
+
         """
         extra_headers = extra_headers or {}
         jwk = to_jwk(jwk)
         alg = select_alg_class(
             jwk.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=jwk.alg, alg=alg
         ).name
 
@@ -180,45 +184,63 @@
 
     PBES2_ALGORITHMS: Mapping[str, Type[BasePbes2]] = {
         alg.name: alg
         for alg in [Pbes2_HS256_A128KW, Pbes2_HS384_A192KW, Pbes2_HS512_A256KW]
     }
 
     def unwrap_cek(
-        self, jwk_or_password: Union[Jwk, Dict[str, Any], bytes, str]
+        self,
+        jwk_or_password: Union[Jwk, Dict[str, Any], bytes, str],
+        alg: Optional[str] = None,
+        algs: Optional[Iterable[str]] = None,
     ) -> Jwk:
-        """Unwrap the CEK from this JWE token using the provided key or password.
+        """Unwrap the CEK from this `Jwe` using the provided key or password.
 
         Args:
           jwk_or_password: the decryption JWK or password
+          alg: allowed key management algorithm, if there is only 1
+          algs: allowed key managements algorithms, if there are several
 
         Returns:
             the unwrapped CEK, as a SymmetricJwk
+
         """
         if isinstance(jwk_or_password, (bytes, str)):
             password = jwk_or_password
             return self.unwrap_cek_with_password(password)
 
         jwk = Jwk(jwk_or_password)
+        select_alg_classes(
+            jwk.KEY_MANAGEMENT_ALGORITHMS,
+            jwk_alg=self.alg,
+            alg=alg,
+            algs=algs,
+            strict=True,
+        )
         cek = jwk.recipient_key(self.wrapped_cek, **self.headers)
         return cek
 
     def decrypt(
         self,
         jwk: Union[Jwk, Dict[str, Any]],
+        alg: Optional[str] = None,
+        algs: Optional[Iterable[str]] = None,
     ) -> BinaPy:
-        """Decrypts this Jwe payload using a JWK.
+        """Decrypts this `Jwe` payload using a `Jwk`.
 
         Args:
           jwk: the decryption key
+          alg: allowed key management algorithm, if there is only 1
+          algs: allowed keys management algorithms, if there are several
 
         Returns:
           the decrypted payload
+
         """
-        cek_jwk = self.unwrap_cek(jwk)
+        cek_jwk = self.unwrap_cek(jwk, alg=alg, algs=algs)
 
         plaintext = cek_jwk.decrypt(
             ciphertext=self.ciphertext,
             iv=self.initialization_vector,
             tag=self.authentication_tag,
             aad=self.additional_authenticated_data,
             alg=self.enc,
@@ -254,14 +276,15 @@
 
         Returns:
             the resulting JweCompact
 
         Raises:
             UnsupportedAlg: if the key management alg is not supported
             ValueError: if the `count` parameter is not a positive integer
+
         """
         keyalg = cls.PBES2_ALGORITHMS.get(alg)
         if keyalg is None:
             raise UnsupportedAlg(
                 f"Unsupported password-based encryption algorithm '{alg}'. "
                 f"Value must be one of {list(cls.PBES2_ALGORITHMS.keys())}."
             )
@@ -303,14 +326,15 @@
 
         Returns:
             the CEK, as a SymmetricJwk instance
 
         Raises:
             UnsupportedAlg: if the token key management algorithm is not supported
             AttributeError: if the token misses the PBES2-related headers
+
         """
         keyalg = self.PBES2_ALGORITHMS.get(self.alg)
         if keyalg is None:
             raise UnsupportedAlg(
                 f"Unsupported password-based encryption algorithm '{self.alg}'. "
                 f"Value must be one of {list(self.PBES2_ALGORITHMS.keys())}."
             )
@@ -333,14 +357,15 @@
         """Decrypt the JWE token with a password. This only works for tokens encrypted with a password.
 
         Args:
           password: the password to use
 
         Returns:
             the unencrypted payload
+
         """
         cek_jwk = self.unwrap_cek_with_password(password)
         plaintext = cek_jwk.decrypt(
             ciphertext=self.ciphertext,
             iv=self.initialization_vector,
             tag=self.authentication_tag,
             aad=self.additional_authenticated_data,
```

### Comparing `jwskate-0.6.0/jwskate/jwk/__init__.py` & `jwskate-0.7.0/jwskate/jwk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module implements [Json Web Key RFC7517](https://tools.ietf.org/html/rfc7517)."""
 
 from .alg import (
     ExpectedAlgRequired,
+    MismatchingAlg,
     UnsupportedAlg,
     select_alg_class,
     select_alg_classes,
 )
 from .base import InvalidJwk, Jwk, UnsupportedKeyType, to_jwk
 from .ec import ECJwk, UnsupportedEllipticCurve
 from .jwks import JwkSet
@@ -15,14 +16,15 @@
 
 __all__ = [
     "ECJwk",
     "ExpectedAlgRequired",
     "InvalidJwk",
     "Jwk",
     "JwkSet",
+    "MismatchingAlg",
     "OKPJwk",
     "RSAJwk",
     "SymmetricJwk",
     "UnsupportedAlg",
     "UnsupportedEllipticCurve",
     "UnsupportedKeyType",
     "UnsupportedOKPCurve",
```

### Comparing `jwskate-0.6.0/jwskate/jwk/alg.py` & `jwskate-0.7.0/jwskate/jwk/alg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 """This module contains several utilities for algorithmic agility."""
 
 import warnings
-from typing import Iterable, List, Mapping, Optional, Type, TypeVar
+from typing import Iterable, List, Mapping, Optional, Type, TypeVar, Union
 
 from jwskate.jwa import BaseAlg
 
 
 class UnsupportedAlg(ValueError):
     """Raised when a unsupported alg is requested."""
 
 
 class ExpectedAlgRequired(ValueError):
     """Raised when the expected signature alg(s) must be provided."""
 
 
+class MismatchingAlg(ValueError):
+    """Raised when attempting a cryptographic operation with an unexpected algorithm.
+
+    Signature verification or a decryption operation with an algorithm that does not
+    match the algorithm specified in the key or the token.
+    """
+
+    def __init__(
+        self,
+        target_alg: str,
+        alg: Optional[str] = None,
+        algs: Union[Iterable[str], None] = None,
+    ) -> None:
+        self.target_alg = target_alg
+        self.alg = alg
+        self.algs = list(algs) if algs else None
+
+
 T = TypeVar("T", bound=Type[BaseAlg])
 
 
 def select_alg_class(
     supported_algs: Mapping[str, T],
     *,
     jwk_alg: Optional[str] = None,
     alg: Optional[str] = None,
+    strict: bool = False,
 ) -> T:
     """Choose the appropriate alg class to use for cryptographic operations.
 
     Given:
     - a mapping of supported algs names to wrapper classes
     - a preferred alg name (usually the one mentioned in a JWK)
     - and/or a user-specified alg
@@ -34,44 +53,47 @@
     This checks the coherency between the user specified `alg` and the `jwk_alg`, and will emit a warning
     if the user specified alg is different from the `jwk_alg`.
 
     Args:
       supported_algs: a mapping of supported alg names to alg wrapper
       jwk_alg: the alg from the JWK, if any
       alg: a user specified alg
+      strict: if `True` and alg does not match `jwk_alg`, raise a `MismatchingAlg` exception. If `False`, warn instead.
 
     Returns:
       the alg to use
 
-    Warnings:
-        A warning is emitted if `jwk_alg` is supplied and `alg` doesn't match its value.
-
     Raises:
-        UnsupportedAlg: if the requested alg is not supported
-        ValueError: if supported_algs is empty
+        UnsupportedAlg: if the requested `alg` is not supported
+        ValueError: if `supported_algs` is empty
+        MismatchingAlg: if `alg` does not match `jwk_alg`
 
     """
     if not supported_algs:
         raise ValueError("No possible algorithms to choose from!")
 
     choosen_alg: str
     if jwk_alg is not None:
         if alg is not None:
             if jwk_alg != alg:
-                warnings.warn(
-                    "This key has an 'alg' parameter, you should use that alg for each operation."
-                )
+                if strict:
+                    raise MismatchingAlg(jwk_alg, alg)
+                else:
+                    warnings.warn(
+                        "This key has an 'alg' parameter, you should use that alg for each operation."
+                    )
             choosen_alg = alg
         else:
             choosen_alg = jwk_alg
     elif alg is not None:
         choosen_alg = alg
     else:
         raise ExpectedAlgRequired(
-            "This key doesn't have an 'alg' parameter, so you need to provide the expected signing alg(s) for each operation."
+            "This key doesn't have an 'alg' parameter specifying which algorithm to use with that key, "
+            "so you need to provide the expected signing alg(s) for each operation."
         )
 
     try:
         return supported_algs[choosen_alg]
     except KeyError:
         raise UnsupportedAlg(
             f"Alg {choosen_alg} is not supported. Supported algs: {list(supported_algs)}."
@@ -80,14 +102,15 @@
 
 def select_alg_classes(
     supported_algs: Mapping[str, T],
     *,
     jwk_alg: Optional[str] = None,
     alg: Optional[str] = None,
     algs: Optional[Iterable[str]] = None,
+    strict: bool = False,
 ) -> List[T]:
     """Select several appropriate algs classes to use on cryptographic operations.
 
     This method is typically used to get the list of valid algorithms when checking a signature, when several algorithms are allowed.
 
     Given:
     - a mapping of supported algorithms name to wrapper classes
@@ -100,37 +123,40 @@
     if the user specified alg is different from the `jwk_alg`.
 
     Args:
       supported_algs: a mapping of alg names to alg wrappers
       jwk_alg: the alg from the JWK, if any
       alg: a user specified alg to use, if any
       algs: a user specified list of algs to use, if several are allowed
+      strict: if `True` and alg does not match `jwk_alg`, raise a `MismatchingAlg` exception. If `False`, warn instead.
 
     Returns:
       a list of possible algs to check
 
     Raises:
         ValueError: if both 'alg' and 'algs' parameters are used
         UnsupportedAlg: if none of the requested alg are supported
 
-    Warnings:
-        if the requested 'alg' is different that the 'jwk_alg', or the 'jwk_alg' is not in the 'algs'
-
     """
     if alg and algs:
         raise ValueError("Please use either parameter 'alg' or 'algs', not both.")
 
     if not supported_algs:
         raise ValueError("No possible algorithms to choose from!")
 
     if jwk_alg is not None:
         if (alg and alg != jwk_alg) or (algs and jwk_alg not in algs):
-            warnings.warn(
-                "This key has an 'alg' parameter, you should use that alg for each operation."
-            )
+            if strict:
+                raise MismatchingAlg(jwk_alg, alg, algs)
+            else:
+                requested_alg = f"{alg=}" if alg else f"{algs=}"
+                warnings.warn(
+                    f"This key has an 'alg' parameter with value {jwk_alg}, so you should use it with that alg only."
+                    f"You requested {requested_alg}."
+                )
 
     possible_algs: List[str] = []
     if alg:
         possible_algs = [alg]
     elif algs:
         possible_algs = list(algs)
     elif jwk_alg:
@@ -144,9 +170,10 @@
             return possible_supported_algs
         else:
             raise UnsupportedAlg(
                 f"None of the user-specified alg(s) are supported. {possible_algs}"
             )
 
     raise ExpectedAlgRequired(
-        "This key doesn't have an 'alg' parameter, so you need to provide the expected signing alg(s) for each operation."
+        "This key doesn't have an 'alg' parameter specifying which algorithm to use with that key, "
+        "so you need to provide the expected signing alg(s) for each operation."
     )
```

### Comparing `jwskate-0.6.0/jwskate/jwk/base.py` & `jwskate-0.7.0/jwskate/jwk/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-"""This module implements the `Jwk` base class, which provides most of the common features of all JWK types."""
+"""This module implements the `Jwk` class, which provides the main interface for using or interacting with a JWK key.
+
+Subclasses of `Jwk` will implement the specific key types, like RSA, EC, OKP, and will provide an interface to access
+the specific attributes for each key type.
+Unless you are dealing with a specific key type and want to access the internal attributes, you should only ever need
+to use the interface from `Jwk`.
+"""
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -15,15 +21,14 @@
     Optional,
     SupportsBytes,
     Tuple,
     Type,
     Union,
 )
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 from cryptography.hazmat.primitives import serialization
 
 from jwskate.jwa import (
     BaseAESEncryptionAlg,
     BaseAesGcmKeyWrap,
     BaseAesKeyWrap,
@@ -62,39 +67,101 @@
     kind: str
 
 
 class Jwk(BaseJsonDict):
     """Represents a Json Web Key (JWK), as specified in RFC7517.
 
     A JWK is a JSON object that represents a cryptographic key.  The
-    members of the object represent properties of the key, including its
-    value. Just like a parsed JSON object, a :class:`Jwk` is a dict, so
-    you can do with a Jwk anything you can do with a `dict`. In
+    members of the object represent properties of the key, also called
+    parameters, which are name and value pairs.
+
+    Just like a parsed JSON object, a `Jwk` is a `dict`, so
+    you can do with a `Jwk` anything you can do with a `dict`. In
     addition, all keys parameters are exposed as attributes. There are
-    subclasses of `Jwk` for each specific Key Type, but you shouldn't
+    subclasses of `Jwk` for each specific Key Type, but unless you are
+    dealing with specific parameters for a given key type, you shouldn't
     have to use the subclasses directly since they all present a common
-    interface.
+    interface for cryptographic operations.
 
     Args:
-        params: a dict with the parsed Jwk parameters, or a `cryptography key`, or another `Jwk`
+        params: a `dict` parsed from a JSON JWK, or a `cryptography key`, or another `Jwk`, or a `str` containing the JSON representation of a JWK, or raw `bytes`
         include_kid_thumbprint: if `True` (default), and there is no kid in the provided params, generate a kid based on the key thumbprint
 
     """
 
-    subclasses: Dict[str, Type[Jwk]] = {}
+    @classmethod
+    def generate_for_alg(cls, alg: str, **kwargs: Any) -> Jwk:
+        """Generate a key for usage with a specific `alg` and return the resulting `Jwk`.
+
+        Args:
+            alg: a signature or key management algorithm identifier
+            **kwargs: specific parameters, depending on the key type, or additional members to include in the `Jwk`
+
+        Returns:
+            the generated `Jwk`
+
+        """
+        for kty, jwk_class in cls.subclasses.items():
+            alg_class: Optional[Type[BaseAlg]]
+            try:
+                alg_class = jwk_class._get_alg_class(alg)
+                # special cases for AES or HMAC based algs which require a specific key size
+                if issubclass(alg_class, (BaseAESEncryptionAlg, BaseAesKeyWrap)):
+                    key_size = kwargs.get("key_size")
+                    if key_size is not None and key_size != alg_class.key_size:
+                        raise ValueError(
+                            f"Key for {alg} must be exactly {alg_class.key_size} bits. "
+                            "You should remove the `key_size` parameter to generate a key of the appropriate length."
+                        )
+                    kwargs.setdefault("key_size", alg_class.key_size)
+                elif issubclass(alg_class, BaseHMACSigAlg):
+                    key_size = kwargs.get("key_size")
+                    if key_size is not None and key_size < alg_class.min_key_size:
+                        warnings.warn(
+                            f"Symmetric keys to use with {alg} should be at least {alg_class.min_key_size} bits "
+                            "in order to make the key at least as hard to brute-force as the signature. "
+                            f"You requested a key size of {key_size} bits."
+                        )
+                    else:
+                        kwargs.setdefault("key_size", alg_class.min_key_size)
+
+                return jwk_class.generate(alg=alg, **kwargs)
+            except UnsupportedAlg:
+                continue
+
+        raise UnsupportedAlg(alg)
+
     """A dict of 'kty' values to subclasses implementing each specific Key Type."""
 
+    @classmethod
+    def generate_for_kty(cls, kty: str, **kwargs: Any) -> Jwk:
+        """Generate a key with a specific type and return the resulting Jwk.
+
+        Args:
+          kty: key type to generate
+          **kwargs: specific parameters depending on the key type, or additional members to include in the Jwk
+
+        Returns:
+            the resulting Jwk
+
+        Raises:
+            UnsupportedKeyType: if the key type is not supported
+
+        """
+        jwk_class = cls.subclasses.get(kty)
+        if jwk_class is None:
+            raise UnsupportedKeyType("Unsupported Key Type:", kty)
+        return jwk_class.generate(**kwargs)
+
+    subclasses: Dict[str, Type[Jwk]] = {}
     cryptography_key_types: Dict[Any, Type[Jwk]] = {}
-    """A dict of cryptography key classes to its specific 'kty' value."""
 
     PARAMS: Mapping[str, JwkParameter]
-    """A dict of parameters. Key is parameter name, value is a tuple (description, is_private, is_required, kind)."""
 
     KTY: ClassVar[str]
-    """The Key Type associated with this JWK."""
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES: ClassVar[Iterable[Any]]
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES: ClassVar[Iterable[Any]]
 
     SIGNATURE_ALGORITHMS: Mapping[str, Type[BaseSignatureAlg]] = {}
     KEY_MANAGEMENT_ALGORITHMS: Mapping[str, Type[BaseKeyManagementAlg]] = {}
     ENCRYPTION_ALGORITHMS: Mapping[str, Type[BaseAESEncryptionAlg]] = {}
@@ -118,15 +185,15 @@
         """
         Jwk.subclasses[cls.KTY] = cls
         for klass in cls.CRYPTOGRAPHY_PRIVATE_KEY_CLASSES:
             Jwk.cryptography_key_types[klass] = cls
         for klass in cls.CRYPTOGRAPHY_PUBLIC_KEY_CLASSES:
             Jwk.cryptography_key_types[klass] = cls
 
-    def __new__(cls, key: Union[Jwk, Dict[str, Any], Any], **kwargs: Any):  # type: ignore
+    def __new__(cls, key: Union[Jwk, Dict[str, Any], Any], **kwargs: Any) -> Jwk:
         """Overridden `__new__` to make the Jwk constructor smarter.
 
         The Jwk constructor will accept:
 
             - a `dict` with the parsed Jwk content
             - another Jwk, which will be used as-is instead of creating a copy
             - an instance from a `cryptography` public or private key class
@@ -143,20 +210,20 @@
                 kty: Optional[str] = key.get("kty")
                 if kty is None:
                     raise InvalidJwk("A Json Web Key must have a Key Type (kty)")
 
                 subclass = Jwk.subclasses.get(kty)
                 if subclass is None:
                     raise InvalidJwk("Unsupported Key Type", kty)
-                return super().__new__(subclass)
+                return super().__new__(subclass)  # type: ignore[type-var]
             elif isinstance(key, str):
                 return cls.from_json(key)
             else:
                 return cls.from_cryptography_key(key, **kwargs)
-        return super().__new__(cls, key, **kwargs)
+        return super().__new__(cls, key, **kwargs)  # type: ignore[type-var]
 
     def __init__(
         self, params: Union[Dict[str, Any], Any], include_kid_thumbprint: bool = False
     ):
         if isinstance(
             params, dict
         ):  # this is to avoid double init due to the __new__ above
@@ -165,16 +232,16 @@
             )
             self._validate()
             if self.get("kid") is None and include_kid_thumbprint:
                 self["kid"] = self.thumbprint()
 
         try:
             self.cryptography_key = self._to_cryptography_key()
-        except AttributeError as exc:
-            raise InvalidJwk("Invalid JWK parameter", *exc.args) from exc
+        except Exception as exc:
+            raise InvalidJwk(params) from exc
 
     @classmethod
     def _get_alg_class(cls, alg: str) -> Type[BaseAlg]:
         """Given an alg identifier, return the matching JWA wrapper.
 
         Args:
             alg: an alg identifier
@@ -245,14 +312,95 @@
             RuntimeError: when trying to modify cryptographic attributes
 
         """
         if key in self.PARAMS:
             raise RuntimeError("JWK key attributes cannot be modified.")
         super().__setitem__(key, value)
 
+    @property
+    def kty(self) -> str:
+        """Return the Key Type.
+
+        Returns:
+            the key type
+
+        """
+        return self.KTY
+
+    @property
+    def alg(self) -> Optional[str]:
+        """Return the configured key alg, if any.
+
+        Returns:
+            the key alg
+
+        """
+        alg = self.get("alg")
+        if alg is not None and not isinstance(alg, str):  # pragma: no branch
+            raise TypeError(f"Invalid alg type {type(alg)}", alg)
+        return alg
+
+    @property
+    def kid(self) -> Optional[str]:
+        """Return the JWK key ID (kid), if present."""
+        kid = self.get("kid")
+        if kid is not None and not isinstance(kid, str):  # pragma: no branch
+            raise TypeError(f"invalid kid type {type(kid)}", kid)
+        return kid
+
+    @property
+    def use(self) -> Optional[str]:
+        """Return the key use.
+
+        If no `alg` parameter is present, this returns the `use` parameter from this JWK. If an `alg` parameter is
+        present, the use is deduced from this alg. To check for the presence of the `use` parameter, use
+        `jwk.get('use')`.
+
+        """
+        if self.alg:
+            return self._get_alg_class(self.alg).use
+        else:
+            return self.get("use")
+
+    @property
+    def key_ops(self) -> Tuple[str, ...]:
+        """Return the key operations.
+
+        If no `alg` parameter is present, this returns the `key_ops` parameter from this JWK. If an `alg` parameter is
+        present, the key operations are deduced from this alg. To check for the presence of the `key_ops` parameter, use
+        `jwk.get('key_ops')`.
+
+        """
+        key_ops: Tuple[str, ...]
+        if self.use == "sig":
+            if self.is_symmetric:
+                key_ops = ("sign", "verify")
+            elif self.is_private:
+                key_ops = ("sign",)
+            else:
+                key_ops = ("verify",)
+        elif self.use == "enc":
+            if self.is_symmetric:
+                if self.alg:
+                    alg_class = self._get_alg_class(self.alg)
+                    if issubclass(alg_class, BaseKeyManagementAlg):
+                        key_ops = ("wrapKey", "unwrapKey")
+                    elif issubclass(alg_class, BaseAESEncryptionAlg):
+                        key_ops = ("encrypt", "decrypt")
+                else:
+                    key_ops = ("wrapKey", "unwrapKey", "encrypt", "decrypt")
+            elif self.is_private:
+                key_ops = ("unwrapKey",)
+            else:
+                key_ops = ("wrapKey",)
+        else:
+            key_ops = self.get("key_ops", ())
+
+        return tuple(key_ops)
+
     def thumbprint(self, hashalg: str = "sha-256") -> str:
         """Return the key thumbprint as specified by RFC 7638.
 
         Args:
           hashalg: A hash function (defaults to SHA256)
 
         Returns:
@@ -285,36 +433,120 @@
              the JWK thumbprint uri for this Jwk
 
         """
         return (
             f"urn:ietf:params:oauth:jwk-thumbprint:{hashalg}:{self.thumbprint(hashalg)}"
         )
 
-    @property
-    def kty(self) -> str:
-        """Return the Key Type.
+    def check(
+        self,
+        *,
+        is_private: Optional[bool] = None,
+        is_symmetric: Optional[bool] = None,
+        kty: Optional[str] = None,
+    ) -> Jwk:
+        """Check this key for type, privateness and/or symmetricness. Raise a ValueError if it not as expected.
+
+        Args:
+            is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
+            is_symmetric: if `True`, check if the key is symmetric, if `False`, check if it is asymmetric, if `None`, do nothing
+            kty: the expected key type, if any
 
         Returns:
-            the key type
+            this key, if all checks passed
+
+        Raises:
+            ValueError: if any check fails
 
         """
-        return self.KTY
+        if is_private is not None:
+            if is_private is True and self.is_private is False:
+                raise ValueError("This key is public while a private key is expected.")
+            elif is_private is False and self.is_private is True:
+                raise ValueError("This key is private while a public key is expected.")
 
-    @property
-    def alg(self) -> Optional[str]:
-        """Return the configured key alg, if any.
+        if is_symmetric is not None:
+            if is_symmetric is True and self.is_symmetric is False:
+                raise ValueError(
+                    "This key is asymmetric while a symmetric key is expected."
+                )
+            if is_symmetric is False and self.is_symmetric is True:
+                raise ValueError(
+                    "This key is symmetric while an asymmetric key is expected."
+                )
 
-        Returns:
-            the key alg
+        if kty is not None:
+            if self.kty != kty:
+                raise ValueError(
+                    f"This key has kty={self.kty} while a kty={kty} is expected."
+                )
+
+        return self
+
+    def _validate(self) -> None:
+        """Validate the content of this JWK.
+
+        It checks that all required parameters are present and well-formed. If the key is private, it sets the `is_private` flag to `True`.
+
+        Raises:
+            TypeError: if the key type doesn't match the subclass
+            InvalidJwk: if the JWK misses required members or has invalid members
 
         """
-        alg = self.get("alg")
-        if alg is not None and not isinstance(alg, str):  # pragma: no branch
-            raise TypeError(f"Invalid alg type {type(alg)}", alg)
-        return alg
+        if self.get("kty") != self.KTY:
+            raise TypeError(
+                f"This key 'kty' {self.get('kty')} doesn't match this Jwk subclass intended 'kty' {self.KTY}!"
+            )
+
+        jwk_is_private = False
+        for name, param in self.PARAMS.items():
+            value = self.get(name)
+
+            if param.is_private and value is not None:
+                jwk_is_private = True
+
+            if not param.is_private and param.is_required and value is None:
+                raise InvalidJwk(
+                    f"Missing required public param {param.description} ({name})"
+                )
+
+            if value is None:
+                pass
+            elif param.kind == "b64u":
+                if not isinstance(value, str):
+                    raise InvalidJwk(
+                        f"Parameter {param.description} ({name}) must be a string with a Base64URL-encoded value"
+                    )
+                if not BinaPy(value).check("b64u"):
+                    raise InvalidJwk(
+                        f"Parameter {param.description} ({name}) must be a Base64URL-encoded value"
+                    )
+            elif param.kind == "unsupported":
+                if value is not None:  # pragma: no cover
+                    raise InvalidJwk(f"Unsupported JWK param '{name}'")
+            elif param.kind == "name":
+                pass
+            else:
+                assert (
+                    False
+                ), f"Unsupported param '{name}' type '{param.kind}'"  # pragma: no cover
+
+        # if at least one of the supplied parameter was private, then all required private parameters must be provided
+        if jwk_is_private:
+            for name, param in self.PARAMS.items():
+                value = self.get(name)
+                if param.is_private and param.is_required and value is None:
+                    raise InvalidJwk(
+                        f"Missing required private param {param.description} ({name})"
+                    )
+
+        # if key is used for signing, it must be private
+        for op in self.get("key_ops", []):
+            if op in ("sign", "unwrapKey") and not self.is_private:
+                raise InvalidJwk(f"Key Operation is '{op}' but the key is public")
 
     def signature_class(self, alg: Optional[str] = None) -> Type[BaseSignatureAlg]:
         """Return the appropriate signature algorithm class (a `BaseSignatureAlg` subclass) to use with this key.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -411,135 +643,14 @@
         alg_class = self.key_management_class(alg)
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):
             return alg_class(self.cryptography_key)
         raise UnsupportedAlg(alg)  # pragma: no cover
 
-    @property
-    def kid(self) -> Optional[str]:
-        """Return the JWK key ID (kid), if present."""
-        kid = self.get("kid")
-        if kid is not None and not isinstance(kid, str):  # pragma: no branch
-            raise TypeError(f"invalid kid type {type(kid)}", kid)
-        return kid
-
-    @cached_property
-    def use(self) -> Optional[str]:
-        """Return the key use.
-
-        If no `alg` parameter is present, this returns the `use` parameter from this JWK. If an `alg` parameter is
-        present, the use is deduced from this alg. To check for the presence of the `use` parameter, use
-        `jwk.get('use')`.
-
-        """
-        if self.alg:
-            return self._get_alg_class(self.alg).use
-        else:
-            return self.get("use")
-
-    @cached_property
-    def key_ops(self) -> Tuple[str, ...]:
-        """Return the key operations.
-
-        If no `alg` parameter is present, this returns the `key_ops` parameter from this JWK. If an `alg` parameter is
-        present, the key operations are deduced from this alg. To check for the presence of the `key_ops` parameter, use
-        `jwk.get('key_ops')`.
-
-        """
-        key_ops: Tuple[str, ...]
-        if self.use == "sig":
-            if self.is_symmetric:
-                key_ops = ("sign", "verify")
-            elif self.is_private:
-                key_ops = ("sign",)
-            else:
-                key_ops = ("verify",)
-        elif self.use == "enc":
-            if self.is_symmetric:
-                if self.alg:
-                    alg_class = self._get_alg_class(self.alg)
-                    if issubclass(alg_class, BaseKeyManagementAlg):
-                        key_ops = ("wrapKey", "unwrapKey")
-                    elif issubclass(alg_class, BaseAESEncryptionAlg):
-                        key_ops = ("encrypt", "decrypt")
-                else:
-                    key_ops = ("wrapKey", "unwrapKey", "encrypt", "decrypt")
-            elif self.is_private:
-                key_ops = ("unwrapKey",)
-            else:
-                key_ops = ("wrapKey",)
-        else:
-            key_ops = self.get("key_ops", ())
-
-        return tuple(key_ops)
-
-    def _validate(self) -> None:
-        """Validate the content of this JWK.
-
-        It checks that all required parameters are present and well-formed. If the key is private, it sets the `is_private` flag to `True`.
-
-        Raises:
-            TypeError: if the key type doesn't match the subclass
-            InvalidJwk: if the JWK misses required members or has invalid members
-
-        """
-        if self.get("kty") != self.KTY:
-            raise TypeError(
-                f"This key 'kty' {self.get('kty')} doesn't match this Jwk subclass intended 'kty' {self.KTY}!"
-            )
-
-        jwk_is_private = False
-        for name, param in self.PARAMS.items():
-
-            value = self.get(name)
-
-            if param.is_private and value is not None:
-                jwk_is_private = True
-
-            if not param.is_private and param.is_required and value is None:
-                raise InvalidJwk(
-                    f"Missing required public param {param.description} ({name})"
-                )
-
-            if value is None:
-                pass
-            elif param.kind == "b64u":
-                if not isinstance(value, str):
-                    raise InvalidJwk(
-                        f"Parameter {param.description} ({name}) must be a string with a Base64URL-encoded value"
-                    )
-                if not BinaPy(value).check("b64u"):
-                    raise InvalidJwk(
-                        f"Parameter {param.description} ({name}) must be a Base64URL-encoded value"
-                    )
-            elif param.kind == "unsupported":
-                if value is not None:  # pragma: no cover
-                    raise InvalidJwk(f"Unsupported JWK param '{name}'")
-            elif param.kind == "name":
-                pass
-            else:
-                assert (
-                    False
-                ), f"Unsupported param '{name}' type '{param.kind}'"  # pragma: no cover
-
-        # if at least one of the supplied parameter was private, then all required private parameters must be provided
-        if jwk_is_private:
-            for name, param in self.PARAMS.items():
-                value = self.get(name)
-                if param.is_private and param.is_required and value is None:
-                    raise InvalidJwk(
-                        f"Missing required private param {param.description} ({name})"
-                    )
-
-        # if key is used for signing, it must be private
-        for op in self.get("key_ops", []):
-            if op in ("sign", "unwrapKey") and not self.is_private:
-                raise InvalidJwk(f"Key Operation is '{op}' but the key is public")
-
     def supported_signing_algorithms(self) -> List[str]:
         """Return the list of Signature algorithms that can be used with this key.
 
         Returns:
           a list of supported algs
 
         """
@@ -559,63 +670,14 @@
 
         Returns:
             a list of supported algs
 
         """
         return list(self.ENCRYPTION_ALGORITHMS)
 
-    def public_jwk(self) -> Jwk:
-        """Return the public Jwk associated with this key.
-
-        Returns:
-          a Jwk with the public key
-
-        """
-        if not self.is_private:
-            return self
-
-        params = {
-            name: self.get(name)
-            for name, param in self.PARAMS.items()
-            if not param.is_private
-        }
-
-        if "key_ops" in self:
-            key_ops = list(self.key_ops)
-            if "sign" in key_ops:
-                key_ops.remove("sign")
-                key_ops.append("verify")
-            if "unwrapKey" in key_ops:
-                key_ops.remove("unwrapKey")
-                key_ops.append("wrapKey")
-        else:
-            key_ops = None
-
-        return Jwk(
-            dict(
-                kty=self.kty,
-                kid=self.get("kid"),
-                alg=self.get("alg"),
-                use=self.get("use"),
-                key_ops=key_ops,
-                **params,
-            )
-        )
-
-    def as_jwks(self) -> JwkSet:
-        """Return a JwkSet with this key as single element.
-
-        Returns:
-            a JwsSet with this single key
-
-        """
-        from .jwks import JwkSet
-
-        return JwkSet(keys=(self,))
-
     def sign(
         self, data: Union[bytes, SupportsBytes], alg: Optional[str] = None
     ) -> BinaPy:
         """Sign a data using this Jwk, and return the generated signature.
 
         Args:
           data: the data to sign
@@ -633,15 +695,15 @@
         self,
         data: Union[bytes, SupportsBytes],
         signature: Union[bytes, SupportsBytes],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
-        """Verify a signature using this Jwk, and return `True` if valid.
+        """Verify a signature using this `Jwk`, and return `True` if valid.
 
         Args:
           data: the data to verify
           signature: the signature to verify
           alg: the allowed signature alg, if there is only one
           algs: the allowed signature algs, if there are several
 
@@ -859,16 +921,16 @@
         Raises:
             UnsupportedAlg: if the requested alg identifier is not supported
 
         """
         from jwskate import SymmetricJwk
 
         if not self.is_symmetric and not self.is_private:
-            warnings.warn(
-                "You are using a public key for recipient key unwrapping. Key wrapping should always be done using the recipient private key."
+            raise ValueError(
+                "You are using a public key for recipient key unwrapping. Key unwrapping must always be done using the recipient private key."
             )
 
         key_alg_wrapper = self.key_management_wrapper(alg)
         enc_alg_class = select_alg_class(SymmetricJwk.ENCRYPTION_ALGORITHMS, alg=enc)
 
         if isinstance(key_alg_wrapper, BaseRsaKeyWrap):
             cek = key_alg_wrapper.unwrap_key(wrapped_cek)
@@ -913,14 +975,63 @@
         else:
             raise UnsupportedAlg(
                 f"Unsupported Key Management Alg {key_alg_wrapper}"
             )  # pragma: no cover
 
         return SymmetricJwk.from_bytes(cek)
 
+    def public_jwk(self) -> Jwk:
+        """Return the public Jwk associated with this key.
+
+        Returns:
+          a Jwk with the public key
+
+        """
+        if not self.is_private:
+            return self
+
+        params = {
+            name: self.get(name)
+            for name, param in self.PARAMS.items()
+            if not param.is_private
+        }
+
+        if "key_ops" in self:
+            key_ops = list(self.key_ops)
+            if "sign" in key_ops:
+                key_ops.remove("sign")
+                key_ops.append("verify")
+            if "unwrapKey" in key_ops:
+                key_ops.remove("unwrapKey")
+                key_ops.append("wrapKey")
+        else:
+            key_ops = None
+
+        return Jwk(
+            dict(
+                kty=self.kty,
+                kid=self.get("kid"),
+                alg=self.get("alg"),
+                use=self.get("use"),
+                key_ops=key_ops,
+                **params,
+            )
+        )
+
+    def as_jwks(self) -> JwkSet:
+        """Return a JwkSet with this key as single element.
+
+        Returns:
+            a JwsSet with this single key
+
+        """
+        from .jwks import JwkSet
+
+        return JwkSet(keys=(self,))
+
     @classmethod
     def from_cryptography_key(cls, cryptography_key: Any, **kwargs: Any) -> Jwk:
         """Initialize a Jwk from a key from the `cryptography` library.
 
         The input key can be any private or public key supported by cryptography.
 
         Args:
@@ -930,184 +1041,202 @@
         Returns:
             the matching `Jwk` instance
 
         Raises:
             TypeError: if the key type is not supported
 
         """
-        for klass in cryptography_key.__class__.mro():
-            jwk_class = cls.cryptography_key_types.get(klass)
-            if jwk_class:
+        for cryptography_class, jwk_class in cls.cryptography_key_types.items():
+            if isinstance(cryptography_key, cryptography_class):
                 return jwk_class.from_cryptography_key(cryptography_key, **kwargs)
 
-        raise TypeError(f"Unsupported Jwk class for this Key Type: {cryptography_key}")
+        raise TypeError(
+            f"Unsupported Jwk class for this Key Type: {type(cryptography_key).__name__}"
+        )
 
     def _to_cryptography_key(self) -> Any:
         """Return a key from the `cryptography` library that matches this Jwk.
 
         This is implemented by subclasses.
 
         Returns:
             a `cryptography`key instance initialized from the current key
 
         """
         raise NotImplementedError
 
     @classmethod
-    def from_pem_key(
+    def from_pem(
         cls,
-        data: Union[bytes, str],
+        der: Union[bytes, str],
         password: Union[bytes, str, None] = None,
         **kwargs: Any,
     ) -> Jwk:
-        """Load a Jwk from a PEM encoded private or public key.
+        """Load a `Jwk` from a PEM encoded private or public key.
 
         Args:
-          data: the PEM encoded data to load
+          der: the PEM encoded data to load
           password: the password to decrypt the PEM, if required. Should be bytes. If it is a string, it will be encoded with UTF-8.
-          **kwargs: additional members to include in the Jwk (e.g. kid, use)
+          **kwargs: additional members to include in the `Jwk` (e.g. `kid`, `use`)
 
         Returns:
-            a Jwk instance from the loaded key
+            a `Jwk` instance from the loaded key
 
         """
-        data = data.encode() if isinstance(data, str) else data
+        der = der.encode() if isinstance(der, str) else der
         password = password.encode("UTF-8") if isinstance(password, str) else password
 
         try:
-            cryptography_key = serialization.load_pem_private_key(data, password)
+            cryptography_key = serialization.load_pem_private_key(der, password)
         except Exception as private_exc:
             try:
-                cryptography_key = serialization.load_pem_public_key(data)
-                if password is not None:
-                    raise ValueError(
-                        "A public key was loaded from PEM, while a password was provided for decryption."
-                        "Only private keys are encrypted in PEM."
-                    )
+                cryptography_key = serialization.load_pem_public_key(der)
+
             except Exception:
                 raise ValueError(
                     "The provided data is not a private or a public PEM encoded key."
                 ) from private_exc
+            if password is not None:
+                raise ValueError(
+                    "A public key was loaded from PEM, while a password was provided for decryption."
+                    "Only private keys are encrypted using a password."
+                )
 
         return cls.from_cryptography_key(cryptography_key, **kwargs)
 
-    def to_pem(self, password: Union[bytes, str, None] = None) -> bytes:
+    def to_pem(self, password: Union[bytes, str, None] = None) -> str:
         """Serialize this key to PEM format.
 
-        For private keys, you can provide a password for encryption. This password should be bytes. A `str` is also
+        For private keys, you can provide a password for encryption. This password should be `bytes`. A `str` is also
         accepted, and will be encoded to `bytes` using UTF-8 before it is used as encryption key.
 
         Args:
-          password: password to use to encrypt the PEM. Should be bytes. If it is a string, it will be encoded with UTF-8.
+          password: password to use to encrypt the PEM.
 
         Returns:
             the PEM serialized key
 
         """
-        password = (
-            str(password).encode("UTF-8") if isinstance(password, str) else password
-        )
+        password = password.encode("UTF-8") if isinstance(password, str) else password
 
         if self.is_private:
             encryption: serialization.KeySerializationEncryption
             if password:
                 encryption = serialization.BestAvailableEncryption(password)
             else:
                 encryption = serialization.NoEncryption()
             return self.cryptography_key.private_bytes(  # type: ignore[no-any-return]
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.PKCS8,
                 encryption,
-            )
+            ).decode()
         else:
             if password:
-                raise ValueError(
-                    "Public keys cannot be encrypted when serialized in PEM format."
-                )
+                raise ValueError("Public keys cannot be encrypted when serialized.")
             return self.cryptography_key.public_bytes(  # type: ignore[no-any-return]
                 serialization.Encoding.PEM,
                 serialization.PublicFormat.SubjectPublicKeyInfo,
-            )
+            ).decode()
 
     @classmethod
-    def generate(cls, **kwargs: Any) -> Jwk:
-        """Generate a Private Key and return it as a `Jwk` instance.
-
-        This method is implemented by subclasses for specific Key Types and returns an instance of that subclass.
+    def from_der(
+        cls,
+        der: bytes,
+        password: Union[bytes, str, None] = None,
+        **kwargs: Any,
+    ) -> Jwk:
+        """Load a `Jwk` from DER."""
+        password = password.encode("UTF-8") if isinstance(password, str) else password
 
-        Args:
-          **kwargs: specific parameters depending on the type of key, or additional members to include in the Jwk
+        try:
+            cryptography_key = serialization.load_der_private_key(der, password)
+        except Exception as private_exc:
+            try:
+                cryptography_key = serialization.load_der_public_key(der)
+            except Exception:
+                raise ValueError(
+                    "The provided data is not a private or a public DER encoded key."
+                ) from private_exc
+            if password is not None:
+                raise ValueError(
+                    "A public key was loaded from DER, while a password was provided for decryption."
+                    "Only private keys are encrypted using a password."
+                )
 
-        Returns:
-            a Jwk instance with a generated key
+        return cls.from_cryptography_key(cryptography_key, **kwargs)
 
-        """
-        raise NotImplementedError
+    def to_der(self, password: Union[bytes, str, None] = None) -> BinaPy:
+        """Serialize this key to DER.
 
-    @classmethod
-    def generate_for_kty(cls, kty: str, **kwargs: Any) -> Jwk:
-        """Generate a key with a specific type and return the resulting Jwk.
+        For private keys, you can provide a password for encryption. This password should be bytes. A `str` is also
+        accepted, and will be encoded to `bytes` using UTF-8 before it is used as encryption key.
 
         Args:
-          kty: key type to generate
-          **kwargs: specific parameters depending on the key type, or additional members to include in the Jwk
+          password: password to use to encrypt the PEM. Should be bytes. If it is a string, it will be encoded to bytes with UTF-8.
 
         Returns:
-            the resulting Jwk
-
-        Raises:
-            UnsupportedKeyType: if the key type is not supported
+            the DER serialized key
 
         """
-        jwk_class = cls.subclasses.get(kty)
-        if jwk_class is None:
-            raise UnsupportedKeyType("Unsupported Key Type:", kty)
-        return jwk_class.generate(**kwargs)
+        password = password.encode("UTF-8") if isinstance(password, str) else password
+
+        if self.is_private:
+            encryption: serialization.KeySerializationEncryption
+            if password:
+                encryption = serialization.BestAvailableEncryption(password)
+            else:
+                encryption = serialization.NoEncryption()
+            return BinaPy(
+                self.cryptography_key.private_bytes(
+                    serialization.Encoding.DER,
+                    serialization.PrivateFormat.PKCS8,
+                    encryption,
+                )
+            )
+        else:
+            if password:
+                raise ValueError("Public keys cannot be encrypted when serialized.")
+            return BinaPy(
+                self.cryptography_key.public_bytes(
+                    serialization.Encoding.DER,
+                    serialization.PublicFormat.SubjectPublicKeyInfo,
+                )
+            )
 
     @classmethod
-    def generate_for_alg(cls, alg: str, **kwargs: Any) -> Jwk:
-        """Generate a key for usage with a specific alg and return the resulting Jwk.
+    def generate(
+        cls, *, alg: Optional[str] = None, kty: Optional[str] = None, **kwargs: Any
+    ) -> Jwk:
+        """Generate a Private Key and return it as a `Jwk` instance.
+
+        This method is implemented by subclasses for specific Key Types and returns an instance of that subclass.
 
         Args:
-            alg: a signature or key management alg
-            **kwargs: specific parameters depending on the key type, or additional members to include in the Jwk
+            alg: intended algorithm to use with the generated key
+            kty: key type identifier
+            **kwargs: specific parameters depending on the type of key, or additional members to include in the `Jwk`
 
         Returns:
-            the resulting Jwk
+            a `Jwk` instance with a generated key
 
         """
-        for kty, jwk_class in cls.subclasses.items():
-            alg_class: Optional[Type[BaseAlg]]
-            try:
-                alg_class = jwk_class._get_alg_class(alg)
-                # special cases for AES or HMAC based algs which require a specific key size
-                if issubclass(alg_class, (BaseAESEncryptionAlg, BaseAesKeyWrap)):
-                    key_size = kwargs.get("key_size")
-                    if key_size is not None and key_size != alg_class.key_size:
-                        raise ValueError(
-                            f"Key for {alg} must be exactly {alg_class.key_size} bits. "
-                            "You should remove the `key_size` parameter to generate a key of the appropriate length."
-                        )
-                    kwargs.setdefault("key_size", alg_class.key_size)
-                elif issubclass(alg_class, BaseHMACSigAlg):
-                    key_size = kwargs.get("key_size")
-                    if key_size is not None and key_size < alg_class.min_key_size:
-                        warnings.warn(
-                            f"Symmetric keys to use with {alg} should be at least {alg_class.min_key_size} bits "
-                            "in order to make the key at least as hard to brute-force as the signature. "
-                            f"You requested a key size of {key_size} bits."
-                        )
-                    else:
-                        kwargs.setdefault("key_size", alg_class.min_key_size)
-
-                return jwk_class.generate(alg=alg, **kwargs)
-            except UnsupportedAlg:
-                continue
-
-        raise UnsupportedAlg(alg)
+        if alg:
+            key = cls.generate_for_alg(alg=alg, **kwargs)
+            if kty is not None and key.kty != kty:
+                raise ValueError(
+                    f"Incompatible `{alg=}` and `{kty=}` parameters. "
+                    f"`{alg=}` points to key with `kty='{key.kty}'`."
+                )
+            return key
+        if kty:
+            return cls.generate_for_kty(kty=kty, **kwargs)
+        raise ValueError(
+            "You must provide a hint for jwskate to know what kind of key it must generate. "
+            "You can either provide an 'alg' identifier as keyword parameter, and/or a 'kty'."
+        )
 
     def copy(self) -> Jwk:
         """Create a copy of this key.
 
         Returns:
             a copy of this key, with the same value
 
@@ -1187,58 +1316,18 @@
         for key in self.keys():
             if key == "kty" or key in self.PARAMS and self.PARAMS[key].is_required:
                 continue
             del jwk[key]
 
         return jwk
 
-    def check(
-        self,
-        *,
-        is_private: Optional[bool] = None,
-        is_symmetric: Optional[bool] = None,
-        kty: Optional[str] = None,
-    ) -> Jwk:
-        """Check this key for type, privateness and/or symmetricness. Raise a ValueError if it not as expected.
-
-        Args:
-            is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
-            is_symmetric: if `True`, check if the key is symmetric, if `False`, check if it is asymmetric, if `None`, do nothing
-            kty: the expected key type, if any
-
-        Returns:
-            this key, if all checks passed
-
-        Raises:
-            ValueError: if any check fails
-
-        """
-        if is_private is not None:
-            if is_private is True and self.is_private is False:
-                raise ValueError("This key is public while a private key is expected.")
-            elif is_private is False and self.is_private is True:
-                raise ValueError("This key is private while a public key is expected.")
-
-        if is_symmetric is not None:
-            if is_symmetric is True and self.is_symmetric is False:
-                raise ValueError(
-                    "This key is asymmetric while a symmetric key is expected."
-                )
-            if is_symmetric is False and self.is_symmetric is True:
-                raise ValueError(
-                    "This key is symmetric while an asymmetric key is expected."
-                )
-
-        if kty is not None:
-            if self.kty != kty:
-                raise ValueError(
-                    f"This key has kty={self.kty} while a kty={kty} is expected."
-                )
-
-        return self
+    def __eq__(self, other: Any) -> bool:
+        """Compare JWK keys, ignoring optional/informational fields."""
+        other = to_jwk(other)
+        return super(Jwk, self.minimize()).__eq__(other.minimize())
 
 
 def to_jwk(
     key: Any,
     *,
     kty: Optional[str] = None,
     is_private: Optional[bool] = None,
```

### Comparing `jwskate-0.6.0/jwskate/jwk/ec.py` & `jwskate-0.7.0/jwskate/jwk/ec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module implements JWK representing Elliptic Curve keys."""
 
 from __future__ import annotations
 
 import warnings
+from functools import cached_property
 from typing import Any, List, Mapping, Optional, Type, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
-from cryptography.hazmat.primitives import asymmetric
 from cryptography.hazmat.primitives.asymmetric import ec
+from typing_extensions import override
 
 from jwskate.jwa import (
     ES256,
     ES256K,
     ES384,
     ES512,
     P_256,
@@ -23,29 +23,34 @@
     EcdhEs_A128KW,
     EcdhEs_A192KW,
     EcdhEs_A256KW,
     EllipticCurve,
     secp256k1,
 )
 
+from .. import KeyTypes
+from .alg import UnsupportedAlg
 from .base import Jwk, JwkParameter
 
 
 class UnsupportedEllipticCurve(KeyError):
-    """Raised when an unsupported Elliptic curve is requested."""
+    """Raised when an unsupported Elliptic Curve is requested."""
 
 
 class ECJwk(Jwk):
-    """Represent an Elliptic Curve Jwk, with `kty=EC`."""
+    """Represent an Elliptic Curve key in JWK format.
 
-    KTY = "EC"
+    Elliptic Curve keys have Key Type `"EC"`.
+    """
 
-    CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (asymmetric.ec.EllipticCurvePrivateKey,)
+    KTY = KeyTypes.EC
 
-    CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (asymmetric.ec.EllipticCurvePublicKey,)
+    CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (ec.EllipticCurvePrivateKey,)
+
+    CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (ec.EllipticCurvePublicKey,)
 
     PARAMS: Mapping[str, JwkParameter] = {
         "crv": JwkParameter("Curve", is_private=False, is_required=True, kind="name"),
         "x": JwkParameter(
             "X Coordinate", is_private=False, is_required=True, kind="b64u"
         ),
         "y": JwkParameter(
@@ -66,256 +71,195 @@
 
     KEY_MANAGEMENT_ALGORITHMS: Mapping[str, Type[EcdhEs]] = {
         keyalg.name: keyalg
         for keyalg in [EcdhEs, EcdhEs_A128KW, EcdhEs_A192KW, EcdhEs_A256KW]
     }
 
     @property
-    def is_private(self) -> bool:  # noqa: D102
+    @override
+    def is_private(self) -> bool:
         return "d" in self
 
+    @override
     def _validate(self) -> None:
         self.get_curve(self.crv)
         super()._validate()
 
     @classmethod
     def get_curve(cls, crv: str) -> EllipticCurve:
         """Get the EllipticCurve instance for a given curve identifier.
 
         Args:
           crv: the curve identifier
 
         Returns:
-            the matching EllipticCurve instance
+            the matching `EllipticCurve` instance
 
         Raises:
             UnsupportedEllipticCurve: if the curve identifier is not supported
 
         """
         curve = cls.CURVES.get(crv)
         if curve is None:
             raise UnsupportedEllipticCurve(crv)
         return curve
 
     @property
     def curve(self) -> EllipticCurve:
-        """Get the EllipticCurve instance for this key.
+        """Get the `EllipticCurve` instance for this key.
 
         Returns:
-            the EllipticCurve instance
+            the `EllipticCurve` instance
 
         """
         return self.get_curve(self.crv)
 
     @classmethod
-    def public(cls, crv: str, x: int, y: int, **params: str) -> "ECJwk":
-        """Initialize a public ECJwk from its public parameters.
+    def public(cls, *, crv: str, x: int, y: int, **params: str) -> ECJwk:
+        """Initialize a public `ECJwk` from its public parameters.
 
         Args:
           crv: the curve to use
           x: the x coordinate
           y: the y coordinate
           **params: additional member to include in the Jwk
 
         Returns:
           an ECJwk initialized with the supplied parameters
 
         """
         coord_size = cls.get_curve(crv).coordinate_size
         return cls(
             dict(
-                key="EC",
+                kty=cls.KTY,
                 crv=crv,
-                x=BinaPy.from_int(x, length=coord_size).to("b64u"),
-                y=BinaPy.from_int(y, length=coord_size).to("b64u"),
+                x=BinaPy.from_int(x, length=coord_size).to("b64u").ascii(),
+                y=BinaPy.from_int(y, length=coord_size).to("b64u").ascii(),
                 **{k: v for k, v in params.items() if v is not None},
             )
         )
 
     @classmethod
-    def private(cls, crv: str, x: int, y: int, d: int, **params: Any) -> "ECJwk":
+    def private(cls, *, crv: str, x: int, y: int, d: int, **params: Any) -> ECJwk:
         """Initialize a private ECJwk from its private parameters.
 
         Args:
           crv: the curve to use
           x: the x coordinate
           y: the y coordinate
           d: the elliptic curve private key
           **params: additional members to include in the JWK
 
         Returns:
-          an ECJWk initialized with the supplied parameters
+          an ECJwk initialized with the supplied parameters
 
         """
         coord_size = cls.get_curve(crv).coordinate_size
         return cls(
             dict(
-                kty="EC",
+                kty=cls.KTY,
                 crv=crv,
                 x=BinaPy.from_int(x, coord_size).to("b64u").ascii(),
                 y=BinaPy.from_int(y, coord_size).to("b64u").ascii(),
                 d=BinaPy.from_int(d, coord_size).to("b64u").ascii(),
                 **{k: v for k, v in params.items() if v is not None},
             )
         )
 
-    @property
-    def coordinate_size(self) -> int:
-        """The coordinate size to use with the key curve.
+    @classmethod
+    @override
+    def generate(
+        cls, *, crv: Optional[str] = None, alg: Optional[str] = None, **kwargs: Any
+    ) -> ECJwk:
+        curve: EllipticCurve = P_256
 
-        Returns:
-          32, 48, or 66 (bits)
+        if crv is None and alg is None:
+            raise ValueError(
+                "No Curve identifier (crv) or Algorithm identifier (alg) have been provided "
+                "when generating an Elliptic Curve JWK. So there is no hint to determine which curve to use. "
+                "You must explicitly pass an 'alg' or 'crv' parameter to select the appropriate Curve."
+            )
+        elif crv:
+            curve = cls.get_curve(crv)
+        elif alg:
+            if alg in cls.SIGNATURE_ALGORITHMS:
+                curve = cls.SIGNATURE_ALGORITHMS[alg].curve
+            elif alg in cls.KEY_MANAGEMENT_ALGORITHMS:
+                warnings.warn(
+                    "No Curve identifier (crv) specified when generating an Elliptic Curve Jwk for Key Management. "
+                    "Curve 'P-256' is used by default. You should explicitly pass a 'crv' parameter "
+                    "to select the appropriate Curve and avoid this warning."
+                )
+            else:
+                raise UnsupportedAlg(alg)
 
-        """
-        return self.curve.coordinate_size
+        x, y, d = curve.generate()
+        return cls.private(
+            crv=curve.name,
+            alg=alg,
+            x=x,
+            y=y,
+            d=d,
+            **kwargs,
+        )
 
     @classmethod
+    @override
     def from_cryptography_key(cls, cryptography_key: Any, **kwargs: Any) -> ECJwk:
-        """Initialize an ECJwk from a `cryptography` key.
-
-        Args:
-          cryptography_key: `cryptography` key
-          **kwargs: additional members to include in the Jwk
-
-        Returns:
-            an ECJwk initialized from the provided `cryptography` key
-
-        """
         parameters = EllipticCurve.get_jwk_parameters(cryptography_key)
         return cls(parameters)
 
+    @override
     def _to_cryptography_key(
         self,
-    ) -> Union[
-        asymmetric.ec.EllipticCurvePrivateKey,
-        asymmetric.ec.EllipticCurvePublicKey,
-    ]:
-        """Initialize a `cryptography` key based on this Jwk.
-
-        Returns:
-            an EllipticCurvePublicKey or EllipticCurvePrivateKey
-
-        """
+    ) -> Union[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey,]:
         if self.is_private:
-            return asymmetric.ec.EllipticCurvePrivateNumbers(
+            return ec.EllipticCurvePrivateNumbers(
                 private_value=self.ecc_private_key,
-                public_numbers=asymmetric.ec.EllipticCurvePublicNumbers(
+                public_numbers=ec.EllipticCurvePublicNumbers(
                     x=self.x_coordinate,
                     y=self.y_coordinate,
                     curve=self.curve.cryptography_curve,
                 ),
             ).private_key()
         else:
-            return asymmetric.ec.EllipticCurvePublicNumbers(
+            return ec.EllipticCurvePublicNumbers(
                 x=self.x_coordinate,
                 y=self.y_coordinate,
                 curve=self.curve.cryptography_curve,
             ).public_key()
 
-    @classmethod
-    def generate(
-        cls, crv: Optional[str] = None, alg: Optional[str] = None, **params: str
-    ) -> "ECJwk":
-        """Generate a random ECJwk.
-
-        Args:
-          alg: the alg
-          crv: the curve to use
-          **params:
-
-        Returns:
-          a generated ECJwk
-
-        Raises:
-            UnsupportedEllipticCurve: if the provided curve identifier is not supported.
-
-        """
-        if crv is None and alg is None:
-            warnings.warn(
-                "No Curve identifier (crv) or an Algorithm identifier (alg) have been provided "
-                "when generating an Elliptic Curve JWK. So there is no hint to determine which curve to use. "
-                "Curve 'P-256' is used by default. You should explicitly pass an 'alg' or 'crv' parameter "
-                "to explicitly select the appropriate Curve and avoid this warning."
-            )
-            crv = "P-256"
-        curve: Optional[EllipticCurve] = None
-        if crv:
-            curve = cls.get_curve(crv)
-        elif alg:
-            if alg in cls.SIGNATURE_ALGORITHMS:
-                curve = cls.SIGNATURE_ALGORITHMS[alg].curve
-            elif alg in cls.KEY_MANAGEMENT_ALGORITHMS:
-                curve = P_256
-
-        if curve is None:
-            raise UnsupportedEllipticCurve(crv)
-
-        x, y, d = curve.generate()
-        return cls.private(
-            crv=curve.name,
-            alg=alg,
-            x=x,
-            y=y,
-            d=d,
-            **params,
-        )
+    @property
+    def coordinate_size(self) -> int:
+        """The coordinate size to use with the key curve. This is 32, 48, or 66 bits."""
+        return self.curve.coordinate_size
 
     @cached_property
     def x_coordinate(self) -> int:
-        """Return the x coordinate from this ECJwk.
-
-        Returns:
-         the x coordinate (from parameter `x`)
-
-        """
+        """Return the *x coordinate*, parameter `x` from this `ECJwk`."""
         return BinaPy(self.x).decode_from("b64u").to_int()
 
     @cached_property
     def y_coordinate(self) -> int:
-        """Return the y coordinate from this ECJwk.
-
-        Returns:
-            the y coordinate (from parameter `y`)
-
-        """
+        """Return the *y coordinate*, parameter `y` from this `ECJwk`."""
         return BinaPy(self.y).decode_from("b64u").to_int()
 
     @cached_property
     def ecc_private_key(self) -> int:
-        """Return the ECC private key from this ECJwk.
-
-        Returns:
-             the ECC private key (from parameter `d`)
-
-        """
+        """Return the *ECC private key*, parameter `d` from this `ECJwk`."""
         return BinaPy(self.d).decode_from("b64u").to_int()
 
+    @override
     def supported_signing_algorithms(self) -> List[str]:
-        """Return the list of supported signature algorithms for this key.
-
-        Returns:
-            a list of supported algorithms identifiers
-
-        """
         return [
             name
             for name, alg in self.SIGNATURE_ALGORITHMS.items()
             if alg.curve == self.curve
         ]
 
+    @override
     def supported_key_management_algorithms(self) -> List[str]:
-        """Return the list of supported Key Management algorithms for this key.
-
-        Returns:
-             a list of supported algorithms identifiers
-
-        """
         return list(self.KEY_MANAGEMENT_ALGORITHMS)
 
+    @override
     def supported_encryption_algorithms(self) -> List[str]:
-        """Return the list of support Encryption algorithms for this key.
-
-        Returns:
-             a list of supported algorithms identifiers
-
-        """
         return list(self.ENCRYPTION_ALGORITHMS)
```

### Comparing `jwskate-0.6.0/jwskate/jwk/jwks.py` & `jwskate-0.7.0/jwskate/jwk/jwks.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,15 @@
 
         Returns:
           the kid from the added Jwk (it may be generated if no kid is provided)
 
         """
         jwk = to_jwk(jwk)
 
-        if "keys" not in self:
-            self["keys"] = []
+        self.setdefault("keys", [])
 
         kid = jwk.get("kid", kid)
         if not kid:
             kid = jwk.thumbprint()
         jwk["kid"] = kid
         use = jwk.get("use", use)
         if use:
@@ -145,37 +144,53 @@
 
         Returns:
             a public JwkSet
 
         """
         return JwkSet(keys=(key.public_jwk() for key in self.jwks))
 
+    def verification_keys(self) -> List[Jwk]:
+        """Return the list of keys from this JWKS that are usable for signature verification.
+
+        To be usable for signature verification, a key must:
+
+        - be asymmetric
+        - be public
+        - be flagged for signature, either with `use=sig` or an `alg` that is compatible with signature
+
+        Returns:
+            a list of `Jwk` that are usable for signature verification
+
+        """
+        return [
+            jwk
+            for jwk in self.jwks
+            if not jwk.is_symmetric and not jwk.is_private and jwk.use == "sig"
+        ]
+
     def verify(
         self,
         data: bytes,
         signature: bytes,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
         kid: Optional[str] = None,
     ) -> bool:
-        """Verify a signature with the key from this key set.
+        """Verify a signature with the keys from this key set.
 
-        It implements multiple techniques to avoid trying all keys:
-        If a `kid` is provided, only the key with this `kid` will be tried.
-        Otherwise, if an `alg` or several `algs` are provided, only keys that are compatible with the supplied `alg` will be tried.
-        Otherwise, keys that have use = signature will be tried.
-        And if the signature is still not verified at that point, the keys with no specified alg and use will be tried.
+        If a `kid` is provided, only that Key ID will be tried. Otherwise, all keys that are compatible with the
+        specified alg(s) will be tried.
 
         Args:
           data: the signed data to verify
           signature: the signature to verify against the signed data
           alg: alg to verify the signature, if there is only 1
           algs: list of allowed signature algs, if there are several
           kid: the kid of the Jwk that will be used to validate the signature. If no kid is provided, multiple keys
-        from this key set may be tried.
+            from this key set may be tried.
 
         Returns:
           `True` if the signature validates with any of the tried keys, `False` otherwise
 
         """
         if not alg and not algs:
             raise ValueError("Please provide either 'alg' or 'algs' parameter")
@@ -197,39 +212,22 @@
                 if alg in jwk.supported_signing_algorithms():
                     if jwk.verify(data, signature, alg=alg):
                         return True
 
         # no key matches, so consider the signature invalid
         return False
 
-    def verification_keys(self) -> List[Jwk]:
-        """Return the list of keys from this JWKS that a usable for signature verification.
-
-        To be usable for signature verification, a key must:
-        - be asymmetric
-        - be public
-        - have an "alg" parameter that is a signature alg
-
-        Returns:
-            a list of `Jwk` that are usable for signature verification
-
-        """
-        return [
-            jwk
-            for jwk in self.jwks
-            if not jwk.is_symmetric and not jwk.is_private and jwk.use == "sig"
-        ]
-
     def encryption_keys(self) -> List[Jwk]:
         """Return the list of keys from this JWKS that are usable for encryption.
 
         To be usable for encryption, a key must:
+
         - be asymmetric
         - be public
-        - have an "alg" parameter that is an encryption alg
+        - be flagged for encryption, either with `use=enc` or an `alg` parameter that is an encryption alg
 
         Returns:
             a list of `Jwk` that are suitable for encryption
 
         """
         return [
             jwk
```

### Comparing `jwskate-0.6.0/jwskate/jwk/okp.py` & `jwskate-0.7.0/jwskate/jwk/okp.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,47 +2,51 @@
 
 [RFC8037]: https://www.rfc-editor.org/rfc/rfc8037.html
 
 """
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import Any, Mapping, Optional
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519, x448, x25519
+from typing_extensions import override
 
 from jwskate.jwa import (
     X448,
     X25519,
     EcdhEs,
     EcdhEs_A128KW,
     EcdhEs_A192KW,
     EcdhEs_A256KW,
     Ed448,
     Ed25519,
     EdDsa,
     OKPCurve,
 )
-from jwskate.jwa.okp import PrivateKeyProtocol, PublicKeyProtocol
 
+from .. import KeyTypes
 from .alg import UnsupportedAlg
 from .base import Jwk, JwkParameter
 
 
 class UnsupportedOKPCurve(KeyError):
     """Raised when an unsupported OKP curve is requested."""
 
 
 class OKPJwk(Jwk):
-    """Represent an OKP Jwk, with `kty=OKP`."""
+    """Represent an Octet Key Pair keys in JWK format.
 
-    KTY = "OKP"
+    Octet Key Pair keys have Key Type `"OKP"`.
+    """
+
+    KTY = KeyTypes.OKP
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (
         ed25519.Ed25519PrivateKey,
         ed448.Ed448PrivateKey,
         x25519.X25519PrivateKey,
         x448.X448PrivateKey,
     )
@@ -72,210 +76,181 @@
 
     KEY_MANAGEMENT_ALGORITHMS = {
         keyalg.name: keyalg
         for keyalg in [EcdhEs, EcdhEs_A128KW, EcdhEs_A192KW, EcdhEs_A256KW]
     }
 
     @property
-    def is_private(self) -> bool:  # noqa: D102
+    @override
+    def is_private(self) -> bool:
         return "d" in self
 
+    @override
     def _validate(self) -> None:
         if not isinstance(self.crv, str) or self.crv not in self.CURVES:
             raise UnsupportedOKPCurve(self.crv)
         super()._validate()
 
     @classmethod
     def get_curve(cls, crv: str) -> OKPCurve:
-        """Get the OKPCurve instance from a curve identifier.
+        """Get the `OKPCurve` instance from a curve identifier.
 
         Args:
-          crv: a crv identifier
+          crv: a curve identifier
 
         Returns:
-            the matching OKPCurve instance
+            the matching `OKPCurve` instance
 
         Raises:
             UnsupportedOKPCurve: if the curve is not supported
 
         """
         curve = cls.CURVES.get(crv)
         if curve is None:
             raise UnsupportedOKPCurve(crv)
         return curve
 
     @property
     def curve(self) -> OKPCurve:
-        """Get the OKPCurve instance for this key.
-
-        Returns:
-            the OKPCurve for this key
-
-        """
+        """Get the `OKPCurve` instance for this key."""
         return self.get_curve(self.crv)
 
     @cached_property
     def public_key(self) -> bytes:
-        """Get the public key from this Jwk.
-
-        Returns:
-            the public key (from param `x`)
-
-        """
+        """Get the public key from this `Jwk`, from param `x`, base64url-decoded."""
         return BinaPy(self.x).decode_from("b64u")
 
     @cached_property
     def private_key(self) -> bytes:
-        """Get the private key from this Jwk.
-
-        Returns:
-            the private key (from param `d`)
-
-        """
+        """Get the private key from this `Jwk`, from param `d`, base64url-decoded."""
         return BinaPy(self.d).decode_from("b64u")
 
     @classmethod
     def from_bytes(
         cls,
         private_key: bytes,
         crv: Optional[str] = None,
         use: Optional[str] = None,
         **kwargs: Any,
     ) -> OKPJwk:
-        """Initialize an `OKPJwk` from its private key.
+        """Initialize an `OKPJwk` from its private key, as `bytes`.
 
-        The public key will be automatically derived from the supplied private key,
+        The public key will be automatically derived from the supplied private key, according to the OKP curve.
 
         The appropriate curve will be guessed based on the key length or supplied `crv`/`use` hints:
-        - 56 bytes will use X448
-        - 57 bytes will use Ed448
-        - 32 bytes will use Ed25519 or X25519. Since there is no way to guess which one you want, it needs an hint with either a `crv` or `use` parameter.
+
+        - 56 bytes will use `X448`
+        - 57 bytes will use `Ed448`
+        - 32 bytes will use `Ed25519` or `X25519`. Since there is no way to guess which one you want,
+          it needs a hint with either a `crv` or `use` parameter.
 
         Args:
-            private_key: the 32, 56 or 57 bytes private key, as raw bytes
-            crv: the curve to use
+            private_key: the 32, 56 or 57 bytes private key, as raw `bytes`
+            crv: the curve identifier to use
             use: the key usage
-            **kwargs: additional members to include in the Jwk
+            **kwargs: additional members to include in the `Jwk`
 
         Returns:
-            the matching OKPJwk
+            the matching `OKPJwk`
 
         """
         if crv and use:
             if (crv in ("Ed25519", "Ed448") and use != "sig") or (
                 crv in ("X25519", "X448") and use != "enc"
             ):
                 raise ValueError(
-                    f"Inconsistent `crv={crv}` and `use={use}` parameters."
+                    f"Inconsistent `crv={crv}` and `use={use}` parameters. "
+                    "Ed25519 and Ed448 are used for signing (use='sig'). "
+                    "X25519 and X448 are used for encryption (use='enc'). "
                 )
         elif crv:
             if crv in ("Ed25519", "Ed448"):
                 use = "sig"
             elif crv in ("X25519", "X448"):
                 use = "enc"
             else:
                 raise UnsupportedOKPCurve(crv)
         elif use:
             if use not in ("sig", "enc"):
-                raise ValueError(f"Invalid `use={use}` parameter, need 'sig' or 'enc'.")
+                raise ValueError(
+                    f"Invalid `use={use}` parameter, it must be either 'sig' or 'enc'."
+                )
 
         cryptography_key: Any
         if len(private_key) == 32:
             if use == "sig":
                 cryptography_key = ed25519.Ed25519PrivateKey.from_private_bytes(
                     private_key
                 )
             elif use == "enc":
                 cryptography_key = x25519.X25519PrivateKey.from_private_bytes(
                     private_key
                 )
             else:
                 raise ValueError(
-                    "You need to specify either crv={'Ed25519', 'X25519'} or use={'sig', 'enc'} when providing a 32 bytes private key."
+                    "You provided a 32 bytes private key, which is appropriate for both Ed25519 and X25519 curves. "
+                    "There is no way to guess which curve you need, "
+                    "so please specify either `crv='Ed25519'` or `use='sig'` for an Ed25519 key, "
+                    "or either `crv='X25519'` or `use='enc'` for a X25519 key."
                 )
         elif len(private_key) == 56:
             cryptography_key = x448.X448PrivateKey.from_private_bytes(private_key)
             if use and use != "enc":
                 raise ValueError(
-                    f"Invalid `use={use}` parameter. Keys of length 56 bytes are for curve X448."
+                    f"Invalid `use='{use}'` parameter. Keys of length 56 bytes are only suitable for curve 'X448'."
                 )
             use = "enc"
         elif len(private_key) == 57:
             cryptography_key = ed448.Ed448PrivateKey.from_private_bytes(private_key)
             if use and use != "sig":
                 raise ValueError(
-                    f"Invalid `use={use}` parameter. Keys of length 57 bytes are for curve Ed448."
+                    f"Invalid `use='{use}'` parameter. Keys of length 57 bytes are only suitable for curve 'Ed448'."
                 )
             use = "sig"
         else:
             raise ValueError(
-                "Invalid private key. It must be bytes of length 32, 56 or 57."
+                "Invalid private key. It must be `bytes`, of length 32, 56 or 57 bytes."
             )
 
         return OKPJwk.from_cryptography_key(cryptography_key, use=use, **kwargs)
 
     @classmethod
+    @override
     def from_cryptography_key(cls, cryptography_key: Any, **kwargs: Any) -> OKPJwk:
-        """Initialize an `OKPJwk` from a `cryptography` key.
-
-        Args:
-          cryptography_key: a `cryptography` key
-          **kwargs: additional members to include in the Jwk
-
-        Returns:
-            the matching OKPJwk
-
-        """
         crv = OKPCurve.get_curve(cryptography_key)
-        if isinstance(cryptography_key, PrivateKeyProtocol):
+        if isinstance(cryptography_key, cls.CRYPTOGRAPHY_PRIVATE_KEY_CLASSES):
             priv = cryptography_key.private_bytes(
                 encoding=serialization.Encoding.Raw,
                 format=serialization.PrivateFormat.Raw,
                 encryption_algorithm=serialization.NoEncryption(),
             )
             pub = cryptography_key.public_key().public_bytes(
                 encoding=serialization.Encoding.Raw,
                 format=serialization.PublicFormat.Raw,
             )
             return cls.private(
                 crv=crv.name,
                 x=pub,
                 d=priv,
             )
-        elif isinstance(cryptography_key, PublicKeyProtocol):
+        elif isinstance(cryptography_key, cls.CRYPTOGRAPHY_PUBLIC_KEY_CLASSES):
             pub = cryptography_key.public_bytes(
                 encoding=serialization.Encoding.Raw,
                 format=serialization.PublicFormat.Raw,
             )
             return cls.public(
                 crv=crv.name,
                 x=pub,
             )
-        else:
-            raise TypeError(
-                "Unsupported key type for OKP. Supported key types are: "
-                + ", ".join(
-                    kls.__name__
-                    for kls in (
-                        cls.CRYPTOGRAPHY_PRIVATE_KEY_CLASSES
-                        + cls.CRYPTOGRAPHY_PUBLIC_KEY_CLASSES
-                    )
-                )
-            )
+        raise TypeError(
+            "Unsupported key type", type(cryptography_key)
+        )  # pragma: no-cover
 
+    @override
     def _to_cryptography_key(self) -> Any:
-        """Intialize a `cryptography` key based on this Jwk.
-
-        Returns:
-            a Ed25519PrivateKey or a Ed25519PublicKey or a Ed448PrivateKey or a Ed448PublicKey based on the current Jwk
-
-        Raises:
-            UnsupportedOKPCurve: if this Jwk curve is not supported.
-
-        """
         if self.curve.name == "Ed25519":
             if self.is_private:
                 return ed25519.Ed25519PrivateKey.from_private_bytes(self.private_key)
             else:
                 return ed25519.Ed25519PublicKey.from_public_bytes(self.public_key)
         elif self.curve.name == "Ed448":
             if self.is_private:
@@ -292,94 +267,76 @@
                 return x448.X448PrivateKey.from_private_bytes(self.private_key)
             else:
                 return x448.X448PublicKey.from_public_bytes(self.public_key)
         else:
             raise UnsupportedOKPCurve(self.curve)  # pragma: no cover
 
     @classmethod
-    def public(cls, crv: str, x: bytes, **params: Any) -> OKPJwk:
-        """Initialize a public OKPJwk based on the provided parameters.
+    def public(cls, *, crv: str, x: bytes, **params: Any) -> OKPJwk:
+        """Initialize a public `OKPJwk` based on the provided parameters.
 
         Args:
           crv: the key curve
           x: the public key
-          **params: additional members to include in the Jwk
+          **params: additional members to include in the `Jwk`
 
         Returns:
-            the resulting OKPJwk
+            the resulting `OKPJwk`
 
         """
-        return cls(dict(kty="OKP", crv=crv, x=BinaPy(x).to("b64u").ascii(), **params))
+        return cls(dict(kty=cls.KTY, crv=crv, x=BinaPy(x).to("b64u").ascii(), **params))
 
     @classmethod
-    def private(cls, crv: str, x: bytes, d: bytes, **params: Any) -> OKPJwk:
-        """Initialize a private OKPJwk based on the provided parameters.
+    def private(cls, *, crv: str, x: bytes, d: bytes, **params: Any) -> OKPJwk:
+        """Initialize a private `OKPJwk` based on the provided parameters.
 
         Args:
           crv: the OKP curve
           x: the public key
           d: the private key
-          **params: additional members to include in the Jwk
+          **params: additional members to include in the `Jwk`
 
         Returns:
-            the resulting OKPJwk
+            the resulting `OKPJwk`
 
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 crv=crv,
                 x=BinaPy(x).to("b64u").ascii(),
                 d=BinaPy(d).to("b64u").ascii(),
                 **params,
             )
         )
 
     @classmethod
+    @override
     def generate(
-        cls, crv: Optional[str] = None, alg: Optional[str] = None, **params: Any
+        cls, *, crv: Optional[str] = None, alg: Optional[str] = None, **params: Any
     ) -> OKPJwk:
-        """Generate a private OKPJwk on a given curve.
-
-        You can specify either a curve or an algorithm identifier, or both.
-        If using an alg identifier, crv will default to Ed25519 for signature algs,
-        or X25519 for encryption algs.
-
-        Args:
-          crv: the curve to use
-          alg: algorithm to use
-          **params: additional members to include in the Jwk
-
-        Returns:
-            the resulting OKPJwk
-
-        """
         if crv:
             curve = cls.get_curve(crv)
         elif alg:
             if alg in cls.SIGNATURE_ALGORITHMS:
                 curve = Ed25519
             elif alg in cls.KEY_MANAGEMENT_ALGORITHMS:
                 curve = X25519
             else:
                 raise UnsupportedAlg(alg)
         else:
             raise ValueError(
                 "You must supply at least a Curve identifier (crv) or an Algorithm identifier (alg) "
-                "in order to generate an OKP JWK."
+                "in order to generate an OKPJwk."
             )
 
         x, d = curve.generate()
         return cls.private(crv=curve.name, x=x, d=d, alg=alg, **params)
 
     @cached_property
+    @override
     def use(self) -> Optional[str]:
-        """Return the key use.
-
-        For OKP keys, this can be directly deduced from the curve.
-
-        """
         if self.curve in (Ed25519, Ed448):
             return "sig"
         elif self.curve in (X25519, X448):
             return "enc"
-        return None  # pragma: no cover
+        raise UnsupportedOKPCurve(self.curse)  # pragma: no-cover
```

### Comparing `jwskate-0.6.0/jwskate/jwk/rsa.py` & `jwskate-0.7.0/jwskate/jwk/rsa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module implements JWK representing RSA keys."""
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import Any, Optional, Tuple, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 from cryptography.hazmat.primitives.asymmetric import rsa
+from typing_extensions import override
 
 from jwskate.jwa import (
     PS256,
     PS384,
     PS512,
     RS256,
     RS384,
@@ -18,21 +19,25 @@
     RsaEsOaep,
     RsaEsOaepSha256,
     RsaEsOaepSha384,
     RsaEsOaepSha512,
     RsaEsPcks1v1_5,
 )
 
+from .. import KeyTypes
 from .base import Jwk, JwkParameter
 
 
 class RSAJwk(Jwk):
-    """Represent a RSA Jwk, with `kty=RSA`."""
+    """Represent an RSA key in JWK format.
 
-    KTY = "RSA"
+    RSA (Rivest-Shamir-Adleman) keys have Key Type `"RSA"`.
+    """
+
+    KTY = KeyTypes.RSA
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (rsa.RSAPrivateKey,)
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (rsa.RSAPublicKey,)
 
     PARAMS = {
         "n": JwkParameter("Modulus", is_private=False, is_required=True, kind="b64u"),
         "e": JwkParameter("Exponent", is_private=False, is_required=True, kind="b64u"),
         "d": JwkParameter(
@@ -73,32 +78,21 @@
             RsaEsOaepSha256,
             RsaEsOaepSha384,
             RsaEsOaepSha512,
         ]
     }
 
     @property
-    def is_private(self) -> bool:  # noqa: D102
+    @override
+    def is_private(self) -> bool:
         return "d" in self
 
     @classmethod
+    @override
     def from_cryptography_key(cls, cryptography_key: Any, **kwargs: Any) -> RSAJwk:
-        """Initialize a Jwk from a `cryptography` RSA key.
-
-        Args:
-          cryptography_key: a `cryptography` RSA key
-          **kwargs: additional members to include in the Jwk
-
-        Returns:
-            a RSAJwk initialized with the given key
-
-        Raises:
-            TypeError: if the given key type is not supported
-
-        """
         if isinstance(cryptography_key, rsa.RSAPrivateKey):
             priv = cryptography_key.private_numbers()  # type: ignore[attr-defined]
             pub = cryptography_key.public_key().public_numbers()
             return cls.private(
                 n=pub.n,
                 e=pub.e,
                 d=priv.d,
@@ -113,61 +107,57 @@
             return cls.public(
                 n=pub.n,
                 e=pub.e,
             )
         else:
             raise TypeError("A RSAPrivateKey or a RSAPublicKey is required.")
 
+    @override
     def _to_cryptography_key(self) -> Union[rsa.RSAPrivateKey, rsa.RSAPublicKey]:
-        """Initialize a `cryptography` key based on this Jwk.
-
-        Returns:
-            a cryptography RSAPrivateKey or RSAPublicKey
-
-        """
         if self.is_private:
             return rsa.RSAPrivateNumbers(
                 self.first_prime_factor,
                 self.second_prime_factor,
                 self.private_exponent,
                 self.first_factor_crt_exponent,
                 self.second_factor_crt_exponent,
                 self.first_crt_coefficient,
                 rsa.RSAPublicNumbers(self.exponent, self.modulus),
             ).private_key()
         else:
             return rsa.RSAPublicNumbers(e=self.exponent, n=self.modulus).public_key()
 
     @classmethod
-    def public(cls, n: int, e: int, **params: Any) -> RSAJwk:
+    def public(cls, *, n: int, e: int = 65537, **params: Any) -> RSAJwk:
         """Initialize a public `RsaJwk` from a modulus and an exponent.
 
         Args:
           n: the modulus
           e: the exponent
-          **params: additional members to include in the Jwk
+          **params: additional parameters to include in the `Jwk`
 
         Returns:
-          a RsaJwk initialized from the provided parameters
+          a `RsaJwk` initialized from the provided parameters
 
         """
         return cls(
             dict(
-                kty="RSA",
+                kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 **params,
             )
         )
 
     @classmethod
     def private(
         cls,
+        *,
         n: int,
-        e: int,
+        e: int = 65537,
         d: int,
         p: Optional[int] = None,
         q: Optional[int] = None,
         dp: Optional[int] = None,
         dq: Optional[int] = None,
         qi: Optional[int] = None,
         **params: Any,
@@ -179,45 +169,50 @@
           e: the exponent
           d: the private exponent
           p: the first prime factor
           q: the second prime factor
           dp: the first factor CRT exponent
           dq: the second factor CRT exponent
           qi: the first CRT coefficient
-          **params: additional members to include in the Jwk
+          **params: additional parameters to include in the `Jwk`
 
         Returns:
-            a RSAJwk initialized from the given parameters
+            a `RSAJwk` initialized from the given parameters
 
         """
         return cls(
             dict(
-                kty="RSA",
+                kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 d=BinaPy.from_int(d).to("b64u").ascii(),
                 p=BinaPy.from_int(p).to("b64u").ascii() if p is not None else None,
                 q=BinaPy.from_int(q).to("b64u").ascii() if q is not None else None,
                 dp=BinaPy.from_int(dp).to("b64u").ascii() if dp is not None else None,
                 dq=BinaPy.from_int(dq).to("b64u").ascii() if dq is not None else None,
                 qi=BinaPy.from_int(qi).to("b64u").ascii() if qi is not None else None,
                 **params,
             )
         )
 
+    @cached_property
+    def key_size(self) -> int:
+        """Key size, in bits."""
+        return len(BinaPy(self.n).decode_from("b64u")) * 8
+
     @classmethod
     def generate(cls, key_size: int = 4096, **params: Any) -> RSAJwk:
         """Generate a new random private `RSAJwk`.
 
         Args:
           key_size: the key size to use for the generated key, in bits
-          **params: additional members to include in the Jwk
+          **params: additional parameters to include in the `Jwk`
 
         Returns:
-          a generated RSAJwk
+          a generated `RSAJwk`
 
         """
         private_key = rsa.generate_private_key(65537, key_size=key_size)
         pn = private_key.private_numbers()
         return cls.private(
             n=pn.public_numbers.n,
             e=pn.public_numbers.e,
@@ -228,125 +223,76 @@
             dq=pn.dmq1,
             qi=pn.iqmp,
             **params,
         )
 
     @cached_property
     def modulus(self) -> int:
-        """Return the modulus `n` from this Jwk.
-
-        Returns:
-            the key modulus (from parameter `n`)
-
-        """
+        """Return the modulus `n` from this `Jwk`."""
         return BinaPy(self.n).decode_from("b64u").to_int()
 
     @cached_property
     def exponent(self) -> int:
-        """Return the public exponent `e` from this Jwk.
-
-        Returns:
-            the key exponent (from parameter `e`)
-
-        """
+        """Return the public exponent `e` from this `Jwk`."""
         return BinaPy(self.e).decode_from("b64u").to_int()
 
     @cached_property
     def private_exponent(self) -> int:
-        """Return the private exponent `d` from this Jwk.
-
-        Returns:
-            the key private exponent (from parameter `d`)
-
-        """
+        """Return the private exponent `d` from this `Jwk`."""
         return BinaPy(self.d).decode_from("b64u").to_int()
 
     @cached_property
-    def first_prime_factor(self) -> int:
-        """Return the first prime factor `p` from this Jwk.
-
-        Returns:
-            the first prime factor (from parameter `p`)
-
-        """
-        return self.prime_factors[0]
-
-    @cached_property
-    def second_prime_factor(self) -> int:
-        """Return the second prime factor `q` from this Jwk.
-
-        Returns:
-            the second prime factor (from parameter `q`)
-
-        """
-        return self.prime_factors[1]
-
-    @cached_property
     def prime_factors(self) -> Tuple[int, int]:
-        """Return the 2 prime factors `p` and `q` from this Jwk."""
+        """Return the 2 prime factors `p` and `q` from this `Jwk`."""
         if "p" not in self or "q" not in self:
             p, q = rsa.rsa_recover_prime_factors(
                 self.modulus, self.exponent, self.private_exponent
             )
             return (p, q) if p < q else (q, p)
         return (
             BinaPy(self.p).decode_from("b64u").to_int(),
             BinaPy(self.q).decode_from("b64u").to_int(),
         )
 
     @cached_property
-    def first_factor_crt_exponent(self) -> int:
-        """Return the first factor CRT exponent `dp` from this Jwk.
+    def first_prime_factor(self) -> int:
+        """Return the first prime factor `p` from this `Jwk`."""
+        return self.prime_factors[0]
 
-        Returns:
-            the first factor CRT coefficient (from parameter `dp`)
+    @cached_property
+    def second_prime_factor(self) -> int:
+        """Return the second prime factor `q` from this `Jwk`."""
+        return self.prime_factors[1]
 
-        """
+    @cached_property
+    def first_factor_crt_exponent(self) -> int:
+        """Return the first factor CRT exponent `dp` from this `Jwk`."""
         if "dp" in self:
             return BinaPy(self.dp).decode_from("b64u").to_int()
         return rsa.rsa_crt_dmp1(self.private_exponent, self.first_prime_factor)
 
     @cached_property
     def second_factor_crt_exponent(self) -> int:
-        """Return the second factor CRT exponent `dq` from this Jwk.
-
-        Returns:
-            the second factor CRT coefficient (from parameter `dq`)
-
-        """
+        """Return the second factor CRT exponent `dq` from this `Jwk`."""
         if "dq" in self:
             return BinaPy(self.dq).decode_from("b64u").to_int()
         return rsa.rsa_crt_dmq1(self.private_exponent, self.second_prime_factor)
 
     @cached_property
     def first_crt_coefficient(self) -> int:
-        """Return the first CRT coefficient `qi` from this Jwk.
-
-        Returns:
-            the first CRT coefficient (from parameter `qi`)
-
-        """
+        """Return the first CRT coefficient `qi` from this `Jwk`."""
         if "qi" in self:
             return BinaPy(self.qi).decode_from("b64u").to_int()
         return rsa.rsa_crt_iqmp(self.first_prime_factor, self.second_prime_factor)
 
-    @cached_property
-    def key_size(self) -> int:
-        """Key size, in bits.
-
-        Returns:
-            the key size
-
-        """
-        return len(BinaPy(self.n).decode_from("b64u")) * 8
-
     def with_optional_private_parameters(self) -> RSAJwk:
-        """Compute the optional RSA private parameters and add them into the JWK.
+        """Compute the optional RSA private parameters and return a new `Jwk` with those additional params included.
 
         The optional parameters are:
+
         - p: first prime factor
         - q: second prime factor
         - dp: first factor Chinese Remainder Theorem exponent
         - dq: second factor Chinese Remainder Theorem exponent
         - qi: first Chinese Remainder Theorem coefficient
 
         """
@@ -370,13 +316,13 @@
                 "qi": BinaPy.from_int(self.first_crt_coefficient).to("b64u").ascii(),
             }
         )
 
         return RSAJwk(jwk)
 
     def without_optional_private_parameters(self) -> RSAJwk:
-        """Remove the optional private parameters and return another Jwk instance without them."""
+        """Remove the optional private parameters and return another `Jwk` instance without them."""
         jwk = dict(self)
         for param in "p", "q", "dp", "dq", "qi":
             jwk.pop(param, None)
 
         return RSAJwk(jwk)
```

### Comparing `jwskate-0.6.0/jwskate/jws/compact.py` & `jwskate-0.7.0/jwskate/jws/compact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module implements the JWS Compact format."""
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, SupportsBytes, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 
 from jwskate.jwk.base import Jwk, to_jwk
 from jwskate.token import BaseCompactToken
 
 from .signature import JwsSignature
```

### Comparing `jwskate-0.6.0/jwskate/jws/json.py` & `jwskate-0.7.0/jwskate/jws/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module implement the JWS JSON flat and general formats."""
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 
 from jwskate.jwk.base import Jwk
 from jwskate.token import BaseJsonDict
 
 from .compact import JwsCompact
 from .signature import JwsSignature
```

### Comparing `jwskate-0.6.0/jwskate/jws/signature.py` & `jwskate-0.7.0/jwskate/jws/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module implement JWS signatures."""
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import Any, Dict, Iterable, Mapping, Optional, Type, TypeVar, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 
 from jwskate.jwk import Jwk, to_jwk
 from jwskate.token import BaseJsonDict
 
 S = TypeVar("S", bound="JwsSignature")
 
@@ -64,15 +64,15 @@
         Raises:
             AttributeError: if this signature doesn't have protected headers.
 
         """
         protected = self.get("protected")
         if protected is None:
             raise AttributeError("This Jws JSON does not contain a 'protected' member")
-        return BinaPy(protected).decode_from("b64u").parse_from("json")  # type: ignore
+        return BinaPy(protected).decode_from("b64u").parse_from("json")  # type: ignore[no-any-return]
 
     @property
     def header(self) -> Any:
         """The unprotected header, unaltered.
 
         Returns:
             The unprotected header
```

### Comparing `jwskate-0.6.0/jwskate/jwt/base.py` & `jwskate-0.7.0/jwskate/jwt/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class InvalidJwt(ValueError):
     """Raised when an invalid Jwt is parsed."""
 
 
 class Jwt(BaseCompactToken):
     """Represents a Json Web Token."""
 
-    def __new__(cls, value: Union[bytes, str]):  # type: ignore
+    def __new__(cls, value: Union[bytes, str]) -> Union[SignedJwt, JweCompact, Jwt]:  # type: ignore[misc]
         """Allow parsing both Signed and Encrypted JWTs.
 
         This returns the appropriate subclass or instance depending on the number of dots (.) in the serialized JWT.
 
         Args:
             value: the token value
 
@@ -39,24 +39,25 @@
                 from .signed import SignedJwt
 
                 return super().__new__(SignedJwt)
             elif value.count(b".") == 4:
                 from ..jwe import JweCompact
 
                 return JweCompact(value)
+
         return super().__new__(cls)
 
     @classmethod
     def sign(
         cls,
         claims: Dict[str, Any],
         jwk: Union[Jwk, Dict[str, Any]],
         alg: Optional[str] = None,
         extra_headers: Optional[Dict[str, Any]] = None,
-    ) -> "SignedJwt":
+    ) -> SignedJwt:
         """Sign a JSON payload with a `Jwk` and returns the resulting `SignedJwt`.
 
         This method cannot generate a token without a signature. If you want to use an unsigned token (with alg=none),
         use `.unprotected()` instead.
 
         Args:
           claims: the payload to sign
@@ -89,15 +90,15 @@
         return SignedJwt(b".".join((signed_value, signature)))
 
     @classmethod
     def unprotected(
         cls,
         claims: Dict[str, Any],
         extra_headers: Optional[Dict[str, Any]] = None,
-    ) -> "SignedJwt":
+    ) -> SignedJwt:
         """Generate a JWT that is not signed and not encrypted (with alg=none).
 
         Args:
           claims: the claims to set in the token.
           extra_headers: additional headers to insert in the token.
 
         Returns:
```

### Comparing `jwskate-0.6.0/jwskate/jwt/signed.py` & `jwskate-0.7.0/jwskate/jwt/signed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This modules contains classes and utilities to generate and validate signed JWT."""
 
 from datetime import datetime, timedelta, timezone
+from functools import cached_property
 from typing import Any, Dict, Iterable, List, Optional, Union
 
-from backports.cached_property import cached_property
 from binapy import BinaPy
 
 from jwskate.jwk import Jwk, to_jwk
 
 from .base import InvalidJwt, Jwt
 
 
@@ -114,15 +114,15 @@
         exp = self.expires_at
         if exp is None:
             return None
         return exp < (datetime.now(timezone.utc) + timedelta(seconds=leeway))
 
     @cached_property
     def expires_at(self) -> Optional[datetime]:
-        """Get the "Expires At" (exp) date from this token.
+        """Get the *Expires At* (`exp`) date from this token.
 
         Returns:
           a `datetime` initialized from the `exp` claim, or `None` if there is no `exp` claim
 
         Raises:
             AttributeError: if the `exp` claim cannot be parsed to a date
 
@@ -134,15 +134,15 @@
             exp_dt = Jwt.timestamp_to_datetime(exp)
             return exp_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `exp `claim", exp)
 
     @cached_property
     def issued_at(self) -> Optional[datetime]:
-        """Get the "Issued At" (iat) date from this token.
+        """Get the *Issued At* (`iat`) date from this token.
 
         Returns:
           a `datetime` initialized from the `iat` claim, or `None` if there is no `iat` claim
 
         Raises:
             AttributeError: if the `iss` claim cannot be parsed to a date
 
@@ -154,15 +154,15 @@
             iat_dt = Jwt.timestamp_to_datetime(iat)
             return iat_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `iat `claim", iat)
 
     @cached_property
     def not_before(self) -> Optional[datetime]:
-        """Get the "Not Before" (nbf) date from this token.
+        """Get the *Not Before* (nbf) date from this token.
 
         Returns:
           a `datetime` initialized from the `nbf` claim, or `None` if there is no `nbf` claim
 
         Raises:
             AttributeError: if the `nbf` claim cannot be parsed to a date
 
@@ -174,15 +174,15 @@
             nbf_dt = Jwt.timestamp_to_datetime(nbf)
             return nbf_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `nbf `claim", nbf)
 
     @cached_property
     def issuer(self) -> Optional[str]:
-        """Get the Issuer (iss) claim from this token.
+        """Get the *Issuer* (`iss`) claim from this token.
 
         Returns:
           the issuer, as `str`, or `None` if there is no `ìss` claim
 
         Raises:
             AttributeError: if the `ìss` claim value is not a string
 
@@ -190,15 +190,15 @@
         iss = self.get_claim("iss")
         if iss is None or isinstance(iss, str):
             return iss
         raise AttributeError("iss has an unexpected type", type(iss))
 
     @cached_property
     def audiences(self) -> List[str]:
-        """Get the audience(s) (aud) claim from this token.
+        """Get the *Audience(s)* (`aud`) claim from this token.
 
         If this token has a single audience, this will return a `list` anyway.
 
         Returns:
             the list of audiences from this token, from the `aud` claim.
 
         Raises:
@@ -212,15 +212,15 @@
             return [aud]
         if isinstance(aud, list):
             return aud
         raise AttributeError("aud has an unexpected type", type(aud))
 
     @cached_property
     def subject(self) -> Optional[str]:
-        """Get the Subject (sub) from this token claims.
+        """Get the *Subject* (`sub`) from this token.
 
         Returns:
           the subject, as `str`, or `None` if there is no `sub` claim
 
         Raises:
             AttributeError: if the `sub` value is not a string
 
@@ -228,43 +228,43 @@
         sub = self.get_claim("sub")
         if sub is None or isinstance(sub, str):
             return sub
         raise AttributeError("sub has an unexpected type", type(sub))
 
     @cached_property
     def jwt_token_id(self) -> Optional[str]:
-        """Get the JWT Token ID (jti) from this token claims.
+        """Get the *JWT Token ID* (`jti`) from this token.
 
         Returns:
           the token identifier, as `str`, or `None` if there is no `jti` claim
 
         Raises:
           AttributeError: if the `jti` value is not a string
 
         """
         jti = self.get_claim("jti")
         if jti is None or isinstance(jti, str):
             return jti
         raise AttributeError("jti has an unexpected type", type(jti))
 
     def get_claim(self, key: str, default: Any = None) -> Any:
-        """Get a claim from this Jwt.
+        """Get a claim by name from this Jwt.
 
         Args:
           key: the claim name.
           default: a default value if the claim is not found
 
         Returns:
           the claim value if found, or `default` if not found
 
         """
         return self.claims.get(key, default)
 
     def __getitem__(self, item: str) -> Any:
-        """Allow claim access with subscription.
+        """Allow access to claim by name with subscription.
 
         Args:
           item: the claim name
 
         Returns:
          the claim value
```

### Comparing `jwskate-0.6.0/jwskate/token.py` & `jwskate-0.7.0/jwskate/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module contains base classes for all tokens types handled by `jwskate`."""
 import json
+from functools import cached_property
 from typing import Any, Dict, Type, TypeVar, Union
 
-from backports.cached_property import cached_property
-
 
 class BaseCompactToken:
     """Base class for all tokens in Compact representation.
 
     This includes JWS, JWE, and JWT tokens.
 
     Args:
```

### Comparing `jwskate-0.6.0/pyproject.toml` & `jwskate-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 [tool]
 [tool.poetry]
 name = "jwskate"
-version = "0.6.0"
+version = "0.7.0"
 homepage = "https://github.com/guillp/jwskate"
 description = "A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "jwskate" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<3.12"
 cryptography = ">=3.4"
 typing-extensions = ">=4.3.0"
-"backports.cached-property" = "^1"
 binapy = "^0.6.0"
+mypy = "^1.1.1"
 
 [tool.poetry.dev-dependencies]
 black  = ">=22"
 coverage = ">=6.0"
 freezegun = "^1.2.2"
-isort  = ">=5.0"
+isort  = ">=5.11.5"
 jwcrypto = ">=1.0"
 livereload = ">=2.0"
 mypy = ">=0.990"
 mkdocs  = ">=1.4.2"
 mkdocstrings = { version = ">=0.18.0", extras = ["python"] }
 mkdocs-autorefs = ">=0.4"
-mkdocs-include-markdown-plugin  = ">=3.9.1"
+mkdocs-include-markdown-plugin  = ">=4.0.4"
 mkdocs-material  = ">=8.5.8"
 mkdocs-material-extensions  = ">=1.1"
 pip  = ">=22.0"
-pre-commit = ">=2.12.0"
+pre-commit = ">=2.21.0"
 pytest  = ">=7.2"
 pytest-cov  = ">=3.0"
 pytest-mypy = ">=0.9"
 requests-mock = ">=1.9"
 toml = ">=0.10"
 tox  = ">=3.25,<4.0"
 types-requests = ">=2.27"
@@ -86,27 +85,26 @@
   | build
   | dist
 )/
 '''
 
 [tool.mypy]
 strict = true
-implicit_reexport = true
 pretty = true
 show_error_context = true
 show_column_numbers = true
 show_error_codes = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 
 
 [tool.pydocstyle]
 convention = "google"
 match_dir = 'jwskate'
-
+ignore_decorators = 'override'
 
 [tool.docformatter]
 recursive = true
 wrap-summaries = 120
 wrap-descriptions = 120
 blank = true
```

### Comparing `jwskate-0.6.0/tests/conftest.py` & `jwskate-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/tests/test_jwa/test_encryption.py` & `jwskate-0.7.0/tests/test_jwa/test_encryption.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return self.payload
 
 
 @pytest.mark.parametrize(
     "alg", [A128GCM, A192GCM, A256GCM, A128CBC_HS256, A192CBC_HS384, A256CBC_HS512]
 )
 def test_encryption(alg: BaseAESEncryptionAlg) -> None:
-    jwa = alg.init_random_key()
+    jwa = alg.with_random_key()
     plaintext = b"this is a test"
     iv = alg.generate_iv()
     assert len(iv) * 8 == alg.iv_size
     ciphertext, tag = jwa.encrypt(plaintext, iv=iv)
     assert (ciphertext, tag) == jwa.encrypt(
         SupportsBytesTester(plaintext), iv=SupportsBytesTester(iv)
     )
@@ -64,7 +64,28 @@
     )
     assert jwa.decrypt(ciphertext_aad, auth_tag=tag_aad, iv=iv, aad=aad) == jwa.decrypt(
         ciphertext_aad, auth_tag=tag_aad, iv=iv, aad=SupportsBytesTester(aad)
     )
 
     with pytest.raises(MismatchingAuthTag):
         jwa.decrypt(ciphertext_aad, auth_tag=tag_aad, iv=iv)
+
+
+def test_aescbchmac() -> None:
+    key = "57b7ded6d9aafd3f3a9274d9e89cc0290865f3a404e25f8b99fe7116e509ef2e"
+    aescbchmac = A128CBC_HS256(bytes.fromhex(key))
+    assert (
+        aescbchmac.mac(bytearray(b"this_is_a_test"), iv=bytearray(b"this_is_a_test_iv"))
+        == aescbchmac.mac(b"this_is_a_test", iv=b"this_is_a_test_iv")
+        == b"\xbe\x0b$\x13}\xb3\x7fz\xa4\xa0\xc3-I\xa77K"
+    )
+    assert (
+        aescbchmac.mac(
+            bytearray(b"this_is_a_test"),
+            iv=bytearray(b"this_is_a_test_iv"),
+            aad=bytearray(b"this_is_a_test_aad"),
+        )
+        == aescbchmac.mac(
+            b"this_is_a_test", iv=b"this_is_a_test_iv", aad=b"this_is_a_test_aad"
+        )
+        == b"\xc5\xcb\xa0\xa1\xf0t\x8c\x80-\x1a\xd2Ti \x85F"
+    )
```

### Comparing `jwskate-0.6.0/tests/test_jwa/test_examples.py` & `jwskate-0.7.0/tests/test_jwa/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,30 @@
     aad = bytes.fromhex(
         (
             "54 68 65 20 73 65 63 6f 6e 64 20 70 72 69 6e 63"
             "69 70 6c 65 20 6f 66 20 41 75 67 75 73 74 65 20"
             "4b 65 72 63 6b 68 6f 66 66 73"
         ).replace(" ", "")
     )
-    al = bytes.fromhex("00 00 00 00 00 00 01 50".replace(" ", ""))  # noqa
+    al = bytes.fromhex("00 00 00 00 00 00 01 50".replace(" ", ""))  # noqa: F841
     ciphertext = bytes.fromhex(
         (
             "c8 0e df a3 2d df 39 d5 ef 00 c0 b4 68 83 42 79"
             "a2 e4 6a 1b 80 49 f7 92 f7 6b fe 54 b9 03 a9 c9"
             "a9 4a c9 b4 7a d2 65 5c 5f 10 f9 ae f7 14 27 e2"
             "fc 6f 9b 3f 39 9a 22 14 89 f1 63 62 c7 03 23 36"
             "09 d4 5a c6 98 64 e3 32 1c f8 29 35 ac 40 96 c8"
             "6e 13 33 14 c5 40 19 e8 ca 79 80 df a4 b9 cf 1b"
             "38 4c 48 6f 3a 54 c5 10 78 15 8e e5 d7 9d e5 9f"
             "bd 34 d8 48 b3 d6 95 50 a6 76 46 34 44 27 ad e5"
             "4b 88 51 ff b5 98 f7 f8 00 74 b9 47 3c 82 e2 db"
         ).replace(" ", "")
     )
 
-    mac = bytes.fromhex(  # noqa
+    mac = bytes.fromhex(  # noqa: F841
         (
             "65 2c 3f a3 6b 0a 7c 5b 32 19 fa b3 a3 0b c1 c4"
             "e6 e5 45 82 47 65 15 f0 ad 9f 75 a2 b7 1c 73 ef"
         ).replace(" ", "")
     )
 
     tag = bytes.fromhex(
@@ -111,30 +111,30 @@
     aad = bytes.fromhex(
         (
             "54 68 65 20 73 65 63 6f 6e 64 20 70 72 69 6e 63"
             "69 70 6c 65 20 6f 66 20 41 75 67 75 73 74 65 20"
             "4b 65 72 63 6b 68 6f 66 66 73"
         ).replace(" ", "")
     )
-    al = bytes.fromhex("00 00 00 00 00 00 01 50".replace(" ", ""))  # noqa
+    al = bytes.fromhex("00 00 00 00 00 00 01 50".replace(" ", ""))  # noqa: F841
     ciphertext = bytes.fromhex(
         (
             "ea 65 da 6b 59 e6 1e db 41 9b e6 2d 19 71 2a e5"
             "d3 03 ee b5 00 52 d0 df d6 69 7f 77 22 4c 8e db"
             "00 0d 27 9b dc 14 c1 07 26 54 bd 30 94 42 30 c6"
             "57 be d4 ca 0c 9f 4a 84 66 f2 2b 22 6d 17 46 21"
             "4b f8 cf c2 40 0a dd 9f 51 26 e4 79 66 3f c9 0b"
             "3b ed 78 7a 2f 0f fc bf 39 04 be 2a 64 1d 5c 21"
             "05 bf e5 91 ba e2 3b 1d 74 49 e5 32 ee f6 0a 9a"
             "c8 bb 6c 6b 01 d3 5d 49 78 7b cd 57 ef 48 49 27"
             "f2 80 ad c9 1a c0 c4 e7 9c 7b 11 ef c6 00 54 e3"
         ).replace(" ", "")
     )
 
-    mac = bytes.fromhex(  # noqa
+    mac = bytes.fromhex(  # noqa: F841
         (
             "84 90 ac 0e 58 94 9b fe 51 87 5d 73 3f 93 ac 20"
             "75 16 80 39 cc c7 33 d7 45 94 f8 86 b3 fa af d4"
             "86 f2 5c 71 31 e3 28 1e 36 c7 a2 d1 30 af de 57"
         ).replace(" ", "")
     )
```

### Comparing `jwskate-0.6.0/tests/test_jwe.py` & `jwskate-0.7.0/tests/test_jwe.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 @pytest.fixture(scope="module")
 def ec_p384_private_jwk() -> Jwk:
     return Jwk.generate_for_kty("EC", crv="P-384")
 
 
 @pytest.fixture(scope="module")
 def ec_p256_private_jwk() -> Jwk:
-    return ECJwk.generate("P-256")
+    return ECJwk.generate(crv="P-256")
 
 
 @pytest.fixture(scope="module")
 def okp_x25519_private_jwk() -> Jwk:
     return Jwk.generate_for_kty("OKP", crv="X25519")
 
 
@@ -426,15 +426,15 @@
 @pytest.fixture(
     scope="module",
     params=[
         'pAvkcJv!$N8HtIuf3W@KaF&2Gv"EAD/BK[_FEoLIuvMS*aG0tm4,.?'.encode(),
     ],
 )
 def password(request: pytest.FixtureRequest) -> bytes:
-    return request.param  # type: ignore
+    return request.param  # type: ignore[no-any-return]
 
 
 @pytest.fixture(scope="module")
 def decryption_jwk(
     key_management_alg: str,
     encryption_alg: str,
     rsa_private_jwk: Jwk,
```

### Comparing `jwskate-0.6.0/tests/test_jwk/test_alg.py` & `jwskate-0.7.0/tests/test_jwk/test_alg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from jwskate import (
     ExpectedAlgRequired,
+    MismatchingAlg,
     RSAJwk,
     UnsupportedAlg,
     select_alg_class,
     select_alg_classes,
 )
 
 
@@ -52,14 +53,20 @@
             jwk_alg="HS256",
         )
 
     # no supported algs: raise a ValueError
     with pytest.raises(ValueError):
         select_alg_class({}, alg="HS256")
 
+    # strict mode
+    with pytest.raises(MismatchingAlg):
+        select_alg_class(
+            RSAJwk.SIGNATURE_ALGORITHMS, jwk_alg="RS512", alg="RS256", strict=True
+        )
+
 
 def test_select_alg_classes() -> None:
     # selecting a single alg from the supported algs
     assert select_alg_classes(
         RSAJwk.SIGNATURE_ALGORITHMS,
         alg="RS256",
     ) == [RSAJwk.SIGNATURE_ALGORITHMS["RS256"]]
@@ -109,7 +116,16 @@
             alg="RS256",
             algs=["RS256", "RS512"],
         )
 
     # if no algs are supported, a ValueError is raised
     with pytest.raises(ValueError):
         select_alg_classes({}, alg="HS256")
+
+    # strict mode
+    with pytest.raises(MismatchingAlg):
+        select_alg_classes(
+            RSAJwk.SIGNATURE_ALGORITHMS,
+            jwk_alg="RS512",
+            algs=("RS256", "RS384"),
+            strict=True,
+        )
```

### Comparing `jwskate-0.6.0/tests/test_jwk/test_jwk.py` & `jwskate-0.7.0/tests/test_jwk/test_jwk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+import secrets
 from typing import Tuple
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from jwskate import (
     A128GCM,
     ES256,
     EcdhEs_A128KW,
+    EncryptionAlgs,
     InvalidJwk,
     Jwk,
+    KeyManagementAlgs,
     RSAJwk,
+    SignatureAlgs,
     SymmetricJwk,
     UnsupportedKeyType,
+    select_alg_class,
     to_jwk,
 )
 
 
 def test_public_jwk() -> None:
     private_jwk = Jwk.generate_for_alg("RS256")
     assert private_jwk.is_private
@@ -143,14 +148,26 @@
 def test_invalid_params() -> None:
     with pytest.raises(TypeError):
         Jwk({"kty": "oct", "k": "foobar", "alg": 1.34}).alg
 
     with pytest.raises(TypeError):
         Jwk({"kty": "oct", "k": "foobar", "kid": 1.34}).kid
 
+    with pytest.raises(InvalidJwk):
+        Jwk(
+            {
+                "kty": "EC",
+                "crv": "P-256",
+                "x": "SOlwe9_nRwz2f9Y2aSB9d7D-AXTSSBlAQd5HZUIEGLA",
+                "y": "Pzk9Gd4wwbx9STkK_RfWqxnfU9AwpvWZzf_K0GpaQZo",
+                "d": "Invalid-private-key--EHzgbRaNKRCMhk6jiCT-ZQ",
+                "alg": "ES256",
+            }
+        )
+
 
 def test_invalid_class_for_kty() -> None:
     with pytest.raises(TypeError):
         RSAJwk({"kty": "oct", "k": "foobar"})
 
 
 @pytest.mark.parametrize(
@@ -305,7 +322,91 @@
         to_jwk(GOOGLE_KEY, kty="EC")
 
     with pytest.raises(ValueError):
         to_jwk(GOOGLE_KEY, is_private=True)
 
     with pytest.raises(ValueError):
         to_jwk(GOOGLE_KEY, is_symmetric=True)
+
+
+@pytest.mark.parametrize("alg", SignatureAlgs.ALL)
+def test_sign_verify(alg: str) -> None:
+    payload = b"this_is_a_payload"
+    jwk = Jwk.generate(alg=alg)
+    signature = jwk.sign(payload)
+    if not jwk.is_symmetric:
+        assert jwk.public_jwk().verify(payload, signature)
+        with pytest.warns(match="private key"):
+            assert jwk.verify(payload, signature)
+    else:
+        assert jwk.verify(payload, signature)
+
+
+@pytest.mark.parametrize(
+    "alg",
+    KeyManagementAlgs.ALL_KEY_BASED - {KeyManagementAlgs.RSA1_5, KeyManagementAlgs.dir},
+)
+@pytest.mark.parametrize("enc", EncryptionAlgs.ALL)
+def test_sender_receiver_key(alg: str, enc: str) -> None:
+    recipient_jwk = Jwk.generate(alg=alg)
+    if recipient_jwk.is_symmetric:
+        sender_cek, wrapped_cek, extra_headers = recipient_jwk.sender_key(enc=enc)
+    else:
+        sender_cek, wrapped_cek, extra_headers = recipient_jwk.public_jwk().sender_key(
+            enc=enc
+        )
+        with pytest.warns(match="private key"):
+            recipient_jwk.sender_key(enc=enc)
+
+    if recipient_jwk.is_symmetric:
+        recipient_cek = recipient_jwk.recipient_key(
+            wrapped_cek, enc=enc, **extra_headers
+        )
+        assert sender_cek == recipient_cek
+    else:
+        with pytest.raises(ValueError):
+            recipient_jwk.public_jwk().recipient_key(
+                wrapped_cek, enc=enc, **extra_headers
+            )
+
+
+@pytest.mark.parametrize(
+    "alg", KeyManagementAlgs.ALL_AES | KeyManagementAlgs.ALL_AESGCM
+)
+@pytest.mark.parametrize("enc", EncryptionAlgs.ALL)
+def test_aeskw_with_choosen_cek(alg: str, enc: str) -> None:
+    recipient_jwk = Jwk.generate(alg=alg)
+    choosen_cek = select_alg_class(
+        SymmetricJwk.ENCRYPTION_ALGORITHMS, alg=enc
+    ).generate_key()
+
+    sender_cek, wrapped_cek, extra_headers = recipient_jwk.sender_key(
+        enc=enc, cek=choosen_cek
+    )
+    assert sender_cek.key == choosen_cek
+
+
+def test_der_pem() -> None:
+    jwk = Jwk.generate(alg="ES256")
+    password = secrets.token_urlsafe(16)
+    der = jwk.to_der(password)
+    assert Jwk.from_der(der, password) == jwk
+
+    pem = jwk.to_pem(password)
+    assert Jwk.from_pem(pem, password) == jwk
+
+    with pytest.raises(ValueError, match="public key was loaded"):
+        Jwk.from_der(jwk.public_jwk().to_der(), password=password)
+    with pytest.raises(ValueError, match="not a private or a public DER encoded key"):
+        Jwk.from_der(secrets.token_bytes(512))
+
+    with pytest.raises(ValueError, match="public key was loaded"):
+        Jwk.from_pem(jwk.public_jwk().to_pem(), password=password)
+    with pytest.raises(ValueError, match="not a private or a public PEM encoded key"):
+        Jwk.from_pem(
+            """\
+-----BEGIN PRIVATE KEY-----
+MIGHAgRandomGarbage/zrsfsdfsdfszer
+lJPkaLBw
+-----END PRIVATE KEY-----
+"""
+        )
```

### Comparing `jwskate-0.6.0/tests/test_jwk/test_jwks.py` & `jwskate-0.7.0/tests/test_jwk/test_jwks.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,7 +139,27 @@
     enc_kids = set(jwk.kid for jwk in enc_keys)
     assert enc_kids == set(
         (
             "xAgzqjWdBD8cRifXbpmcv-9vIgjKHTdjelI-Vvu0K9Q",
             "zjY2pjFnBc4rOHWEwfS5Cjyxsjo2aprsctM-4oS1r8I",
         )
     )
+
+
+def test_contains() -> None:
+    key1 = Jwk.generate_for_alg("RS256")
+    key2 = Jwk.generate_for_alg("ES256")
+
+    jwkset = JwkSet(keys=(key1, key2.public_jwk()))
+    assert key1 in jwkset.jwks
+    assert key2.public_jwk() in jwkset.jwks
+
+    assert key1.with_kid_thumbprint().with_usage_parameters() in jwkset.jwks
+    assert (
+        key2.public_jwk().with_kid_thumbprint().with_usage_parameters() in jwkset.jwks
+    )
+
+    key3 = Jwk.generate_for_alg("HS256")
+    assert key3 not in jwkset.jwks
+
+    assert key1.public_jwk() not in jwkset.jwks
+    assert key2 not in jwkset.jwks
```

### Comparing `jwskate-0.6.0/tests/test_jwk/test_okp.py` & `jwskate-0.7.0/tests/test_jwk/test_okp.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,21 @@
 
 
 def test_generate_no_crv_no_alg() -> None:
     with pytest.raises(ValueError):
         OKPJwk.generate()
 
 
-def test_generate_unsuppored_alg() -> None:
+def test_generate_unsupported() -> None:
     with pytest.raises(UnsupportedAlg):
         OKPJwk.generate(alg="foo")
 
+    with pytest.raises(UnsupportedOKPCurve):
+        OKPJwk.generate(crv="foo")
+
 
 def test_rfc8037_ed25519() -> None:
     """Test from [RFC8037][https://www.rfc-editor.org/rfc/rfc8037.html#appendix-A]."""
     jwk = Jwk(
         {
             "kty": "OKP",
             "crv": "Ed25519",
@@ -180,14 +183,17 @@
     )
 
 
 def test_unknown_curve() -> None:
     with pytest.raises(UnsupportedOKPCurve):
         Jwk({"kty": "OKP", "crv": "foobar", "x": "abcd"})
 
+    with pytest.raises(UnsupportedOKPCurve):
+        OKPJwk.get_curve("foobar")
+
 
 @pytest.mark.parametrize(
     "crv,private_key_class,public_key_class",
     [
         ("Ed25519", ed25519.Ed25519PrivateKey, ed25519.Ed25519PublicKey),
         ("Ed448", ed448.Ed448PrivateKey, ed448.Ed448PublicKey),
         ("X448", x448.X448PrivateKey, x448.X448PublicKey),
@@ -213,31 +219,31 @@
     assert isinstance(cryptography_public_key, public_key_class)
 
 
 @pytest.mark.parametrize("crv", ["Ed25519", "Ed448", "X25519", "X448"])
 def test_pem_key(crv: str) -> None:
     private_jwk = OKPJwk.generate(crv=crv)
     private_pem = private_jwk.to_pem()
-    assert Jwk.from_pem_key(private_pem) == private_jwk
+    assert Jwk.from_pem(private_pem) == private_jwk
 
     public_jwk = private_jwk.public_jwk()
     public_pem = public_jwk.to_pem()
-    assert Jwk.from_pem_key(public_pem) == public_jwk
+    assert Jwk.from_pem(public_pem) == public_jwk
 
     # serialize private key with password
     password = b"th1s_i5_a_p4ssW0rd!"
     private_pem = private_jwk.to_pem(password)
-    assert Jwk.from_pem_key(private_pem, password) == private_jwk
+    assert Jwk.from_pem(private_pem, password) == private_jwk
 
     # try to serialize the public key with password
     with pytest.raises(ValueError):
         public_jwk.to_pem(password)
 
     with pytest.raises(ValueError):
-        assert Jwk.from_pem_key(public_pem, password) == public_jwk
+        assert Jwk.from_pem(public_pem, password) == public_jwk
 
 
 def test_from_cryptography_key_unknown_type() -> None:
     with pytest.raises(TypeError):
         OKPJwk.from_cryptography_key("this is not a cryptography key")
 
 
@@ -301,7 +307,40 @@
     # trying an unknown use with raise a ValueError:
     with pytest.raises(ValueError):
         OKPJwk.from_bytes(private_key, use="foo")
 
     # trying to initialize an OKPJwk with a wrong key size will not work
     with pytest.raises(ValueError):
         OKPJwk.from_bytes(private_key + b"bb")
+
+    # key of length 56 with use != "enc", or len 57 with use != "sig"
+    if len(private_key) != 32:
+        with pytest.raises(ValueError):
+            OKPJwk.from_bytes(private_key, use="sig" if use == "enc" else "enc")
+
+
+def test_public_private() -> None:
+    jwk = Jwk(
+        {
+            "kty": "OKP",
+            "crv": "Ed25519",
+            "x": "SghwA3Kg8e1Z2v1xnfnexH7OE4G-cd1z__Q64RQR4EQ",
+            "d": "V7P8eIm8sZsvIlhOXMLiamWTUW68wpyFyW_1QrnzkAI",
+        }
+    )
+
+    assert (
+        OKPJwk.public(
+            crv="Ed25519",
+            x=b"J\x08p\x03r\xa0\xf1\xedY\xda\xfdq\x9d\xf9\xde\xc4~\xce\x13\x81\xbeq\xdds\xff\xf4:\xe1\x14\x11\xe0D",
+        )
+        == jwk.public_jwk()
+    )
+
+    assert (
+        OKPJwk.private(
+            crv="Ed25519",
+            x=b"J\x08p\x03r\xa0\xf1\xedY\xda\xfdq\x9d\xf9\xde\xc4~\xce\x13\x81\xbeq\xdds\xff\xf4:\xe1\x14\x11\xe0D",
+            d=b'W\xb3\xfcx\x89\xbc\xb1\x9b/"XN\\\xc2\xe2je\x93Qn\xbc\xc2\x9c\x85\xc9o\xf5B\xb9\xf3\x90\x02',
+        )
+        == jwk
+    )
```

### Comparing `jwskate-0.6.0/tests/test_jwk/test_symmetric.py` & `jwskate-0.7.0/tests/test_jwk/test_symmetric.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.6.0/tests/test_jws.py` & `jwskate-0.7.0/tests/test_jws.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     P_521,
     ECJwk,
     InvalidJws,
     Jwk,
     JwsCompact,
     JwsJsonFlat,
     JwsJsonGeneral,
+    JwsSignature,
     OKPJwk,
     RSAJwk,
     SymmetricJwk,
 )
 
 
 def test_jws_compact(private_jwk: Jwk) -> None:
@@ -128,15 +129,15 @@
         == 111516411687364059110290785888309499157003632541675704481981366909658327544236421609398595734137119337357107861242367481230550517706674527460992238934209133
     )
     return jwk
 
 
 @pytest.fixture(scope="session")
 def ec_p256_private_jwk() -> Jwk:
-    return ECJwk.generate("P-256")
+    return ECJwk.generate(crv="P-256")
 
 
 @pytest.fixture(scope="session")
 def ec_p384_private_jwk() -> Jwk:
     return Jwk.generate_for_kty("EC", crv="P-384")
 
 
@@ -558,7 +559,33 @@
 def test_invalid_jws_json() -> None:
     with pytest.raises(AttributeError):
         JwsJsonFlat({}).payload
     with pytest.raises(AttributeError):
         JwsJsonGeneral({}).payload
     with pytest.raises(AttributeError):
         JwsJsonGeneral({}).signatures
+    with pytest.raises(AttributeError):
+        JwsSignature({}).protected
+    with pytest.raises(AttributeError):
+        JwsSignature({}).signature
+
+
+def test_jws_from_parts() -> None:
+    assert JwsCompact.from_parts(
+        "eyJhbGciOm51bGx9.dGhpc19pc19hX3Rlc3Q",
+        BinaPy(
+            "xZdQ-v6xqUpJGeuRIGVTs9gv56eQ_T_q-4OQdFS3IkkC3o-QM6vP39wHf5iNoHrZww9SrXHXb0oaF4RQZyKRGg"
+        ).decode_from("b64u"),
+    ) == JwsCompact(
+        "eyJhbGciOm51bGx9.dGhpc19pc19hX3Rlc3Q.xZdQ-v6xqUpJGeuRIGVTs9gv56eQ_T_q-4OQdFS3IkkC3o-QM6vP39wHf5iNoHrZww9SrXHXb0oaF4RQZyKRGg"
+    )
+
+    assert JwsCompact.from_parts(
+        bytearray(b"eyJhbGciOm51bGx9.dGhpc19pc19hX3Rlc3Q"),
+        bytearray(
+            BinaPy(
+                b"xZdQ-v6xqUpJGeuRIGVTs9gv56eQ_T_q-4OQdFS3IkkC3o-QM6vP39wHf5iNoHrZww9SrXHXb0oaF4RQZyKRGg"
+            ).decode_from("b64u")
+        ),
+    ) == JwsCompact(
+        "eyJhbGciOm51bGx9.dGhpc19pc19hX3Rlc3Q.xZdQ-v6xqUpJGeuRIGVTs9gv56eQ_T_q-4OQdFS3IkkC3o-QM6vP39wHf5iNoHrZww9SrXHXb0oaF4RQZyKRGg"
+    )
```

### Comparing `jwskate-0.6.0/tests/test_jwt.py` & `jwskate-0.7.0/tests/test_jwt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,128 @@
+from builtins import ValueError
 from datetime import datetime, timezone
 
 import pytest
-from freezegun import freeze_time  # type: ignore[import]
+from freezegun import freeze_time
 
 from jwskate import (
     ExpectedAlgRequired,
     ExpiredJwt,
     InvalidClaim,
     InvalidJwt,
     InvalidSignature,
     JweCompact,
     Jwk,
     Jwt,
     JwtSigner,
+    JwtVerifier,
     SignatureAlgs,
     SignedJwt,
     SymmetricJwk,
     UnsupportedAlg,
 )
 
 
 def test_signed_jwt() -> None:
+    jwk = Jwk(
+        {
+            "kty": "EC",
+            "alg": "ES256",
+            "kid": "my_key",
+            "crv": "P-256",
+            "x": "WtjnvHG9b_IKBLn4QYTHz-AdoAiO_ork5LH1BL_5tyI",
+            "y": "C0YfOUDuCOvTCt7hAqO-f9z8_JdOnOPbfYmUk-RosHA",
+            "d": "EnGZlkoa4VUsnl72LcRRychNJ2FFknm_ph855tNuPZ8",
+        }
+    )
+
     jwt = Jwt(
-        "eyJhbGciOiJSUzI1NiIsImtpZCI6Im15X2tleSJ9.eyJhY3IiOiIyIiwiYW1yIjpbInB3ZCIsIm90cCJdLCJhdWQiOiJjbGllbnRfaWQiLCJhdXRoX3RpbWUiOjE2MjkyMDQ1NjAsImV4cCI6MTYyOTIwNDYyMCwiaWF0IjoxNjI5MjA0NTYwLCJpc3MiOiJodHRwczovL215YXMubG9jYWwiLCJub25jZSI6Im5vbmNlIiwic3ViIjoiMTIzNDU2In0.wUfjMyjlOSdvbFGFP8O8wGcNBK7akeyOUBMvYcNZclFUtokOyxhLUPxmo1THo1DV1BHUVd6AWfeKUnyTxl_8-G3E_a9u5wJfDyfghPDhCmfkYARvqQnnV_3aIbfTfUBC4f0bHr08d_q0fED88RLu77wESIPCVqQYy2bk4FLucc63yGBvaCskqzthZ85DbBJYWLlR8qBUk_NA8bWATYEtjwTrxoZe-uA-vB6NwUv1h8DKRsDF-9HSVHeWXXAeoG9UW7zgxoY3KbDIVzemvGzs2R9OgDBRRafBBVeAkDV6CdbdMNJDmHzcjase5jX6LE-3YCy7c7AMM1uWRCnK3f-azA"
+        "eyJhbGciOiJFUzI1NiIsImtpZCI6Im15X2tleSJ9.eyJhY3IiOiIyIiwiYW1yIjpbInB3ZCIsIm90cCJdLCJhdWQiOiJjbGllbnRfaWQiLCJhdXRoX3RpbWUiOjE2MjkyMDQ1NjAsImV4cCI6MTYyOTIwNDYyMCwiaWF0IjoxNjI5MjA0NTYwLCJuYmYiOjE2MjkyMDQ1NjAsImlzcyI6Imh0dHBzOi8vbXlhcy5sb2NhbCIsIm5vbmNlIjoibm9uY2UiLCJzdWIiOiIxMjM0NTYifQ.RhLqE8VGBjIRag4w9ps1oUQlxumma1fQzFH2UTrMDCjW2iTGdqhkOjpzb5bdI6tkQRRP64IGP4_CBa2BR7p26Q"
     )
 
     assert isinstance(jwt, SignedJwt)
-    assert jwt.headers == {"alg": "RS256", "kid": "my_key"}
+    assert jwt.headers == {"alg": "ES256", "kid": "my_key"}
     assert jwt.claims == {
         "acr": "2",
         "amr": ["pwd", "otp"],
         "aud": "client_id",
         "auth_time": 1629204560,
         "exp": 1629204620,
         "iat": 1629204560,
+        "nbf": 1629204560,
         "iss": "https://myas.local",
         "nonce": "nonce",
         "sub": "123456",
     }
     assert jwt.is_expired()
     assert jwt.sub == "123456"
     assert jwt.subject == "123456"
     assert jwt.audiences == ["client_id"]
     assert jwt.nonce == "nonce"
     assert jwt.amr == ["pwd", "otp"]
     assert jwt.exp == 1629204620
     assert jwt.expires_at == datetime.fromtimestamp(1629204620, tz=timezone.utc)
     assert jwt.issued_at == datetime.fromtimestamp(1629204560, tz=timezone.utc)
+    assert jwt.not_before == datetime.fromtimestamp(1629204560, tz=timezone.utc)
     assert jwt.nonce == jwt["nonce"]
 
     # validating with the appropriate key must work
+
     jwt.validate(
-        jwk={
-            "kty": "RSA",
-            "alg": "RS256",
-            "kid": "my_key",
-            "n": "2m4QVSHdUo2DFSbGY24cJbxE10KbgdkSCtm0YZ1q0Zmna8pJg8YhaWCJHV7D5AxQ_L1b1PK0jsdpGYWc5-Pys0FB2hyABGPxXIdg1mjxn6geHLpWzsA3MHD29oqfl0Rt7g6AFc5St3lBgJCyWtci6QYBmBkX9oIMOx9pgv4BaT6y1DdrNh27-oSMXZ0a58KwnC6jbCpdA3V3Eume-Be1Tx9lJN3j6S8ydT7CGY1Xd-sc3oB8pXfkr1_EYf0Sgb9EwOJfqlNK_kVjT3GZ-1JJMKJ6zkU7H0yXe2SKXAzfayvJaIcYrk-sYwmf-u7yioOLLvjlGjysN7SOSM8socACcw",
-            "e": "AQAB",
-        },
+        jwk=jwk.public_jwk(),
         issuer="https://myas.local",
         audience="client_id",
         check_exp=False,
     )
 
     # validating with another key must fail
     with pytest.raises(InvalidSignature):
         jwt.validate(Jwk.generate_for_alg("RS256").public_jwk())
 
+    # invalid audience
+    with pytest.raises(InvalidClaim, match="audience"):
+        jwt.validate(
+            jwk.public_jwk(),
+            audience="foo",
+        )
+
 
 def test_unprotected() -> None:
     jwt = Jwt.unprotected({"foo": "bar"})
     assert jwt == "eyJhbGciOiJub25lIn0.eyJmb28iOiJiYXIifQ."
 
 
-def test_jwt_signer(issuer: str, private_jwk: Jwk) -> None:
-    signer = JwtSigner(issuer, private_jwk)
+def test_jwt_signer_and_verifier(issuer: str) -> None:
+    audience = "some_audience"
+    signer = JwtSigner.with_random_key(issuer, alg="ES256")
     now = datetime.now(timezone.utc)
-    jwt = signer.sign(subject="some_id", audience="some_audience")
-    assert isinstance(jwt, Jwt)
+    jwt = signer.sign(subject="some_id", audience=audience, extra_claims={"foo": "bar"})
+    assert isinstance(jwt, SignedJwt)
     assert jwt.subject == "some_id"
-    assert jwt.audiences == ["some_audience"]
+    assert jwt.audiences == [audience]
     assert jwt.iat == pytest.approx(now.timestamp())
     assert jwt.expires_at is not None
     assert jwt.expires_at > now
 
+    verifier = signer.verifier(audience=audience)
+
+    @verifier.custom_verifier
+    def foobar_verifier(jwt: SignedJwt) -> None:
+        if jwt.foo != "bar":
+            raise ValueError("This JWT is not FooBar compliant!")
+
+    verifier.verify(jwt)
+
+    @verifier.custom_verifier
+    def failing_verifier(jwt: SignedJwt) -> None:
+        raise ValueError("This token will never be valid")
+
+    with pytest.raises(ValueError):
+        verifier.verify(jwt)
+
 
 def test_invalid_signed_jwt() -> None:
     with pytest.raises(InvalidJwt):
         SignedJwt("garbage")
     with pytest.raises(InvalidJwt):
         SignedJwt("garbage!.foo!.bar!")
     with pytest.raises(InvalidJwt):
@@ -97,14 +132,15 @@
             "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.garbage!"
         )
 
 
 def test_empty_jwt(private_jwk: Jwk) -> None:
     jwt = Jwt.sign({}, private_jwk)
     assert jwt.is_expired() is None
+    assert jwt.issued_at is None
     assert jwt.expires_at is None
     assert jwt.not_before is None
     assert jwt.issuer is None
     assert jwt.audiences == []
     assert jwt.subject is None
     assert jwt.jwt_token_id is None
     assert jwt.kid == private_jwk.kid
@@ -241,14 +277,29 @@
     assert jwt.decrypt(jwk).parse_from("json") == {
         "iss": "joe",
         "exp": 1300819380,
         "http://example.com/is_root": True,
     }
 
 
+def test_audience() -> None:
+    assert SignedJwt(
+        "eyJhbGciOiJFUzI1NiJ9.eyJhdWQiOiJjbGllbnRfaWQifQ.S1FheqDgFtSCUg2YLvBjyTp7U_oTAdNeBU5DWJWG7nhdQ94kPEjz1aP8ALfHQI-V-SPA34FTm6a3NkG6C1opsg"
+    ).audiences == ["client_id"]
+    assert SignedJwt(
+        "eyJhbGciOiJFUzI1NiJ9.eyJhdWQiOlsiY2xpZW50X2lkIl19.eLuTnfzUXE09-SwUfL70py-SlESZHom3SPK0deiy27QX5iCDjSk2rlSVAfcNpAO5DjnKKua3HHtAv6oE7Ox9vg"
+    ).audiences == ["client_id"]
+    assert (
+        SignedJwt(
+            "eyJhbGciOiJFUzI1NiJ9.e30.b7t6qRWXypeNf2GE2BnBqjfLbQ5FTcMFVGm6zjgbXSVZIKXNvkK-K4oRYurDD2YY8955JtnpajcVurns1PH-1Q"
+        ).audiences
+        == []
+    )
+
+
 def test_decrypt_nested_jwt() -> None:
     jwt = """
     eyJhbGciOiJSU0ExXzUiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2IiwiY3R5IjoiSldUIn0.
      g_hEwksO1Ax8Qn7HoN-BVeBoa8FXe0kpyk_XdcSmxvcM5_P296JXXtoHISr_DD_M
      qewaQSH4dZOQHoUgKLeFly-9RI11TG-_Ge1bZFazBPwKC5lJ6OLANLMd0QSL4fYE
      b9ERe-epKYE3xb2jfY1AltHqBO-PM6j23Guj2yDKnFv6WO72tteVzm_2n17SBFvh
      DuR9a2nHTE67pe0XGBUS_TK7ecA-iVq5COeVdJR4U4VZGGlxRGPLRHvolVLEHx6D
@@ -314,15 +365,15 @@
     sign_jwk = (
         Jwk.generate_for_alg(sign_alg).with_kid_thumbprint().with_usage_parameters()
     )
     enc_jwk = (
         Jwk.generate_for_alg(enc_alg).with_kid_thumbprint().with_usage_parameters()
     )
 
-    claims = {"iat": 1661759343, "exp": 1661759403, "sub": "mysub"}
+    claims = {"iat": 1661759343, "exp": 1661759403, "nbf": 1661759323, "sub": "mysub"}
     enc_jwt = Jwt.sign_and_encrypt(claims, sign_jwk, enc_jwk.public_jwk(), enc)
     assert isinstance(enc_jwt, JweCompact)
     assert enc_jwt.cty == "JWT"
     assert enc_jwt.alg == enc_alg
     assert enc_jwt.enc == enc
     assert enc_jwt.kid == enc_jwk.kid
 
@@ -409,34 +460,222 @@
         jwt.typ
     with pytest.raises(AttributeError):
         jwt.cty
 
 
 def test_invalid_claims() -> None:
     jwt = SignedJwt(
-        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOjEsImlhdCI6ImZvbyIsImV4cCI6ImZvbyIsIm5iZiI6ImZvbyIsImF1ZCI6MSwianRpIjoxfQ.lcNMSH9LNXbIpQUAqtbIjMv-kSWXeC0VamsrHNESTq0"
+        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOjEsImlhdCI6ImZvbyIsImV4cCI6ImZvbyIsIm5iZiI6ImZvbyIsImlzcyI6MTExMSwiYXVkIjoxLCJqdGkiOjF9.XeKnvnirIE7LmkTVwVyWOVTKLawybdolAZTFtM4NfoI"
     )
     with pytest.raises(AttributeError):
+        jwt.issuer
+    with pytest.raises(AttributeError):
         jwt.subject
     with pytest.raises(AttributeError):
         jwt.issued_at
     with pytest.raises(AttributeError):
         jwt.expires_at
     with pytest.raises(AttributeError):
         jwt.not_before
     with pytest.raises(AttributeError):
         jwt.audiences
     with pytest.raises(AttributeError):
         jwt.jwt_token_id
 
 
-@freeze_time("2022-10-07 10:40:15 UTC")  # type: ignore[misc]
+@freeze_time("2022-10-07 10:40:15 UTC")
 def test_timestamp() -> None:
     now_ts = Jwt.timestamp()
     assert isinstance(now_ts, int)
     assert now_ts == 1665139215
     assert Jwt.timestamp_to_datetime(now_ts) == datetime(
         year=2022, month=10, day=7, hour=10, minute=40, second=15, tzinfo=timezone.utc
     )
 
     assert Jwt.timestamp(+60) == 1665139275
     assert Jwt.timestamp(-60) == 1665139155
+
+
+@freeze_time("2023-04-03 11:56:20 UTC")
+def test_verifier() -> None:
+    issuer = "https://my.issuer.local"
+    audience = "myaudience"
+    subject = "mysubject"
+    private_jwk = Jwk(
+        {
+            "kty": "EC",
+            "crv": "P-256",
+            "alg": "ES256",
+            "kid": "MUBAl25sdPAIlnA_8-BnMcIe5e8LnlI5pHF6Zy-icvw",
+            "x": "ftZqn6yrLR_4AytQz8Q_badHRTQ2Vc6Eg46ICsMuuMM",
+            "y": "C4wIeHH0aIW5Tf1_EPnJkse-vcoDNd-kh8P6-Ci2MI8",
+            "d": "3vyhseJLd51ZXdlrCHAPH1uv5Bp9IvnA8UB92ksu4MU",
+        }
+    )
+    jwks = private_jwk.public_jwk().as_jwks()
+
+    def suject_verifier(jwt: SignedJwt) -> None:
+        if jwt.subject != subject:
+            raise ValueError("Invalid Subject", jwt)
+
+    def not_foo(jwt: SignedJwt) -> None:
+        if "foo" in jwt.claims:
+            raise ValueError("Token is foo!", jwt)
+
+    verifier = JwtVerifier(
+        jwks,
+        issuer=issuer,
+        audience=audience,
+        alg="ES256",
+        verifiers=[suject_verifier, not_foo],
+    )
+
+    verifier.verify(
+        Jwt.sign(
+            {
+                "iss": "https://my.issuer.local",
+                "aud": "myaudience",
+                "iat": 1680523071,
+                "exp": 1680523131,
+                "sub": "mysubject",
+            },
+            private_jwk,
+        )
+    )
+
+    with pytest.raises(InvalidClaim, match="issuer"):
+        verifier.verify(
+            Jwt.sign(
+                {
+                    "iss": "https://wrong.issuer.local",
+                    "aud": "myaudience",
+                    "iat": 1680522980,
+                    "exp": 1680523040,
+                    "sub": "mysubject",
+                },
+                private_jwk,
+            )
+        )
+
+    with pytest.raises(InvalidClaim, match="audience"):
+        verifier.verify(
+            Jwt.sign(
+                {
+                    "iss": "https://my.issuer.local",
+                    "aud": "wrong_audience",
+                    "iat": 1680522980,
+                    "exp": 1680523040,
+                    "sub": "mysubject",
+                },
+                private_jwk,
+            )
+        )
+
+    with pytest.raises(InvalidSignature):
+        jwt = Jwt.sign(
+            {
+                "iss": "https://my.issuer.local",
+                "aud": "myaudience",
+                "iat": 1680523071,
+                "exp": 1680523131,
+                "sub": "mysubject",
+            },
+            private_jwk,
+        )
+        verifier.verify(str(jwt)[:-17] + "--wrong_signature")
+
+    with pytest.raises(ExpiredJwt):
+        verifier.verify(
+            Jwt.sign(
+                {
+                    "iss": "https://my.issuer.local",
+                    "aud": "myaudience",
+                    "iat": 1680522860,  # expired
+                    "exp": 1680522920,
+                    "sub": "mysubject",
+                },
+                private_jwk,
+            )
+        )
+
+    with pytest.raises(ValueError):
+        verifier.verify(
+            Jwt.sign(
+                {
+                    "iss": "https://my.issuer.local",
+                    "aud": "wrong_audience",
+                    "iat": 1680522980,
+                    "exp": 1680523040,
+                    "sub": "wrong_subject",
+                },
+                private_jwk,
+            )
+        )
+
+    with pytest.raises(ValueError):
+        verifier.verify(
+            Jwt.sign(
+                {
+                    "iss": "https://my.issuer.local",
+                    "aud": "myaudience",
+                    "iat": 1680522860,
+                    "exp": 1680522920,
+                    "sub": "mysubject",
+                    "foo": "bar",
+                },
+                private_jwk,
+            )
+        )
+
+    valid_jwt_without_kid = Jwt.sign(
+        {
+            "iss": "https://my.issuer.local",
+            "aud": "myaudience",
+            "iat": 1680523071,
+            "exp": 1680523131,
+            "sub": "mysubject",
+        },
+        private_jwk.minimize(),
+        alg="ES256",
+    )
+
+    verifier.verify(valid_jwt_without_kid)
+
+    with pytest.raises(InvalidSignature):
+        verifier.verify(str(valid_jwt_without_kid)[:-17] + "--wrong-signature")
+
+    # init with a single Jwk
+    JwtVerifier(
+        private_jwk.public_jwk(),
+        issuer=issuer,
+        audience=audience,
+        alg="ES256",
+        verifiers=[suject_verifier, not_foo],
+    ).verify(valid_jwt_without_kid)
+
+    # init with a single Jwk as a dict
+    JwtVerifier(
+        dict(private_jwk.public_jwk()),
+        issuer=issuer,
+        audience=audience,
+        alg="ES256",
+        verifiers=[suject_verifier, not_foo],
+    ).verify(valid_jwt_without_kid)
+
+    # init with a JwkSet as a dict
+    JwtVerifier(
+        dict(private_jwk.public_jwk().as_jwks()),
+        issuer=issuer,
+        audience=audience,
+        alg="ES256",
+        verifiers=[suject_verifier, not_foo],
+    ).verify(valid_jwt_without_kid)
+
+    # init with a private key
+    with pytest.raises(ValueError):
+        JwtVerifier(
+            dict(private_jwk),
+            issuer=issuer,
+            audience=audience,
+            alg="ES256",
+            verifiers=[suject_verifier, not_foo],
+        ).verify(valid_jwt_without_kid)
```

### Comparing `jwskate-0.6.0/setup.py` & `jwskate-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,339 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jwskate
+Version: 0.7.0
+Summary: A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module.
+Home-page: https://github.com/guillp/jwskate
+License: MIT
+Author: Guillaume Pujol
+Author-email: guill.p.linux@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: doc
+Provides-Extra: test
+Requires-Dist: binapy (>=0.6.0,<0.7.0)
+Requires-Dist: cryptography (>=3.4)
+Requires-Dist: mypy (>=1.1.1,<2.0.0)
+Requires-Dist: typing-extensions (>=4.3.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['jwskate',
- 'jwskate.jwa',
- 'jwskate.jwa.encryption',
- 'jwskate.jwa.key_mgmt',
- 'jwskate.jwa.signature',
- 'jwskate.jwe',
- 'jwskate.jwk',
- 'jwskate.jws',
- 'jwskate.jwt',
- 'tests',
- 'tests.test_jwa',
- 'tests.test_jwk']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['backports.cached-property>=1,<2',
- 'binapy>=0.6.0,<0.7.0',
- 'cryptography>=3.4',
- 'typing-extensions>=4.3.0']
-
-setup_kwargs = {
-    'name': 'jwskate',
-    'version': '0.6.0',
-    'description': 'A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module.',
-    'long_description': '# JwSkate\n\n[![PyPi](https://img.shields.io/pypi/v/jwskate.svg)](https://pypi.python.org/pypi/jwskate)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nA Pythonic implementation of the JOSE set of IETF specifications: [Json Web Signature][rfc7515], [Keys][rfc7517],\n[Algorithms][rfc7518], [Tokens][rfc7519] and [Encryption][rfc7516] (RFC7515 to 7519), and their extensions\n[ECDH Signatures][rfc8037] (RFC8037), [JWK Thumbprints][rfc7638] (RFC7638), and [JWK Thumbprint URI][rfc9278] (RFC9278),\nand with respect to [JWT Best Current Practices][rfc8725].\n\n- Free software: MIT\n- Documentation: <https://guillp.github.io/jwskate/>\n\nA quick usage example, generating an RSA private key, signing some data, then validating that signature:\n\n```python\nfrom jwskate import Jwk\n\n# let\'s generate a random private key\nrsa_private_jwk = (\n    Jwk.generate_for_alg(  # generated key will automatically be RSA, based on the required \'alg\'\n        alg="RS256", key_size=2048\n    )\n    .with_kid_thumbprint()  # include an RFC7638 thumbprint as key id\n    .with_usage_parameters()  # include the appropriate \'use\' and \'key_ops\' parameters in the JWK, based on the \'alg\'\n)\n\ndata = b"Signing is easy!"\nsignature = rsa_private_jwk.sign(data)\n\n# extract the public key, and verify the signature with it\nrsa_public_jwk = rsa_private_jwk.public_jwk()\nassert rsa_public_jwk.verify(data, signature)\n\n# let\'s see what a Jwk looks like:\nassert isinstance(rsa_private_jwk, dict)  # Jwk are dict\n\nprint(rsa_private_jwk)\n```\n\nThe result of this print will look like this (with the random parts abbreviated to `...` for display purposes only):\n\n```\n{\'kty\': \'RSA\',\n \'n\': \'...\',\n \'e\': \'AQAB\',\n \'d\': \'...\',\n \'p\': \'...\',\n \'q\': \'...\',\n \'dp\': \'...\',\n \'dq\': \'...\',\n \'qi\': \'...\',\n \'alg\': \'RS256\',\n \'kid\': \'...\',\n \'use\': \'sig\',\n \'key_ops\': [\'sign\']}\n```\n\nNow let\'s sign a JWT containing arbitrary claims, this time using an EC key:\n\n```python\nfrom jwskate import Jwk, Jwt\n\nprivate_jwk = Jwk.generate_for_alg(\n    "ES256", kid="my_key"\n)  # let\'s specify a kid manually\nclaims = {"sub": "some_sub", "claim1": "value1"}\n\njwt = Jwt.sign(claims, private_jwk)\n# that\'s it! we have a signed JWT\nassert jwt.claims == claims  # claims can be accessed as a dict\nassert jwt.sub == "some_sub"  # or individual claims can be accessed as attributes\nassert jwt["claim1"] == "value1"  # or as dict items\nassert jwt.alg == "ES256"  # alg and kid headers are also accessible as attributes\nassert jwt.kid == private_jwk.kid\nassert jwt.verify_signature(private_jwk.public_jwk())\n\nprint(jwt)\n# eyJhbGciOiJFUzI1NiIsImtpZCI6Im15a2V5In0.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.C1KcDyDT8qXwUqcWzPKkQD7f6xai-gCgaRFMdKPe80Vk7XeYNa8ovuLwvdXgGW4ZZ_lL73QIyncY7tHGXUthag\n# This will output the full JWT compact representation. You can inspect it for example at <https://jwt.io>\n\nprint(jwt.headers)\n# {\'alg\': \'ES256\', \'kid\': \'my_key\'}\n```\n\nNote above that the JWT headers are automatically generated with the appropriate values.\n\nOr let\'s sign a JWT with the standardised lifetime, subject, audience and ID claims:\n\n```python\nfrom jwskate import Jwk, JwtSigner\n\nprivate_jwk = Jwk.generate_for_alg("ES256")\nsigner = JwtSigner(issuer="https://myissuer.com", jwk=private_jwk)\njwt = signer.sign(\n    subject="some_sub",\n    audience="some_aud",\n    extra_claims={"custom_claim1": "value1", "custom_claim2": "value2"},\n)\n\nprint(jwt.claims)\n```\n\nThe generated JWT claims will include the standardised claims:\n\n```\n{\'custom_claim1\': \'value1\',\n \'custom_claim2\': \'value2\',\n \'iss\': \'https://myissuer.com\',\n \'aud\': \'some_aud\',\n \'sub\': \'some_sub\',\n \'iat\': 1648823184,\n \'exp\': 1648823244,\n \'jti\': \'3b400e27-c111-4013-84e0-714acd76bf3a\'\n}\n```\n\n## Features\n\n- Simple, Clean, Pythonic interface\n- Convenience wrappers around `cryptography` for all algorithms described in JWA\n- Json Web Keys (JWK) loading and generation\n- Arbitrary data signature and verification using Json Web Keys\n- Json Web Signatures (JWS) signing and verification\n- Json Web Encryption (JWE) encryption and decryption\n- Json Web Tokens (JWT) signing, verification and validation\n- 100% type annotated\n- nearly 100% code coverage\n- Relies on [cryptography](https://cryptography.io) for all cryptographic operations\n- Relies on [BinaPy](https://guillp.github.io/binapy/) for binary data manipulations\n\n### Supported Token Types\n\n| Token Type                | Support                                                                  |\n|---------------------------|--------------------------------------------------------------------------|\n| Json Web Signature (JWS)  | ☑ Compact <br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |\n| Json Web Encryption (JWE) | ☑ Compact <br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |\n| Json Web Tokens (JWT)     | ☑ Signed <br/> ☑ Signed and Encrypted                        |\n\n### Supported Signature algorithms\n\n`jwskate` supports the following signature algorithms:\n\n| Signature Alg | Description                                    | Key Type | Reference                          | Note                           |\n|---------------|------------------------------------------------|----------|------------------------------------|--------------------------------|\n| HS256         | HMAC using SHA-256                             | oct      | [RFC7518, Section 3.2]             |                                |\n| HS384         | HMAC using SHA-384                             | oct      | [RFC7518, Section 3.2]             |                                |\n| HS512         | HMAC using SHA-512                             | oct      | [RFC7518, Section 3.2]             |                                |\n| RS256         | RSASSA-PKCS1-v1_5 using SHA-256                | RSA      | [RFC7518, Section 3.3]             |                                |\n| RS384         | RSASSA-PKCS1-v1_5 using SHA-384                | RSA      | [RFC7518, Section 3.3]             |                                |\n| RS512         | RSASSA-PKCS1-v1_5 using SHA-512                | RSA      | [RFC7518, Section 3.3]             |                                |\n| ES256         | ECDSA using P-256 and SHA-256                  | EC       | [RFC7518, Section 3.4]             |                                |\n| ES384         | ECDSA using P-384 and SHA-384                  | EC       | [RFC7518, Section 3.4]             |                                |\n| ES512         | ECDSA using P-521 and SHA-512                  | EC       | [RFC7518, Section 3.4]             |                                |\n| PS256         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 3.5]             |                                |\n| PS384         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384 | RSA      | [RFC7518, Section 3.5]             |                                |\n| PS512         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512 | RSA      | [RFC7518, Section 3.5]             |                                |\n| EdDSA         | EdDSA signature algorithms                     | OKP      | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |\n| ES256K        | ECDSA using secp256k1 curve and SHA-256        | EC       | [RFC8812, Section 3.2]             |                                |\n| HS1           | HMAC using SHA-1                               | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |\n| RS1           | RSASSA-PKCS1-v1_5 with SHA-1                   | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |\n| none          | No digital signature or MAC performed          |          | [RFC7518, Section 3.6]             | Not usable by mistake          |\n\n### Supported Key Management algorithms\n\n`jwskate` supports the following key management algorithms:\n\n| Signature Alg      | Description                                     | Key Type | Reference                          | Note        |\n|--------------------|-------------------------------------------------|----------|------------------------------------|-------------|\n| RSA1_5             | RSAES-PKCS1-v1_5                                | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |\n| RSA-OAEP           | RSAES OAEP using default parameters             | RSA      | [RFC7518, Section 4.3]             |             |\n| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256  | RSA      | [RFC7518, Section 4.3]             |             |\n| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384    | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |\n| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512    | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |\n| A128KW             | AES Key Wrap using 128-bit key                  | oct      | [RFC7518, Section 4.4]             |             |\n| A192KW             | AES Key Wrap using 192-bit key                  | oct      | [RFC7518, Section 4.4]             |             |\n| A256KW             | AES Key Wrap using 256-bit key                  | oct      | [RFC7518, Section 4.4]             |             |\n| dir                | Direct use of a shared symmetric key            | oct      | [RFC7518, Section 4.5]             |             |\n| ECDH-ES            | ECDH-ES using Concat KDF                        | EC       | [RFC7518, Section 4.6]             |             |\n| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |\n| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |\n| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping  | EC       | [RFC7518, Section 4.6]             |             |\n| A128GCMKW          | Key wrapping with AES GCM using 128-bit key     | oct      | [RFC7518, Section 4.7]             |             |\n| A192GCMKW          | Key wrapping with AES GCM using 192-bit key     | oct      | [RFC7518, Section 4.7]             |             |\n| A256GCMKW          | Key wrapping with AES GCM using 256-bit key     | oct      | [RFC7518, Section 4.7]             |             |\n| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping   | password | [RFC7518, Section 4.8]             |             |\n| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping   | password | [RFC7518, Section 4.8]             |             |\n| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping   | password | [RFC7518, Section 4.8]             |             |\n\n### Supported Encryption algorithms\n\n`jwskate` supports the following encryption algorithms:\n\n| Signature Alg  | Description                                                 | Reference                |\n|----------------|-------------------------------------------------------------|--------------------------|\n| A128CBC-HS256  | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |\n| A192CBC-HS384  | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |\n| A256CBC-HS512  | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |\n| A128GCM        | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |\n| A192GCM        | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |\n| A256GCM        | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |\n\n### Supported Elliptic Curves\n\n`jwskate` supports the following Elliptic Curves:\n\n| Curve     | Description                           | Key Type | Usage                 | Reference                  |\n|-----------|---------------------------------------|----------|-----------------------|----------------------------|\n| P-256     | P-256 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |\n| P-384     | P-384 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |\n| P-521     | P-521 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |\n| Ed25519   | Ed25519 signature algorithm key pairs | OKP      | signature             | [RFC8037, Section 3.1]     |\n| Ed448     | Ed448 signature algorithm key pairs   | OKP      | signature             | [RFC8037, Section 3.1]     |\n| X25519    | X25519 function key pairs             | OKP      | encryption            | [RFC8037, Section 3.2]     |\n| X448      | X448 function key pairs               | OKP      | encryption            | [RFC8037, Section 3.2]     |\n| secp256k1 | SECG secp256k1 curve                  | EC       | signature, encryption | [RFC8812, Section 3.1]     |\n\n## Why a new lib ?\n\nThere are already multiple modules implementing JOSE and Json Web Crypto related specifications in Python. However, I\nhave been dissatisfied by all of them so far, so I decided to come up with my own module.\n\n- [PyJWT](https://pyjwt.readthedocs.io)\n- [JWCrypto](https://jwcrypto.readthedocs.io/)\n- [Python-JOSE](https://python-jose.readthedocs.io/)\n- [AuthLib](https://docs.authlib.org/en/latest/jose/)\n\nNot to say that those are _bad_ libs (I actually use `jwcrypto` myself for `jwskate` unit tests), but they either don\'t\nsupport some important features, lack documentation, or generally have APIs that don\'t feel easy-enough, Pythonic-enough\nto use.\n\n## Design\n\n### JWK are dicts\n\nJWK are specified as JSON objects, which are parsed as `dict` in Python. The `Jwk` class in `jwskate` is actually a\n`dict` subclass, so you can use it exactly like you would use a dict: you can access its members, dump it back as JSON,\netc. The same is true for Signed or Encrypted Json Web tokens in JSON format.\n\n### JWA Wrappers\n\nYou can use `cryptography` to do the cryptographic operations that are described in\n[JWA](https://www.rfc-editor.org/info/rfc7518), but since `cryptography` is a general purpose library, its usage is not\nstraightforward and gives you plenty of options to carefully select and combine, leaving room for errors. It has also a\nquite inconsistent API to handle the different type of keys and algorithms. To work around\nthis, `jwskate` comes with a set of consistent wrappers that implement the exact JWA specifications, with minimum risk\nof mistakes.\n\n### Safe Signature Verification\n\nAs advised in [JWT Best Practices][rfc8725] $3.1:\n\nFor every signature verification method in `jwskate`, the expected signature(s) algorithm(s) must be specified. That is\nto avoid a security flaw where your application accepts tokens with a weaker encryption scheme than what your security\npolicy mandates; or even worse, where it accepts unsigned tokens, or tokens that are symmetrically signed with an\nimproperly used public key, leaving your application exposed to exploitation by attackers.\n\nTo specify which signature algorithms are accepted, each signature verification method accepts, in order of preference:\n\n- an `alg` parameter which contains the expected algorithm, or an `algs` parameter which contains a list of acceptable\n  algorithms\n- the `alg` parameter from the signature verification `Jwk`, if present. This `alg` is the algorithm intended for use\n  with that key.\n\nNote that you cannot use `alg` and `algs` at the same time. If your `Jwk` contains an `alg` parameter, and you provide\nan `alg` or `algs` which does not match that value, a `Warning` will be emitted.\n\n## Credits\n\nAll cryptographic operations are handled by [cryptography](https://cryptography.io).\n\n[rfc7515]: https://www.rfc-editor.org/rfc/rfc7515.html\n[rfc7516]: https://www.rfc-editor.org/rfc/rfc7516.html\n[rfc7517]: https://www.rfc-editor.org/rfc/rfc7517.html\n[rfc7518]: https://www.rfc-editor.org/rfc/rfc7518.html\n[rfc7518, section 3.2]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.2\n[rfc7518, section 3.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.3\n[rfc7518, section 3.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.4\n[rfc7518, section 3.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.5\n[rfc7518, section 3.6]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.6\n[rfc7518, section 4.2]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.2\n[rfc7518, section 4.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.3\n[rfc7518, section 4.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.4\n[rfc7518, section 4.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.5\n[rfc7518, section 4.6]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.6\n[rfc7518, section 4.7]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.7\n[rfc7518, section 4.8]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.8\n[rfc7518, section 5.2.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.3\n[rfc7518, section 5.2.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.4\n[rfc7518, section 5.2.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.5\n[rfc7518, section 5.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.3\n[rfc7518, section 6.2.1.1]: https://www.rfc-editor.org/rfc/rfc7518.html#section-6.2.1.1\n[rfc7519]: https://www.rfc-editor.org/rfc/rfc7519.html\n[rfc7638]: https://www.rfc-editor.org/rfc/rfc7638.html\n[rfc8037]: https://www.rfc-editor.org/rfc/rfc8037.html\n[rfc8037, section 3.1]: https://www.rfc-editor.org/rfc/rfc8037.html#section-3.1\n[rfc8037, section 3.2]: https://www.rfc-editor.org/rfc/rfc8037.html#section-3.2\n[rfc8725]: https://www.rfc-editor.org/rfc/rfc8725\n[rfc8812, section 3.1]: https://www.rfc-editor.org/rfc/rfc8812.html#section-3.1\n[rfc8812, section 3.2]: https://www.rfc-editor.org/rfc/rfc8812.html#name-ecdsa-signature-with-secp25\n[rfc9278]: https://www.rfc-editor.org/rfc/rfc9278.html\n',
-    'author': 'Guillaume Pujol',
-    'author_email': 'guill.p.linux@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/guillp/jwskate',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+# JwSkate
+
+[![PyPi](https://img.shields.io/pypi/v/jwskate.svg)](https://pypi.python.org/pypi/jwskate)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A Pythonic implementation of the JOSE set of IETF specifications: [Json Web Signature][rfc7515], [Keys][rfc7517],
+[Algorithms][rfc7518], [Tokens][rfc7519] and [Encryption][rfc7516] (RFC7515 to 7519), and their extensions
+[ECDH Signatures][rfc8037] (RFC8037), [JWK Thumbprints][rfc7638] (RFC7638), and [JWK Thumbprint URI][rfc9278] (RFC9278),
+and with respect to [JWT Best Current Practices][rfc8725].
+
+- Free software: MIT
+- Documentation: [https://guillp.github.io/jwskate/](https://guillp.github.io/jwskate/)
+
+A quick usage example, generating an RSA private key, signing some data, then validating that signature:
+
+```python
+from jwskate import Jwk
+
+# Let's generate a random private key, to use with alg 'RS256'.
+# Based on that alg, jwskate knows it must be an RSA key.
+rsa_private_jwk = Jwk.generate(alg="RS256", key_size=2048)
+
+data = b"Signing is easy!"
+signature = rsa_private_jwk.sign(data)
+
+# extract the public key, and verify the signature with it
+rsa_public_jwk = rsa_private_jwk.public_jwk()
+assert rsa_public_jwk.verify(data, signature)
+
+# let's see what a Jwk looks like:
+assert isinstance(rsa_private_jwk, dict)  # Jwk are dict
+
+print(rsa_private_jwk.with_usage_parameters())
+```
+
+The result of this print will look like this (with the random parts abbreviated to `...` for display purposes only):
+
+```
+{'kty': 'RSA',
+ 'n': '...',
+ 'e': 'AQAB',
+ 'd': '...',
+ 'p': '...',
+ 'q': '...',
+ 'dp': '...',
+ 'dq': '...',
+ 'qi': '...',
+ 'alg': 'RS256',
+ 'kid': '...',
+ 'use': 'sig',
+ 'key_ops': ['sign']}
+```
+
+Now let's sign a JWT containing arbitrary claims, this time using an EC key:
+
+```python
+from jwskate import Jwk, Jwt
+
+# This time let's try an EC key, based on `alg` parameter,
+# and let's specigy an arbitrary Key ID (kid).
+private_jwk = Jwk.generate(alg="ES256", kid="my_key")
+
+# here are claims to sign in a JWT:
+claims = {"sub": "some_sub", "claim1": "value1"}
+
+jwt = Jwt.sign(claims, private_jwk)
+# that's it! we have a signed JWT
+assert isinstance(jwt, Jwt)  # Jwt are objects
+assert jwt.claims == claims  # claims can be accessed as a dict
+assert jwt.headers == {"alg": "ES256", "kid": "my_key"}  # headers too
+assert jwt.sub == "some_sub"  # individual claims can be accessed as attributes
+assert jwt["claim1"] == "value1"  # or as dict items (with "subscription")
+assert jwt.alg == "ES256"  # alg and kid headers are also accessible as attributes
+assert jwt.kid == private_jwk.kid
+# notice that alg and kid are automatically set with appropriate values
+assert isinstance(jwt.signature, bytes)  # signature is accessible too
+# verifying the jwt signature is as easy as:
+assert jwt.verify_signature(private_jwk.public_jwk())
+# since our jwk contains an 'alg' parameter (here 'ES256'), the signature is automatically verified using that alg
+# you could also specify an alg manually, useful for keys with no "alg" hint:
+assert jwt.verify_signature(private_jwk.public_jwk(), alg="ES256")
+
+print(jwt)
+# eyJhbGciOiJFUzI1NiIsImtpZCI6Im15a2V5In0.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.C1KcDyDT8qXwUqcWzPKkQD7f6xai-gCgaRFMdKPe80Vk7XeYNa8ovuLwvdXgGW4ZZ_lL73QIyncY7tHGXUthag
+# This will output the full JWT compact representation. You can inspect it for example at <https://jwt.io>
+```
+
+Or let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
+
+```python
+from jwskate import Jwk, JwtSigner
+
+private_jwk = Jwk.generate(alg="ES256")
+signer = JwtSigner(issuer="https://myissuer.com", jwk=private_jwk)
+jwt = signer.sign(
+    subject="some_sub",
+    audience="some_aud",
+    extra_claims={"custom_claim1": "value1", "custom_claim2": "value2"},
+)
+
+print(jwt.claims)
+```
+
+The generated JWT claims will include the standardised claims:
+
+```
+{'custom_claim1': 'value1',
+ 'custom_claim2': 'value2',
+ 'iss': 'https://myissuer.com',
+ 'aud': 'some_aud',
+ 'sub': 'some_sub',
+ 'iat': 1648823184,
+ 'exp': 1648823244,
+ 'jti': '3b400e27-c111-4013-84e0-714acd76bf3a'
 }
+```
+
+## Features
+
+- Simple, Clean, Pythonic interface
+- Convenience wrappers around `cryptography` for all algorithms described in JWA
+- Json Web Keys (JWK) loading, dumping and generation
+- Arbitrary data signature and verification using Json Web Keys
+- Json Web Signatures (JWS) signing and verification
+- Json Web Encryption (JWE) encryption and decryption
+- Json Web Tokens (JWT) signing, verification and validation
+- 100% type annotated, verified with `mypy --strict`
+- nearly 100% code coverage
+- Relies on [cryptography](https://cryptography.io) for all cryptographic operations
+- Relies on [BinaPy](https://guillp.github.io/binapy/) for binary data manipulations
+
+### Supported Token Types
+
+
+| Token Type                | Support                                                  |
+| ------------------------- | -------------------------------------------------------- |
+| Json Web Signature (JWS)  | ☑ Compact<br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |
+| Json Web Encryption (JWE) | ☑ Compact<br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |
+| Json Web Tokens (JWT)     | ☑ Signed<br/> ☑ Signed and Encrypted                   |
+
+### Supported Signature algorithms
+
+
+| Signature Alg | Description                                    | Key Type | Reference                          | Note                           |
+| ------------- | ---------------------------------------------- | -------- | ---------------------------------- | ------------------------------ |
+| HS256         | HMAC using SHA-256                             | oct      | [RFC7518, Section 3.2]             |                                |
+| HS384         | HMAC using SHA-384                             | oct      | [RFC7518, Section 3.2]             |                                |
+| HS512         | HMAC using SHA-512                             | oct      | [RFC7518, Section 3.2]             |                                |
+| RS256         | RSASSA-PKCS1-v1_5 using SHA-256                | RSA      | [RFC7518, Section 3.3]             |                                |
+| RS384         | RSASSA-PKCS1-v1_5 using SHA-384                | RSA      | [RFC7518, Section 3.3]             |                                |
+| RS512         | RSASSA-PKCS1-v1_5 using SHA-512                | RSA      | [RFC7518, Section 3.3]             |                                |
+| ES256         | ECDSA using P-256 and SHA-256                  | EC       | [RFC7518, Section 3.4]             |                                |
+| ES384         | ECDSA using P-384 and SHA-384                  | EC       | [RFC7518, Section 3.4]             |                                |
+| ES512         | ECDSA using P-521 and SHA-512                  | EC       | [RFC7518, Section 3.4]             |                                |
+| PS256         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 3.5]             |                                |
+| PS384         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384 | RSA      | [RFC7518, Section 3.5]             |                                |
+| PS512         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512 | RSA      | [RFC7518, Section 3.5]             |                                |
+| EdDSA         | EdDSA signature algorithms                     | OKP      | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |
+| ES256K        | ECDSA using secp256k1 curve and SHA-256        | EC       | [RFC8812, Section 3.2]             |                                |
+| HS1           | HMAC using SHA-1                               | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| RS1           | RSASSA-PKCS1-v1_5 with SHA-1                   | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| none          | No digital signature or MAC performed          |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
+
+### Supported Key Management algorithms
+
+
+| Signature Alg      | Description                                    | Key Type | Reference                          | Note        |
+| ------------------ | ---------------------------------------------- | -------- | ---------------------------------- | ----------- |
+| RSA1_5             | RSAES-PKCS1-v1_5                               | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |
+| RSA-OAEP           | RSAES OAEP using default parameters            | RSA      | [RFC7518, Section 4.3]             |             |
+| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 4.3]             |             |
+| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
+| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
+| A128KW             | AES Key Wrap using 128-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| A192KW             | AES Key Wrap using 192-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| A256KW             | AES Key Wrap using 256-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
+| dir                | Direct use of a shared symmetric key           | oct      | [RFC7518, Section 4.5]             |             |
+| ECDH-ES            | ECDH-ES using Concat KDF                       | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
+| A128GCMKW          | Key wrapping with AES GCM using 128-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| A192GCMKW          | Key wrapping with AES GCM using 192-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| A256GCMKW          | Key wrapping with AES GCM using 256-bit key    | oct      | [RFC7518, Section 4.7]             |             |
+| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+
+### Supported Encryption algorithms
+
+
+| Signature Alg | Description                                                 | Reference                |
+| ------------- | ----------------------------------------------------------- | ------------------------ |
+| A128CBC-HS256 | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
+| A192CBC-HS384 | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
+| A256CBC-HS512 | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
+| A128GCM       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
+| A192GCM       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
+| A256GCM       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
+
+### Supported Elliptic Curves
+
+
+| Curve     | Description                           | Key Type | Usage                 | Reference                  |
+| --------- | ------------------------------------- | -------- | --------------------- | -------------------------- |
+| P-256     | P-256 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| P-384     | P-384 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| P-521     | P-521 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| Ed25519   | Ed25519 signature algorithm key pairs | OKP      | signature             | [RFC8037, Section 3.1]     |
+| Ed448     | Ed448 signature algorithm key pairs   | OKP      | signature             | [RFC8037, Section 3.1]     |
+| X25519    | X25519 function key pairs             | OKP      | encryption            | [RFC8037, Section 3.2]     |
+| X448      | X448 function key pairs               | OKP      | encryption            | [RFC8037, Section 3.2]     |
+| secp256k1 | SECG secp256k1 curve                  | EC       | signature, encryption | [RFC8812, Section 3.1]     |
+
+## Why a new lib ?
+
+There are already multiple modules implementing JOSE and Json Web Crypto related specifications in Python. However, I
+have been dissatisfied by all of them so far, so I decided to come up with my own module.
+
+- [PyJWT](https://pyjwt.readthedocs.io)
+- [JWCrypto](https://jwcrypto.readthedocs.io/)
+- [Python-JOSE](https://python-jose.readthedocs.io/)
+- [AuthLib](https://docs.authlib.org/en/latest/jose/)
+
+Not to say that those are _bad_ libs (I actually use `jwcrypto` myself for `jwskate` unit tests), but they either don't
+support some important features, lack documentation, or generally have APIs that don't feel easy-enough, Pythonic-enough
+to use.
+
+## Design
+
+### JWK are dicts
+
+JWK are specified as JSON objects, which are parsed as `dict` in Python. The `Jwk` class in `jwskate` is actually a
+`dict` subclass, so you can use it exactly like you would use a dict: you can access its members, dump it back as JSON,
+etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. You cannot change the key cryptographic
+material, however, since that would lead to unusable keys.
+
+### JWA Wrappers
+
+You can use `cryptography` to do the cryptographic operations that are described in
+[JWA](https://www.rfc-editor.org/info/rfc7518), but since `cryptography` is a general purpose library, its usage is not
+straightforward and gives you plenty of options to carefully select and combine, leaving room for mistakes, errors and
+confusion. It has also a quite inconsistent API to handle the different type of keys and algorithms. To work around
+this, `jwskate` comes with a set of consistent wrappers that implement the exact JWA specifications, with minimum risk
+of mistakes.
+
+### Safe Signature Verification
+
+As advised in [JWT Best Practices][rfc8725] $3.1:
+
+For every signature verification method in `jwskate`, the expected signature(s) algorithm(s) must be specified. That is
+to avoid a security flaw where your application accepts tokens with a weaker encryption scheme than what your security
+policy mandates; or even worse, where it accepts unsigned tokens, or tokens that are symmetrically signed with an
+improperly used public key, leaving your application exposed to exploitation by attackers.
+
+To specify which signature algorithms are accepted, each signature verification method accepts, in order of preference:
+
+- an `alg` parameter which contains the expected algorithm, or an `algs` parameter which contains a list of acceptable
+  algorithms
+- the `alg` parameter from the signature verification `Jwk`, if present. This `alg` is the algorithm intended for use
+  with that key.
+
+Note that you cannot use `alg` and `algs` at the same time. If your `Jwk` contains an `alg` parameter, and you provide
+an `alg` or `algs` which does not match that value, a `Warning` will be emitted.
+
+## TODO
+
+- Complete/enhance/proof-read documentation
+- Better exceptions (create dedicated exception classes, better messages, etc.)
+- Support for JWE in JSON format
+- Better tests
+- Support for Selective-Disclosure JWT
+
+## Credits
+
+All cryptographic operations are handled by [cryptography](https://cryptography.io).
 
+[rfc7515]: https://www.rfc-editor.org/rfc/rfc7515.html
+[rfc7516]: https://www.rfc-editor.org/rfc/rfc7516.html
+[rfc7517]: https://www.rfc-editor.org/rfc/rfc7517.html
+[rfc7518]: https://www.rfc-editor.org/rfc/rfc7518.html
+[rfc7518, section 3.2]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.2
+[rfc7518, section 3.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.3
+[rfc7518, section 3.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.4
+[rfc7518, section 3.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.5
+[rfc7518, section 3.6]: https://www.rfc-editor.org/rfc/rfc7518.html#section-3.6
+[rfc7518, section 4.2]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.2
+[rfc7518, section 4.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.3
+[rfc7518, section 4.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.4
+[rfc7518, section 4.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.5
+[rfc7518, section 4.6]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.6
+[rfc7518, section 4.7]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.7
+[rfc7518, section 4.8]: https://www.rfc-editor.org/rfc/rfc7518.html#section-4.8
+[rfc7518, section 5.2.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.3
+[rfc7518, section 5.2.4]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.4
+[rfc7518, section 5.2.5]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.2.5
+[rfc7518, section 5.3]: https://www.rfc-editor.org/rfc/rfc7518.html#section-5.3
+[rfc7518, section 6.2.1.1]: https://www.rfc-editor.org/rfc/rfc7518.html#section-6.2.1.1
+[rfc7519]: https://www.rfc-editor.org/rfc/rfc7519.html
+[rfc7638]: https://www.rfc-editor.org/rfc/rfc7638.html
+[rfc8037]: https://www.rfc-editor.org/rfc/rfc8037.html
+[rfc8037, section 3.1]: https://www.rfc-editor.org/rfc/rfc8037.html#section-3.1
+[rfc8037, section 3.2]: https://www.rfc-editor.org/rfc/rfc8037.html#section-3.2
+[rfc8725]: https://www.rfc-editor.org/rfc/rfc8725
+[rfc8812, section 3.1]: https://www.rfc-editor.org/rfc/rfc8812.html#section-3.1
+[rfc8812, section 3.2]: https://www.rfc-editor.org/rfc/rfc8812.html#name-ecdsa-signature-with-secp25
+[rfc9278]: https://www.rfc-editor.org/rfc/rfc9278.html
 
-setup(**setup_kwargs)
```

