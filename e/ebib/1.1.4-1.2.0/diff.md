# Comparing `tmp/ebib-1.1.4.tar.gz` & `tmp/ebib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebib-1.1.4.tar", last modified: Wed Apr 19 18:09:16 2023, max compression
+gzip compressed data, was "ebib-1.2.0.tar", last modified: Wed Apr 19 18:29:45 2023, max compression
```

## Comparing `ebib-1.1.4.tar` & `ebib-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:09:16.467371 ebib-1.1.4/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.4/LICENSE
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 18:09:16.467371 ebib-1.1.4/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.4/README.md
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:09:16.464038 ebib-1.1.4/ebib/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.4/ebib/__init__.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:09:16.467371 ebib-1.1.4/ebib/assets/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      179 2023-04-19 17:30:42.000000 ebib-1.1.4/ebib/assets/.gitlab-ci.yml
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.4/ebib/assets/english-stemmer.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 18:06:54.000000 ebib-1.1.4/ebib/assets/index.html
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.4/ebib/assets/index.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6070 2023-04-19 17:57:55.000000 ebib-1.1.4/ebib/cli.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.4/ebib/english_stemmer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.4/ebib/indexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.4/ebib/lexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-19 17:10:28.000000 ebib-1.1.4/ebib/utils.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:09:16.467371 ebib-1.1.4/ebib.egg-info/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      401 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/SOURCES.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/dependency_links.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/entry_points.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/requires.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 18:09:16.000000 ebib-1.1.4/ebib.egg-info/top_level.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      634 2023-04-19 18:08:52.000000 ebib-1.1.4/pyproject.toml
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 18:09:16.467371 ebib-1.1.4/setup.cfg
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:29:45.376025 ebib-1.2.0/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.2.0/LICENSE
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 18:29:45.376025 ebib-1.2.0/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.2.0/README.md
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:29:45.372691 ebib-1.2.0/ebib/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.2.0/ebib/__init__.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:29:45.376025 ebib-1.2.0/ebib/assets/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      179 2023-04-19 17:30:42.000000 ebib-1.2.0/ebib/assets/.gitlab-ci.yml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.2.0/ebib/assets/english-stemmer.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 18:06:54.000000 ebib-1.2.0/ebib/assets/index.html
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6061 2023-04-19 18:21:50.000000 ebib-1.2.0/ebib/assets/index.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6070 2023-04-19 17:57:55.000000 ebib-1.2.0/ebib/cli.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.2.0/ebib/english_stemmer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.2.0/ebib/indexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.2.0/ebib/lexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-19 17:10:28.000000 ebib-1.2.0/ebib/utils.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 18:29:45.372691 ebib-1.2.0/ebib.egg-info/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      401 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/SOURCES.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/dependency_links.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/entry_points.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/requires.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 18:29:45.000000 ebib-1.2.0/ebib.egg-info/top_level.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      634 2023-04-19 18:28:53.000000 ebib-1.2.0/pyproject.toml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 18:29:45.376025 ebib-1.2.0/setup.cfg
```

### Comparing `ebib-1.1.4/LICENSE` & `ebib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/PKG-INFO` & `ebib-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.4
+Version: 1.2.0
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-1.1.4/ebib/__init__.py` & `ebib-1.2.0/ebib/__init__.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/assets/english-stemmer.js` & `ebib-1.2.0/ebib/assets/english-stemmer.js`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/assets/index.html` & `ebib-1.2.0/ebib/assets/index.html`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/assets/index.js` & `ebib-1.2.0/ebib/assets/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 const PAGE_SIZE = 20;
 const THRESHOLD = 0.1;
 
 let tags = [];
 let active_tags = [];
 let authors = [];
 let active_authors = [];
-let scores = [];
+let scores = Object.keys(data['pdfs']).map((a) => [a, THRESHOLD + 1]);
 let selected_articles = [];
 let page = 0;
 
 const main_panel = document.getElementById('main-panel');
 const authors_div = document.getElementById('authors');
 const tags_div = document.getElementById('tags');
 const query_input = document.getElementById('query');
@@ -118,14 +118,15 @@
         for (const term of query) {
             const k1 = 1.2;
             const b = 0.75;
             const f = term in data['pdfs'][pdf]['index'] ? data['pdfs'][pdf]['index'][term] : 0;
             const idf = term in data['idf'] ? data['idf'][term] : 0;
             s += idf * f * (k1 + 1) / (f + k1 * (1 - b + b * data['pdfs'][pdf]['length'] / data['avgdl']));
         }
+        if (query.length == 0) s = THRESHOLD + 1;
         scores.push([pdf, s]);
     }
     scores.sort((a, b) => a[1] < b[1]);
     scores = scores.filter(x => x[1] > THRESHOLD);
 
     page = 0;
     authors = [];
```

### Comparing `ebib-1.1.4/ebib/cli.py` & `ebib-1.2.0/ebib/cli.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/english_stemmer.py` & `ebib-1.2.0/ebib/english_stemmer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/indexer.py` & `ebib-1.2.0/ebib/indexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/lexer.py` & `ebib-1.2.0/ebib/lexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib/utils.py` & `ebib-1.2.0/ebib/utils.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.4/ebib.egg-info/PKG-INFO` & `ebib-1.2.0/ebib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.4
+Version: 1.2.0
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-1.1.4/pyproject.toml` & `ebib-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ebib"
-version = "1.1.4"
+version = "1.2.0"
 authors = [
 	{ name = "Ernesto Lanchares", email = "elancha98@gmail.com" },
 ]
 description = "ebib is a bibliography manager system aimed to work with Gitlab/Github pages"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["Click", "requests", "pymupdf"]
```

