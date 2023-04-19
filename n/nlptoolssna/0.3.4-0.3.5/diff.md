# Comparing `tmp/nlptoolssna-0.3.4.tar.gz` & `tmp/nlptoolssna-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.3.4.tar", last modified: Tue Apr 18 22:21:03 2023, max compression
+gzip compressed data, was "nlptoolssna-0.3.5.tar", last modified: Wed Apr 19 21:40:33 2023, max compression
```

## Comparing `nlptoolssna-0.3.4.tar` & `nlptoolssna-0.3.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.611446 nlptoolssna-0.3.4/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-18 22:21:03.611446 nlptoolssna-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.545837 nlptoolssna-0.3.4/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.554413 nlptoolssna-0.3.4/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.562734 nlptoolssna-0.3.4/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.4/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-04-18 22:20:52.000000 nlptoolssna-0.3.4/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.562734 nlptoolssna-0.3.4/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.4/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.570736 nlptoolssna-0.3.4/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.4/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.4/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.578734 nlptoolssna-0.3.4/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.4/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.3.4/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.3.4/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7504 2023-04-18 21:40:58.000000 nlptoolssna-0.3.4/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.4/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.4/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.586798 nlptoolssna-0.3.4/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.4/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.4/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.594809 nlptoolssna-0.3.4/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.4/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.4/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.4/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.603419 nlptoolssna-0.3.4/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 22:21:03.000000 nlptoolssna-0.3.4/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-18 22:21:03.611446 nlptoolssna-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:21:03.611446 nlptoolssna-0.3.4/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.4/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.902891 nlptoolssna-0.3.5/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.911047 nlptoolssna-0.3.5/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.911047 nlptoolssna-0.3.5/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.5/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-04-18 22:20:52.000000 nlptoolssna-0.3.5/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.920300 nlptoolssna-0.3.5/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.5/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.920300 nlptoolssna-0.3.5/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.5/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.5/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.941124 nlptoolssna-0.3.5/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.5/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.3.5/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.3.5/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     7505 2023-04-19 21:39:18.000000 nlptoolssna-0.3.5/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.5/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.5/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.941124 nlptoolssna-0.3.5/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.5/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.5/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.951335 nlptoolssna-0.3.5/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.5/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.5/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.5/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.974601 nlptoolssna-0.3.5/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.3.4/CONTRIBUTING.rst` & `nlptoolssna-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/LICENSE` & `nlptoolssna-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/PKG-INFO` & `nlptoolssna-0.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.4/README.rst` & `nlptoolssna-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/docs/Makefile` & `nlptoolssna-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/docs/conf.py` & `nlptoolssna-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/docs/installation.rst` & `nlptoolssna-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/docs/make.bat` & `nlptoolssna-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.3.5/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/data/my_data.pickle` & `nlptoolssna-0.3.5/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.3.5/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/morph/charsets.py` & `nlptoolssna-0.3.5/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.3.5/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.3.5/nlptools/morph/morph_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     path =downloader.get_appdatadir()
     file_path = os.path.join(path, filename)
     
 
     with open(file_path, 'rb') as f:
        #Load the serialized data from the file
        ALMA_dic = pickle.load(f)
-       print(ALMA_dic)
+       #print(ALMA_dic)
        return ALMA_dic
 
 def tag(word, lang, task):
     """
     given a token, this method retrives the possible morphological solutions (lemma, pos, and frequency) filterd by spesific
     language and task.
```

### Comparing `nlptoolssna-0.3.4/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.3.5/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/parse/parser.py` & `nlptoolssna-0.3.5/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/salma/implication.py` & `nlptoolssna-0.3.5/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.3.5/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.3.5/nlptoolssna.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.4/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.3.5/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/setup.cfg` & `nlptoolssna-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.4/setup.py` & `nlptoolssna-0.3.5/setup.py`

 * *Files identical despite different names*

