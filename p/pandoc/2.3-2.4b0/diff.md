# Comparing `tmp/pandoc-2.3.tar.gz` & `tmp/pandoc-2.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-2.3.tar", last modified: Wed Nov 23 19:35:43 2022, max compression
+gzip compressed data, was "pandoc-2.4b0.tar", last modified: Wed Apr 19 12:05:36 2023, max compression
```

## Comparing `pandoc-2.3.tar` & `pandoc-2.4b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2022-11-23 19:35:43.746394 pandoc-2.3/
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     1115 2021-10-06 15:51:13.000000 pandoc-2.3/LICENSE
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       73 2016-03-18 12:11:26.000000 pandoc-2.3/MANIFEST.in
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     3865 2022-11-23 19:35:43.746394 pandoc-2.3/PKG-INFO
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     2847 2022-05-02 09:45:47.000000 pandoc-2.3/README.md
--rw-r--r--   0 boisgera  (1000) boisgera  (1000)       75 2022-11-23 19:35:43.746394 pandoc-2.3/setup.cfg
--rwxrwxr-x   0 boisgera  (1000) boisgera  (1000)      874 2022-11-23 15:45:35.000000 pandoc-2.3/setup.py
-drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2022-11-23 19:35:43.742395 pandoc-2.3/src/
-drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2022-11-23 19:35:43.742395 pandoc-2.3/src/pandoc/
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    25133 2022-11-23 16:09:56.000000 pandoc-2.3/src/pandoc/__init__.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       55 2020-04-05 10:44:52.000000 pandoc-2.3/src/pandoc/__main__.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      406 2022-11-23 18:21:54.000000 pandoc-2.3/src/pandoc/about.py
-drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2022-11-23 19:35:43.746394 pandoc-2.3/src/pandoc/doctest/
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     5120 2020-03-28 13:35:45.000000 pandoc-2.3/src/pandoc/doctest/__init__.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    10623 2022-05-06 10:02:49.000000 pandoc-2.3/src/pandoc/labs.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)   128807 2022-11-23 18:10:35.000000 pandoc-2.3/src/pandoc/pandoc-types.js
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    57128 2020-03-28 13:35:45.000000 pandoc-2.3/src/pandoc/tests.md
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      429 2020-04-05 10:44:52.000000 pandoc-2.3/src/pandoc/tests.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     5159 2021-11-26 09:22:26.000000 pandoc-2.3/src/pandoc/types.py
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     8424 2022-11-23 17:33:52.000000 pandoc-2.3/src/pandoc/utils.py
-drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2022-11-23 19:35:43.746394 pandoc-2.3/src/pandoc.egg-info/
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     3865 2022-11-23 19:35:43.000000 pandoc-2.3/src/pandoc.egg-info/PKG-INFO
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      440 2022-11-23 19:35:43.000000 pandoc-2.3/src/pandoc.egg-info/SOURCES.txt
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)        1 2022-11-23 19:35:43.000000 pandoc-2.3/src/pandoc.egg-info/dependency_links.txt
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       12 2022-11-23 19:35:43.000000 pandoc-2.3/src/pandoc.egg-info/requires.txt
--rw-rw-r--   0 boisgera  (1000) boisgera  (1000)        7 2022-11-23 19:35:43.000000 pandoc-2.3/src/pandoc.egg-info/top_level.txt
+drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2023-04-19 12:05:36.928961 pandoc-2.4b0/
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     1115 2021-10-06 15:51:13.000000 pandoc-2.4b0/LICENSE
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       73 2016-03-18 12:11:26.000000 pandoc-2.4b0/MANIFEST.in
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     3297 2023-04-19 12:05:36.928961 pandoc-2.4b0/PKG-INFO
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     2841 2023-04-19 09:08:26.000000 pandoc-2.4b0/README.md
+-rw-r--r--   0 boisgera  (1000) boisgera  (1000)       75 2023-04-19 12:05:36.928961 pandoc-2.4b0/setup.cfg
+-rwxrwxr-x   0 boisgera  (1000) boisgera  (1000)      874 2022-11-23 15:45:35.000000 pandoc-2.4b0/setup.py
+drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2023-04-19 12:05:36.924961 pandoc-2.4b0/src/
+drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2023-04-19 12:05:36.924961 pandoc-2.4b0/src/pandoc/
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    25133 2022-11-23 16:09:56.000000 pandoc-2.4b0/src/pandoc/__init__.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       55 2020-04-05 10:44:52.000000 pandoc-2.4b0/src/pandoc/__main__.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      408 2023-04-19 08:21:14.000000 pandoc-2.4b0/src/pandoc/about.py
+drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2023-04-19 12:05:36.928961 pandoc-2.4b0/src/pandoc/doctest/
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     5120 2020-03-28 13:35:45.000000 pandoc-2.4b0/src/pandoc/doctest/__init__.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    13401 2023-02-05 18:15:15.000000 pandoc-2.4b0/src/pandoc/labs.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)   131925 2023-04-19 07:49:01.000000 pandoc-2.4b0/src/pandoc/pandoc-types.js
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)    57128 2020-03-28 13:35:45.000000 pandoc-2.4b0/src/pandoc/tests.md
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      429 2020-04-05 10:44:52.000000 pandoc-2.4b0/src/pandoc/tests.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     5159 2021-11-26 09:22:26.000000 pandoc-2.4b0/src/pandoc/types.py
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     8540 2023-02-05 18:15:15.000000 pandoc-2.4b0/src/pandoc/utils.py
+drwxrwxr-x   0 boisgera  (1000) boisgera  (1000)        0 2023-04-19 12:05:36.928961 pandoc-2.4b0/src/pandoc.egg-info/
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)     3297 2023-04-19 12:05:36.000000 pandoc-2.4b0/src/pandoc.egg-info/PKG-INFO
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)      440 2023-04-19 12:05:36.000000 pandoc-2.4b0/src/pandoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)        1 2023-04-19 12:05:36.000000 pandoc-2.4b0/src/pandoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)       12 2023-04-19 12:05:36.000000 pandoc-2.4b0/src/pandoc.egg-info/requires.txt
+-rw-rw-r--   0 boisgera  (1000) boisgera  (1000)        7 2023-04-19 12:05:36.000000 pandoc-2.4b0/src/pandoc.egg-info/top_level.txt
```

### Comparing `pandoc-2.3/LICENSE` & `pandoc-2.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/PKG-INFO` & `pandoc-2.4b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,67 @@
-Metadata-Version: 2.1
-Name: pandoc
-Version: 2.3
-Summary: Pandoc Documents for Python
-Home-page: UNKNOWN
-Author: Sébastien Boisgérault
-Author-email: Sebastien.Boisgerault@minesparis.psl.eu
-License: MIT License
-Description: 
-        Pandoc – 🐍 Python Library
-        ================================================================================
-        
-        ![Python](https://img.shields.io/pypi/pyversions/pandoc.svg)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc.svg)](https://pypi.python.org/pypi/pandoc)
-        [![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://boisgera.github.io/pandoc)
-        [![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/boisgera/pandoc/discussions)
-        [![Downloads](https://pepy.tech/badge/pandoc)](https://pepy.tech/project/pandoc)
-        [![GitHub stars](https://img.shields.io/github/stars/boisgera/pandoc?style=flat)](https://github.com/boisgera/pandoc/stargazers)
-        
-        [![linux](https://github.com/boisgera/pandoc/actions/workflows/linux.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/linux.yml)
-        [![macos](https://github.com/boisgera/pandoc/actions/workflows/macos.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/macos.yml)
-        [![windows](https://github.com/boisgera/pandoc/actions/workflows/windows.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/windows.yml)
-        
-        
-        🚀 Getting started
-        --------------------------------------------------------------------------------
-        
-        [Pandoc] – the general markup converter (and Haskell library) written by 
-        [John MacFarlane] – needs to be available. 
-        You may follow the official [installation instructions][pandoc-install] 
-        or use [conda]:
-        
-            $ conda install -c conda-forge pandoc
-        
-        Then, install the latest stable version of the pandoc Python library with pip:
-        
-            $ pip install --upgrade pandoc
-        
-        
-        🌌 Overview 
-        --------------------------------------------------------------------------------
-        
-        This project brings [Pandoc]'s data model for markdown documents to Python:
-        
-            $ echo "Hello world!" | python -m pandoc read 
-            Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
-        
-        It can be used to analyze, create and transform documents, in Python :
-        
-            >>> import pandoc
-            >>> text = "Hello world!"
-            >>> doc = pandoc.read(text)
-            >>> doc
-            Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
-        
-            >>> paragraph = doc[1][0]
-            >>> paragraph
-            Para([Str('Hello'), Space(), Str('world!')])
-            >>> from pandoc.types import Str
-            >>> paragraph[0][2] = Str('Python!')
-            >>> text = pandoc.write(doc)
-            >>> print(text)
-            Hello Python!
-        
-        For more information, refer to the  [📖 documentation][doc].
-        
-        
-        [Pandoc]: https://pandoc.org/
-        [John MacFarlane]: https://johnmacfarlane.net/
-        [pandoc-install]: https://pandoc.org/installing.html
-        [conda]: https://docs.conda.io
-        [Haskell]: https://www.haskell.org/
-        [Python]: https://www.python.org/
-        [TPD]: https://hackage.haskell.org/package/pandoc-types-1.20/docs/Text-Pandoc-Definition.html
-        [doc]: https://boisgera.github.io/pandoc
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development
-Classifier: Topic :: Text Editors :: Text Processing
-Description-Content-Type: text/markdown
+
+Pandoc (Python Library)
+================================================================================
+
+![Python](https://img.shields.io/pypi/pyversions/pandoc.svg)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc.svg)](https://pypi.python.org/pypi/pandoc)
+[![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://boisgera.github.io/pandoc)
+[![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/boisgera/pandoc/discussions)
+[![Downloads](https://pepy.tech/badge/pandoc)](https://pepy.tech/project/pandoc)
+[![GitHub stars](https://img.shields.io/github/stars/boisgera/pandoc?style=flat)](https://github.com/boisgera/pandoc/stargazers)
+
+[![linux](https://github.com/boisgera/pandoc/actions/workflows/linux.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/linux.yml)
+[![macos](https://github.com/boisgera/pandoc/actions/workflows/macos.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/macos.yml)
+[![windows](https://github.com/boisgera/pandoc/actions/workflows/windows.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/windows.yml)
+
+
+🚀 Getting started
+--------------------------------------------------------------------------------
+
+Install [Pandoc] first, for example with [conda]:
+
+    $ conda install -c conda-forge pandoc
+
+Then, install the Pandoc Python Library with pip:
+
+    $ pip install --upgrade pandoc
+
+
+🌌 Overview 
+--------------------------------------------------------------------------------
+
+[Pandoc] is the awesome open-source command-line tool that converts documents 
+from one format to another. The project was initiated by [John MacFarlane]; 
+under the hood, it's a [Haskell] library.
+
+The Pandoc Python Library brings [Pandoc]'s document model to Python:
+
+    $ echo "Hello world!" | python -m pandoc read 
+    Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
+
+It can be used to analyze, create and transform documents, in Python:
+
+    >>> import pandoc
+    >>> text = "Hello world!"
+    >>> doc = pandoc.read(text)
+    >>> doc
+    Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
+
+    >>> paragraph = doc[1][0]
+    >>> paragraph
+    Para([Str('Hello'), Space(), Str('world!')])
+    >>> from pandoc.types import Str
+    >>> paragraph[0][2] = Str('Python!')
+    >>> text = pandoc.write(doc)
+    >>> print(text)
+    Hello Python!
+
+For more information, refer to the  [📖 documentation][doc].
+
+[Pandoc]: https://pandoc.org/
+[John MacFarlane]: https://johnmacfarlane.net/
+[pandoc-install]: https://pandoc.org/installing.html
+[conda]: https://docs.conda.io
+[Haskell]: https://www.haskell.org/
+[Python]: https://www.python.org/
+[TPD]: https://hackage.haskell.org/package/pandoc-types-1.20/docs/Text-Pandoc-Definition.html
+[doc]: https://boisgera.github.io/pandoc
```

### Comparing `pandoc-2.3/setup.py` & `pandoc-2.4b0/setup.py`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/src/pandoc/__init__.py` & `pandoc-2.4b0/src/pandoc/__init__.py`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/src/pandoc/doctest/__init__.py` & `pandoc-2.4b0/src/pandoc/doctest/__init__.py`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/src/pandoc/pandoc-types.js` & `pandoc-2.4b0/src/pandoc/pandoc-types.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1499,14 +1499,54 @@
                 ">=",
                 "1.22.2"
             ],
             [
                 "<",
                 "1.23"
             ]
+        ],
+        "3.0": [
+            [
+                ">=",
+                "1.23"
+            ],
+            [
+                "<",
+                "1.24"
+            ]
+        ],
+        "3.0.1": [
+            [
+                ">=",
+                "1.23"
+            ],
+            [
+                "<",
+                "1.24"
+            ]
+        ],
+        "3.1.0": [
+            [
+                ">=",
+                "1.23"
+            ],
+            [
+                "<",
+                "1.24"
+            ]
+        ],
+        "3.1.1": [
+            [
+                ">=",
+                "1.23"
+            ],
+            [
+                "<",
+                "1.24"
+            ]
         ]
     },
     "definitions": {
         "1.8": "data Pandoc = Pandoc Meta [Block]\ndata Meta\n  = Meta {docTitle :: [Inline],\n docAuthors :: [[Inline]],\n docDate :: [Inline]}\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\ntype Format = String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | EmDash\n  | EnDash\n  | Apostrophe\n  | Ellipses\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link [Inline] Target\n  | Image [Inline] Target\n  | Note [Block]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\n",
         "1.8.0.2": "data Pandoc = Pandoc Meta [Block]\ndata Meta\n  = Meta {docTitle :: [Inline],\n docAuthors :: [[Inline]],\n docDate :: [Inline]}\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\ntype Format = String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | EmDash\n  | EnDash\n  | Apostrophe\n  | Ellipses\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link [Inline] Target\n  | Image [Inline] Target\n  | Note [Block]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\n",
         "1.8.2": "data Pandoc = Pandoc Meta [Block]\ndata Meta\n  = Meta {docTitle :: [Inline],\n docAuthors :: [[Inline]],\n docDate :: [Inline]}\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\ntype Format = String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | EmDash\n  | EnDash\n  | Apostrophe\n  | Ellipses\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link [Inline] Target\n  | Image [Inline] Target\n  | Note [Block]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\n",
         "1.9.0.1": "data Pandoc = Pandoc Meta [Block]\ndata Meta\n  = Meta {docTitle :: [Inline],\n docAuthors :: [[Inline]],\n docDate :: [Inline]}\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\ntype Format = String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link [Inline] Target\n  | Image [Inline] Target\n  | Note [Block]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\n",
@@ -1552,10 +1592,11 @@
         "1.19": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map String MetaValue}\ndata MetaValue\n  = MetaMap (Map String MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString String\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: String -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\nnewtype Format = Format String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.17.6": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map String MetaValue}\ndata MetaValue\n  = MetaMap (Map String MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString String\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: String -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\nnewtype Format = Format String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.17.6.1": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map String MetaValue}\ndata MetaValue\n  = MetaMap (Map String MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString String\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: String -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (String, [String], [(String, String)])\nnullAttr :: Attr\ntype TableCell = [Block]\nnewtype Format = Format String\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr String\n  | RawBlock Format String\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (String, String)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str String\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr String\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType String\n  | RawInline Format String\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: String,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.20": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\ntype TableCell = [Block]\nnewtype Format = Format Text\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table [Inline] [Alignment] [Double] [TableCell] [[TableCell]]\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.22": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row Attr [Cell]\ndata TableHead = TableHead Attr [Row]\ndata TableBody = TableBody Attr RowHeadColumns [Row] [Row]\ndata TableFoot = TableFoot Attr [Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption (Maybe ShortCaption) [Block]\ndata Cell = Cell Attr Alignment RowSpan ColSpan [Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table Attr Caption [ColSpec] TableHead [TableBody] TableFoot\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Underline [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.22.1": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row Attr [Cell]\ndata TableHead = TableHead Attr [Row]\ndata TableBody = TableBody Attr RowHeadColumns [Row] [Row]\ndata TableFoot = TableFoot Attr [Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption (Maybe ShortCaption) [Block]\ndata Cell = Cell Attr Alignment RowSpan ColSpan [Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table Attr Caption [ColSpec] TableHead [TableBody] TableFoot\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\npattern SimpleFigure :: Attr -> [Inline] -> Target -> Block\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Underline [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
         "1.22.2": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row Attr [Cell]\ndata TableHead = TableHead Attr [Row]\ndata TableBody = TableBody Attr RowHeadColumns [Row] [Row]\ndata TableFoot = TableFoot Attr [Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption (Maybe ShortCaption) [Block]\ndata Cell = Cell Attr Alignment RowSpan ColSpan [Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table Attr Caption [ColSpec] TableHead [TableBody] TableFoot\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\npattern SimpleFigure :: Attr -> [Inline] -> Target -> Block\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Underline [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
-        "1.22.2.1": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row Attr [Cell]\ndata TableHead = TableHead Attr [Row]\ndata TableBody = TableBody Attr RowHeadColumns [Row] [Row]\ndata TableFoot = TableFoot Attr [Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption (Maybe ShortCaption) [Block]\ndata Cell = Cell Attr Alignment RowSpan ColSpan [Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table Attr Caption [ColSpec] TableHead [TableBody] TableFoot\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\npattern SimpleFigure :: Attr -> [Inline] -> Target -> Block\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Underline [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n"
+        "1.22.2.1": "data Pandoc = Pandoc Meta [Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap (Map Text MetaValue)\n  | MetaList [MetaValue]\n  | MetaBool Bool\n  | MetaString Text\n  | MetaInlines [Inline]\n  | MetaBlocks [Block]\nnullMeta :: Meta\nisNullMeta :: Meta -> Bool\nlookupMeta :: Text -> Meta -> Maybe MetaValue\ndocTitle :: Meta -> [Inline]\ndocAuthors :: Meta -> [[Inline]]\ndocDate :: Meta -> [Inline]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnullAttr :: Attr\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row Attr [Cell]\ndata TableHead = TableHead Attr [Row]\ndata TableBody = TableBody Attr RowHeadColumns [Row] [Row]\ndata TableFoot = TableFoot Attr [Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption (Maybe ShortCaption) [Block]\ndata Cell = Cell Attr Alignment RowSpan ColSpan [Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain [Inline]\n  | Para [Inline]\n  | LineBlock [[Inline]]\n  | CodeBlock Attr Text\n  | RawBlock Format Text\n  | BlockQuote [Block]\n  | OrderedList ListAttributes [[Block]]\n  | BulletList [[Block]]\n  | DefinitionList [([Inline], [[Block]])]\n  | Header Int Attr [Inline]\n  | HorizontalRule\n  | Table Attr Caption [ColSpec] TableHead [TableBody] TableFoot\n  | Div Attr [Block]\n  | Null\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\npattern SimpleFigure :: Attr -> [Inline] -> Target -> Block\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str Text\n  | Emph [Inline]\n  | Underline [Inline]\n  | Strong [Inline]\n  | Strikeout [Inline]\n  | Superscript [Inline]\n  | Subscript [Inline]\n  | SmallCaps [Inline]\n  | Quoted QuoteType [Inline]\n  | Cite [Citation] [Inline]\n  | Code Attr Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math MathType Text\n  | RawInline Format Text\n  | Link Attr [Inline] Target\n  | Image Attr [Inline] Target\n  | Note [Block]\n  | Span Attr [Inline]\ndata Citation\n  = Citation {citationId :: Text,\n     citationPrefix :: [Inline],\n     citationSuffix :: [Inline],\n     citationMode :: CitationMode,\n     citationNoteNum :: Int,\n     citationHash :: Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\npandocTypesVersion :: Version\n",
+        "1.23": "data Pandoc = Pandoc !Meta ![Block]\nnewtype Meta = Meta {unMeta :: Map Text MetaValue}\ndata MetaValue\n  = MetaMap !(Map Text MetaValue)\n  | MetaList ![MetaValue]\n  | MetaBool !Bool\n  | MetaString !Text\n  | MetaInlines ![Inline]\n  | MetaBlocks ![Block]\ntype ListAttributes = (Int, ListNumberStyle, ListNumberDelim)\ndata ListNumberStyle\n  = DefaultStyle\n  | Example\n  | Decimal\n  | LowerRoman\n  | UpperRoman\n  | LowerAlpha\n  | UpperAlpha\ndata ListNumberDelim = DefaultDelim | Period | OneParen | TwoParens\ntype Attr = (Text, [Text], [(Text, Text)])\nnewtype Format = Format Text\nnewtype RowHeadColumns = RowHeadColumns Int\ndata Alignment\n  = AlignLeft | AlignRight | AlignCenter | AlignDefault\ndata ColWidth = ColWidth !Double | ColWidthDefault\ntype ColSpec = (Alignment, ColWidth)\ndata Row = Row !Attr ![Cell]\ndata TableHead = TableHead !Attr ![Row]\ndata TableBody = TableBody !Attr !RowHeadColumns ![Row] ![Row]\ndata TableFoot = TableFoot !Attr ![Row]\ntype ShortCaption = [Inline]\ndata Caption = Caption !(Maybe ShortCaption) ![Block]\ndata Cell = Cell !Attr !Alignment !RowSpan !ColSpan ![Block]\nnewtype RowSpan = RowSpan Int\nnewtype ColSpan = ColSpan Int\ndata Block\n  = Plain ![Inline]\n  | Para ![Inline]\n  | LineBlock ![[Inline]]\n  | CodeBlock !Attr !Text\n  | RawBlock !Format !Text\n  | BlockQuote ![Block]\n  | OrderedList !ListAttributes ![[Block]]\n  | BulletList ![[Block]]\n  | DefinitionList ![([Inline], [[Block]])]\n  | Header !Int !Attr ![Inline]\n  | HorizontalRule\n  | Table !Attr\n          !Caption\n          ![ColSpec]\n          !TableHead\n          ![TableBody]\n          !TableFoot\n  | Figure !Attr !Caption ![Block]\n  | Div !Attr ![Block]\ndata QuoteType = SingleQuote | DoubleQuote\ntype Target = (Text, Text)\ndata MathType = DisplayMath | InlineMath\ndata Inline\n  = Str !Text\n  | Emph ![Inline]\n  | Underline ![Inline]\n  | Strong ![Inline]\n  | Strikeout ![Inline]\n  | Superscript ![Inline]\n  | Subscript ![Inline]\n  | SmallCaps ![Inline]\n  | Quoted !QuoteType ![Inline]\n  | Cite ![Citation] ![Inline]\n  | Code !Attr !Text\n  | Space\n  | SoftBreak\n  | LineBreak\n  | Math !MathType !Text\n  | RawInline !Format !Text\n  | Link !Attr ![Inline] !Target\n  | Image !Attr ![Inline] !Target\n  | Note ![Block]\n  | Span !Attr ![Inline]\ndata Citation\n  = Citation {citationId :: !Text,\n              citationPrefix :: ![Inline],\n              citationSuffix :: ![Inline],\n              citationMode :: !CitationMode,\n              citationNoteNum :: !Int,\n              citationHash :: !Int}\ndata CitationMode = AuthorInText | SuppressAuthor | NormalCitation\n"
     }
 }
```

### Comparing `pandoc-2.3/src/pandoc/tests.md` & `pandoc-2.4b0/src/pandoc/tests.md`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/src/pandoc/types.py` & `pandoc-2.4b0/src/pandoc/types.py`

 * *Files identical despite different names*

### Comparing `pandoc-2.3/src/pandoc/utils.py` & `pandoc-2.4b0/src/pandoc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     "DCOLON",
     "LPAREN",
     "RPAREN",
     "LBRACKET",
     "RBRACKET",
     "LBRACE",
     "RBRACE",
+    "EXCLAMATION",
 ]
 keywords = {
     "data": "DATA",
     "type": "TYPE",
     "newtype": "NEWTYPE",
     "Map": "MAP",
     "Maybe": "MAYBE",
@@ -114,14 +115,15 @@
 t_DCOLON = r"\:\:"
 t_LPAREN = r"\("
 t_RPAREN = r"\)"
 t_LBRACKET = r"\["
 t_RBRACKET = r"\]"
 t_LBRACE = r"\{"
 t_RBRACE = r"\}"
+t_EXCLAMATION = r"\!"
 
 t_ignore = " \t\n"
 
 
 def t_error(t):
     print("Illegal character '%s'" % t.value[0])
     t.lexer.skip(1)
@@ -144,14 +146,19 @@
 
 
 def p_type_paren(p):
     "type : LPAREN type RPAREN"
     p[0] = p[2]
 
 
+def p_type_exclamation(p):
+    "type : EXCLAMATION type"
+    p[0] = p[2]
+
+
 def p_type_conid(p):
     "type : CONID"
     p[0] = p[1]
 
 
 def p_type_list(p):
     "type : LBRACKET type RBRACKET"
```

### Comparing `pandoc-2.3/src/pandoc.egg-info/PKG-INFO` & `pandoc-2.4b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 Metadata-Version: 2.1
 Name: pandoc
-Version: 2.3
+Version: 2.4b0
 Summary: Pandoc Documents for Python
-Home-page: UNKNOWN
 Author: Sébastien Boisgérault
 Author-email: Sebastien.Boisgerault@minesparis.psl.eu
 License: MIT License
-Description: 
-        Pandoc – 🐍 Python Library
-        ================================================================================
-        
-        ![Python](https://img.shields.io/pypi/pyversions/pandoc.svg)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc.svg)](https://pypi.python.org/pypi/pandoc)
-        [![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://boisgera.github.io/pandoc)
-        [![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/boisgera/pandoc/discussions)
-        [![Downloads](https://pepy.tech/badge/pandoc)](https://pepy.tech/project/pandoc)
-        [![GitHub stars](https://img.shields.io/github/stars/boisgera/pandoc?style=flat)](https://github.com/boisgera/pandoc/stargazers)
-        
-        [![linux](https://github.com/boisgera/pandoc/actions/workflows/linux.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/linux.yml)
-        [![macos](https://github.com/boisgera/pandoc/actions/workflows/macos.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/macos.yml)
-        [![windows](https://github.com/boisgera/pandoc/actions/workflows/windows.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/windows.yml)
-        
-        
-        🚀 Getting started
-        --------------------------------------------------------------------------------
-        
-        [Pandoc] – the general markup converter (and Haskell library) written by 
-        [John MacFarlane] – needs to be available. 
-        You may follow the official [installation instructions][pandoc-install] 
-        or use [conda]:
-        
-            $ conda install -c conda-forge pandoc
-        
-        Then, install the latest stable version of the pandoc Python library with pip:
-        
-            $ pip install --upgrade pandoc
-        
-        
-        🌌 Overview 
-        --------------------------------------------------------------------------------
-        
-        This project brings [Pandoc]'s data model for markdown documents to Python:
-        
-            $ echo "Hello world!" | python -m pandoc read 
-            Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
-        
-        It can be used to analyze, create and transform documents, in Python :
-        
-            >>> import pandoc
-            >>> text = "Hello world!"
-            >>> doc = pandoc.read(text)
-            >>> doc
-            Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
-        
-            >>> paragraph = doc[1][0]
-            >>> paragraph
-            Para([Str('Hello'), Space(), Str('world!')])
-            >>> from pandoc.types import Str
-            >>> paragraph[0][2] = Str('Python!')
-            >>> text = pandoc.write(doc)
-            >>> print(text)
-            Hello Python!
-        
-        For more information, refer to the  [📖 documentation][doc].
-        
-        
-        [Pandoc]: https://pandoc.org/
-        [John MacFarlane]: https://johnmacfarlane.net/
-        [pandoc-install]: https://pandoc.org/installing.html
-        [conda]: https://docs.conda.io
-        [Haskell]: https://www.haskell.org/
-        [Python]: https://www.python.org/
-        [TPD]: https://hackage.haskell.org/package/pandoc-types-1.20/docs/Text-Pandoc-Definition.html
-        [doc]: https://boisgera.github.io/pandoc
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors :: Text Processing
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+Pandoc (Python Library)
+================================================================================
+
+![Python](https://img.shields.io/pypi/pyversions/pandoc.svg)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc.svg)](https://pypi.python.org/pypi/pandoc)
+[![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://boisgera.github.io/pandoc)
+[![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/boisgera/pandoc/discussions)
+[![Downloads](https://pepy.tech/badge/pandoc)](https://pepy.tech/project/pandoc)
+[![GitHub stars](https://img.shields.io/github/stars/boisgera/pandoc?style=flat)](https://github.com/boisgera/pandoc/stargazers)
+
+[![linux](https://github.com/boisgera/pandoc/actions/workflows/linux.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/linux.yml)
+[![macos](https://github.com/boisgera/pandoc/actions/workflows/macos.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/macos.yml)
+[![windows](https://github.com/boisgera/pandoc/actions/workflows/windows.yml/badge.svg)](https://github.com/boisgera/pandoc/actions/workflows/windows.yml)
+
+
+🚀 Getting started
+--------------------------------------------------------------------------------
+
+Install [Pandoc] first, for example with [conda]:
+
+    $ conda install -c conda-forge pandoc
+
+Then, install the Pandoc Python Library with pip:
+
+    $ pip install --upgrade pandoc
+
+
+🌌 Overview 
+--------------------------------------------------------------------------------
+
+[Pandoc] is the awesome open-source command-line tool that converts documents 
+from one format to another. The project was initiated by [John MacFarlane]; 
+under the hood, it's a [Haskell] library.
+
+The Pandoc Python Library brings [Pandoc]'s document model to Python:
+
+    $ echo "Hello world!" | python -m pandoc read 
+    Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
+
+It can be used to analyze, create and transform documents, in Python:
+
+    >>> import pandoc
+    >>> text = "Hello world!"
+    >>> doc = pandoc.read(text)
+    >>> doc
+    Pandoc(Meta({}), [Para([Str('Hello'), Space(), Str('world!')])])
+
+    >>> paragraph = doc[1][0]
+    >>> paragraph
+    Para([Str('Hello'), Space(), Str('world!')])
+    >>> from pandoc.types import Str
+    >>> paragraph[0][2] = Str('Python!')
+    >>> text = pandoc.write(doc)
+    >>> print(text)
+    Hello Python!
+
+For more information, refer to the  [📖 documentation][doc].
+
+[Pandoc]: https://pandoc.org/
+[John MacFarlane]: https://johnmacfarlane.net/
+[pandoc-install]: https://pandoc.org/installing.html
+[conda]: https://docs.conda.io
+[Haskell]: https://www.haskell.org/
+[Python]: https://www.python.org/
+[TPD]: https://hackage.haskell.org/package/pandoc-types-1.20/docs/Text-Pandoc-Definition.html
+[doc]: https://boisgera.github.io/pandoc
```

