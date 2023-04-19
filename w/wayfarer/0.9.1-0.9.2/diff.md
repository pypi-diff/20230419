# Comparing `tmp/wayfarer-0.9.1.tar.gz` & `tmp/wayfarer-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wayfarer-0.9.1.tar", last modified: Fri Mar 31 08:09:21 2023, max compression
+gzip compressed data, was "wayfarer-0.9.2.tar", last modified: Wed Apr 19 14:31:42 2023, max compression
```

## Comparing `wayfarer-0.9.1.tar` & `wayfarer-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:09:21.318369 wayfarer-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-31 08:08:16.000000 wayfarer-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 08:09:21.318369 wayfarer-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-31 08:08:16.000000 wayfarer-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 08:09:21.318369 wayfarer-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-31 08:08:16.000000 wayfarer-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:09:21.314369 wayfarer-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_linearref.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_routing_ordered_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-03-31 08:08:16.000000 wayfarer-0.9.1/tests/test_splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:09:21.314369 wayfarer-0.9.1/wayfarer/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/linearref.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-31 08:08:16.000000 wayfarer-0.9.1/wayfarer/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:09:21.318369 wayfarer-0.9.1/wayfarer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 08:09:21.000000 wayfarer-0.9.1/wayfarer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-31 08:09:21.000000 wayfarer-0.9.1/wayfarer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:09:21.000000 wayfarer-0.9.1/wayfarer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:08:50.000000 wayfarer-0.9.1/wayfarer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 08:09:21.000000 wayfarer-0.9.1/wayfarer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 08:09:21.000000 wayfarer-0.9.1/wayfarer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:31:42.781298 wayfarer-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-19 14:30:31.000000 wayfarer-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 14:31:42.781298 wayfarer-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-19 14:30:31.000000 wayfarer-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:31:42.781298 wayfarer-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 14:30:32.000000 wayfarer-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:31:42.777298 wayfarer-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_linearref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_routing_ordered_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-19 14:30:32.000000 wayfarer-0.9.2/tests/test_splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:31:42.781298 wayfarer-0.9.2/wayfarer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/linearref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-19 14:30:32.000000 wayfarer-0.9.2/wayfarer/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:31:42.781298 wayfarer-0.9.2/wayfarer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 14:31:42.000000 wayfarer-0.9.2/wayfarer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 14:31:42.000000 wayfarer-0.9.2/wayfarer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:31:42.000000 wayfarer-0.9.2/wayfarer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:31:12.000000 wayfarer-0.9.2/wayfarer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 14:31:42.000000 wayfarer-0.9.2/wayfarer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 14:31:42.000000 wayfarer-0.9.2/wayfarer.egg-info/top_level.txt
```

### Comparing `wayfarer-0.9.1/LICENSE` & `wayfarer-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/PKG-INFO` & `wayfarer-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.1/README.rst` & `wayfarer-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/setup.py` & `wayfarer-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_functions.py` & `wayfarer-0.9.2/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def test_get_multiple_edges_by_attribute():
     net = networkx.MultiGraph()
 
     net.add_edge(0, 0, key=1, **{"EDGE_ID": 1, "LEN_": 100})
     net.add_edge(0, 0, key=2, **{"EDGE_ID": 1, "LEN_": 100})
 
-    edges = list(functions.get_edge_by_attribute(net, "EDGE_ID", 1))
+    edges = list(functions.get_edges_by_attribute(net, "EDGE_ID", 1))
     assert edges == [
         (0, 0, 1, {"EDGE_ID": 1, "LEN_": 100}),
         (0, 0, 2, {"EDGE_ID": 1, "LEN_": 100}),
     ]
 
 
 def test_get_single_path_from_nodes():
@@ -400,36 +400,45 @@
 
 def test_get_path_length():
     edges = [Edge(0, 1, "A", {"LEN_": 5}), Edge(1, 2, "B", {"LEN_": 5})]
     assert functions.get_path_length(edges) == 10
 
 
 def test_has_overlaps():
-
     edges = [
         Edge(0, 1, "A", {"EDGE_ID": 1}),
         Edge(1, 2, "B", {"EDGE_ID": 2}),
         Edge(2, 3, "C", {"EDGE_ID": 3}),
         Edge(2, 3, "C", {"EDGE_ID": 2}),
         Edge(2, 3, "C", {"EDGE_ID": 4}),
     ]
     assert functions.has_overlaps(edges) is True
 
 
 def test_has_no_overlaps():
-
     edges = [
         Edge(0, 1, "A", {"EDGE_ID": 1}),
         Edge(1, 2, "B", {"EDGE_ID": 2}),
         Edge(2, 3, "C", {"EDGE_ID": 3}),
         Edge(2, 3, "C", {"EDGE_ID": 4}),
     ]
     assert functions.has_overlaps(edges) is False
 
 
+def test_has_no_overlaps_loop():
+    edges = [
+        Edge(0, 1, "A", {"EDGE_ID": 1}),
+        Edge(1, 2, "B", {"EDGE_ID": 2}),
+        Edge(2, 3, "C", {"EDGE_ID": 3}),
+        Edge(0, 1, "D", {"EDGE_ID": 1}),
+    ]
+
+    assert functions.has_overlaps(edges) is False
+
+
 def test_doctest():
     import doctest
 
     print(doctest.testmod(functions))
 
 
 if __name__ == "__main__":
@@ -446,9 +455,10 @@
     # test_to_edge_no_attributes()
     # test_edges_to_graph_no_keys()
     # test_get_edge_by_key_missing()
     # test_get_all_paths_from_nodes_with_direction()
     # test_get_path_length()
     # test_doctest()
     # test_get_edges_from_nodes_non_unique()
-    test_has_no_overlaps()
+    # test_has_no_overlaps()
+    test_has_no_overlaps_loop()
     print("Done!")
```

### Comparing `wayfarer-0.9.1/tests/test_linearref.py` & `wayfarer-0.9.2/tests/test_linearref.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_loader.py` & `wayfarer-0.9.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_loops.py` & `wayfarer-0.9.2/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_osmnx_compat.py` & `wayfarer-0.9.2/tests/test_osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_routing.py` & `wayfarer-0.9.2/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_routing_ordered_path.py` & `wayfarer-0.9.2/tests/test_routing_ordered_path.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/tests/test_splitting.py` & `wayfarer-0.9.2/tests/test_splitting.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pytest
 from wayfarer import splitter, functions, loader, routing
 from tests.helper import simple_features
 
 
 @pytest.mark.parametrize("use_reverse_lookup", [(True), (False)])
 def test_split_network_edge(use_reverse_lookup):
-
     feats = simple_features()
     net = loader.load_network_from_geometries(
         feats, use_reverse_lookup=use_reverse_lookup
     )
 
     assert len(net.nodes()) == 4
     assert len(net.edges()) == 3
@@ -28,15 +27,15 @@
 
     # after the split operation there should be one extra edge
     # and one extra node
     assert len(net.nodes()) == 5
     assert len(net.edges()) == 4
 
     # the split edges no longer have the EdgeId as a key
-    split_edges = functions.get_edge_by_attribute(net, "EDGE_ID", edge_id_to_split)
+    split_edges = functions.get_edges_by_attribute(net, "EDGE_ID", edge_id_to_split)
     split_edges = list(split_edges)
     assert len(split_edges) == 2
 
     # if use_reverse_lookup: print(net.graph["keys"].keys())
 
     split_edge_id = splitter.create_split_key(edge_id_to_split, measure)
 
@@ -48,15 +47,14 @@
     split_edge = functions.get_edge_by_key(net, split_edge_id, with_data=True)
     assert split_edge.attributes["LEN_"] == 50
     assert split_edge.attributes["OFFSET"] == 50
 
 
 @pytest.mark.parametrize("use_reverse_lookup", [(True), (False)])
 def test_multiple_split_network_edge(use_reverse_lookup):
-
     feats = simple_features()
     net = loader.load_network_from_geometries(
         feats, use_reverse_lookup=use_reverse_lookup
     )
 
     # split the second edge multiple times
     edge_id_to_split = 2
@@ -94,15 +92,14 @@
 
     assert len(net.nodes()) == 8
     assert len(net.edges()) == 7
 
 
 @pytest.mark.parametrize("use_reverse_lookup", [(True), (False)])
 def test_split_invalid_measure(use_reverse_lookup):
-
     feats = simple_features()
     net = loader.load_network_from_geometries(
         feats, use_reverse_lookup=use_reverse_lookup
     )
     error = False
 
     try:
@@ -112,15 +109,14 @@
         error = True
 
     assert error
 
 
 @pytest.mark.parametrize("use_reverse_lookup", [(True), (False)])
 def test_split_invalid_measure2(use_reverse_lookup):
-
     feats = simple_features()
     net = loader.load_network_from_geometries(
         feats, use_reverse_lookup=use_reverse_lookup
     )
     error = False
 
     try:
@@ -130,15 +126,14 @@
         error = True
 
     assert error
 
 
 @pytest.mark.parametrize("use_reverse_lookup", [(True), (False)])
 def test_split_with_points(use_reverse_lookup):
-
     feats = simple_features()
     net = loader.load_network_from_geometries(
         feats, use_reverse_lookup=use_reverse_lookup
     )
 
     recs = [
         {"EDGE_ID": 1, "POINT_ID": "A", "MEASURE": 50, "LEN_": 12},
@@ -156,24 +151,65 @@
 
     # run a solve from start to finish across the original (now split) edges
     edges = routing.solve_shortest_path(net, "0|0", "300|0", with_direction_flag=True)
     # print(edges)
     assert len(edges) == 6
 
 
+def test_unsplit_network_edges():
+    """
+    Test splitting a network edge and then joining it back
+    together again
+    """
+    feats = simple_features()
+    net = loader.load_network_from_geometries(feats, use_reverse_lookup=True)
+
+    edge_id_to_split = 2
+
+    assert len((net.graph["keys"])) == 3
+    assert len(net.nodes()) == 4
+
+    original_edge = functions.get_edge_by_key(net, edge_id_to_split)
+    # custom fields should be persisted
+    original_edge.attributes["CUSTOM_FIELD"] = "CUSTOM_VALUE"
+    # print(original_edge)
+
+    # split the second edge multiple times
+
+    new_edges = splitter.split_network_edge(net, edge_id_to_split, [20, 40, 60])
+
+    assert len((net.graph["keys"])) == 6
+
+    for ne in new_edges:
+        print(ne)
+
+    network_edges = list(
+        functions.get_edges_by_attribute(net, "EDGE_ID", edge_id_to_split)
+    )
+    # for ne in network_edges: print(ne)
+
+    unsplit_edge = splitter.unsplit_network_edges(net, network_edges)
+
+    assert len((net.graph["keys"])) == 3
+
+    assert len(net.nodes()) == 4
+    assert unsplit_edge == original_edge
+
+
 def test_doctest():
     import doctest
 
     print(doctest.testmod(splitter))
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
     # test_multiple_split_network_edge(True)
     # test_split_invalid_measure(True)
     # test_split_invalid_measure2(True)
     # test_multiple_split_network_edge(True)
     # test_multiple_split_network_edge(True)
     # test_double_split_network_edge(True)
-    test_split_with_points(True)
-    test_split_network_edge(True)
+    # test_split_with_points(True)
+    # test_split_network_edge(True)
+    test_unsplit_network_edges()
     print("Done!")
```

### Comparing `wayfarer-0.9.1/wayfarer/__init__.py` & `wayfarer-0.9.2/wayfarer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 LENGTH_FIELD = "LEN_"
 EDGE_ID_FIELD = "EDGE_ID"
 OFFSET_FIELD = "OFFSET"
 
 NODEID_FROM_FIELD = "NODEID_FROM"
 NODEID_TO_FIELD = "NODEID_TO"
```

### Comparing `wayfarer-0.9.1/wayfarer/functions.py` & `wayfarer-0.9.2/wayfarer/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         start_node: The start node of the edge
         end_node: The end node of the edge
         key: The unique key of the edge
         attributes: Any attributes associated with the edge
 
     >>> net = networkx.MultiGraph()
     >>> add_edge(net, 1, 2, "A", {"LEN_": 10})
+    Edge(start_node=1, end_node=2, key='A', attributes={'LEN_': 10})
     >>> print(net)
     MultiGraph with 2 nodes and 1 edges
     """
     new_edge = Edge(start_node, end_node, key, attributes)
     net.add_edge(
         new_edge.start_node, new_edge.end_node, new_edge.key, **new_edge.attributes
     )
@@ -108,14 +109,25 @@
     if "keys" in net.graph.keys():
         # we are using a reverse lookup dict so update this also
         net.graph["keys"][key] = (start_node, end_node)
 
     return new_edge
 
 
+def remove_edge_by_key(
+    net: (networkx.MultiGraph | networkx.MultiDiGraph), key: (int | str)
+):
+    edge = get_edge_by_key(net, key, with_data=False)
+    net.remove_edge(edge.start_node, edge.end_node, key=edge.key)
+
+    # remove from the keys dictionary if it exists
+    if "keys" in net.graph.keys():
+        del net.graph["keys"][key]
+
+
 def get_edge_by_key(
     net: (networkx.MultiGraph | networkx.MultiDiGraph),
     key: (int | str),
     with_data: bool = True,
 ) -> Edge:
     """
     Go through all edge property dicts until the relevant key is found
@@ -152,24 +164,20 @@
         edge = Edge(u, v, key, atts)
     else:
         edge = Edge(u, v, key, {})
 
     return edge
 
 
-def get_edge_by_attribute(net, attribute_field: str, value) -> Iterable[Edge]:
+def get_edges_by_attribute(net, attribute_field: str, value) -> Iterable[Edge]:
     """
-    Go through all edge property dicts until the relevant attribute is found
-    Return an iterator
-    For getting data see
-    https://networkx.github.io/documentation/stable/reference/classes/generated/networkx.Graph.get_edge_data.html
-
-    TODO returns a generator so rename to get_edges_by_attribute or make this return the first instance?
-    If the attribute_field does not exist for a particular edge then it is ignored
-    Edges can have different attribute dicts
+    Go through all edge property dicts until the relevant attribute is found.
+    Edges can have different attribute dicts, so add a check that the key exists
+    If the attribute_field does not exist for a particular edge then it is ignored.
+    Returns an iterator
     """
 
     return (
         Edge(u, v, k, d)
         for u, v, k, d in net.edges(keys=True, data=True)
         if attribute_field in d and d[attribute_field] == value
     )
@@ -242,15 +250,14 @@
                     # there is an edge between the start and end of the path
                     # possible loop
                     extra_path = list(np)
                     extra_path.append(sn)
                     node_paths.append(extra_path)
 
     for node_path in node_paths:
-
         node_pairs = list(pairwise(node_path))
 
         path_list = []
         for u, v in node_pairs:  # loop through all pairs and get all edges between them
             node_edges = []
             edges = get_edges_from_node_pair(net, u, v)
 
@@ -274,21 +281,20 @@
         all_paths.append(combinatations)
 
     # return a flat list of paths
     return itertools.chain(*all_paths)
 
 
 def get_path_length(path_edges):
-
     return sum([edge.attributes[LENGTH_FIELD] for edge in path_edges])
 
 
 def get_edges_from_node_pair(
     net, start_node: (int | str), end_node: (int | str), hide_log_output: bool = False
-) -> (networkx.classes.coreviews.AtlasView | None):
+) -> networkx.classes.coreviews.AtlasView | None:
     """
     Get all edges between two nodes
 
     This function can return multiple edges when there is more than
     one edge between two nodes
 
     >>> net = networkx.MultiGraph()
```

### Comparing `wayfarer-0.9.1/wayfarer/io.py` & `wayfarer-0.9.2/wayfarer/io.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer/linearref.py` & `wayfarer-0.9.2/wayfarer/linearref.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     Returns:
         If the line is valid
 
     >>> check_valid_m(m_value=10, length=20)
     True
 
     >>> check_valid_m(m_value=-0.213, length=20)
-    False
+    Traceback (most recent call last):
+    ...
+    ValueError: The m value (-0.213) must be a positive number
     """
 
     if m_value < 0:
         raise ValueError(f"The m value ({m_value}) must be a positive number")
 
     if m_value > length + tolerance:
         raise ValueError(
@@ -179,16 +181,18 @@
         start_m: The start measure
         end_m: The end measure
         tolerance: The tolerance the m-value can be beyond the length of the line
     Returns:
         A tuple of the new snapped measures
 
     >>> ls = LineString([(0, 0), (0, 100)])
-    >>> snap_to_ends(ls, start_m=4, end_m=96, tolerance=3)
-    (0, 100)
+    >>> snap_to_ends(ls, start_m=4, end_m=96, tolerance=5)
+    (0, 100.0)
+    >>> snap_to_ends(ls, start_m=4, end_m=96, tolerance=4)
+    (4, 96)
     """
 
     check_valid_m(start_m, line.length, tolerance)
     check_valid_m(end_m, line.length, tolerance)
 
     if start_m > end_m:
         raise ValueError(
@@ -250,15 +254,15 @@
     Returns:
         A tuple of the start and end measures
 
     >>> ls = LineString([(0, 0), (100, 0)])
     >>> pt1 = Point(4, 0)
     >>> pt2 = Point(96, 0)
     >>> get_measures(ls, pt1, pt2)
-    (4, 96)
+    (4.0, 96.0)
     """
 
     m1 = line.project(pt1)
     m2 = line.project(pt2)
     start_m, end_m = sorted([m1, m2])
 
     return (start_m, end_m)
@@ -270,17 +274,18 @@
 
     Args:
         line: The LineString
         point: The point
     Returns:
         The measure (m-value) of the point along the line
 
-    >>> ls = LineString([(0, 0), (100, 0)])
-    >>> pt1 = Point(50, 0)
-    50
+    >>> line = LineString([(0, 0), (100, 0)])
+    >>> point = Point(50, 0)
+    >>> get_measure_on_line(line, point)
+    50.0
     """
     return line.project(point)
 
 
 def get_closest_point_to_measure(
     line: LineString, points: list[Point], measure: float
 ) -> Point:
@@ -294,17 +299,17 @@
         measure: A measure along the line
     Returns:
         The measure (m-value) of the point along the line
 
     >>> ls = LineString([(0, 0), (0, 50), (0, 100)])
     >>> points = [Point(0, 10), Point(0, 55)]
     >>> get_closest_point_to_measure(ls, points, measure=20)
-    POINT (0 10)
+    <POINT (0 10)>
     >>> get_closest_point_to_measure(ls, points, measure=80)
-    POINT (0 55)
+    <POINT (0 55)>
     """
     measures_with_points = {}
 
     for point in points:
         m = line.project(point)
         measures_with_points[m] = point
 
@@ -356,16 +361,16 @@
         pt1: The first point
         pt2: The second point
     Returns:
         The distance between the two points
 
     >>> pt1 = Point(0, 0)
     >>> pt2 = Point(100, 100)
-    >>> magnitude(pt1, pt2)
-    100.0
+    >>> round(magnitude(pt1, pt2))
+    141
     """
     vect_x = pt2.x - pt1.x
     vect_y = pt2.y - pt1.y
     return sqrt(vect_x**2 + vect_y**2)
 
 
 def remove_duplicates_in_line(line: LineString):
@@ -376,15 +381,15 @@
     Args:
         line: The LineString
     Returns:
         A new LineString with any duplicate coordinates removed
 
     >>> ls = LineString([(0, 0), (1, 1), (1,1)])
     >>> remove_duplicates_in_line(ls)
-    LineString([(0, 0), (1,1)])
+    <LINESTRING (0 0, 1 1)>
     """
 
     if line.geom_type != "LineString":
         raise NotImplementedError(f"Geometry type {line.geom_type} is not valid")
 
     clean_coords = [k for k, g in itertools.groupby(line.coords)]
     return LineString(clean_coords)
```

### Comparing `wayfarer-0.9.1/wayfarer/loader.py` & `wayfarer-0.9.2/wayfarer/loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer/loops.py` & `wayfarer-0.9.2/wayfarer/loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer/osmnx_compat.py` & `wayfarer-0.9.2/wayfarer/osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer/routing.py` & `wayfarer-0.9.2/wayfarer/routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer/validator.py` & `wayfarer-0.9.2/wayfarer/validator.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.1/wayfarer.egg-info/PKG-INFO` & `wayfarer-0.9.2/wayfarer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.1/wayfarer.egg-info/SOURCES.txt` & `wayfarer-0.9.2/wayfarer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

