# Comparing `tmp/fps_lab-0.1.3.tar.gz` & `tmp/fps_lab-0.1.4.tar.gz`

## Comparing `fps_lab-0.1.3.tar` & `fps_lab-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.1.3/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fps_lab-0.1.3/fps_lab/main.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 fps_lab-0.1.3/fps_lab/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_lab-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.1.3/COPYING.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.1.3/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fps_lab-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fps_lab-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.1.4/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fps_lab-0.1.4/fps_lab/main.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 fps_lab-0.1.4/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_lab-0.1.4/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_lab-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.1.4/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fps_lab-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fps_lab-0.1.4/PKG-INFO
```

### Comparing `fps_lab-0.1.3/fps_lab/main.py` & `fps_lab-0.1.4/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.3/.gitignore` & `fps_lab-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.3/COPYING.md` & `fps_lab-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.3/pyproject.toml` & `fps_lab-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.3/PKG-INFO` & `fps_lab-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_lab
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the JupyterLab/RetroLab API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

