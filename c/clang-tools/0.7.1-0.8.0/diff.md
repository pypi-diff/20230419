# Comparing `tmp/clang_tools-0.7.1-py3-none-any.whl.zip` & `tmp/clang_tools-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10208 bytes, number of entries: 10
--rw-r--r--  2.0 unx      209 b- defN 23-Mar-12 02:38 clang_tools/__init__.py
--rw-r--r--  2.0 unx    10568 b- defN 23-Mar-12 02:38 clang_tools/install.py
--rw-r--r--  2.0 unx     1932 b- defN 23-Mar-12 02:38 clang_tools/main.py
--rw-r--r--  2.0 unx     3443 b- defN 23-Mar-12 02:38 clang_tools/util.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5841 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      816 b- defN 23-Mar-12 02:39 clang_tools-0.7.1.dist-info/RECORD
-10 files, 24034 bytes uncompressed, 8814 bytes compressed:  63.3%
+Zip file size: 10215 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      209 b- defN 23-Apr-19 05:19 clang_tools/__init__.py
+-rw-r--r--  2.0 unx    10568 b- defN 23-Apr-19 05:19 clang_tools/install.py
+-rw-r--r--  2.0 unx     1932 b- defN 23-Apr-19 05:19 clang_tools/main.py
+-rw-r--r--  2.0 unx     3443 b- defN 23-Apr-19 05:19 clang_tools/util.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5922 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      816 b- defN 23-Apr-19 05:19 clang_tools-0.8.0.dist-info/RECORD
+10 files, 24115 bytes uncompressed, 8821 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: clang_tools/main.py
 Comment: 
 
 Filename: clang_tools/util.py
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/LICENSE
+Filename: clang_tools-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/METADATA
+Filename: clang_tools-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/WHEEL
+Filename: clang_tools-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/entry_points.txt
+Filename: clang_tools-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/top_level.txt
+Filename: clang_tools-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clang_tools-0.7.1.dist-info/RECORD
+Filename: clang_tools-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clang_tools/install.py

```diff
@@ -59,15 +59,15 @@
         ver_num is None or ver_num[0] != ver_major
     ):
         return None  # version is unknown or not the desired major release
     return path
 
 
 def clang_tools_binary_url(
-    tool: str, version: str, release_tag: str = "master-1d7ec53d"
+    tool: str, version: str, release_tag: str = "master-9ba48406"
 ) -> str:
     """Assemble the URL to the binary.
 
     :param tool: The name of the tool to download.
     :param version: The version of the tool to download.
     :param release_tag: The release tag used in the base URL.
```

## Comparing `clang_tools-0.7.1.dist-info/LICENSE` & `clang_tools-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clang_tools-0.7.1.dist-info/METADATA` & `clang_tools-0.8.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clang-tools
-Version: 0.7.1
+Version: 0.8.0
 Summary: Install clang-tools (clang-format, clang-tidy) with pip
 Author-email: Peter Shen <xianpeng.shen@gmail.com>, Brendan Doherty <2bndy5@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/cpp-linter/clang-tools-pip
 Project-URL: tracker, https://github.com/cpp-linter/clang-tools-pip/issues
 Keywords: clang,clang-tools,clang-extra,clang-tidy,clang-format
 Classifier: Development Status :: 4 - Beta
@@ -142,32 +142,32 @@
 
 Supported versions
 ------------------
 
 clang-format
 ************
 .. csv-table::
-    :header: "Version", "15", "14", "13", "12", "11", "10", "9", "8", "7", "6", "5", "4", "3.9"
+    :header: "Version", "16", "15", "14", "13", "12", "11", "10", "9", "8", "7", "6", "5", "4", "3.9"
     :stub-columns: 1
 
-    Linux,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
-    Windows,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
-    macOS,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    Linux,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    Windows,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    macOS,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
 
 clang-tidy
 **********
 .. csv-table::
-    :header: "Version", "15", "14", "13", "12", "11", "10", "9", "8", "7", "6", "5", "4", "3.9"
+    :header: "Version", "16", "15", "14", "13", "12", "11", "10", "9", "8", "7", "6", "5", "4", "3.9"
     :stub-columns: 1
 
-    Linux,❌,❌,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
-    Windows,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
-    macOS,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    Linux,❌,❌,❌,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    Windows,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
+    macOS,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️,✔️
 
 Know issues:
 
-1. clang-tidy-14 and clang-tidy-15 has Segmentation fault on Ubuntu 22.02.
-2. clang-tidy-14 and clang-tidy-15 is over 1 GB for MacOSX
+1. clang-tidy-14, clang-tidy-15 and clang-tidy-16 has Segmentation fault on Ubuntu 22.02.
+2. clang-tidy-14, clang-tidy-15 and clang-tidy-16 is over 1 GB for MacOSX
 
 Thanks to the project
 `clang-tools-static-binaries <https://github.com/muttleyxd/clang-tools-static-binaries>`_
 for all the binaries.
```

## Comparing `clang_tools-0.7.1.dist-info/RECORD` & `clang_tools-0.8.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 clang_tools/__init__.py,sha256=3b9IYik-KHkyUd416rhK3MfXOVdwPTB5jrg0nJnatjo,209
-clang_tools/install.py,sha256=sKMAY2RbPWo1EMETN0gakoGq8wKuNLFKRQKLvgbR9Kw,10568
+clang_tools/install.py,sha256=_ix5MfILJ0SAKeMnW3J5LKSiboNQa-4XNrk2bOzanLE,10568
 clang_tools/main.py,sha256=sSztwi3p-yc3iC2MXAI2ii3m2SXtwTz99W3uOM_2JF0,1932
 clang_tools/util.py,sha256=x9sKUBcunOQWAxHVzUDBu-DWKzbsqJR-ldrYDhlQhro,3443
-clang_tools-0.7.1.dist-info/LICENSE,sha256=8jYtzp-KuZ4iRI55Gyi1CsGpjwkQe-Jzc0ekP254TdE,1067
-clang_tools-0.7.1.dist-info/METADATA,sha256=7iOyzxjsQVSaA_UykNhH_qNsFv2ViRmJ4mInA7IMPn0,5841
-clang_tools-0.7.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-clang_tools-0.7.1.dist-info/entry_points.txt,sha256=XyeMmYDJvU0g6SrifX71jFpGuOFAKL0fh_h1ln8mzHQ,54
-clang_tools-0.7.1.dist-info/top_level.txt,sha256=DTkgJyAN8hk0g-e2m8luhAyyfCT-8sPHtcJfjfCfQkA,12
-clang_tools-0.7.1.dist-info/RECORD,,
+clang_tools-0.8.0.dist-info/LICENSE,sha256=8jYtzp-KuZ4iRI55Gyi1CsGpjwkQe-Jzc0ekP254TdE,1067
+clang_tools-0.8.0.dist-info/METADATA,sha256=4TSrpS5N8wlu96LyAqaF74SF0Iatsvd-AgW4AZJq2aw,5922
+clang_tools-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+clang_tools-0.8.0.dist-info/entry_points.txt,sha256=XyeMmYDJvU0g6SrifX71jFpGuOFAKL0fh_h1ln8mzHQ,54
+clang_tools-0.8.0.dist-info/top_level.txt,sha256=DTkgJyAN8hk0g-e2m8luhAyyfCT-8sPHtcJfjfCfQkA,12
+clang_tools-0.8.0.dist-info/RECORD,,
```

