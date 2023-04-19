# Comparing `tmp/cmip-0.0.5.tar.gz` & `tmp/cmip-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip-0.0.5.tar", last modified: Mon Apr 17 02:48:33 2023, max compression
+gzip compressed data, was "cmip-0.0.6.tar", last modified: Wed Apr 19 10:30:50 2023, max compression
```

## Comparing `cmip-0.0.5.tar` & `cmip-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.547712 cmip-0.0.5/
--rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1128 2023-04-17 02:48:33.545710 cmip-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-04-17 02:44:31.000000 cmip-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.509003 cmip-0.0.5/cmip/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.519984 cmip-0.0.5/cmip/data/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/ad.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/chinese_frequency.tsv
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/letter_mapping.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/pinyin.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.521971 cmip-0.0.5/cmip/gibberish/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/gibberish/__init__.py
--rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/gibberish/gibberish.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.523972 cmip-0.0.5/cmip/image/
--rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.529977 cmip-0.0.5/cmip/text/
--rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.5/cmip/text/__init__.py
--rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.5/cmip/text/ac_automation.py
--rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/text/normalize.py
--rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/text/similarity.py
--rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.5/cmip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.537704 cmip-0.0.5/cmip/web/
--rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.5/cmip/web/__init__.py
--rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.5/cmip/web/html.py
--rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/web/simhash_utils.py
--rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/web/utils.py
--rw-rw-rw-   0        0        0     3445 2023-04-17 02:42:39.000000 cmip-0.0.5/cmip/web/web_scraping.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.540705 cmip-0.0.5/cmip/word_discover/
--rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/ngram.py
--rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/word_discover.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.515975 cmip-0.0.5/cmip.egg-info/
--rw-rw-rw-   0        0        0     1128 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 02:48:33.547712 cmip-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-17 02:45:11.000000 cmip-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.542705 cmip-0.0.5/test/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.5/test/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.5/test/test_ac_automation.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.541176 cmip-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-04-19 10:30:50.540175 cmip-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-04-17 02:51:43.000000 cmip-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.504080 cmip-0.0.6/cmip/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.512839 cmip-0.0.6/cmip/data/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/ad.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/chinese_frequency.tsv
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/letter_mapping.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/pinyin.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.515841 cmip-0.0.6/cmip/gibberish/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/gibberish/__init__.py
+-rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/gibberish/gibberish.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.517845 cmip-0.0.6/cmip/image/
+-rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.523840 cmip-0.0.6/cmip/text/
+-rw-rw-rw-   0        0        0     2886 2023-04-19 10:30:05.000000 cmip-0.0.6/cmip/text/__init__.py
+-rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.6/cmip/text/ac_automation.py
+-rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/text/normalize.py
+-rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/text/similarity.py
+-rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.6/cmip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.532837 cmip-0.0.6/cmip/web/
+-rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.6/cmip/web/__init__.py
+-rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.6/cmip/web/html.py
+-rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/web/simhash_utils.py
+-rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/web/utils.py
+-rw-rw-rw-   0        0        0     3445 2023-04-17 02:42:39.000000 cmip-0.0.6/cmip/web/web_scraping.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.537175 cmip-0.0.6/cmip/word_discover/
+-rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/ngram.py
+-rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/word_discover.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.509837 cmip-0.0.6/cmip.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 10:30:50.541176 cmip-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-19 10:29:33.000000 cmip-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.539174 cmip-0.0.6/test/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.6/test/__init__.py
+-rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.6/test/test_ac_automation.py
```

### Comparing `cmip-0.0.5/LICENSE` & `cmip-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/PKG-INFO` & `cmip-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cmip
-Version: 0.0.5
+Version: 0.0.6
 Summary: An efficient information processing program.
 Home-page: https://github.com/mikuh/cmip
 Author: geb
 Author-email: 853934146@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cmip
-An efficient information processing program.
+一个高效的信息处理库。
 
 ## 安装
 ```shell
-pip install cmip
+pip install -U cmip
 ```
 
 ## 用法
 
 ### 1. 动态渲染异步爬虫
 example: 
 ```python
```

### Comparing `cmip-0.0.5/README.md` & `cmip-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cmip
-An efficient information processing program.
+一个高效的信息处理库。
 
 ## 安装
 ```shell
-pip install cmip
+pip install -U cmip
 ```
 
 ## 用法
 
 ### 1. 动态渲染异步爬虫
 example: 
 ```python
```

### Comparing `cmip-0.0.5/cmip/gibberish/gibberish.py` & `cmip-0.0.6/cmip/gibberish/gibberish.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/image/__init__.py` & `cmip-0.0.6/cmip/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/text/__init__.py` & `cmip-0.0.6/cmip/text/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Text(object):
 
     def __init__(self, case_sensitive=True):
         self.aca = ACAutomation(case_sensitive=case_sensitive)
         self.norm = Normalize()
         self.add_keywords_from_list = self.aca.add_keywords_from_list
-        self.get_keywords = self.aca.get_keywords
+        self.get_keywords = self.aca.get_all_keywords
         self.replace_keywords = self.aca.replace_keywords
         self.extract_keywords = self.aca.extract_keywords
         self.normalize = self.norm.normalize
         self.pinyin = self.norm.pinyin
 
     def clean(self, sentence, patten: str = None, keep_space: bool = True, norm: bool = True, lower: bool = True,
               digital_norm: bool = False, max_repeat: int = 0) -> str:
```

### Comparing `cmip-0.0.5/cmip/text/ac_automation.py` & `cmip-0.0.6/cmip/text/ac_automation.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/text/normalize.py` & `cmip-0.0.6/cmip/text/normalize.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/text/similarity.py` & `cmip-0.0.6/cmip/text/similarity.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/utils.py` & `cmip-0.0.6/cmip/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/web/html.py` & `cmip-0.0.6/cmip/web/html.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/web/simhash_utils.py` & `cmip-0.0.6/cmip/web/simhash_utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/web/utils.py` & `cmip-0.0.6/cmip/web/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/web/web_scraping.py` & `cmip-0.0.6/cmip/web/web_scraping.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/word_discover/ngram.py` & `cmip-0.0.6/cmip/word_discover/ngram.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip/word_discover/word_discover.py` & `cmip-0.0.6/cmip/word_discover/word_discover.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/cmip.egg-info/PKG-INFO` & `cmip-0.0.6/cmip.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cmip
-Version: 0.0.5
+Version: 0.0.6
 Summary: An efficient information processing program.
 Home-page: https://github.com/mikuh/cmip
 Author: geb
 Author-email: 853934146@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cmip
-An efficient information processing program.
+一个高效的信息处理库。
 
 ## 安装
 ```shell
-pip install cmip
+pip install -U cmip
 ```
 
 ## 用法
 
 ### 1. 动态渲染异步爬虫
 example: 
 ```python
```

### Comparing `cmip-0.0.5/cmip.egg-info/SOURCES.txt` & `cmip-0.0.6/cmip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmip-0.0.5/setup.py` & `cmip-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmip",
-    version="0.0.5",
+    version="0.0.6",
     author="geb",
     author_email="853934146@qq.com",
     description="An efficient information processing program.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikuh/cmip",
     packages=setuptools.find_packages(),
```

### Comparing `cmip-0.0.5/test/test_ac_automation.py` & `cmip-0.0.6/test/test_ac_automation.py`

 * *Files identical despite different names*

