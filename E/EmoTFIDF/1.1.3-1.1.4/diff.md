# Comparing `tmp/EmoTFIDF-1.1.3.tar.gz` & `tmp/EmoTFIDF-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmoTFIDF-1.1.3.tar", last modified: Tue Apr 18 17:10:45 2023, max compression
+gzip compressed data, was "EmoTFIDF-1.1.4.tar", last modified: Wed Apr 19 10:40:23 2023, max compression
```

## Comparing `EmoTFIDF-1.1.3.tar` & `EmoTFIDF-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 17:10:45.610976 EmoTFIDF-1.1.3/
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 17:10:45.610564 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/requires.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/top_level.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.3/LICENSE
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 17:10:45.610794 EmoTFIDF-1.1.3/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.3/README.md
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4804 2023-04-18 12:02:05.000000 EmoTFIDF-1.1.3/emotfidf.py
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 17:10:45.611027 EmoTFIDF-1.1.3/setup.cfg
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 17:10:18.000000 EmoTFIDF-1.1.3/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-19 10:40:23.057296 EmoTFIDF-1.1.4/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-19 10:40:23.056827 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.4/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-19 10:40:23.057073 EmoTFIDF-1.1.4/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.4/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4840 2023-04-19 10:39:31.000000 EmoTFIDF-1.1.4/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-19 10:40:23.057357 EmoTFIDF-1.1.4/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-19 10:40:07.000000 EmoTFIDF-1.1.4/setup.py
```

### Comparing `EmoTFIDF-1.1.3/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.1.4/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.3/LICENSE` & `EmoTFIDF-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.3/PKG-INFO` & `EmoTFIDF-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.3/README.md` & `EmoTFIDF-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.3/emotfidf.py` & `EmoTFIDF-1.1.4/emotfidf.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     # get emotions
     em_list = []
     em_dict = dict()
     em_frequencies = Counter()
     lexicon_keys = self.lexicon.keys()
     for word in self.words:
         if word in lexicon_keys:
-            emotions_found = list(set([s for s in self.lexicon[word] if s.strip()]))
+            emotions_found = list(set(self.lexicon[word]))
+            emotions_found = list(filter(None, emotions_found))
             if emotions_found is not None:
                 if 'negative' in emotions_found:
                     emotions_found.remove('negative')
                 elif 'positive' in emotions_found:
                     emotions_found.remove('positive')
                 em_list.extend(emotions_found)
                 em_dict.update({word: self.lexicon[word]})
@@ -101,14 +102,14 @@
         em_frequencies = Counter()
         for word in self.em_list:
             em_frequencies[word] += 1
         for e in self.em_dict.keys():
             if e in self.ifidf_for_words:
                 tfidf_weight = self.ifidf_for_words[e]
                 for a in self.em_dict[e]:
-                    new_fre = round(em_frequencies[a] / tfidf_weight*2 , 2)
+                    new_fre = round(em_frequencies[a] / tfidf_weight, 2)
                     em_frequencies[a] = new_fre
         sum_values = sum(em_frequencies.values())
         for key in em_frequencies.keys():
             em_percent.update({key: round(float(em_frequencies[key]) / float(sum_values), 3)})
         self.em_tfidf = em_percent
         self.em_tfidf = em_percent
```

### Comparing `EmoTFIDF-1.1.3/setup.py` & `EmoTFIDF-1.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.1.3",
+    version="1.1.4",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

