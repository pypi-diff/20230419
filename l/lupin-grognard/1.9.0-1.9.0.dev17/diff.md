# Comparing `tmp/lupin-grognard-1.9.0.tar.gz` & `tmp/lupin-grognard-1.9.0.dev17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-1.9.0.tar", last modified: Wed Apr 19 07:44:20 2023, max compression
+gzip compressed data, was "lupin-grognard-1.9.0.dev17.tar", last modified: Thu Apr 13 08:07:28 2023, max compression
```

## Comparing `lupin-grognard-1.9.0.tar` & `lupin-grognard-1.9.0.dev17.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0/LICENCE
--rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.576193 lupin-grognard-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.493409 lupin-grognard-1.9.0/lupin_grognard/
--rw-rw-rw-   0        0        0       23 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.517953 lupin-grognard-1.9.0/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-03-30 22:12:23.000000 lupin-grognard-1.9.0/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.522952 lupin-grognard-1.9.0/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     7379 2023-03-31 14:48:46.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     5739 2023-04-06 08:21:25.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1319 2023-04-06 08:19:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.526457 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/
--rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/__init__.py
--rw-rw-rw-   0        0        0    11845 2023-03-28 14:31:51.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/changelog.py
--rw-rw-rw-   0        0        0     1472 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/jinja_generator.py
--rw-rw-rw-   0        0        0     4958 2023-03-30 13:35:56.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/reviewlog.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.528466 lupin-grognard-1.9.0/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2709 2023-03-26 23:00:29.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/cmake_format.py
--rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-1.9.0/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.530464 lupin-grognard-1.9.0/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/__init__.py
--rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     5854 2023-03-31 13:35:54.000000 lupin-grognard-1.9.0/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/lupin_grognard/templates/
--rw-rw-rw-   0        0        0     1848 2023-03-28 13:46:34.000000 lupin-grognard-1.9.0/lupin_grognard/templates/changelog.j2
--rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-1.9.0/lupin_grognard/templates/reviewlog.j2
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.512439 lupin-grognard-1.9.0/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      933 2023-04-19 07:44:20.577191 lupin-grognard-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.696843 lupin-grognard-1.9.0.dev17/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0.dev17/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev17/MANIFEST.in
+-rw-rw-rw-   0        0        0      514 2023-04-13 08:07:28.697842 lupin-grognard-1.9.0.dev17/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0.dev17/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.616973 lupin-grognard-1.9.0.dev17/lupin_grognard/
+-rw-rw-rw-   0        0        0       29 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.638194 lupin-grognard-1.9.0.dev17/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-03-30 22:12:23.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.644258 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     7379 2023-03-31 14:48:46.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     5739 2023-04-06 08:21:25.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1319 2023-04-06 08:19:58.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.648257 lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    11845 2023-03-28 14:31:51.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     1472 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     4958 2023-03-30 13:35:56.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/reviewlog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.650764 lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-03-26 23:00:29.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.651770 lupin-grognard-1.9.0.dev17/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     5854 2023-03-31 13:35:54.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.696843 lupin-grognard-1.9.0.dev17/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1848 2023-03-28 13:46:34.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-1.9.0.dev17/lupin_grognard/templates/reviewlog.j2
+drwxrwxrwx   0        0        0        0 2023-04-13 08:07:28.634194 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      514 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 08:07:28.000000 lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      939 2023-04-13 08:07:28.701841 lupin-grognard-1.9.0.dev17/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev17/setup.py
```

### Comparing `lupin-grognard-1.9.0/LICENCE` & `lupin-grognard-1.9.0.dev17/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/check.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/check.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/cmd.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_error.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/commit/commit_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/config.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/config.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/changelog.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/changelog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/jinja_generator.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/jinja_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/reviewlog.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/doc_generator/reviewlog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/clang_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/format/cmake_format.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/format/cmake_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/git.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/git.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/run.py` & `lupin-grognard-1.9.0.dev17/lupin_grognard/run.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/templates/changelog.j2` & `lupin-grognard-1.9.0.dev17/lupin_grognard/templates/changelog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/templates/reviewlog.j2` & `lupin-grognard-1.9.0.dev17/lupin_grognard/templates/reviewlog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-1.9.0.dev17/lupin_grognard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/setup.cfg` & `lupin-grognard-1.9.0.dev17/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
 00000020: 640d 0a76 6572 7369 6f6e 203d 2031 2e39  d..version = 1.9
-00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
-00000040: 3d20 4c75 7069 6e20 6c69 6e74 6572 2074  = Lupin linter t
-00000050: 6f6f 6c0d 0a6c 6f6e 675f 6465 7363 7269  ool..long_descri
-00000060: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000070: 4144 4d45 2e6d 640d 0a6b 6579 776f 7264  ADME.md..keyword
-00000080: 7320 3d20 636c 692c 206c 696e 7465 720d  s = cli, linter.
-00000090: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
-000000a0: 6963 656e 7365 0d0a 636c 6173 7369 6669  icense..classifi
-000000b0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000000c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000000d0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-000000e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000000f0: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
-00000100: 6e6f 6c6f 6779 0d0a 0954 6f70 6963 203a  nology...Topic :
-00000110: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000120: 6f70 6d65 6e74 203a 3a20 5175 616c 6974  opment :: Qualit
-00000130: 7920 4173 7375 7261 6e63 650d 0a09 5072  y Assurance...Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 332e 3130 0d0a 094c 6963 656e 7365 203a  3.10...License :
-00000170: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000180: 3a20 4d49 5420 4c69 6365 6e73 650d 0a0d  : MIT License...
-00000190: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
-000001a0: 7361 6665 203d 2046 616c 7365 0d0a 696e  safe = False..in
-000001b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000001c0: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
-000001d0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001f0: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
-00000200: 6571 7569 7265 7320 3d20 0d0a 0974 7970  equires = ...typ
-00000210: 6572 5b61 6c6c 5d3d 3d30 2e36 2e31 0d0a  er[all]==0.6.1..
-00000220: 0970 7974 686f 6e2d 646f 7465 6e76 3d3d  .python-dotenv==
-00000230: 302e 3231 2e30 0d0a 0965 6d6f 6a69 3d3d  0.21.0...emoji==
-00000240: 322e 322e 300d 0a09 4a69 6e6a 6132 3d3d  2.2.0...Jinja2==
-00000250: 332e 312e 320d 0a09 636d 616b 656c 616e  3.1.2...cmakelan
-00000260: 673d 3d30 2e36 2e31 330d 0a09 5079 5941  g==0.6.13...PyYA
-00000270: 4d4c 3d3d 362e 300d 0a0d 0a5b 6f70 7469  ML==6.0....[opti
-00000280: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
-00000290: 7265 5d0d 0a74 6573 7420 3d20 0d0a 0970  re]..test = ...p
-000002a0: 7974 6573 743d 3d37 2e31 2e33 0d0a 0966  ytest==7.1.3...f
-000002b0: 6c61 6b65 383d 3d35 2e30 2e34 0d0a 0d0a  lake8==5.0.4....
-000002c0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-000002d0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-000002e0: 7363 7269 7074 7320 3d20 0d0a 0967 726f  scripts = ...gro
-000002f0: 6720 3d20 6c75 7069 6e5f 6772 6f67 6e61  g = lupin_grogna
-00000300: 7264 2e72 756e 3a63 6c69 0d0a 0d0a 5b6f  rd.run:cli....[o
-00000310: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000320: 6174 615d 0d0a 2a20 3d20 2a2e 636c 616e  ata]..* = *.clan
-00000330: 672d 666f 726d 6174 0d0a 0d0a 5b6f 7074  g-format....[opt
-00000340: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000350: 6e64 5d0d 0a65 7863 6c75 6465 203d 200d  nd]..exclude = .
-00000360: 0a09 6c75 7069 6e5f 6772 6f67 6e61 7264  ..lupin_grognard
-00000370: 2e74 6573 7473 2a0d 0a0d 0a5b 6567 675f  .tests*....[egg_
-00000380: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000390: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000003a0: 300d 0a0d 0a                             0....
+00000030: 2e30 2e64 6576 3137 0d0a 6465 7363 7269  .0.dev17..descri
+00000040: 7074 696f 6e20 3d20 4c75 7069 6e20 6c69  ption = Lupin li
+00000050: 6e74 6572 2074 6f6f 6c0d 0a6c 6f6e 675f  nter tool..long_
+00000060: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+00000070: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6b  le: README.md..k
+00000080: 6579 776f 7264 7320 3d20 636c 692c 206c  eywords = cli, l
+00000090: 696e 7465 720d 0a6c 6963 656e 7365 203d  inter..license =
+000000a0: 204d 4954 204c 6963 656e 7365 0d0a 636c   MIT License..cl
+000000b0: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
+000000c0: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+000000d0: 7320 3a3a 2033 202d 2041 6c70 6861 0d0a  s :: 3 - Alpha..
+000000e0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000000f0: 6365 203a 3a20 496e 666f 726d 6174 696f  ce :: Informatio
+00000100: 6e20 5465 6368 6e6f 6c6f 6779 0d0a 0954  n Technology...T
+00000110: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000120: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000130: 5175 616c 6974 7920 4173 7375 7261 6e63  Quality Assuranc
+00000140: 650d 0a09 5072 6f67 7261 6d6d 696e 6720  e...Programming 
+00000150: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000160: 6f6e 203a 3a20 332e 3130 0d0a 094c 6963  on :: 3.10...Lic
+00000170: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000180: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000190: 6e73 650d 0a0d 0a5b 6f70 7469 6f6e 735d  nse....[options]
+000001a0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
+000001b0: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
+000001c0: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+000001d0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000001e0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000001f0: 6573 203d 203e 3d33 2e31 300d 0a69 6e73  es = >=3.10..ins
+00000200: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000210: 0d0a 0974 7970 6572 5b61 6c6c 5d3d 3d30  ...typer[all]==0
+00000220: 2e36 2e31 0d0a 0970 7974 686f 6e2d 646f  .6.1...python-do
+00000230: 7465 6e76 3d3d 302e 3231 2e30 0d0a 0965  tenv==0.21.0...e
+00000240: 6d6f 6a69 3d3d 322e 322e 300d 0a09 4a69  moji==2.2.0...Ji
+00000250: 6e6a 6132 3d3d 332e 312e 320d 0a09 636d  nja2==3.1.2...cm
+00000260: 616b 656c 616e 673d 3d30 2e36 2e31 330d  akelang==0.6.13.
+00000270: 0a09 5079 5941 4d4c 3d3d 362e 300d 0a0d  ..PyYAML==6.0...
+00000280: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000290: 5f72 6571 7569 7265 5d0d 0a74 6573 7420  _require]..test 
+000002a0: 3d20 0d0a 0970 7974 6573 743d 3d37 2e31  = ...pytest==7.1
+000002b0: 2e33 0d0a 0966 6c61 6b65 383d 3d35 2e30  .3...flake8==5.0
+000002c0: 2e34 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  .4....[options.e
+000002d0: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
+000002e0: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
+000002f0: 0d0a 0967 726f 6720 3d20 6c75 7069 6e5f  ...grog = lupin_
+00000300: 6772 6f67 6e61 7264 2e72 756e 3a63 6c69  grognard.run:cli
+00000310: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000320: 6b61 6765 5f64 6174 615d 0d0a 2a20 3d20  kage_data]..* = 
+00000330: 2a2e 636c 616e 672d 666f 726d 6174 0d0a  *.clang-format..
+00000340: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000350: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
+00000360: 6465 203d 200d 0a09 6c75 7069 6e5f 6772  de = ...lupin_gr
+00000370: 6f67 6e61 7264 2e74 6573 7473 2a0d 0a0d  ognard.tests*...
+00000380: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000390: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000003a0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

