# Comparing `tmp/neo_grammar_graph-0.0.1.tar.gz` & `tmp/neo_grammar_graph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_grammar_graph-0.0.1.tar", last modified: Tue Apr 18 14:58:01 2023, max compression
+gzip compressed data, was "neo_grammar_graph-0.0.2.tar", last modified: Wed Apr 19 09:36:31 2023, max compression
```

## Comparing `neo_grammar_graph-0.0.1.tar` & `neo_grammar_graph-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-18 14:58:01.076873 neo_grammar_graph-0.0.1/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.1/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    43363 2023-04-18 14:58:01.077150 neo_grammar_graph-0.0.1/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2023 2023-04-18 09:44:21.000000 neo_grammar_graph-0.0.1/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-18 09:19:41.000000 neo_grammar_graph-0.0.1/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1087 2023-04-18 14:58:01.077676 neo_grammar_graph-0.0.1/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.1/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-18 14:58:01.070146 neo_grammar_graph-0.0.1/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-18 14:58:01.074127 neo_grammar_graph-0.0.1/src/neo_grammar_graph/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-18 10:03:06.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     6298 2023-04-18 10:18:48.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph/gg.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      208 2023-04-18 10:01:08.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph/helpers.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph/type_defs.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-18 14:58:01.075946 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    43363 2023-04-18 14:58:01.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-18 14:58:01.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-18 14:58:01.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      234 2023-04-18 14:58:01.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-18 14:58:01.000000 neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-18 14:58:01.076239 neo_grammar_graph-0.0.1/tests/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      277 2023-04-18 09:30:38.000000 neo_grammar_graph-0.0.1/tests/test_doctests.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:36:31.851657 neo_grammar_graph-0.0.2/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.2/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44470 2023-04-19 09:36:31.852019 neo_grammar_graph-0.0.2/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3130 2023-04-19 09:31:10.000000 neo_grammar_graph-0.0.2/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-19 09:30:11.000000 neo_grammar_graph-0.0.2/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1087 2023-04-19 09:36:31.852745 neo_grammar_graph-0.0.2/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.2/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:36:31.843324 neo_grammar_graph-0.0.2/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:36:31.848002 neo_grammar_graph-0.0.2/src/neo_grammar_graph/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-19 09:30:01.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    20127 2023-04-19 09:19:34.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph/gg.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      208 2023-04-18 10:01:08.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph/helpers.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph/type_defs.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:36:31.850682 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44470 2023-04-19 09:36:31.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-19 09:36:31.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-19 09:36:31.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      234 2023-04-19 09:36:31.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-19 09:36:31.000000 neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:36:31.850969 neo_grammar_graph-0.0.2/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      277 2023-04-18 09:30:38.000000 neo_grammar_graph-0.0.2/tests/test_doctests.py
```

### Comparing `neo_grammar_graph-0.0.1/LICENSE` & `neo_grammar_graph-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.0.1/PKG-INFO` & `neo_grammar_graph-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo_grammar_graph
-Version: 0.0.1
+Version: 0.0.2
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -691,31 +691,38 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # NeoGrammarGraph
 
+[![Python](https://img.shields.io/pypi/pyversions/neo-grammar-graph.svg)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![Version](https://img.shields.io/pypi/v/neo-grammar-graph)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![BuildStatus](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/rindPHI/NeoGrammarGraph/badge.svg?branch=main)](https://coveralls.io/github/rindPHI/NeoGrammarGraph?branch=main)
+[![Dependencies](https://img.shields.io/librariesio/release/github/rindphi/NeoGrammarGraph)](https://libraries.io/github/rindPHI/NeoGrammarGraph)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Creating graphs from context-free grammars for fun and profit.
 
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
-* Reachability
+* Reachability of grammar symbols.
+* Computing shortest paths between grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
-* Dijkstra's algorithm for shortest paths between nodes
 * Checking whether a (sub) graph represents a tree
 * Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
   k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
   derivation trees based on that.
 
 ## Install
 
@@ -742,8 +749,16 @@
 
 ```shell
 ln -s \
     /usr/local/Cellar/graph-tool/2.51/lib/python3.11/site-packages/graph_tool \
     venv/lib/python3.10/site-packages
 ```
 
+For the GitHub workflow, the following line was required:
+
+```shell
+sudo ln -s \
+    /usr/lib/python3/dist-packages/graph_tool \
+    /opt/hostedtoolcache/Python/3.10.11/x64/lib/python3.10/site-packages
+```
+
 Author: [Dominic Steinhöfel](https://www.dominic-steinhoefel.de).
```

### Comparing `neo_grammar_graph-0.0.1/README.md` & `neo_grammar_graph-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # NeoGrammarGraph
 
+[![Python](https://img.shields.io/pypi/pyversions/neo-grammar-graph.svg)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![Version](https://img.shields.io/pypi/v/neo-grammar-graph)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![BuildStatus](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/rindPHI/NeoGrammarGraph/badge.svg?branch=main)](https://coveralls.io/github/rindPHI/NeoGrammarGraph?branch=main)
+[![Dependencies](https://img.shields.io/librariesio/release/github/rindphi/NeoGrammarGraph)](https://libraries.io/github/rindPHI/NeoGrammarGraph)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Creating graphs from context-free grammars for fun and profit.
 
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
-* Reachability
+* Reachability of grammar symbols.
+* Computing shortest paths between grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
-* Dijkstra's algorithm for shortest paths between nodes
 * Checking whether a (sub) graph represents a tree
 * Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
   k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
   derivation trees based on that.
 
 ## Install
 
@@ -47,8 +54,16 @@
 
 ```shell
 ln -s \
     /usr/local/Cellar/graph-tool/2.51/lib/python3.11/site-packages/graph_tool \
     venv/lib/python3.10/site-packages
 ```
 
+For the GitHub workflow, the following line was required:
+
+```shell
+sudo ln -s \
+    /usr/lib/python3/dist-packages/graph_tool \
+    /opt/hostedtoolcache/Python/3.10.11/x64/lib/python3.10/site-packages
+```
+
 Author: [Dominic Steinhöfel](https://www.dominic-steinhoefel.de).
```

### Comparing `neo_grammar_graph-0.0.1/pyproject.toml` & `neo_grammar_graph-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neo_grammar_graph"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "Graphs from Context-Free Grammars."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `neo_grammar_graph-0.0.1/setup.cfg` & `neo_grammar_graph-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.0.1/src/neo_grammar_graph.egg-info/PKG-INFO` & `neo_grammar_graph-0.0.2/src/neo_grammar_graph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-grammar-graph
-Version: 0.0.1
+Version: 0.0.2
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -691,31 +691,38 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # NeoGrammarGraph
 
+[![Python](https://img.shields.io/pypi/pyversions/neo-grammar-graph.svg)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![Version](https://img.shields.io/pypi/v/neo-grammar-graph)](https://pypi.python.org/pypi/neo-grammar-graph/)
+[![BuildStatus](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)](https://img.shields.io/github/actions/workflow/status/rindPHI/NeoGrammarGraph/test-gg.yml?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/rindPHI/NeoGrammarGraph/badge.svg?branch=main)](https://coveralls.io/github/rindPHI/NeoGrammarGraph?branch=main)
+[![Dependencies](https://img.shields.io/librariesio/release/github/rindphi/NeoGrammarGraph)](https://libraries.io/github/rindPHI/NeoGrammarGraph)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Creating graphs from context-free grammars for fun and profit.
 
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
-* Reachability
+* Reachability of grammar symbols.
+* Computing shortest paths between grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
-* Dijkstra's algorithm for shortest paths between nodes
 * Checking whether a (sub) graph represents a tree
 * Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
   k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
   derivation trees based on that.
 
 ## Install
 
@@ -742,8 +749,16 @@
 
 ```shell
 ln -s \
     /usr/local/Cellar/graph-tool/2.51/lib/python3.11/site-packages/graph_tool \
     venv/lib/python3.10/site-packages
 ```
 
+For the GitHub workflow, the following line was required:
+
+```shell
+sudo ln -s \
+    /usr/lib/python3/dist-packages/graph_tool \
+    /opt/hostedtoolcache/Python/3.10.11/x64/lib/python3.10/site-packages
+```
+
 Author: [Dominic Steinhöfel](https://www.dominic-steinhoefel.de).
```

