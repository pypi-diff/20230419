# Comparing `tmp/neo_grammar_graph-0.0.3.tar.gz` & `tmp/neo_grammar_graph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_grammar_graph-0.0.3.tar", last modified: Wed Apr 19 09:52:35 2023, max compression
+gzip compressed data, was "neo_grammar_graph-0.0.4.tar", last modified: Wed Apr 19 10:19:24 2023, max compression
```

## Comparing `neo_grammar_graph-0.0.3.tar` & `neo_grammar_graph-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:52:35.125342 neo_grammar_graph-0.0.3/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.3/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44470 2023-04-19 09:52:35.125611 neo_grammar_graph-0.0.3/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3130 2023-04-19 09:31:10.000000 neo_grammar_graph-0.0.3/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-19 09:51:49.000000 neo_grammar_graph-0.0.3/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1087 2023-04-19 09:52:35.126110 neo_grammar_graph-0.0.3/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.3/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:52:35.118529 neo_grammar_graph-0.0.3/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:52:35.122927 neo_grammar_graph-0.0.3/src/neo_grammar_graph/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-19 09:51:45.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    21440 2023-04-19 09:50:28.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph/gg.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      208 2023-04-18 10:01:08.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph/helpers.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph/type_defs.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:52:35.124564 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44470 2023-04-19 09:52:35.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-19 09:52:35.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-19 09:52:35.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      234 2023-04-19 09:52:35.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-19 09:52:35.000000 neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 09:52:35.124805 neo_grammar_graph-0.0.3/tests/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      277 2023-04-18 09:30:38.000000 neo_grammar_graph-0.0.3/tests/test_doctests.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.255835 neo_grammar_graph-0.0.4/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.4/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44490 2023-04-19 10:19:24.256153 neo_grammar_graph-0.0.4/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3150 2023-04-19 10:18:28.000000 neo_grammar_graph-0.0.4/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-19 10:17:33.000000 neo_grammar_graph-0.0.4/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1088 2023-04-19 10:19:24.257107 neo_grammar_graph-0.0.4/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.4/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.248058 neo_grammar_graph-0.0.4/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.252315 neo_grammar_graph-0.0.4/src/neo_grammar_graph/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-19 10:17:29.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    24306 2023-04-19 10:16:21.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/gg.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      208 2023-04-18 10:01:08.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/helpers.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/type_defs.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.254882 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44490 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      237 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.255159 neo_grammar_graph-0.0.4/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      277 2023-04-18 09:30:38.000000 neo_grammar_graph-0.0.4/tests/test_doctests.py
```

### Comparing `neo_grammar_graph-0.0.3/LICENSE` & `neo_grammar_graph-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.0.3/PKG-INFO` & `neo_grammar_graph-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo_grammar_graph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -708,15 +708,15 @@
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
 * Reachability of grammar symbols.
-* Computing shortest paths between grammar symbols.
+* Computing the shortest path or all paths between two grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
 * Checking whether a (sub) graph represents a tree
```

### Comparing `neo_grammar_graph-0.0.3/README.md` & `neo_grammar_graph-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
 * Reachability of grammar symbols.
-* Computing shortest paths between grammar symbols.
+* Computing the shortest path or all paths between two grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
 * Checking whether a (sub) graph represents a tree
```

### Comparing `neo_grammar_graph-0.0.3/pyproject.toml` & `neo_grammar_graph-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neo_grammar_graph"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "Graphs from Context-Free Grammars."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `neo_grammar_graph-0.0.3/setup.cfg` & `neo_grammar_graph-0.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	numpy>=1.24.2
+	proxyorderedset>=0.3.0
 	scipy>=1.10.1
 
 [options.extras_require]
 test = 
 	pytest-pycharm>=0.7.0
 	pytest-xdist==2.5.0
 	pytest>=6.2.5
-	
 	pytest-cov>=3.0.0
 	pytest-html>=3.1.1
 	pytest-randomly>=3.12.0
-	pytest-xdist>=2.4.0
 dev = 
 	black>=22.8.0
 	build>=0.8.0
 	flake8>=5.0.4
 	twine>=4.0.1
 
 [options.packages.find]
```

### Comparing `neo_grammar_graph-0.0.3/src/neo_grammar_graph/gg.py` & `neo_grammar_graph-0.0.4/src/neo_grammar_graph/gg.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NeoGrammarGraph.  If not, see <http://www.gnu.org/licenses/>.
 
 import os.path
-from typing import Dict, List, Callable, Optional
+from typing import Dict, List, Callable, Optional, Tuple
 
 from graph_tool import Graph, Vertex, Edge
 from graph_tool.search import bfs_search, BFSVisitor, StopSearch
-from graph_tool.topology import transitive_closure
+from graph_tool.topology import transitive_closure, all_paths
+from orderedset import OrderedSet
 
 from neo_grammar_graph.helpers import split_expansion
 from neo_grammar_graph.type_defs import Grammar
 
 
 class NeoGrammarGraph:
     def __init__(self, grammar: Grammar):
@@ -219,18 +220,15 @@
         :return: The children of :code:`symbol` in the graph.
         """
 
         vertex = self.vertex(symbol)
         if vertex is None:
             return None
 
-        return [
-            self.symbol(child_vertex)
-            for child_vertex in vertex.out_neighbors()
-        ]
+        return [self.symbol(child_vertex) for child_vertex in vertex.out_neighbors()]
 
     def reachable(self, from_nonterminal: str, to_nonterminal: str) -> bool:
         """
         Checks whether the nonterminal symbol :code:`to_nonterminal` is reachable
         in the graph from the nonterminal symbol :code:`from_nonterminal`. Note that
         reachability is not reflexive; a nonterminal is only reachable from itself if
         there is an actual path starting and ending at that nonterminal.
@@ -543,14 +541,86 @@
         assert (
             not node_filter(len(result) - 1, target_symbol)
             or result[-1] == target_symbol
         )
 
         return result
 
+    def paths_between(
+        self,
+        start_symbol: str,
+        target_symbol: str,
+        node_filter: Callable[[int, str], bool] = lambda idx, _: idx % 2 == 0,
+    ) -> Optional[OrderedSet[Tuple[str, ...]]]:
+        """
+        Returns a list of all paths between the given grammar symbols.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        There are two paths from :code:`<stmt>` to :code:`digit` if we omit the
+        filtering of intermediate choice nodes:
+
+        >>> str(graph.paths_between("<stmt>", "<digit>", lambda idx, sym: True))
+        "{('<stmt>', '<stmt>-choice-1', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>'), ('<stmt>', '<stmt>-choice-2', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>')}"
+
+        With the default node filter, those paths collapse to a single one:
+
+        >>> str(graph.paths_between("<stmt>", "<digit>"))
+        "{('<stmt>', '<assgn>', '<rhs>', '<digit>')}"
+
+        There is no path from :code:`<digit>` to itself:
+
+        >>> str(graph.paths_between("<digit>", "<digit>"))
+        '{}'
+
+        If a symbol does not exist, we obtain :code:`None`:
+
+        >>> graph.paths_between("<some-digit>", "<digit>") is None
+        True
+
+        :param start_symbol: The start symbol of the desired paths.
+        :param target_symbol: The target symbol of the desired paths.
+        :param node_filter: A function for filtering out elements of the returned paths,
+            if any. The function must accept two arguments, the first will be an
+            integer, the position of the path element, and the second a string, the path
+            element itself. Indices/positions start at 0 for the first element.
+        :return: A list of all paths between the given grammar symbols or :code:`None`
+            if start or target symbols do not exist in the grammar graph.
+        """
+
+        start_vertex = self.vertex(start_symbol)
+        target_vertex = self.vertex(target_symbol)
+
+        if start_vertex is None or target_vertex is None:
+            return None
+
+        return OrderedSet([
+            tuple([
+                self.symbol(self.graph.vertex(vid))
+                for idx, vid in enumerate(path)
+                if node_filter(idx, self.symbol(self.graph.vertex(vid)))
+            ])
+            for path in all_paths(self.graph, start_vertex, target_vertex)
+        ])
+
     def save_to_dot(self, file_name: str) -> None:
         """
         Saves the graph as a DOT digraph that can be, e.g., exported to a PNG file
         using :code:`dot -Tpng dot_file_name.dot -o out.png`. If the given file name
         does not end in :code:`.dot`, this ending is appended to the file name.
 
         >>> import string
```

### Comparing `neo_grammar_graph-0.0.3/src/neo_grammar_graph.egg-info/PKG-INFO` & `neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-grammar-graph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -708,15 +708,15 @@
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
 * Reachability of grammar symbols.
-* Computing shortest paths between grammar symbols.
+* Computing the shortest path or all paths between two grammar symbols.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
 * Creating sub graphs
 * Filter abstraction
 * Checking whether a (sub) graph represents a tree
```

