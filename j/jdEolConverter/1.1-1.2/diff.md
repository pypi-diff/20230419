# Comparing `tmp/jdEolConverter-1.1.tar.gz` & `tmp/jdEolConverter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdEolConverter-1.1.tar", last modified: Thu Jul 28 13:57:36 2022, max compression
+gzip compressed data, was "jdEolConverter-1.2.tar", last modified: Wed Apr 19 13:51:03 2023, max compression
```

## Comparing `jdEolConverter-1.1.tar` & `jdEolConverter-1.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 13:57:36.601846 jdEolConverter-1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35071 2022-07-28 13:57:16.000000 jdEolConverter-1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-07-28 13:57:16.000000 jdEolConverter-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1608 2022-07-28 13:57:36.601846 jdEolConverter-1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-07-28 13:57:16.000000 jdEolConverter-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 13:57:36.599846 jdEolConverter-1.1/jdEolConverter/
--rw-rw-rw-   0 root         (0) root         (0)     1278 2022-07-28 13:57:16.000000 jdEolConverter-1.1/jdEolConverter/Icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     4287 2022-07-28 13:57:16.000000 jdEolConverter-1.1/jdEolConverter/MainWindow.ui
--rw-rw-rw-   0 root         (0) root         (0)     6203 2022-07-28 13:57:16.000000 jdEolConverter-1.1/jdEolConverter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-28 13:57:16.000000 jdEolConverter-1.1/jdEolConverter/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 13:57:36.601846 jdEolConverter-1.1/jdEolConverter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1608 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      375 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-07-28 13:57:36.000000 jdEolConverter-1.1/jdEolConverter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-28 13:57:36.601846 jdEolConverter-1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3052 2022-07-28 13:57:16.000000 jdEolConverter-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:51:03.399907 jdEolConverter-1.2/
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-04-19 13:50:20.000000 jdEolConverter-1.2/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35082 2023-04-19 13:50:20.000000 jdEolConverter-1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      125 2023-04-19 13:50:20.000000 jdEolConverter-1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-19 13:51:03.399907 jdEolConverter-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3424 2023-04-19 13:50:20.000000 jdEolConverter-1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:51:03.399907 jdEolConverter-1.2/jdEolConverter/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     6207 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:51:03.399907 jdEolConverter-1.2/jdEolConverter/translations/
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/translations/jdEolConverter_de.ts
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-04-19 13:50:20.000000 jdEolConverter-1.2/jdEolConverter/translations/jdEolConverter_nl.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:51:03.399907 jdEolConverter-1.2/jdEolConverter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-19 13:51:03.000000 jdEolConverter-1.2/jdEolConverter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-04-19 13:50:20.000000 jdEolConverter-1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 13:51:03.399907 jdEolConverter-1.2/setup.cfg
```

### Comparing `jdEolConverter-1.1/LICENSE` & `jdEolConverter-1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -627,16 +627,16 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    jdAppdataEdit
-    Copyright (C) 2022  JakobDev
+    jdEolConverter
+    Copyright (C) 2022-2023  JakobDev
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) 2022  JakobDev
+    <program>  Copyright (C) 2022-2023  JakobDev
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `jdEolConverter-1.1/jdEolConverter/Icon.svg` & `jdEolConverter-1.2/jdEolConverter/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdEolConverter-1.1/jdEolConverter/MainWindow.ui` & `jdEolConverter-1.2/jdEolConverter/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdEolConverter-1.1/jdEolConverter/__init__.py` & `jdEolConverter-1.2/jdEolConverter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         self._convert_thread.start()
 
 
 def main():
     app = QApplication(sys.argv)
 
     app.setWindowIcon(QIcon(os.path.join(os.path.dirname(__file__), "Icon.svg")))
-    app.setDesktopFileName("com.gitlab.JakobDev.jdEolConverter")
+    app.setDesktopFileName("page.codeberg..JakobDev.jdEolConverter")
     app.setApplicationName("jdEolConverter")
 
     translator = QTranslator()
     system_language = QLocale.system().name()
     translator.load(os.path.join(os.path.dirname(__file__), "translations", "jdEolConverter_" + system_language.split("_")[0] + ".qm"))
     translator.load(os.path.join(os.path.dirname(__file__), "translations", "jdEolConverter_" + system_language + ".qm"))
     app.installTranslator(translator)
```

