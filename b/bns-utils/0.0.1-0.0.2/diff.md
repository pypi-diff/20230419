# Comparing `tmp/bns_utils-0.0.1.tar.gz` & `tmp/bns_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bns_utils-0.0.1.tar", last modified: Tue Feb 21 07:13:35 2023, max compression
+gzip compressed data, was "bns_utils-0.0.2.tar", last modified: Wed Apr 19 13:30:36 2023, max compression
```

## Comparing `bns_utils-0.0.1.tar` & `bns_utils-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 07:13:35.608694 bns_utils-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-02-21 06:46:37.000000 bns_utils-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      514 2023-02-21 07:13:35.607689 bns_utils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-02-21 07:12:54.000000 bns_utils-0.0.1/README.md
--rw-rw-rw-   0        0        0      727 2023-02-21 07:11:43.000000 bns_utils-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-21 07:13:35.608694 bns_utils-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-21 07:13:35.583680 bns_utils-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-21 07:13:35.602692 bns_utils-0.0.1/src/BNS_UTILS.egg-info/
--rw-rw-rw-   0        0        0      514 2023-02-21 07:13:35.000000 bns_utils-0.0.1/src/BNS_UTILS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-02-21 07:13:35.000000 bns_utils-0.0.1/src/BNS_UTILS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 07:13:35.000000 bns_utils-0.0.1/src/BNS_UTILS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-02-21 07:13:35.000000 bns_utils-0.0.1/src/BNS_UTILS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-21 07:13:35.000000 bns_utils-0.0.1/src/BNS_UTILS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-21 07:13:35.604690 bns_utils-0.0.1/src/bns_utils/
--rw-rw-rw-   0        0        0     6539 2023-02-21 07:12:53.000000 bns_utils-0.0.1/src/bns_utils/BNS_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-21 06:31:53.000000 bns_utils-0.0.1/src/bns_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:30:36.005570 bns_utils-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 06:46:37.000000 bns_utils-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3246 2023-04-19 13:30:36.004570 bns_utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2773 2023-02-21 13:01:48.000000 bns_utils-0.0.2/README.md
+-rw-rw-rw-   0        0        0      784 2023-04-19 11:23:57.000000 bns_utils-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:30:36.005570 bns_utils-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 13:30:35.940053 bns_utils-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 13:30:35.982568 bns_utils-0.0.2/src/BNS_UTILS.egg-info/
+-rw-rw-rw-   0        0        0     3246 2023-04-19 13:30:35.000000 bns_utils-0.0.2/src/BNS_UTILS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-04-19 13:30:35.000000 bns_utils-0.0.2/src/BNS_UTILS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:30:35.000000 bns_utils-0.0.2/src/BNS_UTILS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-19 13:30:35.000000 bns_utils-0.0.2/src/BNS_UTILS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 13:30:35.000000 bns_utils-0.0.2/src/BNS_UTILS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 13:30:35.999568 bns_utils-0.0.2/src/bns_utils/
+-rw-rw-rw-   0        0        0        0 2023-02-21 06:31:53.000000 bns_utils-0.0.2/src/bns_utils/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-02-21 12:09:02.000000 bns_utils-0.0.2/src/bns_utils/data.py
+-rw-rw-rw-   0        0        0    13703 2023-03-08 10:08:43.000000 bns_utils-0.0.2/src/bns_utils/fluidreports.py
+-rw-rw-rw-   0        0        0     6519 2023-02-21 10:34:32.000000 bns_utils-0.0.2/src/bns_utils/general.py
+-rw-rw-rw-   0        0        0     1904 2023-04-19 11:23:18.000000 bns_utils-0.0.2/src/bns_utils/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:30:36.002570 bns_utils-0.0.2/tests/
+-rw-rw-rw-   0        0        0      385 2023-03-08 10:32:12.000000 bns_utils-0.0.2/tests/test_fluidreports.py
```

### Comparing `bns_utils-0.0.1/LICENSE` & `bns_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.1/pyproject.toml` & `bns_utils-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bns_utils"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Some utilities for BNS internal use"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,13 @@
     'matplotlib >= 3.5.0, < 5',
     'tqdm >= 4.64.0, < 5',
     'pandas >= 1.5.0, < 2',
     'scipy >= 1.9.0, < 2'
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Dave-the-python-developer/BNS_utils"
+"Homepage" = "https://github.com/Dave-the-python-developer/BNS_utils"
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `bns_utils-0.0.1/src/bns_utils/BNS_utils.py` & `bns_utils-0.0.2/src/bns_utils/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,12 +170,7 @@
         #print(start_date,end_date,type(widget[0]))
         data[widget[0]][start_date:end_date].plot()
         plt.legend(widget)
         plt.show()
 
     #now I will create the interactive plot
     interact(plot_data, widget = widget, start_date = start_date, end_date = end_date)
-
-
-    
-
-
```

