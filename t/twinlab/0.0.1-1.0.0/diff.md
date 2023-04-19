# Comparing `tmp/twinlab-0.0.1.tar.gz` & `tmp/twinlab-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-0.0.1.tar", max compression
+gzip compressed data, was "twinlab-1.0.0.tar", max compression
```

## Comparing `twinlab-0.0.1.tar` & `twinlab-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1048 2023-04-11 13:00:56.988184 twinlab-0.0.1/README.md
--rw-r--r--   0        0        0      599 2023-04-13 18:59:14.918264 twinlab-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      567 2023-04-13 18:03:34.457859 twinlab-0.0.1/twinlab/__init__.py
--rw-r--r--   0        0        0     5314 2023-04-13 18:03:34.464734 twinlab-0.0.1/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-04-13 18:03:34.464988 twinlab-0.0.1/twinlab/plotting.py
--rw-r--r--   0        0        0      532 2023-04-05 20:53:11.331012 twinlab-0.0.1/twinlab/settings.py
--rw-r--r--   0        0        0     3846 2023-04-13 18:03:34.469148 twinlab-0.0.1/twinlab/utils.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.0.0/README.md
+-rw-r--r--   0        0        0      599 2023-04-19 16:13:39.405004 twinlab-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-04-19 16:13:39.405689 twinlab-1.0.0/twinlab/__init__.py
+-rw-r--r--   0        0        0     5340 2023-04-19 16:13:39.406087 twinlab-1.0.0/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-04-13 16:09:18.757239 twinlab-1.0.0/twinlab/plotting.py
+-rw-r--r--   0        0        0      532 2023-04-11 15:58:49.585681 twinlab-1.0.0/twinlab/settings.py
+-rw-r--r--   0        0        0     3864 2023-04-19 16:13:39.406342 twinlab-1.0.0/twinlab/utils.py
+-rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-1.0.0/PKG-INFO
```

### Comparing `twinlab-0.0.1/README.md` & `twinlab-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-0.0.1/pyproject.toml` & `twinlab-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "0.0.1"
+version = "1.0.0"
 description = "Client interface for twinLab"
 authors = ["Alexander Mead <alexander@digilab.co.uk>", "Freddy Wordingham <freddy@digilab.co.uk>"]
 repository = "https://github.com/digiLab-ai/twinLab-client"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
```

### Comparing `twinlab-0.0.1/twinlab/client.py` & `twinlab-1.0.0/twinlab/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 # Project imports
 from . import utils
 
 ### Dataset functions ###
 
 
-def upload_dataset(filepath: str, server="cloud", verbose=False) -> None:
-    """
-    Upload dataset
-    TODO: Retire in favour of upload_big_dataset?
-    """
-    url = utils.get_server_url(server) + "/upload_dataset"
-    files = {"file": (filepath, open(filepath, "rb"), "text/csv")}
-    headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
-    r = requests.post(url, files=files, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
+# def upload_small_dataset(filepath: str, server="cloud", verbose=False) -> None:
+#     """
+#     Upload dataset
+#     TODO: Retire in favour of upload_big_dataset?
+#     """
+#     url = utils.get_server_url(server) + "/upload_dataset"
+#     files = {"file": (filepath, open(filepath, "rb"), "text/csv")}
+#     headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
+#     r = requests.post(url, files=files, headers=headers)
+#     utils.check_response(r)
+#     if verbose:
+#         utils.print_response_message(r)
 
 
-def upload_big_dataset(filepath: str, server="cloud", verbose=False) -> None:
+def upload_dataset(filepath: str, server="cloud", verbose=False) -> None:
     """
     Upload big dataset
     TODO: Replace upload_dataset with this?
     """
     lambda_url = utils.get_server_url(server) + "/generate_upload_url"
     headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
     headers["X-Dataset"] = filepath
```

### Comparing `twinlab-0.0.1/twinlab/settings.py` & `twinlab-1.0.0/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-0.0.1/twinlab/utils.py` & `twinlab-1.0.0/twinlab/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return baseURL
 
 ### ###
 
 ### HTTP requests ###
 
 
-def upload_file_to_presigned_url(file_path, presigned_url, verbose=False):
+def upload_file_to_presigned_url(file_path: str, presigned_url: str, verbose=False) -> None:
     """
     Upload a file to the specified pre-signed URL.
 
     :param file_path: The path to the file you want to upload.
     :param presigned_url: The pre-signed URL generated for uploading the file.
     :return: True if the upload is successful, False otherwise.
     """
```

### Comparing `twinlab-0.0.1/PKG-INFO` & `twinlab-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 0.0.1
+Version: 1.0.0
 Summary: Client interface for twinLab
 Home-page: https://github.com/digiLab-ai/twinLab-client
 Author: Alexander Mead
 Author-email: alexander@digilab.co.uk
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

