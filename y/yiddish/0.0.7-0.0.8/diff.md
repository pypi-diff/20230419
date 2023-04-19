# Comparing `tmp/yiddish-0.0.7.tar.gz` & `tmp/yiddish-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yiddish-0.0.7.tar", last modified: Sat Feb 18 18:03:28 2023, max compression
+gzip compressed data, was "yiddish-0.0.8.tar", last modified: Wed Apr 19 16:48:02 2023, max compression
```

## Comparing `yiddish-0.0.7.tar` & `yiddish-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 18:03:28.114206 yiddish-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-18 18:03:19.000000 yiddish-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-18 18:03:28.114206 yiddish-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-18 18:03:19.000000 yiddish-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-18 18:03:19.000000 yiddish-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 18:03:28.114206 yiddish-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-18 18:03:19.000000 yiddish-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 18:03:28.114206 yiddish-0.0.7/yiddish/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-18 18:03:19.000000 yiddish-0.0.7/yiddish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-02-18 18:03:19.000000 yiddish-0.0.7/yiddish/yiddish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 18:03:28.114206 yiddish-0.0.7/yiddish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-18 18:03:28.000000 yiddish-0.0.7/yiddish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-18 18:03:28.000000 yiddish-0.0.7/yiddish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 18:03:28.000000 yiddish-0.0.7/yiddish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-18 18:03:28.000000 yiddish-0.0.7/yiddish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.570180 yiddish-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-19 16:47:53.000000 yiddish-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-19 16:48:02.566180 yiddish-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-19 16:47:53.000000 yiddish-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 16:47:53.000000 yiddish-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:48:02.570180 yiddish-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 16:47:53.000000 yiddish-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.566180 yiddish-0.0.8/yiddish/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 16:47:53.000000 yiddish-0.0.8/yiddish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-04-19 16:47:53.000000 yiddish-0.0.8/yiddish/yiddish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.566180 yiddish-0.0.8/yiddish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/top_level.txt
```

### Comparing `yiddish-0.0.7/LICENSE` & `yiddish-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yiddish-0.0.7/PKG-INFO` & `yiddish-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yiddish
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for processing Yiddish text
 Home-page: https://github.com/ibleaman/yiddish
 Author: Isaac L. Bleaman
 Author-email: bleaman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yiddish-0.0.7/README.md` & `yiddish-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `yiddish-0.0.7/yiddish/yiddish.py` & `yiddish-0.0.8/yiddish/yiddish.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 ]
 
 # if loshn_koydesh, look up string in LK dictionary
 def transliterate(string, loshn_koydesh=False):
     romanized = replace_with_precombined(string)
     
     if loshn_koydesh:
-        tokens = re.findall(r"[אאַאָבבֿגדהוװוּױזחטייִײײַככּךלמםנןסעפּפֿףצץקרששׂתּת\-־]+|[^אאַאָבבֿגדהוװוּױזחטייִײײַככּךלמםנןסעפּפֿףצץקרששׂתּת\-־]", romanized)
+        tokens = re.findall(r"[אאַאָבבֿגדהוװוּױזחטייִײײַככּךלמםנןסעפּפֿףצץקרששׂתּת\-־']+|[^אאַאָבבֿגדהוװוּױזחטייִײײַככּךלמםנןסעפּפֿףצץקרששׂתּת\-־']", romanized)
         new_tokens = []
         for token in tokens:
             if token in lk and token not in germanic_semitic_homographs:
                 if lk[token][0] in less_common_lk_pronunciations and len(lk[token]) > 1:
                     new_tokens.append(lk[token][1].replace('־', '-'))
                 else:
                     new_tokens.append(lk[token][0].replace('־', '-'))
@@ -335,14 +335,15 @@
     (r'\barbets', 'אַרבעטס'),
     (r'\barbayts', 'אַרבײַטס'),
     (r'\bdemolts', 'דעמאָלטס'),
     (r'\bgots', 'גאָטס'),
     (r'\bguts', 'גוטס'),
     (r'\bgeshefts', 'געשעפֿטס'),
     (r'(\b|ba|far|der)haltst', r'\1האַלטסט'),
+    (r'\bshlekhts\b', 'שלעכטס'),
     (r'(\b|tse)shpaltst', r'\1שפּאַלטסט'),
     (r'(\b|tse|far)shpreytst', r'\1שפּרײטסט'),
     (r'shpetst', 'שפּעטסט'),
     (r'\brekhts\b', 'רעכטס'),
     (r'du shatst', 'דו שאַטסט'), # cf. ער שאַצט
     (r'\bforverts\b', 'פֿאָרװערטס'),
```

### Comparing `yiddish-0.0.7/yiddish.egg-info/PKG-INFO` & `yiddish-0.0.8/yiddish.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yiddish
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for processing Yiddish text
 Home-page: https://github.com/ibleaman/yiddish
 Author: Isaac L. Bleaman
 Author-email: bleaman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

