# Comparing `tmp/strplus-1.0.0.tar.gz` & `tmp/strplus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.0.tar", max compression
+gzip compressed data, was "strplus-1.0.1.tar", max compression
```

## Comparing `strplus-1.0.0.tar` & `strplus-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.0/LICENSE
--rw-r--r--   0        0        0     2648 2023-04-17 12:01:38.724379 strplus-1.0.0/README.md
--rw-r--r--   0        0        0      876 2023-04-19 11:37:41.659603 strplus-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-1.0.0/strplus/__init__.py
--rw-r--r--   0        0        0     4243 2023-04-16 20:37:20.991093 strplus-1.0.0/strplus/cases.py
--rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-1.0.0/strplus/functions.py
--rw-r--r--   0        0        0     4231 2023-04-19 13:33:32.077536 strplus-1.0.0/strplus/strplus.py
--rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 strplus-1.0.0/setup.py
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 strplus-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2648 2023-04-19 13:35:54.517492 strplus-1.0.1/README.md
+-rw-r--r--   0        0        0      876 2023-04-19 13:36:34.317481 strplus-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-1.0.1/strplus/__init__.py
+-rw-r--r--   0        0        0     4243 2023-04-16 20:37:20.991093 strplus-1.0.1/strplus/cases.py
+-rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-1.0.1/strplus/functions.py
+-rw-r--r--   0        0        0     4231 2023-04-19 13:35:54.527492 strplus-1.0.1/strplus/strplus.py
+-rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 strplus-1.0.1/setup.py
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 strplus-1.0.1/PKG-INFO
```

### Comparing `strplus-1.0.0/LICENSE` & `strplus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.0/README.md` & `strplus-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `strplus-1.0.0/pyproject.toml` & `strplus-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.0"
+version = "1.0.1"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-1.0.0/strplus/cases.py` & `strplus-1.0.1/strplus/cases.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.0/strplus/functions.py` & `strplus-1.0.1/strplus/functions.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.0/strplus/strplus.py` & `strplus-1.0.1/strplus/strplus.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.0/setup.py` & `strplus-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Python extra functions for strings',
     'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'this_is-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n<br>\n\n> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.0', 'description': 'Python extra functions for strings',
+'1.0.1', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
```

### Comparing `strplus-1.0.0/PKG-INFO` & `strplus-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.0 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.1 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
```

