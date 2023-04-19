# Comparing `tmp/ygt-0.1.3.tar.gz` & `tmp/ygt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.1.3.tar", last modified: Mon Apr 17 22:47:49 2023, max compression
+gzip compressed data, was "ygt-0.1.4.tar", last modified: Wed Apr 19 18:35:13 2023, max compression
```

## Comparing `ygt-0.1.3.tar` & `ygt-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.022160 ygt-0.1.3/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.3/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.3/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     2417 2023-04-17 22:47:49.022026 ygt-0.1.3/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     2021 2023-04-17 21:42:41.000000 ygt-0.1.3/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-17 21:31:23.000000 ygt-0.1.3/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-17 22:47:49.022198 ygt-0.1.3/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.3/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.006921 ygt-0.1.3/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.013398 ygt-0.1.3/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.3/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.3/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.3/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     4771 2023-04-17 11:45:55.000000 ygt-0.1.3/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.014352 ygt-0.1.3/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.3/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    12008 2023-04-17 10:52:42.000000 ygt-0.1.3/src/ygt/freetypeFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.021816 ygt-0.1.3/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.3/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.3/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.3/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.3/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.3/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.3/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.3/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.3/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.3/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    55765 2023-04-11 17:09:51.000000 ygt-0.1.3/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    64711 2023-04-17 10:32:58.000000 ygt-0.1.3/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.3/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   112941 2023-04-16 17:05:35.000000 ygt-0.1.3/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   136647 2023-04-15 23:29:54.000000 ygt-0.1.3/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.3/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    22475 2023-04-17 16:29:50.000000 ygt-0.1.3/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10000 2023-04-13 02:48:06.000000 ygt-0.1.3/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     4847 2023-04-15 15:27:33.000000 ygt-0.1.3/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.3/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.014247 ygt-0.1.3/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     2417 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.3/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.975925 ygt-0.1.4/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.4/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.4/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-19 18:35:13.975801 ygt-0.1.4/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2443 2023-04-19 18:25:54.000000 ygt-0.1.4/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-19 18:06:11.000000 ygt-0.1.4/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-19 18:35:13.975956 ygt-0.1.4/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.4/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.960430 ygt-0.1.4/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.966839 ygt-0.1.4/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.4/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.4/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.4/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5390 2023-04-19 16:46:17.000000 ygt-0.1.4/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.967737 ygt-0.1.4/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.4/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12272 2023-04-19 13:14:59.000000 ygt-0.1.4/src/ygt/freetypeFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.975601 ygt-0.1.4/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.4/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.4/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.4/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.4/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.4/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.4/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.4/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.4/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.4/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    55765 2023-04-11 17:09:51.000000 ygt-0.1.4/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    64711 2023-04-17 10:32:58.000000 ygt-0.1.4/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.4/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   112941 2023-04-16 17:05:35.000000 ygt-0.1.4/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   136673 2023-04-19 17:52:17.000000 ygt-0.1.4/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.4/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22475 2023-04-17 16:29:50.000000 ygt-0.1.4/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10000 2023-04-13 02:48:06.000000 ygt-0.1.4/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4847 2023-04-15 15:27:33.000000 ygt-0.1.4/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.4/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.967619 ygt-0.1.4/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.4/src/ygt.py
```

### Comparing `ygt-0.1.3/LICENSE` & `ygt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/PKG-INFO` & `ygt-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,14 +26,24 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-Version 0.1.23 (2023-4-17) changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
+### Version 0.1.24 (2023-4-19)
+
+When we read a UFO, we do not rename glyphs. This prevents incompatibilities between in-memory font and font on disk, and it simplifies export. However, it may complicate shifting back and forth between UFO and YAML modes.
+
+Ygt sometimes hung when summoning a Font View window for fonts read from UFO. This is now fixed.
+
+Program now (partly) honors dark themes on various platforms.
+
+### Version 0.1.23 (2023-4-17)
+
+changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
 ```
 s/blackspace/blackdist/g
 s/whitesapce/whitedist/g
 s/grayspace/graydist/g
 ```
 Among other changes intended to improve stability, this version consolidates various font-level edits in a “Font Info” dialog, summoned with Ctrl-I or Cmd-I, and honors “dark themes” on various platforms.
```

### Comparing `ygt-0.1.3/README.md` & `ygt-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-Version 0.1.23 (2023-4-17) changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
+### Version 0.1.24 (2023-4-19)
+
+When we read a UFO, we do not rename glyphs. This prevents incompatibilities between in-memory font and font on disk, and it simplifies export. However, it may complicate shifting back and forth between UFO and YAML modes.
+
+Ygt sometimes hung when summoning a Font View window for fonts read from UFO. This is now fixed.
+
+Program now (partly) honors dark themes on various platforms.
+
+### Version 0.1.23 (2023-4-17)
+
+changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
 ```
 s/blackspace/blackdist/g
 s/whitesapce/whitedist/g
 s/grayspace/graydist/g
 ```
 Among other changes intended to improve stability, this version consolidates various font-level edits in a “Font Info” dialog, summoned with Ctrl-I or Cmd-I, and honors “dark themes” on various platforms.
```

### Comparing `ygt-0.1.3/pyproject.toml` & `ygt-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ygt"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "A graphical hint editor for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
@@ -17,15 +17,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "PyQt6 >= 6.4.0",
     "fonttools >= 4.38.0",
     "freetype-py >= 2.3.0",
     "defcon >= 0.10.1",
-    "xgridfit >= 3.2.16",
+    "xgridfit >= 3.2.17",
     "setuptools >= 65.3.0",
     "PyYAML >= 6.0",
     "schema >= 0.7.5",
     "fs >= 2.4.15",
     "ufo2ft >= 2.28.0",
     "numpy",
 ]
```

### Comparing `ygt-0.1.3/src/ygt/autohint_trash.py` & `ygt-0.1.4/src/ygt/autohint_trash.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/cvGuesser.py` & `ygt-0.1.4/src/ygt/cvGuesser.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/fontViewDialog.py` & `ygt-0.1.4/src/ygt/fontViewDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from .freetypeFont import freetypeFont, RENDER_GRAYSCALE
+from fontTools import subset
 from .ygModel import ygFont
 from math import ceil
 from PyQt6.QtCore import Qt, QRect, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QDialog, QGridLayout, QVBoxLayout, QScrollArea
 from PyQt6.QtGui import QPainter, QBrush, QPen, QColor, QPalette
 import numpy
 from tempfile import SpooledTemporaryFile
+import copy
 
 
 # A window (not a dialog, despite the filename, retained to avoid complicating
 # the history in the repository) that displays all the non-composite glyphs
 # in the font, with those already hinted highlighted in blue. Click on any
 # glyph in the window to navigate to that glyph.
 
@@ -27,20 +29,31 @@
     def __init__(
             self, filename: str, yg_font: ygFont, glyph_list: list, top_window
         ) -> None:
         super().__init__()
         self.valid = True
         self.top_window = top_window
         self.setWindowTitle("Font View")
+        self.glyph_name_list = []
+        self.name_to_index = {}
+        for g in glyph_list:
+            self.glyph_name_list.append(g[1])
+            self.name_to_index[g[1]] = g[0]
         self.yg_font = yg_font
         if self.yg_font.source_file.source_type == "yaml":
             self.face = freetypeFont(filename, size=24, render_mode=RENDER_GRAYSCALE)
         else:
+            temp_font = copy.deepcopy(self.yg_font.preview_font)
             tf = SpooledTemporaryFile(max_size=3000000, mode='b')
-            self.yg_font.preview_font.save(tf, 1)
+            options = subset.Options(glyph_names=True)
+            options.layout_features = []
+            subsetter = subset.Subsetter(options)
+            subsetter.populate(glyphs=self.glyph_name_list)
+            subsetter.subset(temp_font)
+            temp_font.save(tf, 1)
             tf.seek(0)
             self.face = freetypeFont(tf, size=24, render_mode=RENDER_GRAYSCALE)
             tf.close()
         if not self.face.valid:
             self.valid = False
             return
         self.glyph_list = glyph_list
@@ -116,15 +129,17 @@
                 brush.setColor(QColor("black"))
             else:
                 brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
-        self.dialog.face.set_char(self.dialog.face.name_to_index(self.glyph))
+        # self.dialog.face.set_char(self.dialog.face.name_to_index(self.glyph))
+        ind = self.dialog.face.name_to_index(self.glyph)
+        self.dialog.face.set_char(ind)
         baseline = (
             round((36 - self.dialog.face.face_height) / 2) + self.dialog.face.ascender
         )
         xpos = round((36 - self.dialog.face.advance) / 2)
         self.dialog.face.draw_char(painter, xpos, baseline, dark_theme = dark_theme)
 
         painter.end()
```

### Comparing `ygt-0.1.3/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.1.4/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/freetypeFont.py` & `ygt-0.1.4/src/ygt/freetypeFont.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
         """
         self.glyph_index = glyph_index
         flags = 4  # i.e. grayscale
         if self.render_mode in [RENDER_LCD_1, RENDER_LCD_2]:
             flags = ft.FT_LOAD_RENDER | ft.FT_LOAD_TARGET_LCD
         if not self.hinting_on:
             flags = flags | ft.FT_LOAD_NO_HINTING | ft.FT_LOAD_NO_AUTOHINT
+        # For some UFOs, font view is hanging here (with load_glyph). It doesn't
+        # hang except with
+        # UFOs, and it generates the preview well from the same in-memory TTFont.
+        # So what are we doing differently when generating the font view?
         self.face.load_glyph(self.glyph_index, flags=flags)
         self.glyph_slot = self.face.glyph
         self.advance = round(self.glyph_slot.advance.x / 64)
         self.bitmap_top = self.glyph_slot.bitmap_top
         self.bitmap_left = self.glyph_slot.bitmap_left
         self.top_offset = self.ascender - self.bitmap_top
```

### Comparing `ygt-0.1.3/src/ygt/icons/align.png` & `ygt-0.1.4/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/anchor.png` & `ygt-0.1.4/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/black_distance.png` & `ygt-0.1.4/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/cursor-icon-off.png` & `ygt-0.1.4/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/cursor-icon-on.png` & `ygt-0.1.4/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/cv.png` & `ygt-0.1.4/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/cv_guess.png` & `ygt-0.1.4/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/gray_distance.png` & `ygt-0.1.4/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/hand-icon-off.png` & `ygt-0.1.4/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/hand-icon-on.png` & `ygt-0.1.4/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/horizontal-off.png` & `ygt-0.1.4/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/horizontal-on.png` & `ygt-0.1.4/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/interpolate.png` & `ygt-0.1.4/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/make_set.png` & `ygt-0.1.4/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/program.png` & `ygt-0.1.4/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/shift.png` & `ygt-0.1.4/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/stem_distance.png` & `ygt-0.1.4/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/vertical-off.png` & `ygt-0.1.4/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/vertical-on.png` & `ygt-0.1.4/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/icons/white_distance.png` & `ygt-0.1.4/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/macfuncDialog.py` & `ygt-0.1.4/src/ygt/macfuncDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/makeCVDialog.py` & `ygt-0.1.4/src/ygt/makeCVDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/window.py` & `ygt-0.1.4/src/ygt/window.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygError.py` & `ygt-0.1.4/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygHintEditor.py` & `ygt-0.1.4/src/ygt/ygHintEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygModel.py` & `ygt-0.1.4/src/ygt/ygModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
             try:
                 self.ft_font = ttLib.TTFont(fontfile)
             except FileNotFoundError as ferr:
                 ft_open_error = True
         elif extension == ".ufo":
             try:
                 ufo = defcon.Font(fontfile)
-                self.ft_font = compileTTF(ufo)
+                self.ft_font = compileTTF(ufo, useProductionNames=False)
             except Exception as e:
                 print(e)
                 ft_open_error = True
         if ft_open_error:
             raise Exception("Can't find font file " + str(fontfile))
             # Fix this! Need a dialog box and a chance to try again for a valid font.
```

### Comparing `ygt-0.1.3/src/ygt/ygPreferences.py` & `ygt-0.1.4/src/ygt/ygPreferences.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygPreview.py` & `ygt-0.1.4/src/ygt/ygPreview.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygSchema.py` & `ygt-0.1.4/src/ygt/ygSchema.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygStems.py` & `ygt-0.1.4/src/ygt/ygStems.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt/ygYAMLEditor.py` & `ygt-0.1.4/src/ygt/ygYAMLEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.3/src/ygt.egg-info/PKG-INFO` & `ygt-0.1.4/src/ygt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,14 +26,24 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-Version 0.1.23 (2023-4-17) changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
+### Version 0.1.24 (2023-4-19)
+
+When we read a UFO, we do not rename glyphs. This prevents incompatibilities between in-memory font and font on disk, and it simplifies export. However, it may complicate shifting back and forth between UFO and YAML modes.
+
+Ygt sometimes hung when summoning a Font View window for fonts read from UFO. This is now fixed.
+
+Program now (partly) honors dark themes on various platforms.
+
+### Version 0.1.23 (2023-4-17)
+
+changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
 ```
 s/blackspace/blackdist/g
 s/whitesapce/whitedist/g
 s/grayspace/graydist/g
 ```
 Among other changes intended to improve stability, this version consolidates various font-level edits in a “Font Info” dialog, summoned with Ctrl-I or Cmd-I, and honors “dark themes” on various platforms.
```

### Comparing `ygt-0.1.3/src/ygt.egg-info/SOURCES.txt` & `ygt-0.1.4/src/ygt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

