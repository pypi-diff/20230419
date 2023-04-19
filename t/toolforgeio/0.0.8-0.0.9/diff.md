# Comparing `tmp/toolforgeio-0.0.8.tar.gz` & `tmp/toolforgeio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforgeio-0.0.8.tar", last modified: Mon Jan 30 01:09:45 2023, max compression
+gzip compressed data, was "toolforgeio-0.0.9.tar", last modified: Wed Apr 19 03:36:43 2023, max compression
```

## Comparing `toolforgeio-0.0.8.tar` & `toolforgeio-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-01-30 01:09:45.210651 toolforgeio-0.0.8/
--rw-r--r--   0 aboothe    (501) staff       (20)    11357 2023-01-26 17:46:40.000000 toolforgeio-0.0.8/LICENSE
--rw-r--r--   0 aboothe    (501) staff       (20)    13697 2023-01-30 01:09:45.210492 toolforgeio-0.0.8/PKG-INFO
--rw-r--r--   0 aboothe    (501) staff       (20)      186 2023-01-26 17:53:40.000000 toolforgeio-0.0.8/README.md
--rw-r--r--   0 aboothe    (501) staff       (20)      917 2023-01-30 01:06:38.000000 toolforgeio-0.0.8/pyproject.toml
--rw-r--r--   0 aboothe    (501) staff       (20)       38 2023-01-30 01:09:45.210683 toolforgeio-0.0.8/setup.cfg
-drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-01-30 01:09:45.209825 toolforgeio-0.0.8/toolforgeio/
--rw-r--r--   0 aboothe    (501) staff       (20)      150 2023-01-30 01:06:21.000000 toolforgeio-0.0.8/toolforgeio/__init__.py
--rw-r--r--   0 aboothe    (501) staff       (20)     2321 2023-01-27 00:25:29.000000 toolforgeio-0.0.8/toolforgeio/arguments.py
--rw-r--r--   0 aboothe    (501) staff       (20)     6231 2023-01-29 23:54:55.000000 toolforgeio-0.0.8/toolforgeio/io.py
--rw-r--r--   0 aboothe    (501) staff       (20)     7099 2023-01-29 23:54:55.000000 toolforgeio-0.0.8/toolforgeio/manifest.py
-drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-01-30 01:09:45.210341 toolforgeio-0.0.8/toolforgeio.egg-info/
--rw-r--r--   0 aboothe    (501) staff       (20)    13697 2023-01-30 01:09:45.000000 toolforgeio-0.0.8/toolforgeio.egg-info/PKG-INFO
--rw-r--r--   0 aboothe    (501) staff       (20)      297 2023-01-30 01:09:45.000000 toolforgeio-0.0.8/toolforgeio.egg-info/SOURCES.txt
--rw-r--r--   0 aboothe    (501) staff       (20)        1 2023-01-30 01:09:45.000000 toolforgeio-0.0.8/toolforgeio.egg-info/dependency_links.txt
--rw-r--r--   0 aboothe    (501) staff       (20)      121 2023-01-30 01:09:45.000000 toolforgeio-0.0.8/toolforgeio.egg-info/requires.txt
--rw-r--r--   0 aboothe    (501) staff       (20)       12 2023-01-30 01:09:45.000000 toolforgeio-0.0.8/toolforgeio.egg-info/top_level.txt
+drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-04-19 03:36:43.787514 toolforgeio-0.0.9/
+-rw-r--r--   0 aboothe    (501) staff       (20)    11357 2023-01-26 17:46:40.000000 toolforgeio-0.0.9/LICENSE
+-rw-r--r--   0 aboothe    (501) staff       (20)    13697 2023-04-19 03:36:43.787371 toolforgeio-0.0.9/PKG-INFO
+-rw-r--r--   0 aboothe    (501) staff       (20)      186 2023-01-26 17:53:40.000000 toolforgeio-0.0.9/README.md
+-rw-r--r--   0 aboothe    (501) staff       (20)      917 2023-04-19 03:36:12.000000 toolforgeio-0.0.9/pyproject.toml
+-rw-r--r--   0 aboothe    (501) staff       (20)       38 2023-04-19 03:36:43.787548 toolforgeio-0.0.9/setup.cfg
+drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-04-19 03:36:43.786275 toolforgeio-0.0.9/tests/
+-rw-r--r--   0 aboothe    (501) staff       (20)     2050 2023-01-29 23:54:55.000000 toolforgeio-0.0.9/tests/test_arguments.py
+-rw-r--r--   0 aboothe    (501) staff       (20)     1952 2023-04-19 03:28:59.000000 toolforgeio-0.0.9/tests/test_io.py
+-rw-r--r--   0 aboothe    (501) staff       (20)     2197 2023-01-26 21:39:21.000000 toolforgeio-0.0.9/tests/test_manifest.py
+drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-04-19 03:36:43.786705 toolforgeio-0.0.9/toolforgeio/
+-rw-r--r--   0 aboothe    (501) staff       (20)      150 2023-01-30 01:06:21.000000 toolforgeio-0.0.9/toolforgeio/__init__.py
+-rw-r--r--   0 aboothe    (501) staff       (20)     2321 2023-01-27 00:25:29.000000 toolforgeio-0.0.9/toolforgeio/arguments.py
+-rw-r--r--   0 aboothe    (501) staff       (20)     6832 2023-04-19 03:32:13.000000 toolforgeio-0.0.9/toolforgeio/io.py
+-rw-r--r--   0 aboothe    (501) staff       (20)     7099 2023-01-29 23:54:55.000000 toolforgeio-0.0.9/toolforgeio/manifest.py
+drwxr-xr-x   0 aboothe    (501) staff       (20)        0 2023-04-19 03:36:43.787215 toolforgeio-0.0.9/toolforgeio.egg-info/
+-rw-r--r--   0 aboothe    (501) staff       (20)    13697 2023-04-19 03:36:43.000000 toolforgeio-0.0.9/toolforgeio.egg-info/PKG-INFO
+-rw-r--r--   0 aboothe    (501) staff       (20)      361 2023-04-19 03:36:43.000000 toolforgeio-0.0.9/toolforgeio.egg-info/SOURCES.txt
+-rw-r--r--   0 aboothe    (501) staff       (20)        1 2023-04-19 03:36:43.000000 toolforgeio-0.0.9/toolforgeio.egg-info/dependency_links.txt
+-rw-r--r--   0 aboothe    (501) staff       (20)      121 2023-04-19 03:36:43.000000 toolforgeio-0.0.9/toolforgeio.egg-info/requires.txt
+-rw-r--r--   0 aboothe    (501) staff       (20)       12 2023-04-19 03:36:43.000000 toolforgeio-0.0.9/toolforgeio.egg-info/top_level.txt
```

### Comparing `toolforgeio-0.0.8/LICENSE` & `toolforgeio-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforgeio-0.0.8/PKG-INFO` & `toolforgeio-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforgeio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for building tools in the ToolForge Data Science tools ecosystem using Python
 Author-email: Andy Boothe <andy@toolforge.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `toolforgeio-0.0.8/pyproject.toml` & `toolforgeio-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toolforgeio"
-version = "0.0.8"
+version = "0.0.9"
 description = "Library for building tools in the ToolForge Data Science tools ecosystem using Python"
 readme = "README.md"
 authors = [{ name = "Andy Boothe", email = "andy@toolforge.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `toolforgeio-0.0.8/toolforgeio/arguments.py` & `toolforgeio-0.0.9/toolforgeio/arguments.py`

 * *Files identical despite different names*

### Comparing `toolforgeio-0.0.8/toolforgeio/io.py` & `toolforgeio-0.0.9/toolforgeio/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,23 +69,24 @@
         the_encoding = default_encoding
     else:
         the_encoding = detected_encoding["encoding"]
 
     return TextIOWrapper(f, encoding=the_encoding, errors=errors)
 
 
-def read_input_spreadsheet_data_frame(url: str, prefix="/tmp") -> DataFrame:
+def read_input_spreadsheet_data_frame(url: str, prefix="/tmp", sheet_hint=None) -> DataFrame:
     """
     Downloads a spreadsheet file from the given url and returns a pandas dataframe loaded from the
     resulting data. The type of the spreadsheet is detected automatically, and may be either CSV,
     XLS, or XLSX. If the downloaded spreadsheet contains more than one sheet, then the active sheet
     -- or the sheet that shows on file open -- is returned.
 
     :param url: The URL from which to download the spreadsheet
     :param prefix: A directory into which to place the downloaded file
+    :param sheet_hint: If there are multiple sheets, use the named sheet if it exists
     :return: A pandas dataframe containing the data from the spreadsheet
     """
 
     # It turns out that the extension of the file when opened is significant,
     # so to avoid the file copy we generate a filename only the fly as we
     # download to reflect the expected file type.
 
@@ -111,22 +112,38 @@
                 for chunk in iterator:
                     fout.write(chunk)
     else:
         raise ValueError("Unrecognized url protocol", url)
 
     if extension == "xlsx":
         wb = openpyxl.load_workbook(filepath)
-        active_sheet_name = wb.active.title
-        print(f"Found Excel XLSX workbook, processing active sheet {active_sheet_name}...")
-        return read_excel(filepath, sheet_name=active_sheet_name)
+
+        chosen_sheet_name = None
+        if chosen_sheet_name is None:
+            if sheet_hint is not None and sheet_hint in wb.sheetnames:
+                chosen_sheet_name = sheet_hint
+        if chosen_sheet_name is None:
+            chosen_sheet_name = wb.active.title
+
+        print(f"Found Excel XLSX workbook, processing active sheet {chosen_sheet_name}...")
+        
+        return read_excel(filepath, sheet_name=chosen_sheet_name)
     elif extension == "xls":
         wb = xlrd.open_workbook(filepath)
-        active_sheet_name = [s.name for s in wb.sheets() if s.sheet_visible == 1][0]
-        print(f"Found Excel XLS workbook, processing active sheet {active_sheet_name}...")
-        return read_excel(filepath, sheet_name=active_sheet_name)
+
+        chosen_sheet_name = None
+        if chosen_sheet_name is None:
+            if sheet_hint is not None:
+                chosen_sheet_name = next(iter([s.name for s in wb.sheets() if s.name == sheet_hint]), None)
+        if chosen_sheet_name is None:
+            chosen_sheet_name = [s.name for s in wb.sheets() if s.sheet_visible == 1][0]
+
+        print(f"Found Excel XLS workbook, processing sheet {chosen_sheet_name}...")
+
+        return read_excel(filepath, sheet_name=chosen_sheet_name)
     elif extension == "csv":
         with _decode(open(filepath, "rb")) as f:
             result = read_csv(f)
         return result
     else:
         raise ValueError("Unrecognized file extension", extension)
```

### Comparing `toolforgeio-0.0.8/toolforgeio/manifest.py` & `toolforgeio-0.0.9/toolforgeio/manifest.py`

 * *Files identical despite different names*

### Comparing `toolforgeio-0.0.8/toolforgeio.egg-info/PKG-INFO` & `toolforgeio-0.0.9/toolforgeio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforgeio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for building tools in the ToolForge Data Science tools ecosystem using Python
 Author-email: Andy Boothe <andy@toolforge.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

