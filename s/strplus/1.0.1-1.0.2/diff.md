# Comparing `tmp/strplus-1.0.1.tar.gz` & `tmp/strplus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.1.tar", max compression
+gzip compressed data, was "strplus-1.0.2.tar", max compression
```

## Comparing `strplus-1.0.1.tar` & `strplus-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.1/LICENSE
--rw-r--r--   0        0        0     2648 2023-04-19 13:35:54.517492 strplus-1.0.1/README.md
--rw-r--r--   0        0        0      876 2023-04-19 13:36:34.317481 strplus-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-1.0.1/strplus/__init__.py
--rw-r--r--   0        0        0     4243 2023-04-16 20:37:20.991093 strplus-1.0.1/strplus/cases.py
--rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-1.0.1/strplus/functions.py
--rw-r--r--   0        0        0     4231 2023-04-19 13:35:54.527492 strplus-1.0.1/strplus/strplus.py
--rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 strplus-1.0.1/setup.py
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 strplus-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2835 2023-04-19 13:50:23.887228 strplus-1.0.2/README.md
+-rw-r--r--   0        0        0      876 2023-04-19 13:50:38.307230 strplus-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/__init__.py
+-rw-r--r--   0        0        0     4243 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/cases.py
+-rw-r--r--   0        0        0      542 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/functions.py
+-rw-r--r--   0        0        0     4231 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/strplus.py
+-rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 strplus-1.0.2/setup.py
+-rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 strplus-1.0.2/PKG-INFO
```

### Comparing `strplus-1.0.1/LICENSE` & `strplus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.1/README.md` & `strplus-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,21 +49,27 @@
 - +234 test in 32 Tests files!
 - Simple use! 
 
 <br>
 
 ### Simple use example 😍
 ```
->>> my_string = Str('this_is-an_example')
->>> my_string.camel()
-'thisIsAnExample'
+>>> my_string = Str('Cast_this_string_TO_Pascal')
+>>> my_string.pascal
+'CastThisStringToPascal'
+
+>>> my_string = Str('CastMeUseLikeANormalFunction')
+>>> my_string.snake
+'cast_me_use_like_a_normal_function'
+
 ```
 <br>
 
-> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! 
+* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/examples_01.ipynb)
+* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! 
 
 <br>
 <br>
 
 # References 🌍 🗄️
 
 1. [Wise Up Data](https://github.com/wiseupdata)
```

#### html2text {}

```diff
@@ -14,18 +14,21 @@
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 
-### Simple use example ð ``` >>> my_string = Str('this_is-an_example') >>>
-my_string.camel() 'thisIsAnExample' ```
-> Check the documentations for more examples: [Documentation](https://
-wiseupdata.github.io/strplus/index.html)!
+### Simple use example ð ``` >>> my_string = Str
+('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
+>>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
+'cast_me_use_like_a_normal_function' ```
+* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/
+examples_01.ipynb) * [Documentations examples](https://wiseupdata.github.io/
+strplus/index.html)!
 
 # References ð ðï¸ 1. [Wise Up Data](https://github.com/wiseupdata) 2.
 [Emojis](https://github.com/wiseupdata/emojis) 3. [Pypi Deploy](https://
 www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-
 pypi-using-poetry-on-ubuntu-22-04)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
```

### Comparing `strplus-1.0.1/pyproject.toml` & `strplus-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.1"
+version = "1.0.2"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-1.0.1/strplus/cases.py` & `strplus-1.0.2/strplus/cases.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.1/strplus/functions.py` & `strplus-1.0.2/strplus/functions.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.1/strplus/strplus.py` & `strplus-1.0.2/strplus/strplus.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.1/setup.py` & `strplus-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'this_is-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n<br>\n\n> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/examples_01.ipynb)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.1', 'description': 'Python extra functions for strings',
+'1.0.2', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
@@ -18,17 +18,21 @@
 \n
 \n
 \n
 \n
 \n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
 \n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
 Simple use! \n\n
-\n\n### Simple use example ð\n```\n>>> my_string = Str(\'this_is-
-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n
-\n\n> Check the documentations for more examples: [Documentation](https://
+\n\n### Simple use example ð\n```\n>>> my_string = Str
+(\'Cast_this_string_TO_Pascal\')\n>>>
+my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str
+(\'CastMeUseLikeANormalFunction\')\n>>>
+my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n
+\n\n* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/
+examples/examples_01.ipynb)\n* [Documentations examples](https://
 wiseupdata.github.io/strplus/index.html)! \n\n
 \n
 \n\n# References ð ðï¸\n\n1. [Wise Up Data](https://github.com/
 wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi
 Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-
 packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n
 \n
```

### Comparing `strplus-1.0.1/PKG-INFO` & `strplus-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -66,21 +66,27 @@
 - +234 test in 32 Tests files!
 - Simple use! 
 
 <br>
 
 ### Simple use example 😍
 ```
->>> my_string = Str('this_is-an_example')
->>> my_string.camel()
-'thisIsAnExample'
+>>> my_string = Str('Cast_this_string_TO_Pascal')
+>>> my_string.pascal
+'CastThisStringToPascal'
+
+>>> my_string = Str('CastMeUseLikeANormalFunction')
+>>> my_string.snake
+'cast_me_use_like_a_normal_function'
+
 ```
 <br>
 
-> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! 
+* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/examples_01.ipynb)
+* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! 
 
 <br>
 <br>
 
 # References 🌍 🗄️
 
 1. [Wise Up Data](https://github.com/wiseupdata)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.1 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.2 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
@@ -23,18 +23,21 @@
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 
-### Simple use example ð ``` >>> my_string = Str('this_is-an_example') >>>
-my_string.camel() 'thisIsAnExample' ```
-> Check the documentations for more examples: [Documentation](https://
-wiseupdata.github.io/strplus/index.html)!
+### Simple use example ð ``` >>> my_string = Str
+('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
+>>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
+'cast_me_use_like_a_normal_function' ```
+* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/
+examples_01.ipynb) * [Documentations examples](https://wiseupdata.github.io/
+strplus/index.html)!
 
 # References ð ðï¸ 1. [Wise Up Data](https://github.com/wiseupdata) 2.
 [Emojis](https://github.com/wiseupdata/emojis) 3. [Pypi Deploy](https://
 www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-
 pypi-using-poetry-on-ubuntu-22-04)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
```

