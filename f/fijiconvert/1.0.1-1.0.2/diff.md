# Comparing `tmp/fijiconvert-1.0.1.tar.gz` & `tmp/fijiconvert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fijiconvert-1.0.1.tar", last modified: Wed Apr 19 15:31:44 2023, max compression
+gzip compressed data, was "fijiconvert-1.0.2.tar", last modified: Wed Apr 19 15:39:48 2023, max compression
```

## Comparing `fijiconvert-1.0.1.tar` & `fijiconvert-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/
--rw-rw-rw-   0        0        0      399 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-04-17 20:14:58.000000 fijiconvert-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.368366 fijiconvert-1.0.1/fijiconvert/
--rw-rw-rw-   0        0        0       23 2023-04-17 20:16:44.000000 fijiconvert-1.0.1/fijiconvert/__init__.py
--rw-rw-rw-   0        0        0      285 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/buildsetup.py
--rw-rw-rw-   0        0        0     9498 2023-04-17 20:30:04.000000 fijiconvert-1.0.1/fijiconvert/converter.py
--rw-rw-rw-   0        0        0      294 2023-04-17 20:29:38.000000 fijiconvert-1.0.1/fijiconvert/main.py
--rw-rw-rw-   0        0        0     1899 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/reader.py
--rw-rw-rw-   0        0        0     1412 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/setupcheckerr.py
--rw-rw-rw-   0        0        0     3261 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/tacchkdlg.py
--rw-rw-rw-   0        0        0    24180 2023-04-17 20:29:49.000000 fijiconvert-1.0.1/fijiconvert/ui_fijiconvertdialog.py
--rw-rw-rw-   0        0        0     5281 2023-03-28 15:28:28.000000 fijiconvert-1.0.1/fijiconvert/writer.py
--rw-rw-rw-   0        0        0    15104 2023-04-17 20:30:23.000000 fijiconvert-1.0.1/fijiconvert/xml_gui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/fijiconvert.egg-info/
--rw-rw-rw-   0        0        0      399 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 15:31:44.000000 fijiconvert-1.0.1/fijiconvert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2022-12-22 18:55:48.000000 fijiconvert-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      574 2023-04-19 15:31:44.390502 fijiconvert-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-12-22 18:55:48.000000 fijiconvert-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:39:48.743650 fijiconvert-1.0.2/
+-rw-rw-rw-   0        0        0      423 2023-04-19 15:39:48.743650 fijiconvert-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-04-19 15:36:32.000000 fijiconvert-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:39:48.721513 fijiconvert-1.0.2/fijiconvert/
+-rw-rw-rw-   0        0        0       23 2023-04-17 20:16:44.000000 fijiconvert-1.0.2/fijiconvert/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-03-28 15:28:28.000000 fijiconvert-1.0.2/fijiconvert/buildsetup.py
+-rw-rw-rw-   0        0        0     9498 2023-04-17 20:30:04.000000 fijiconvert-1.0.2/fijiconvert/converter.py
+-rw-rw-rw-   0        0        0      294 2023-04-17 20:29:38.000000 fijiconvert-1.0.2/fijiconvert/main.py
+-rw-rw-rw-   0        0        0     1899 2023-03-28 15:28:28.000000 fijiconvert-1.0.2/fijiconvert/reader.py
+-rw-rw-rw-   0        0        0     1412 2023-03-28 15:28:28.000000 fijiconvert-1.0.2/fijiconvert/setupcheckerr.py
+-rw-rw-rw-   0        0        0     3261 2023-03-28 15:28:28.000000 fijiconvert-1.0.2/fijiconvert/tacchkdlg.py
+-rw-rw-rw-   0        0        0    24180 2023-04-17 20:29:49.000000 fijiconvert-1.0.2/fijiconvert/ui_fijiconvertdialog.py
+-rw-rw-rw-   0        0        0     5281 2023-03-28 15:28:28.000000 fijiconvert-1.0.2/fijiconvert/writer.py
+-rw-rw-rw-   0        0        0    15104 2023-04-17 20:30:23.000000 fijiconvert-1.0.2/fijiconvert/xml_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:39:48.728020 fijiconvert-1.0.2/fijiconvert.egg-info/
+-rw-rw-rw-   0        0        0      423 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 15:39:48.000000 fijiconvert-1.0.2/fijiconvert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2022-12-22 18:55:48.000000 fijiconvert-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      586 2023-04-19 15:39:48.743650 fijiconvert-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-12-22 18:55:48.000000 fijiconvert-1.0.2/setup.py
```

### Comparing `fijiconvert-1.0.1/fijiconvert/converter.py` & `fijiconvert-1.0.2/fijiconvert/converter.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/reader.py` & `fijiconvert-1.0.2/fijiconvert/reader.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/setupcheckerr.py` & `fijiconvert-1.0.2/fijiconvert/setupcheckerr.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/tacchkdlg.py` & `fijiconvert-1.0.2/fijiconvert/tacchkdlg.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/ui_fijiconvertdialog.py` & `fijiconvert-1.0.2/fijiconvert/ui_fijiconvertdialog.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/writer.py` & `fijiconvert-1.0.2/fijiconvert/writer.py`

 * *Files identical despite different names*

### Comparing `fijiconvert-1.0.1/fijiconvert/xml_gui.py` & `fijiconvert-1.0.2/fijiconvert/xml_gui.py`

 * *Files identical despite different names*

