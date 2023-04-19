# Comparing `tmp/get_certificate_chain-0.1.4.tar.gz` & `tmp/get_certificate_chain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_certificate_chain-0.1.4.tar", max compression
+gzip compressed data, was "get_certificate_chain-0.1.5.tar", max compression
```

## Comparing `get_certificate_chain-0.1.4.tar` & `get_certificate_chain-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     4108 2023-04-18 12:03:44.815919 get_certificate_chain-0.1.4/README.md
--rw-r--r--   0        0        0    17251 2023-04-19 12:10:11.716503 get_certificate_chain-0.1.4/get_certificate_chain/download.py
--rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.4/get_certificate_chain/tests/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-18 12:05:07.771317 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_cert.py
--rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/generate_cert.sh
--rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/root_ca.cnf
--rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/server.cnf
--rw-r--r--   0        0        0      817 2023-04-19 11:36:01.301319 get_certificate_chain-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     4327 2023-04-19 13:06:18.709659 get_certificate_chain-0.1.5/README.md
+-rw-r--r--   0        0        0    17345 2023-04-19 14:41:56.217486 get_certificate_chain-0.1.5/get_certificate_chain/download.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.5/get_certificate_chain/tests/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-19 15:04:54.348306 get_certificate_chain-0.1.5/get_certificate_chain/tests/test_cert.py
+-rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.5/get_certificate_chain/tests/test_data/generate_cert.sh
+-rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.5/get_certificate_chain/tests/test_data/root_ca.cnf
+-rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.5/get_certificate_chain/tests/test_data/server.cnf
+-rw-r--r--   0        0        0      841 2023-04-19 14:36:32.927449 get_certificate_chain-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.5/PKG-INFO
```

### Comparing `get_certificate_chain-0.1.4/LICENSE.md` & `get_certificate_chain-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.4/README.md` & `get_certificate_chain-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 To use the package in your script, simply import the package and create an instance of the `SSLCertificateChainDownloader` object.
 
 To pass arguments into the object, you can use the `argparse` library:
 
 1. Import the argparse library.
 2. Import the SSLCertificateChainDownloader object from the package.
-3. Create a python dictionary with the "url" key and value of the domain.
+3. Create a python dictionary with the "host" key and value of the domain.
 4. Create an instance of the SSLCertificateChainDownloader object.
 5. Run the downloader object with the parsed arguments.
 
 ```python
 from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
@@ -71,15 +71,15 @@
 
 You can pass the arguments directly into the object:
 
 ```python
 from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
-downloader.run({'url': 'www.google.com'})
+downloader.run({'host': 'www.google.com'})
 ```
 
 ![import](images/import.png)
 
 Or pass you can use the `argparse` library to parse the arguments:
 
 ```python
@@ -94,24 +94,32 @@
 ```
 
 ### Command Line CLI
 
 To use the script from the command line, run the following command:
 
 ```bash
-get-certificate-chain --url www.google.com
+get-certificate-chain --host www.google.com
 ```
 
 ![cli](images/cli.png)
 
+```bash
+get-certificate-chain --rm-ca-files
+```
+
+![cli](images/rm.png)
+
 #### Arguments
 
-- `--url`: The url:port pair that the script should connect to. Defaults to www.google.com:443.
+- `--host`: The host:port pair that the script should connect to. Defaults to www.google.com:443.
 - `--rm-ca-files`: Remove the certificate files in the current working directory (`*.crt`, `*.pem`).
-- `--get-ca-cert-pem`: Get cacert.pem from the curl.se website to help find Root CA.
+- `--get-ca-cert-pem`: Get cacert.pem from the chost.se website to help find Root CA.
+- `--log-level`: Set the log level. Defaults to INFO.
+- `--output-dir`: Set the output directory. Defaults to the current working directory.
 
 ## Contributing
 
 Contributions are welcome! To contribute, please follow these guidelines:
 
 1. Write tests for your code using `pytest`. Make sure your tests follow the standards set by the existing tests.
 2. Set up a virtual environment using `Poetry`. You can install Poetry by following the instructions at https://python-poetry.org/docs/#installation.
```

### Comparing `get_certificate_chain-0.1.4/get_certificate_chain/download.py` & `get_certificate_chain-0.1.5/get_certificate_chain/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,70 +10,70 @@
 # Standard library imports
 import os
 import logging
 import re
 import ssl
 import socket
 import sys
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 from urllib.request import urlopen
 from urllib.error import HTTPError, URLError
 
 # Third-party library imports
 import argparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 CERT_CHAIN = []
 
 
 # parse arguments
-def parse_arguments() -> argparse.Namespace:
+def parse_arguments(args: Optional[List[str]] = None) -> argparse.Namespace:
     """
     Parse command line arguments.
 
     Returns:
         argparse.Namespace: Parsed arguments.
     """
     parser = argparse.ArgumentParser(
         description="Export security rules and associated Security Profile Groups to a CSV file."
     )
     parser.add_argument(
-        "--rm-ca-files",
-        dest="remove_ca_files",
-        action="store_true",
-        help="Remove the cert files in current directory (*.crt, *.pem).",
-    )
-    parser.add_argument(
         "--get-ca-cert-pem",
         dest="get_ca_cert_pem",
         action="store_true",
         help="Get cacert.pem from curl.se website to help find Root CA.",
     )
     parser.add_argument(
+        "--host",
+        dest="host",
+        default="www.google.com",
+        help="The host to connect to. (default: %(default)s)",
+    )
+    parser.add_argument(
         "--log-level",
         dest="log_level",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
         default="WARNING",
         help="Set the logging level. (default: %(default)s)",
     )
     parser.add_argument(
         "--output-dir",
         dest="output_dir",
         default=".",
         help="The output directory for the certificate chain files. (default: current directory)",
     )
     parser.add_argument(
-        "--host",
-        dest="host",
-        default="www.google.com",
-        help="The host to connect to. (default: %(default)s)",
+        "--rm-ca-files",
+        dest="remove_ca_files",
+        action="store_true",
+        help="Remove the cert files in current directory (*.crt, *.pem).",
     )
     return parser.parse_args()
 
 
 class SSLCertificateChainDownloader:
     def __init__(self, output_directory: str = None):
         self.cert_chain = []
@@ -114,25 +114,26 @@
                     response.getcode(),
                 )
                 sys.exit(1)
             data = response.read()
             out_file.write(data)
         logging.info("Downloaded %s to %s", cacert_pem_url, cacert_pem_file)
 
-    def check_url(self) -> Dict[str, Any]:
+    @staticmethod
+    def check_url(host: str) -> Dict[str, Any]:
         """
         Check and parse the host provided by the user.
 
         Args:
             host (str): The host provided by the user.
 
         Returns:
             Dict[str, Any]: A dictionary containing the host and port.
         """
-        host, _, port = self.host.partition(":")
+        host, _, port = host.partition(":")
         return {"host": host, "port": int(port) if port else 443}
 
     def get_certificate(self, host: str, port: int) -> x509.Certificate:
         """
         Connect to a server and retrieve the SSL certificate.
 
         Args:
@@ -438,15 +439,15 @@
         elif isinstance(args, dict):
             self.host = args.get("host")
         else:
             raise ValueError(
                 "Invalid argument type. Expected argparse.Namespace or dict."
             )
 
-        self.parsed_url = self.check_url()
+        self.parsed_url = SSLCertificateChainDownloader.check_url(self.host)
 
         if isinstance(args, argparse.Namespace):
             remove_ca_files = args.remove_ca_files
             get_ca_cert_pem = args.get_ca_cert_pem
         else:
             remove_ca_files = args.get("remove_ca_files")
             get_ca_cert_pem = args.get("get_ca_cert_pem")
```

### Comparing `get_certificate_chain-0.1.4/get_certificate_chain/tests/test_cert.py` & `get_certificate_chain-0.1.5/get_certificate_chain/tests/test_cert.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     }
 
 
 def test_check_url():
     downloader = SSLCertificateChainDownloader()
 
     # Test without port
-    downloader.url = "www.google.com"
-    url = downloader.check_url()
-    assert url == {"url": "www.google.com", "port": 443}
+    downloader.host = "www.google.com"
+    host = downloader.check_url()
+    assert host == {"host": "www.google.com", "port": 443}
 
     # Test with port
-    downloader.url = "www.google.com:8443"
-    url = downloader.check_url()
-    assert url == {"url": "www.google.com", "port": 8443}
+    downloader.host = "www.google.com:8443"
+    host = downloader.check_url()
+    assert host == {"host": "www.google.com", "port": 8443}
 
 
 def test_normalize_subject():
     downloader = SSLCertificateChainDownloader()
 
     subject = "/C=US/ST=California/L=Mountain View/O=Google LLC/CN=www.google.com"
     assert (
```

### Comparing `get_certificate_chain-0.1.4/get_certificate_chain/tests/test_data/server.cnf` & `get_certificate_chain-0.1.5/get_certificate_chain/tests/test_data/server.cnf`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.4/pyproject.toml` & `get_certificate_chain-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get_certificate_chain"
-version = "0.1.4"
+version = "0.1.5"
 description = "Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files."
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>", " TheScriptGuy <@nolanrumble>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -18,14 +18,15 @@
 pytest-black = "^0.3.12"
 flake8 = "^6.0.0"
 ipython = "^8.12.0"
 ipdb = "^0.13.13"
 requests = "^2.28.2"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.scripts]
 get-certificate-chain = "get_certificate_chain.download:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `get_certificate_chain-0.1.4/PKG-INFO` & `get_certificate_chain-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-certificate-chain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files.
 License: MIT
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -72,15 +72,15 @@
 
 To use the package in your script, simply import the package and create an instance of the `SSLCertificateChainDownloader` object.
 
 To pass arguments into the object, you can use the `argparse` library:
 
 1. Import the argparse library.
 2. Import the SSLCertificateChainDownloader object from the package.
-3. Create a python dictionary with the "url" key and value of the domain.
+3. Create a python dictionary with the "host" key and value of the domain.
 4. Create an instance of the SSLCertificateChainDownloader object.
 5. Run the downloader object with the parsed arguments.
 
 ```python
 from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
@@ -89,15 +89,15 @@
 
 You can pass the arguments directly into the object:
 
 ```python
 from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
-downloader.run({'url': 'www.google.com'})
+downloader.run({'host': 'www.google.com'})
 ```
 
 ![import](images/import.png)
 
 Or pass you can use the `argparse` library to parse the arguments:
 
 ```python
@@ -112,24 +112,32 @@
 ```
 
 ### Command Line CLI
 
 To use the script from the command line, run the following command:
 
 ```bash
-get-certificate-chain --url www.google.com
+get-certificate-chain --host www.google.com
 ```
 
 ![cli](images/cli.png)
 
+```bash
+get-certificate-chain --rm-ca-files
+```
+
+![cli](images/rm.png)
+
 #### Arguments
 
-- `--url`: The url:port pair that the script should connect to. Defaults to www.google.com:443.
+- `--host`: The host:port pair that the script should connect to. Defaults to www.google.com:443.
 - `--rm-ca-files`: Remove the certificate files in the current working directory (`*.crt`, `*.pem`).
-- `--get-ca-cert-pem`: Get cacert.pem from the curl.se website to help find Root CA.
+- `--get-ca-cert-pem`: Get cacert.pem from the chost.se website to help find Root CA.
+- `--log-level`: Set the log level. Defaults to INFO.
+- `--output-dir`: Set the output directory. Defaults to the current working directory.
 
 ## Contributing
 
 Contributions are welcome! To contribute, please follow these guidelines:
 
 1. Write tests for your code using `pytest`. Make sure your tests follow the standards set by the existing tests.
 2. Set up a virtual environment using `Poetry`. You can install Poetry by following the instructions at https://python-poetry.org/docs/#installation.
```

