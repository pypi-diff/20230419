# Comparing `tmp/ebib-1.1.2.tar.gz` & `tmp/ebib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebib-1.1.2.tar", last modified: Wed Apr 19 17:37:13 2023, max compression
+gzip compressed data, was "ebib-1.1.3.tar", last modified: Wed Apr 19 17:41:33 2023, max compression
```

## Comparing `ebib-1.1.2.tar` & `ebib-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:37:13.371935 ebib-1.1.2/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.2/LICENSE
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:37:13.371935 ebib-1.1.2/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.2/README.md
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:37:13.371935 ebib-1.1.2/ebib/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.2/ebib/__init__.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:37:13.371935 ebib-1.1.2/ebib/assets/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.2/ebib/assets/english-stemmer.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 16:37:29.000000 ebib-1.1.2/ebib/assets/index.html
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.2/ebib/assets/index.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6062 2023-04-19 17:35:32.000000 ebib-1.1.2/ebib/cli.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.2/ebib/english_stemmer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.2/ebib/indexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.2/ebib/lexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-19 17:10:28.000000 ebib-1.1.2/ebib/utils.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:37:13.371935 ebib-1.1.2/ebib.egg-info/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      374 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/SOURCES.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/dependency_links.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/entry_points.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/requires.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 17:37:13.000000 ebib-1.1.2/ebib.egg-info/top_level.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      609 2023-04-19 17:24:54.000000 ebib-1.1.2/pyproject.toml
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:37:13.371935 ebib-1.1.2/setup.cfg
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:41:33.584027 ebib-1.1.3/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.3/LICENSE
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:41:33.584027 ebib-1.1.3/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.3/README.md
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:41:33.584027 ebib-1.1.3/ebib/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.3/ebib/__init__.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:41:33.584027 ebib-1.1.3/ebib/assets/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      179 2023-04-19 17:30:42.000000 ebib-1.1.3/ebib/assets/.gitlab-ci.yml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.3/ebib/assets/english-stemmer.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 16:37:29.000000 ebib-1.1.3/ebib/assets/index.html
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.3/ebib/assets/index.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6062 2023-04-19 17:35:32.000000 ebib-1.1.3/ebib/cli.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.3/ebib/english_stemmer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.3/ebib/indexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.3/ebib/lexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-19 17:10:28.000000 ebib-1.1.3/ebib/utils.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:41:33.584027 ebib-1.1.3/ebib.egg-info/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      401 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/SOURCES.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/dependency_links.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/entry_points.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/requires.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 17:41:33.000000 ebib-1.1.3/ebib.egg-info/top_level.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      634 2023-04-19 17:40:55.000000 ebib-1.1.3/pyproject.toml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:41:33.584027 ebib-1.1.3/setup.cfg
```

### Comparing `ebib-1.1.2/LICENSE` & `ebib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/PKG-INFO` & `ebib-1.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.2
+Version: 1.1.3
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-1.1.2/ebib/__init__.py` & `ebib-1.1.3/ebib/__init__.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/assets/english-stemmer.js` & `ebib-1.1.3/ebib/assets/english-stemmer.js`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/assets/index.html` & `ebib-1.1.3/ebib/assets/index.html`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/assets/index.js` & `ebib-1.1.3/ebib/assets/index.js`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/cli.py` & `ebib-1.1.3/ebib/cli.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/english_stemmer.py` & `ebib-1.1.3/ebib/english_stemmer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/indexer.py` & `ebib-1.1.3/ebib/indexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/lexer.py` & `ebib-1.1.3/ebib/lexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib/utils.py` & `ebib-1.1.3/ebib/utils.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.2/ebib.egg-info/PKG-INFO` & `ebib-1.1.3/ebib.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.2
+Version: 1.1.3
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

