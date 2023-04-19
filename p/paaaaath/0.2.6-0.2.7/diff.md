# Comparing `tmp/paaaaath-0.2.6.tar.gz` & `tmp/paaaaath-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paaaaath-0.2.6.tar", max compression
+gzip compressed data, was "paaaaath-0.2.7.tar", max compression
```

## Comparing `paaaaath-0.2.6.tar` & `paaaaath-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1070 2022-10-12 01:48:37.765787 paaaaath-0.2.6/LICENSE
--rw-r--r--   0        0        0     5558 2022-10-12 01:48:37.765787 paaaaath-0.2.6/README.md
--rw-r--r--   0        0        0      677 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/__init__.py
--rw-r--r--   0        0        0     1034 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/blob.py
--rw-r--r--   0        0        0     8894 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/common.py
--rw-r--r--   0        0        0     2850 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/gcs.py
--rw-r--r--   0        0        0      789 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/http.py
--rw-r--r--   0        0        0      212 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/posix.py
--rw-r--r--   0        0        0     3319 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/s3.py
--rw-r--r--   0        0        0     1956 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/uri.py
--rw-r--r--   0        0        0      222 2022-10-12 01:48:37.765787 paaaaath-0.2.6/paaaaath/windows.py
--rw-r--r--   0        0        0     1591 2022-10-12 01:49:26.206118 paaaaath-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6775 1970-01-01 00:00:00.000000 paaaaath-0.2.6/setup.py
--rw-r--r--   0        0        0     6738 1970-01-01 00:00:00.000000 paaaaath-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-19 15:21:24.342969 paaaaath-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5570 2023-04-19 15:21:24.342969 paaaaath-0.2.7/README.md
+-rw-r--r--   0        0        0      677 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/blob.py
+-rw-r--r--   0        0        0     8894 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/common.py
+-rw-r--r--   0        0        0     2850 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/gcs.py
+-rw-r--r--   0        0        0      789 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/http.py
+-rw-r--r--   0        0        0      212 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/posix.py
+-rw-r--r--   0        0        0     3319 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/s3.py
+-rw-r--r--   0        0        0     1956 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/uri.py
+-rw-r--r--   0        0        0      222 2023-04-19 15:21:24.346969 paaaaath-0.2.7/paaaaath/windows.py
+-rw-r--r--   0        0        0     1597 2023-04-19 15:21:54.103165 paaaaath-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6704 1970-01-01 00:00:00.000000 paaaaath-0.2.7/PKG-INFO
```

### Comparing `paaaaath-0.2.6/LICENSE` & `paaaaath-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/README.md` & `paaaaath-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
 [download-shield]: https://img.shields.io/pypi/dm/paaaaath?style=for-the-badge
 [download-url]: https://pypi.org/project/paaaaath/
 [version-shield]: https://img.shields.io/pypi/v/paaaaath?style=for-the-badge
 [version-url]: https://pypi.org/project/paaaaath/
-[build-shiled]: https://img.shields.io/github/workflow/status/ar90n/paaaaath/CI?style=for-the-badge
+[build-shiled]: https://img.shields.io/github/actions/workflow/status/ar90n/paaaaath/ci.yml?style=for-the-badge
 [build-url]: https://github.com/ar90n/paaaaath/actions/workflows/ci.yml
 [contributors-shield]: https://img.shields.io/github/contributors/ar90n/paaaaath.svg?style=for-the-badge
 [contributors-url]: https://github.com/ar90n/paaaaath/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/ar90n/paaaaath.svg?style=for-the-badge
 [forks-url]: https://github.com/ar90n/paaaaath/network/members
 [stars-shield]: https://img.shields.io/github/stars/ar90n/paaaaath.svg?style=for-the-badge
 [stars-url]: https://github.com/ar90n/paaaaath/stargazers
```

### Comparing `paaaaath-0.2.6/paaaaath/__init__.py` & `paaaaath-0.2.7/paaaaath/__init__.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/blob.py` & `paaaaath-0.2.7/paaaaath/blob.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/common.py` & `paaaaath-0.2.7/paaaaath/common.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/gcs.py` & `paaaaath-0.2.7/paaaaath/gcs.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/http.py` & `paaaaath-0.2.7/paaaaath/http.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/s3.py` & `paaaaath-0.2.7/paaaaath/s3.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/paaaaath/uri.py` & `paaaaath-0.2.7/paaaaath/uri.py`

 * *Files identical despite different names*

### Comparing `paaaaath-0.2.6/pyproject.toml` & `paaaaath-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "paaaaath"
-version = "0.2.6"
+version = "0.2.7"
 description = "a useful alternative Path object"
 authors = ["Masahiro Wada <argon.argon.argon@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/ar90n/paaaaath"
 readme = "README.md"
 keywords = ["path", "s3", "gcs", "cloud"]
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.7,<3.11"
 smart-open = "^5.0"
 
 # optional
 boto3 = {version = "^1.17.36", optional = true}
 google-cloud-storage = {version = "^1.36.2", optional = true}
 requests = {version = "^2.25.1", optional = true}
 importlib_metadata = {version = "^3.7", python = "~3.7"}
@@ -62,8 +62,7 @@
 [tool.pysen.lint.source]
 excludes = ["tests"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
-
```

### Comparing `paaaaath-0.2.6/PKG-INFO` & `paaaaath-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: paaaaath
-Version: 0.2.6
+Version: 0.2.7
 Summary: a useful alternative Path object
 Home-page: https://github.com/ar90n/paaaaath
 License: MIT
 Keywords: path,s3,gcs,cloud
 Author: Masahiro Wada
 Author-email: argon.argon.argon@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: gcs
 Provides-Extra: http
 Provides-Extra: s3
-Requires-Dist: boto3 (>=1.17.36,<2.0.0); extra == "s3" or extra == "all"
-Requires-Dist: google-cloud-storage (>=1.36.2,<2.0.0); extra == "gcs" or extra == "all"
-Requires-Dist: importlib_metadata (>=3.7,<4.0); python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: requests (>=2.25.1,<3.0.0); extra == "http" or extra == "all"
+Requires-Dist: boto3 (>=1.17.36,<2.0.0) ; extra == "s3" or extra == "all"
+Requires-Dist: google-cloud-storage (>=1.36.2,<2.0.0) ; extra == "gcs" or extra == "all"
+Requires-Dist: importlib_metadata (>=3.7,<4.0) ; python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: requests (>=2.25.1,<3.0.0) ; extra == "http" or extra == "all"
 Requires-Dist: smart-open (>=5.0,<6.0)
 Project-URL: Repository, https://github.com/ar90n/paaaaath
 Description-Content-Type: text/markdown
 
 [![Build][build-shiled]][build-url]
 [![Version][version-shield]][version-url]
 [![Downloads][download-shield]][download-url]
@@ -172,15 +171,15 @@
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
 [download-shield]: https://img.shields.io/pypi/dm/paaaaath?style=for-the-badge
 [download-url]: https://pypi.org/project/paaaaath/
 [version-shield]: https://img.shields.io/pypi/v/paaaaath?style=for-the-badge
 [version-url]: https://pypi.org/project/paaaaath/
-[build-shiled]: https://img.shields.io/github/workflow/status/ar90n/paaaaath/CI?style=for-the-badge
+[build-shiled]: https://img.shields.io/github/actions/workflow/status/ar90n/paaaaath/ci.yml?style=for-the-badge
 [build-url]: https://github.com/ar90n/paaaaath/actions/workflows/ci.yml
 [contributors-shield]: https://img.shields.io/github/contributors/ar90n/paaaaath.svg?style=for-the-badge
 [contributors-url]: https://github.com/ar90n/paaaaath/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/ar90n/paaaaath.svg?style=for-the-badge
 [forks-url]: https://github.com/ar90n/paaaaath/network/members
 [stars-shield]: https://img.shields.io/github/stars/ar90n/paaaaath.svg?style=for-the-badge
 [stars-url]: https://github.com/ar90n/paaaaath/stargazers
```

