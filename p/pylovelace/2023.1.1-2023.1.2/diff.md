# Comparing `tmp/pylovelace-2023.1.1-py3-none-any.whl.zip` & `tmp/pylovelace-2023.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17984 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-19 00:09 pylovelace/__init__.py
--rw-rw-rw-  2.0 fat     8097 b- defN 23-Apr-19 03:40 pylovelace/__main__.py
--rw-rw-rw-  2.0 fat     4382 b- defN 23-Apr-19 03:40 pylovelace/protect.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1596 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      753 b- defN 23-Apr-19 05:02 pylovelace-2023.1.1.dist-info/RECORD
-9 files, 50364 bytes uncompressed, 16678 bytes compressed:  66.9%
+Zip file size: 17982 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-19 05:09 pylovelace/__init__.py
+-rw-rw-rw-  2.0 fat     8086 b- defN 23-Apr-19 05:09 pylovelace/__main__.py
+-rw-rw-rw-  2.0 fat     4383 b- defN 23-Apr-19 05:09 pylovelace/protect.py
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1596 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/RECORD
+9 files, 50354 bytes uncompressed, 16676 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pylovelace/__main__.py
 Comment: 
 
 Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/LICENSE
+Filename: pylovelace-2023.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/METADATA
+Filename: pylovelace-2023.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/WHEEL
+Filename: pylovelace-2023.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/entry_points.txt
+Filename: pylovelace-2023.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/top_level.txt
+Filename: pylovelace-2023.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-2023.1.1.dist-info/RECORD
+Filename: pylovelace-2023.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = "2023.1.1"
+__version__ = "2023.1.2"
 __description__ = "Python code protection/obfuscation tool"
```

## pylovelace/__main__.py

```diff
@@ -7,42 +7,42 @@
 @Author: nshout
 @File: __main__.py
 """
 import argparse
 import os
 import getpass
 
-from kernel import lovelace, validate
-from protect import SingleMode
+from .kernel import lovelace, validate
+from .protect import SingleMode
 from secrets import compare_digest
 
 
 def protection_parser(subparser):
     """--------------------------------------------------------------------------------
 most common commands:
 
-protect the given file with pyintellect.
-    usage: pyintellect protect [options] file
+protect the given file with pylovelace.
+    usage: pylovelace protect [options] file
 
-to protect a module that gets compiled with pyintellect, use the --module option
-    usage: pyintellect protect --module [options] file
+to protect a module that gets compiled with pylovelace, use the --module option
+    usage: pylovelace protect --module [options] file
 --------------------------------------------------------------------------------
 (*) = recommended
 (β) = beta
 (α) = alpha
 --------------------------------------------------------------------------------"""
     parser = subparser.add_parser(
         'protect',
         aliases=["protection"],
         help="manage protection and runtime modules",
         description=protection_parser.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog='''\
 more information:
-    https://pyintellect.com
+    https://pylovelace.com
 '''
     )
     parser.add_argument(
         'file',
         help='.py file to protect'
     )
 
@@ -141,32 +141,32 @@
     )
 
     return parser
 
 
 def authentication_parser(subparser):
     """---------------------------------------------------------------------------------
-authenticate your pyintellect license if you never did before.
-    usage: pyintellect authenticate --register
+authenticate your pylovelace license if you never did before.
+    usage: pylovelace authenticate --register
 
     this will ask you for a license, username and password to register.
 
-log in to your pyintellect account.
-    usage: pyintellect authenticate --login
+log in to your pylovelace account.
+    usage: pylovelace authenticate --login
 
     this will ask you for your username and password and activate your device.
 ---------------------------------------------------------------------------------"""
     parser = subparser.add_parser(
         'authenticate',
-        help="manage authentication and PyIntellect license",
+        help="manage authentication and PyLovelace license",
         description=authentication_parser.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog='''\
 more information:
-    https://pyintellect.com
+    https://pylovelace.com
 '''
     )
 
     parser.add_argument(
         '--login',
         action='store_true',
         help='log into your account'
@@ -177,15 +177,15 @@
         action='store_true',
         help='register a new account'
     )
 
     parser.add_argument(
         '--buy',
         action='store_true',
-        help='redirect to the PyIntellect store to buy a license'
+        help='redirect to the PyLovelace store to buy a license'
     )
 
     return parser
 
 
 def version():
     """
@@ -292,15 +292,15 @@
         action='store_true',
         help='verbose output'
     )
 
     subparser = parser.add_subparsers(
         title='categories',
         dest='category',
-        description='usage: pyintellect <category>'
+        description='usage: pylovelace <category>'
     )
 
     protection_parser(subparser)
     main_parser(
         parser=parser,
         authenticate_parser=authentication_parser(subparser)
     )
```

## pylovelace/protect.py

```diff
@@ -7,15 +7,15 @@
 @Author: nshout
 @File: protect.py
 """
 import logging
 import os
 import shutil
 
-from kernel import PyLovelace, get_runtime_module, protect_code, compile_module, finalize
+from .kernel import PyLovelace, get_runtime_module, protect_code, compile_module, finalize
 
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)s - %(message)s'
 )
```

## Comparing `pylovelace-2023.1.1.dist-info/LICENSE` & `pylovelace-2023.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylovelace-2023.1.1.dist-info/METADATA` & `pylovelace-2023.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylovelace
-Version: 2023.1.1
+Version: 2023.1.2
 Summary: Python code protection/obfuscation tool
 Home-page: https://github.com/pylovelace/pylovelace
 Author: nshout
 Keywords: obfuscate obfuscation distribute production tool
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
```

## Comparing `pylovelace-2023.1.1.dist-info/RECORD` & `pylovelace-2023.1.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pylovelace/__init__.py,sha256=Bewuwnsw9G53uQU_tgnp2Tr_FsWK1edogZtk6_XzHHY,228
-pylovelace/__main__.py,sha256=SGb5TQOwgnPcKrZ3Dn25aoi8_v52XuVEHoeOcTYWDWM,8097
-pylovelace/protect.py,sha256=9JuloJfJFJOp2rbsrg7GWLh2gomkhPUhjEbCybLhqHU,4382
-pylovelace-2023.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pylovelace-2023.1.1.dist-info/METADATA,sha256=h64HwFLk1xYGmBz-LXwyM296vT3iWvwpE9fzgRowci8,1596
-pylovelace-2023.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pylovelace-2023.1.1.dist-info/entry_points.txt,sha256=-vPFZeB5Oi5SzSri14fSMwAF-co3sgO2M6Fr7ScfPeo,56
-pylovelace-2023.1.1.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
-pylovelace-2023.1.1.dist-info/RECORD,,
+pylovelace/__init__.py,sha256=ccyRZeCCDxgaIr2p9U276uAntqAFXM7rMuTGgf89WtA,228
+pylovelace/__main__.py,sha256=R-eforVO5Zt0n1GyadLvkdS2yauOdOYnXtC1fowUgwU,8086
+pylovelace/protect.py,sha256=66aY-0v6W0Y0cQj1YLiJpkQm0ZNEUNcGjibrTkgCAto,4383
+pylovelace-2023.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pylovelace-2023.1.2.dist-info/METADATA,sha256=xVPN3u18CZq_fTmDQPiav53koJThLDBTvbrJM_V6ypE,1596
+pylovelace-2023.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pylovelace-2023.1.2.dist-info/entry_points.txt,sha256=-vPFZeB5Oi5SzSri14fSMwAF-co3sgO2M6Fr7ScfPeo,56
+pylovelace-2023.1.2.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
+pylovelace-2023.1.2.dist-info/RECORD,,
```

