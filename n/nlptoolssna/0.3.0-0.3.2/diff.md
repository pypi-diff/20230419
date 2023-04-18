# Comparing `tmp/nlptoolssna-0.3.0.tar.gz` & `tmp/nlptoolssna-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.3.0.tar", last modified: Tue Apr 18 22:04:55 2023, max compression
+gzip compressed data, was "nlptoolssna-0.3.2.tar", last modified: Tue Apr 18 22:08:02 2023, max compression
```

## Comparing `nlptoolssna-0.3.0.tar` & `nlptoolssna-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.181846 nlptoolssna-0.3.0/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-18 22:04:55.181846 nlptoolssna-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.123552 nlptoolssna-0.3.0/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.132252 nlptoolssna-0.3.0/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.140325 nlptoolssna-0.3.0/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.0/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-04-18 22:04:24.000000 nlptoolssna-0.3.0/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.140325 nlptoolssna-0.3.0/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.0/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.140325 nlptoolssna-0.3.0/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.0/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.0/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.156800 nlptoolssna-0.3.0/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.0/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.3.0/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.3.0/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7504 2023-04-18 21:40:58.000000 nlptoolssna-0.3.0/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.0/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.0/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.156800 nlptoolssna-0.3.0/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.0/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.0/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.164902 nlptoolssna-0.3.0/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.0/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.0/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.0/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.181846 nlptoolssna-0.3.0/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 22:04:55.000000 nlptoolssna-0.3.0/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-18 22:04:55.188985 nlptoolssna-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:55.181846 nlptoolssna-0.3.0/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.0/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.479880 nlptoolssna-0.3.2/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-18 22:08:02.480631 nlptoolssna-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.421761 nlptoolssna-0.3.2/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.421761 nlptoolssna-0.3.2/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.429921 nlptoolssna-0.3.2/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.2/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-04-18 22:05:46.000000 nlptoolssna-0.3.2/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.429921 nlptoolssna-0.3.2/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.2/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.429921 nlptoolssna-0.3.2/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.2/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.2/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.446195 nlptoolssna-0.3.2/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.2/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.3.2/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.3.2/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     7504 2023-04-18 21:40:58.000000 nlptoolssna-0.3.2/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.2/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.2/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.446195 nlptoolssna-0.3.2/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.2/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.2/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.455391 nlptoolssna-0.3.2/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.2/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.2/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.2/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.471597 nlptoolssna-0.3.2/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 22:08:02.000000 nlptoolssna-0.3.2/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-18 22:08:02.480631 nlptoolssna-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:08:02.471597 nlptoolssna-0.3.2/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.2/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.3.0/CONTRIBUTING.rst` & `nlptoolssna-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/LICENSE` & `nlptoolssna-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/PKG-INFO` & `nlptoolssna-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.0
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.0/README.rst` & `nlptoolssna-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/docs/Makefile` & `nlptoolssna-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/docs/conf.py` & `nlptoolssna-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/docs/installation.rst` & `nlptoolssna-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/docs/make.bat` & `nlptoolssna-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.3.2/nlptools/DataDownload/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,12 +61,11 @@
 
 
 def download_files(urls):
     for url in urls.values():
         download_file(url)
 
 
-download_files(urls)
 
 
 
 #download_file(downloadLink ,_get_appdatadir())
```

### Comparing `nlptoolssna-0.3.0/nlptools/data/my_data.pickle` & `nlptoolssna-0.3.2/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.3.2/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/morph/charsets.py` & `nlptoolssna-0.3.2/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.3.2/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.3.2/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.3.2/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/parse/parser.py` & `nlptoolssna-0.3.2/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/salma/implication.py` & `nlptoolssna-0.3.2/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.3.2/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.3.2/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.0
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.0/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.3.2/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/setup.cfg` & `nlptoolssna-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.0/setup.py` & `nlptoolssna-0.3.2/setup.py`

 * *Files identical despite different names*

