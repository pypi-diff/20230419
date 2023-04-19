# Comparing `tmp/get_certificate_chain-0.1.3.tar.gz` & `tmp/get_certificate_chain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_certificate_chain-0.1.3.tar", max compression
+gzip compressed data, was "get_certificate_chain-0.1.4.tar", max compression
```

## Comparing `get_certificate_chain-0.1.3.tar` & `get_certificate_chain-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     4108 2023-04-18 12:03:44.815919 get_certificate_chain-0.1.3/README.md
--rw-r--r--   0        0        0    15854 2023-04-18 11:55:16.287746 get_certificate_chain-0.1.3/get_certificate_chain/download.py
--rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.3/get_certificate_chain/tests/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-18 11:52:31.295015 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_cert.py
--rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/generate_cert.sh
--rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/root_ca.cnf
--rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/server.cnf
--rw-r--r--   0        0        0      817 2023-04-18 11:43:18.978436 get_certificate_chain-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     4108 2023-04-18 12:03:44.815919 get_certificate_chain-0.1.4/README.md
+-rw-r--r--   0        0        0    17251 2023-04-19 12:10:11.716503 get_certificate_chain-0.1.4/get_certificate_chain/download.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.4/get_certificate_chain/tests/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-18 12:05:07.771317 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_cert.py
+-rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/generate_cert.sh
+-rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/root_ca.cnf
+-rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/server.cnf
+-rw-r--r--   0        0        0      817 2023-04-19 11:36:01.301319 get_certificate_chain-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.4/PKG-INFO
```

### Comparing `get_certificate_chain-0.1.3/LICENSE.md` & `get_certificate_chain-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.3/README.md` & `get_certificate_chain-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.3/get_certificate_chain/download.py` & `get_certificate_chain-0.1.4/get_certificate_chain/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This script connects to a given website, downloads its SSL certificate,
 and saves it as a PEM file. If the certificate has an Authority Information
 Access (AIA) extension, the script will download each certificate in the chain
 and save them as PEM files as well.
 
 """
 # Standard library imports
-import glob
 import os
 import logging
 import re
 import ssl
 import socket
 import sys
 from typing import Any, Dict, List, Union
@@ -22,22 +21,17 @@
 # Third-party library imports
 import argparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 CERT_CHAIN = []
 
-# Configure logging
-logging.basicConfig(
-    level=logging.WARNING, format="%(asctime)s [%(levelname)s] %(message)s"
-)
-
 
 # parse arguments
 def parse_arguments() -> argparse.Namespace:
     """
     Parse command line arguments.
 
     Returns:
@@ -55,34 +49,57 @@
     parser.add_argument(
         "--get-ca-cert-pem",
         dest="get_ca_cert_pem",
         action="store_true",
         help="Get cacert.pem from curl.se website to help find Root CA.",
     )
     parser.add_argument(
-        "--url",
-        dest="url",
+        "--log-level",
+        dest="log_level",
+        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+        default="WARNING",
+        help="Set the logging level. (default: %(default)s)",
+    )
+    parser.add_argument(
+        "--output-dir",
+        dest="output_dir",
+        default=".",
+        help="The output directory for the certificate chain files. (default: current directory)",
+    )
+    parser.add_argument(
+        "--host",
+        dest="host",
         default="www.google.com",
-        help="The url to connect to. (default: %(default)s)",
+        help="The host to connect to. (default: %(default)s)",
     )
     return parser.parse_args()
 
 
 class SSLCertificateChainDownloader:
-    def __init__(self):
+    def __init__(self, output_directory: str = None):
         self.cert_chain = []
+        self._output_directory = output_directory
+
+    @property
+    def output_directory(self) -> str:
+        return self._output_directory if self._output_directory else "."
 
     def remove_cacert_pem(self):
         """
         Remove certificate files from the current directory.
         """
-        for crt_file in glob.glob("*.crt"):
-            os.remove(crt_file)
-        for pem_file in glob.glob("*.pem"):
-            os.remove(pem_file)
+        logging.info("Removing certificate files from current directory.")
+
+        output_directory = self.output_directory if self.output_directory else "."
+
+        for filename in os.listdir(output_directory):
+            if filename.endswith(".crt") or filename == "cacert.pem":
+                filepath = os.path.join(output_directory, filename)
+                os.remove(filepath)
+                logging.info(f"Removed {filename}")
 
     def get_cacert_pem(self):
         """
         Download the cacert.pem file from the curl.se website.
         """
         cacert_pem_url = "https://curl.se/ca/cacert.pem"
         cacert_pem_file = "cacert.pem"
@@ -99,56 +116,56 @@
                 sys.exit(1)
             data = response.read()
             out_file.write(data)
         logging.info("Downloaded %s to %s", cacert_pem_url, cacert_pem_file)
 
     def check_url(self) -> Dict[str, Any]:
         """
-        Check and parse the url provided by the user.
+        Check and parse the host provided by the user.
 
         Args:
-            url (str): The url provided by the user.
+            host (str): The host provided by the user.
 
         Returns:
-            Dict[str, Any]: A dictionary containing the url and port.
+            Dict[str, Any]: A dictionary containing the host and port.
         """
-        url, _, port = self.url.partition(":")
-        return {"url": url, "port": int(port) if port else 443}
+        host, _, port = self.host.partition(":")
+        return {"host": host, "port": int(port) if port else 443}
 
-    def get_certificate(self, url: str, port: int) -> x509.Certificate:
+    def get_certificate(self, host: str, port: int) -> x509.Certificate:
         """
         Connect to a server and retrieve the SSL certificate.
 
         Args:
-            url (str): The url to connect to.
+            host (str): The host to connect to.
             port (int): The port to connect to.
 
         Returns:
             x509.Certificate: The SSL certificate of the server.
         """
         try:
             context = ssl.create_default_context()
-            with socket.create_connection((url, port)) as sock:
-                with context.wrap_socket(sock, server_hostname=url) as ssl_socket:
+            with socket.create_connection((host, port)) as sock:
+                with context.wrap_socket(sock, server_hostname=host) as ssl_socket:
                     cert_pem = ssl.DER_cert_to_PEM_cert(ssl_socket.getpeercert(True))
                     cert = x509.load_pem_x509_certificate(
                         cert_pem.encode(), default_backend()
                     )
             return cert
         except ConnectionRefusedError:
-            logging.error("Connection refused to %s:%s", url, port)
+            logging.error("Connection refused to %s:%s", host, port)
             sys.exit(1)
         except ssl.SSLError as e:
             logging.error("SSL error: %s", e)
             sys.exit(1)
         except socket.timeout:
-            logging.error("Connection timed out to %s:%s", url, port)
+            logging.error("Connection timed out to %s:%s", host, port)
             sys.exit(1)
         except socket.gaierror:
-            logging.error("Hostname could not be resolved: %s", url)
+            logging.error("Hostname could not be resolved: %s", host)
             sys.exit(1)
 
     def normalize_subject(self, subject: str) -> str:
         """
         Normalize the subject of a certificate.
 
         Args:
@@ -178,28 +195,34 @@
         Args:
             ssl_certificate (x509.Certificate): The SSL certificate to save.
             file_name (str): The file name to save the SSL certificate as.
         """
         with open(file_name, "wb") as f:
             f.write(ssl_certificate.public_bytes(encoding=serialization.Encoding.PEM))
 
-    def write_chain_to_file(self, certificate_chain: List[x509.Certificate]) -> None:
+    def write_chain_to_file(
+        self, certificate_chain: List[x509.Certificate], output_dir: str = "."
+    ) -> None:
         """
         Write a certificate chain to files.
 
         Args:
             certificate_chain (List[x509.Certificate]): The certificate chain to write to files.
         """
+        os.makedirs(self.output_directory, exist_ok=True)
         for counter, certificate_item in enumerate(certificate_chain):
             cert_subject = certificate_item.subject.rfc4514_string()
             normalized_subject = self.normalize_subject(cert_subject)
             ssl_certificate_filename = (
                 f"{len(certificate_chain) - 1 - counter}-{normalized_subject}.crt"
             )
-            self.save_ssl_certificate(certificate_item, ssl_certificate_filename)
+            ssl_certificate_filepath = os.path.join(
+                self.output_directory, ssl_certificate_filename
+            )
+            self.save_ssl_certificate(certificate_item, ssl_certificate_filepath)
 
     def return_cert_aia(self, ssl_certificate: x509.Certificate) -> x509.Extensions:
         """
         Get the Authority Information Access (AIA) extension from a certificate.
 
         Args:
             ssl_certificate (x509.Certificate): The SSL certificate.
@@ -407,17 +430,17 @@
 
                     if root_ca_cn is None:
                         logging.error("Root CA NOT found.")
                         sys.exit(1)
 
     def run(self, args: Union[argparse.Namespace, dict]):
         if isinstance(args, argparse.Namespace):
-            self.url = args.url
+            self.host = args.host
         elif isinstance(args, dict):
-            self.url = args.get("url")
+            self.host = args.get("host")
         else:
             raise ValueError(
                 "Invalid argument type. Expected argparse.Namespace or dict."
             )
 
         self.parsed_url = self.check_url()
 
@@ -425,21 +448,23 @@
             remove_ca_files = args.remove_ca_files
             get_ca_cert_pem = args.get_ca_cert_pem
         else:
             remove_ca_files = args.get("remove_ca_files")
             get_ca_cert_pem = args.get("get_ca_cert_pem")
 
         if remove_ca_files:
-            self.remove_ca_files()
+            self.remove_cacert_pem()
+            return
 
         if get_ca_cert_pem:
-            self.get_ca_cert_pem()
+            self.get_cacert_pem()
+            return
 
         ssl_certificate = self.get_certificate(
-            self.parsed_url["url"], self.parsed_url["port"]
+            self.parsed_url["host"], self.parsed_url["port"]
         )
 
         aia = self.return_cert_aia(ssl_certificate)
 
         if aia is not None and not self.return_cert_aia(ssl_certificate):
             logging.error(
                 "Could not find AIA, possible decryption taking place upstream?"
@@ -457,13 +482,22 @@
 
 def main() -> None:
     """
     Main function to execute the script. Parses arguments, retrieves the SSL certificate, walks the chain,
     and writes the certificate chain and PEM-encoded certificates.
     """
     args = parse_arguments()
-    downloader = SSLCertificateChainDownloader()
+
+    log_level = getattr(logging, args.log_level.upper(), None)
+    if not isinstance(log_level, int):
+        raise ValueError(f"Invalid log level: {args.log_level}")
+
+    logging.basicConfig(
+        level=log_level, format="%(asctime)s [%(levelname)s] %(message)s"
+    )
+
+    downloader = SSLCertificateChainDownloader(output_directory=args.output_dir)
     downloader.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `get_certificate_chain-0.1.3/get_certificate_chain/tests/test_cert.py` & `get_certificate_chain-0.1.4/get_certificate_chain/tests/test_cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import pytest
-from main import (
+from download import (
     SSLCertificateChainDownloader,
 )
 
 
 @pytest.fixture
 def root_ca_cert():
     with open(
```

### Comparing `get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/server.cnf` & `get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/server.cnf`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.3/pyproject.toml` & `get_certificate_chain-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get_certificate_chain"
-version = "0.1.3"
+version = "0.1.4"
 description = "Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files."
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>", " TheScriptGuy <@nolanrumble>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `get_certificate_chain-0.1.3/PKG-INFO` & `get_certificate_chain-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-certificate-chain
-Version: 0.1.3
+Version: 0.1.4
 Summary: Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files.
 License: MIT
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

