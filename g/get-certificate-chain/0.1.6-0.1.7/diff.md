# Comparing `tmp/get_certificate_chain-0.1.6.tar.gz` & `tmp/get_certificate_chain-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_certificate_chain-0.1.6.tar", max compression
+gzip compressed data, was "get_certificate_chain-0.1.7.tar", max compression
```

## Comparing `get_certificate_chain-0.1.6.tar` & `get_certificate_chain-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     4613 2023-04-19 15:09:31.250755 get_certificate_chain-0.1.6/README.md
--rw-r--r--   0        0        0    20185 2023-04-19 16:11:38.891013 get_certificate_chain-0.1.6/get_certificate_chain/download.py
--rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.6/get_certificate_chain/tests/__init__.py
--rw-r--r--   0        0        0      918 2023-04-19 15:14:44.588966 get_certificate_chain-0.1.6/get_certificate_chain/tests/test_cert.py
--rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.6/get_certificate_chain/tests/test_data/generate_cert.sh
--rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.6/get_certificate_chain/tests/test_data/root_ca.cnf
--rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.6/get_certificate_chain/tests/test_data/server.cnf
--rw-r--r--   0        0        0      841 2023-04-19 16:04:22.821635 get_certificate_chain-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     4613 2023-04-19 15:09:31.250755 get_certificate_chain-0.1.7/README.md
+-rw-r--r--   0        0        0    20166 2023-04-19 16:41:43.352720 get_certificate_chain-0.1.7/get_certificate_chain/download.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.7/get_certificate_chain/tests/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-19 15:14:44.588966 get_certificate_chain-0.1.7/get_certificate_chain/tests/test_cert.py
+-rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.7/get_certificate_chain/tests/test_data/generate_cert.sh
+-rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.7/get_certificate_chain/tests/test_data/root_ca.cnf
+-rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.7/get_certificate_chain/tests/test_data/server.cnf
+-rw-r--r--   0        0        0      841 2023-04-19 16:41:40.093579 get_certificate_chain-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.7/PKG-INFO
```

### Comparing `get_certificate_chain-0.1.6/LICENSE.md` & `get_certificate_chain-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.6/README.md` & `get_certificate_chain-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.6/get_certificate_chain/download.py` & `get_certificate_chain-0.1.7/get_certificate_chain/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Third-party library imports
 import argparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 CERT_CHAIN = []
 
 
 # parse arguments
 def parse_arguments(args: Optional[List[str]] = None) -> argparse.Namespace:
     """
     Parse command line arguments.
@@ -495,15 +495,14 @@
 
         if remove_ca_files:
             self.remove_cacert_pem()
             return
 
         if get_ca_cert_pem:
             self.get_cacert_pem()
-            return
 
         ssl_certificate = self.get_certificate(
             self.parsed_url["host"], self.parsed_url["port"]
         )
 
         aia = self.return_cert_aia(ssl_certificate)
```

### Comparing `get_certificate_chain-0.1.6/get_certificate_chain/tests/test_cert.py` & `get_certificate_chain-0.1.7/get_certificate_chain/tests/test_cert.py`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.6/get_certificate_chain/tests/test_data/server.cnf` & `get_certificate_chain-0.1.7/get_certificate_chain/tests/test_data/server.cnf`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.6/pyproject.toml` & `get_certificate_chain-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get_certificate_chain"
-version = "0.1.6"
+version = "0.1.7"
 description = "Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files."
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>", " TheScriptGuy <@nolanrumble>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `get_certificate_chain-0.1.6/PKG-INFO` & `get_certificate_chain-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-certificate-chain
-Version: 0.1.6
+Version: 0.1.7
 Summary: Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files.
 License: MIT
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

