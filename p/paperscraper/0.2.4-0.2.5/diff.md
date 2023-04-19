# Comparing `tmp/paperscraper-0.2.4.tar.gz` & `tmp/paperscraper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperscraper-0.2.4.tar", last modified: Wed Aug  3 15:11:28 2022, max compression
+gzip compressed data, was "paperscraper-0.2.5.tar", last modified: Wed Apr 19 16:30:47 2023, max compression
```

## Comparing `paperscraper-0.2.4.tar` & `paperscraper-0.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-08-03 15:11:21.000000 paperscraper-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-08-03 15:11:28.645428 paperscraper-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9974 2022-08-03 15:11:21.000000 paperscraper-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/arxiv/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/arxiv/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/arxiv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/get_dumps/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      894 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/biorxiv.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/chemrxiv.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      908 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/medrxiv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/get_dumps/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/get_dumps/utils/chemrxiv/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/utils/chemrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/get_dumps/utils/chemrxiv/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/journal_if.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/load_dumps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    16483 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/pubmed/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/pubmed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/pubmed/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4106 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/pubmed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/scholar/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/scholar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/scholar/scholar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/server_dumps/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/server_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper/xrxiv/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/xrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/xrxiv/xrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-08-03 15:11:21.000000 paperscraper-0.2.4/paperscraper/xrxiv/xrxiv_query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:11:28.645428 paperscraper-0.2.4/paperscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-03 15:11:28.000000 paperscraper-0.2.4/paperscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 15:11:28.645428 paperscraper-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-08-03 15:11:21.000000 paperscraper-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-04-19 16:30:33.000000 paperscraper-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-04-19 16:30:47.327613 paperscraper-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-04-19 16:30:33.000000 paperscraper-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1484 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/biorxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/chemrxiv.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/medrxiv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/journal_if.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/load_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/pubmed/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/scholar/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/scholar/scholar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/server_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/server_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/xrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 16:30:47.327613 paperscraper-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-19 16:30:33.000000 paperscraper-0.2.5/setup.py
```

### Comparing `paperscraper-0.2.4/LICENSE` & `paperscraper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/PKG-INFO` & `paperscraper-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.4
+Version: 0.2.5
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -52,18 +51,23 @@
 
 ```py
 from paperscraper.get_dumps import biorxiv, medrxiv, chemrxiv
 medrxiv()  #  Takes ~30min and should result in ~35 MB file
 biorxiv()  # Takes ~1h and should result in ~350 MB file
 chemrxiv()  #  Takes ~45min and should result in ~20 MB file
 ```
-
 *NOTE*: Once the dumps are stored, please make sure to restart the python interpreter
 so that the changes take effect. 
 
+Since v0.2.5 `paperscraper` also allows to scrape {med/bio/chem}rxiv for specific dates! Thanks to [@achouhan93 ](https://github.com/achouhan93 ) for contributions!
+```py
+medrxiv(begin_date="2023-04-01", end_date="2023-04-08")
+```
+But watch out. The resulting `.jsonl` file will be labelled according to the current date and all your subsequent searches will be based on this file **only**. If you use this option you might want to keep an eye on the source files (`paperscraper/server_dumps/*jsonl`) to ensure they contain the paper metadata for all papers you're interested in.
+
 ## Examples
 
 `paperscraper` is build on top of the packages [pymed](https://pypi.org/project/pymed/),
 [arxiv](https://pypi.org/project/arxiv/) and [scholarly](https://pypi.org/project/scholarly/). 
 
 ### Publication keyword search
 
@@ -301,9 +305,7 @@
 	pages = {100269},
 	year = {2021},
 	issn = {2666-3899},
 	url = {https://doi.org/10.1016/j.patter.2021.100269},
 	author = {Jannis Born and David Beymer and Deepta Rajan and Adam Coy and Vandana V. Mukherjee and Matteo Manica and Prasanth Prasanna and Deddeh Ballah and Michal Guindy and Dorith Shaham and Pallav L. Shah and Emmanouil Karteris and Jan L. Robertus and Maria Gabrani and Michal Rosen-Zvi}
 }
 ```
-
-
```

### Comparing `paperscraper-0.2.4/README.md` & `paperscraper-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,23 @@
 
 ```py
 from paperscraper.get_dumps import biorxiv, medrxiv, chemrxiv
 medrxiv()  #  Takes ~30min and should result in ~35 MB file
 biorxiv()  # Takes ~1h and should result in ~350 MB file
 chemrxiv()  #  Takes ~45min and should result in ~20 MB file
 ```
-
 *NOTE*: Once the dumps are stored, please make sure to restart the python interpreter
 so that the changes take effect. 
 
+Since v0.2.5 `paperscraper` also allows to scrape {med/bio/chem}rxiv for specific dates! Thanks to [@achouhan93 ](https://github.com/achouhan93 ) for contributions!
+```py
+medrxiv(begin_date="2023-04-01", end_date="2023-04-08")
+```
+But watch out. The resulting `.jsonl` file will be labelled according to the current date and all your subsequent searches will be based on this file **only**. If you use this option you might want to keep an eye on the source files (`paperscraper/server_dumps/*jsonl`) to ensure they contain the paper metadata for all papers you're interested in.
+
 ## Examples
 
 `paperscraper` is build on top of the packages [pymed](https://pypi.org/project/pymed/),
 [arxiv](https://pypi.org/project/arxiv/) and [scholarly](https://pypi.org/project/scholarly/). 
 
 ### Publication keyword search
```

### Comparing `paperscraper-0.2.4/paperscraper/__init__.py` & `paperscraper-0.2.5/paperscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Initialize the module."""
 __name__ = "paperscraper"
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 import logging
 import os
 import sys
 from typing import List, Union
 
 from .load_dumps import QUERY_FN_DICT
```

### Comparing `paperscraper-0.2.4/paperscraper/arxiv/arxiv.py` & `paperscraper-0.2.5/paperscraper/arxiv/arxiv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict, List, Union
 
-import pandas as pd
-
 import arxiv
+import pandas as pd
 
 from ..utils import dump_papers
 from .utils import get_query_from_keywords
 
 arxiv_field_mapper = {
     "published": "date",
     "journal_ref": "journal",
```

### Comparing `paperscraper-0.2.4/paperscraper/arxiv/utils.py` & `paperscraper-0.2.5/paperscraper/arxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/get_dumps/utils/chemrxiv/utils.py` & `paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     Args:
         author_list (list): List of dicts, one per author.
 
     Returns:
         str: ;-concatenated author list.
     """
 
-    return "; ".join(
-        [" ".join([a["firstName"], a["lastName"]]) for a in author_list]
-    )
+    return "; ".join([" ".join([a["firstName"], a["lastName"]]) for a in author_list])
 
 
 def get_categories(category_list: List[Dict]) -> str:
     """Parse ChemRxiv dump entry to extract the categories of the paper
 
     Args:
         category_list (list): List of dicts, one per category.
@@ -139,11 +137,11 @@
         preprint = preprint["item"]
         preprint_id = preprint["id"]
         try:
             preprint = api.preprint(preprint_id)
         except HTTPError:
             logger.warning(f"HTTP API Client error for ID: {preprint_id}")
         except SSLError:
-            logger.warning(f'SSLError for ID: {preprint_id}')
+            logger.warning(f"SSLError for ID: {preprint_id}")
 
         with open(path, "w") as file:
             json.dump(preprint, file, indent=2)
```

### Comparing `paperscraper-0.2.4/paperscraper/journal_if.py` & `paperscraper-0.2.5/paperscraper/journal_if.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/load_dumps.py` & `paperscraper-0.2.5/paperscraper/load_dumps.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/pdf.py` & `paperscraper-0.2.5/paperscraper/pdf.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/plotting.py` & `paperscraper-0.2.5/paperscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/postprocessing.py` & `paperscraper-0.2.5/paperscraper/postprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import sys
-from typing import List, Dict
+from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 logger = logging.getLogger(__name__)
```

### Comparing `paperscraper-0.2.4/paperscraper/pubmed/pubmed.py` & `paperscraper-0.2.5/paperscraper/pubmed/pubmed.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/pubmed/utils.py` & `paperscraper-0.2.5/paperscraper/pubmed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from pymed.article import PubMedArticle
 import warnings
 from typing import List, Union
 
+from pymed.article import PubMedArticle
+
 finalize_disjunction = lambda x: "(" + x[:-4] + ") AND "
 finalize_conjunction = lambda x: x[:-5]
 date_root = '("{0}"[Date - Create] : "{1}"[Date - Create])'
 
 
 def get_query_from_keywords(keywords: List[Union[str, List]]) -> str:
     """Receives a list of keywords and returns the query for the pubmed API.
```

### Comparing `paperscraper-0.2.4/paperscraper/scholar/scholar.py` & `paperscraper-0.2.5/paperscraper/scholar/scholar.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/utils.py` & `paperscraper-0.2.5/paperscraper/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper/xrxiv/xrxiv_api.py` & `paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """API for bioRxiv and medRXiv."""
-import requests
 from datetime import datetime
-from typing import Optional, List, Generator
+from typing import Generator, List, Optional
 
+import requests
 
 launch_dates = {"biorxiv": "2013-01-01", "medrxiv": "2019-06-01"}
 
 
 class XRXivApi:
     """API class."""
```

### Comparing `paperscraper-0.2.4/paperscraper/xrxiv/xrxiv_query.py` & `paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_query.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/paperscraper.egg-info/PKG-INFO` & `paperscraper-0.2.5/paperscraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.4
+Version: 0.2.5
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -52,18 +51,23 @@
 
 ```py
 from paperscraper.get_dumps import biorxiv, medrxiv, chemrxiv
 medrxiv()  #  Takes ~30min and should result in ~35 MB file
 biorxiv()  # Takes ~1h and should result in ~350 MB file
 chemrxiv()  #  Takes ~45min and should result in ~20 MB file
 ```
-
 *NOTE*: Once the dumps are stored, please make sure to restart the python interpreter
 so that the changes take effect. 
 
+Since v0.2.5 `paperscraper` also allows to scrape {med/bio/chem}rxiv for specific dates! Thanks to [@achouhan93 ](https://github.com/achouhan93 ) for contributions!
+```py
+medrxiv(begin_date="2023-04-01", end_date="2023-04-08")
+```
+But watch out. The resulting `.jsonl` file will be labelled according to the current date and all your subsequent searches will be based on this file **only**. If you use this option you might want to keep an eye on the source files (`paperscraper/server_dumps/*jsonl`) to ensure they contain the paper metadata for all papers you're interested in.
+
 ## Examples
 
 `paperscraper` is build on top of the packages [pymed](https://pypi.org/project/pymed/),
 [arxiv](https://pypi.org/project/arxiv/) and [scholarly](https://pypi.org/project/scholarly/). 
 
 ### Publication keyword search
 
@@ -301,9 +305,7 @@
 	pages = {100269},
 	year = {2021},
 	issn = {2666-3899},
 	url = {https://doi.org/10.1016/j.patter.2021.100269},
 	author = {Jannis Born and David Beymer and Deepta Rajan and Adam Coy and Vandana V. Mukherjee and Matteo Manica and Prasanth Prasanna and Deddeh Ballah and Michal Guindy and Dorith Shaham and Pallav L. Shah and Emmanouil Karteris and Jan L. Robertus and Maria Gabrani and Michal Rosen-Zvi}
 }
 ```
-
-
```

### Comparing `paperscraper-0.2.4/paperscraper.egg-info/SOURCES.txt` & `paperscraper-0.2.5/paperscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.4/setup.py` & `paperscraper-0.2.5/setup.py`

 * *Files identical despite different names*

