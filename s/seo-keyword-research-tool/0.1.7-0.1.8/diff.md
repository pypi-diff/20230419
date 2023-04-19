# Comparing `tmp/seo-keyword-research-tool-0.1.7.tar.gz` & `tmp/seo-keyword-research-tool-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seo-keyword-research-tool-0.1.7.tar", last modified: Wed Apr 19 09:54:27 2023, max compression
+gzip compressed data, was "seo-keyword-research-tool-0.1.8.tar", last modified: Wed Apr 19 10:59:41 2023, max compression
```

## Comparing `seo-keyword-research-tool-0.1.7.tar` & `seo-keyword-research-tool-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 09:54:27.676387 seo-keyword-research-tool-0.1.7/
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 09:54:27.676387 seo-keyword-research-tool-0.1.7/PKG-INFO
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     7648 2023-04-18 18:28:59.000000 seo-keyword-research-tool-0.1.7/README.md
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       91 2023-02-16 14:17:19.000000 seo-keyword-research-tool-0.1.7/pyproject.toml
-drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 09:54:27.676387 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/PKG-INFO
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)      329 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/SOURCES.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/dependency_links.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       34 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/entry_points.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       27 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/requires.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 09:54:27.000000 seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/top_level.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       38 2023-04-19 09:54:27.676387 seo-keyword-research-tool-0.1.7/setup.cfg
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     2035 2023-04-19 09:53:06.000000 seo-keyword-research-tool-0.1.7/setup.py
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     1092 2023-01-24 10:20:20.000000 seo-keyword-research-tool-0.1.8/LICENSE
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/PKG-INFO
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     7648 2023-04-18 18:28:59.000000 seo-keyword-research-tool-0.1.8/README.md
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       52 2023-03-29 06:41:45.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/__init__.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     3191 2023-04-19 10:52:57.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/cli.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     5111 2023-04-18 18:45:52.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/seo_keyword_research.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       91 2023-02-16 14:17:19.000000 seo-keyword-research-tool-0.1.8/pyproject.toml
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/PKG-INFO
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)      437 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       53 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/entry_points.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       27 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/requires.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/top_level.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       38 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/setup.cfg
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     2052 2023-04-19 10:56:37.000000 seo-keyword-research-tool-0.1.8/setup.py
```

### Comparing `seo-keyword-research-tool-0.1.7/PKG-INFO` & `seo-keyword-research-tool-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seo-keyword-research-tool
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.
 Home-page: https://github.com/chukhraiartur/seo-keyword-research-tool
 Author: Artur Chukhrai
 Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub
 Maintainer-email: chukhraiartur@gmail.com, dimitryzub@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.8 Summary:
 Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and
 Related Searches. Home-page: https://github.com/chukhraiartur/seo-keyword-
 research-tool Author: Artur Chukhrai Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub Maintainer-email:
 chukhraiartur@gmail.com, dimitryzub@gmail.com License: MIT Project-URL:
 Documentation, https://github.com/chukhraiartur/seo-keyword-research-tool
 Project-URL: Source, https://github.com/chukhraiartur/seo-keyword-research-tool
```

### Comparing `seo-keyword-research-tool-0.1.7/README.md` & `seo-keyword-research-tool-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `seo-keyword-research-tool-0.1.7/seo_keyword_research_tool.egg-info/PKG-INFO` & `seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seo-keyword-research-tool
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.
 Home-page: https://github.com/chukhraiartur/seo-keyword-research-tool
 Author: Artur Chukhrai
 Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub
 Maintainer-email: chukhraiartur@gmail.com, dimitryzub@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.8 Summary:
 Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and
 Related Searches. Home-page: https://github.com/chukhraiartur/seo-keyword-
 research-tool Author: Artur Chukhrai Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub Maintainer-email:
 chukhraiartur@gmail.com, dimitryzub@gmail.com License: MIT Project-URL:
 Documentation, https://github.com/chukhraiartur/seo-keyword-research-tool
 Project-URL: Source, https://github.com/chukhraiartur/seo-keyword-research-tool
```

### Comparing `seo-keyword-research-tool-0.1.7/setup.py` & `seo-keyword-research-tool-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='seo-keyword-research-tool',
     description = 'Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.',
     url='https://github.com/chukhraiartur/seo-keyword-research-tool',
-    version='0.1.7',
+    version='0.1.8',
     license='MIT',
     author='Artur Chukhrai',
     author_email='chukhraiartur@gmail.com',
     maintainer='Artur Chukhrai, Dmitiry Zub',
     maintainer_email='chukhraiartur@gmail.com, dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
@@ -50,11 +50,11 @@
     project_urls={
         'Documentation': 'https://github.com/chukhraiartur/seo-keyword-research-tool',
         'Source': 'https://github.com/chukhraiartur/seo-keyword-research-tool',
         'Tracker': 'https://github.com/chukhraiartur/seo-keyword-research-tool/issues',
     },
     entry_points={
         'console_scripts': [
-            'seo = cli:main',
+            'seo=SeoKeywordResearch.cli:main',
         ],
     },
 )
```

