# Comparing `tmp/pycallflow-0.1.0.tar.gz` & `tmp/pycallflow-0.2.0.tar.gz`

## Comparing `pycallflow-0.1.0.tar` & `pycallflow-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pycallflow-0.1.0/.gitattributes
--rw-r--r--   0        0        0    48861 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/calls_combined.png
--rw-r--r--   0        0        0    89752 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/class_reference.png
--rw-r--r--   0        0        0    56885 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/multi_calls.png
--rw-r--r--   0        0        0    69613 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/no_class_reference.png
--rw-r--r--   0        0        0   495226 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/no_recurse.png
--rw-r--r--   0        0        0    48986 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/no_recursion.png
--rw-r--r--   0        0        0   508641 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/pycallflow-full.png
--rw-r--r--   0        0        0   109121 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/recursion.png
--rw-r--r--   0        0        0    51013 2020-02-02 00:00:00.000000 pycallflow-0.1.0/images/select_entities.png
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/__about__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/__main__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/analyzeCallFlow.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/buildDeclaredEntitiesDB.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/buildFileDB.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/callFlowData.py
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/callflow.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/cflow_importlib.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/finalResults.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pycallflow/output.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pycallflow-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pycallflow-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pycallflow-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 pycallflow-0.1.0/README.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pycallflow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 pycallflow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pycallflow-0.2.0/.gitattributes
+-rw-r--r--   0        0        0    48861 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/calls_combined.png
+-rw-r--r--   0        0        0    89752 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/class_reference.png
+-rw-r--r--   0        0        0    56885 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/multi_calls.png
+-rw-r--r--   0        0        0    69613 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/no_class_reference.png
+-rw-r--r--   0        0        0   495226 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/no_recurse.png
+-rw-r--r--   0        0        0    48986 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/no_recursion.png
+-rw-r--r--   0        0        0   508641 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/pycallflow-full.png
+-rw-r--r--   0        0        0   109121 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/recursion.png
+-rw-r--r--   0        0        0    51013 2020-02-02 00:00:00.000000 pycallflow-0.2.0/images/select_entities.png
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/__about__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/__main__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/analyzeCallFlow.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/buildDeclaredEntitiesDB.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/buildFileDB.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/callFlowData.py
+-rw-r--r--   0        0        0     8156 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/callflow.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/cflow_importlib.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/finalResults.py
+-rw-r--r--   0        0        0    10208 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pycallflow/output.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pycallflow-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pycallflow-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pycallflow-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 pycallflow-0.2.0/README.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pycallflow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 pycallflow-0.2.0/PKG-INFO
```

### Comparing `pycallflow-0.1.0/images/calls_combined.png` & `pycallflow-0.2.0/images/calls_combined.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/class_reference.png` & `pycallflow-0.2.0/images/class_reference.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/multi_calls.png` & `pycallflow-0.2.0/images/multi_calls.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/no_class_reference.png` & `pycallflow-0.2.0/images/no_class_reference.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/no_recurse.png` & `pycallflow-0.2.0/images/no_recurse.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/no_recursion.png` & `pycallflow-0.2.0/images/no_recursion.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/pycallflow-full.png` & `pycallflow-0.2.0/images/pycallflow-full.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/recursion.png` & `pycallflow-0.2.0/images/recursion.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/images/select_entities.png` & `pycallflow-0.2.0/images/select_entities.png`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/analyzeCallFlow.py` & `pycallflow-0.2.0/pycallflow/analyzeCallFlow.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/buildDeclaredEntitiesDB.py` & `pycallflow-0.2.0/pycallflow/buildDeclaredEntitiesDB.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/buildFileDB.py` & `pycallflow-0.2.0/pycallflow/buildFileDB.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/callFlowData.py` & `pycallflow-0.2.0/pycallflow/callFlowData.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/callflow.py` & `pycallflow-0.2.0/pycallflow/callflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from contextlib import closing, redirect_stdout
 import argparse
 import importlib
 from pprint import pprint
 import sys
 import os
+import traceback
 
 from .callFlowData import callFlowData
 from .buildFileDB import buildFileDB
 from .buildDeclaredEntitiesDB import findDeclaredEntities_inlineSave
 from .analyzeCallFlow import buildCallflowDB
 from .finalResults import generateFinalResults_object, generateEntityResults_selectID_object, getEntityList
-from .output import simpleTextOutput, pydot_output, entity_list_output
+from .output import simpleTextOutput, pydot_output, entity_list_output, all_entity_flow
 
     
 def cli_run():
     version = "0.1.0"
     #  Arguments
     description = f"pycallflow v{version}: "
     description += "Maps call flows in python packages, modules, and directories"
     parser = argparse.ArgumentParser(
         description=description, prog="pycallflow")
     parser.add_argument(
         "target", help="Package or module name to attempt to map")
     parser.add_argument("-d", "--directory", action="store_true",
                         help="Consider the 'target' argument a directory, not a package")
-    parser.add_argument("-o", "--output", choices=["dot", "simple", "entity_list"], type=str, default="dot",
-                        help="Choose output type.  'dot' will produce dot-compatible drawing output. 'entity_list' provides table of discovered entity names for use in --select_entity_id.")
+    parser.add_argument("-o", "--output", choices=["dot", "simple", "entity_list", "entity_flow_graphs"], type=str, default="dot",
+                        help="Choose output type.  'dot' will produce dot-compatible drawing output. 'entity_list' provides table of discovered entity names for use in --select_entity_id. 'entity_flow_graphs' will make pycallflow generate a --clean callflow for every function and method entity found (__init__ and __del__ are ignored).  Files will be named by their 'import path' and 'name' and are stored as defined by --save_images_to.  This assumes graphviz is working on your system.  Images are pngs.")
     parser.add_argument("--rankdir", type=str, choices=[
                         "TB", "BT", "RL", "LR"], default="LR", help="See Graphviz documentation")
     parser.add_argument("--edge_color", type=str, default="rotate",
                         help="Use an X11 color scheme name or 'rotate' to rotate through X11 colors")
     parser.add_argument("--suppress_recursive_calls", action="store_true", help="Hides edges for entities that call themselves")
     parser.add_argument("--combine_calls", action="store_true", help="Will only show one directed edge between two entities, regardless of actual number of calls")
     parser.add_argument("--suppress_class_references", action="store_true", help="Will suppress explicit edges representing references to a class (method calls will remain)")
@@ -37,14 +38,15 @@
     parser.add_argument("--db_file", type=str, default=":memory:", help="pycallflow uses an in memory sqlite3 database normally, specify another filename here if you want it stored to disk for your future analysis.")
     parser.add_argument("--stdout_capture_file", type=str, default=os.devnull, help="Since the examined code is actually imported any code not protected with a __main__ clause will run. Stdout is normally redirected to os.devnull to prevent output corruption.  Specify another filename if you would like to capture the output from the analyzed code.")
     parser.add_argument("--select_entity_id", type=str, default=None,
                         help="Comma separated list of specific entity ID numbers to trace.  Use -oentity_list to get the entity ID.  The entity ID will remain constant if there are no changes to the files or added files.")
     parser.add_argument("--suppress_calls_to_init", action="store_true", help="Will not show calls going to __init__ functions.  These can be very noisy if a superclass has many subclasses.")
     parser.add_argument("--clean", action="store_true", help="Will set all graph simplification options to true")
     parser.add_argument("--match_to_file", action="store_true", help="Ambiguous calls happen if there are multiple entities with the same name in seprate files.  Setting this flag will make pycallflow choose calls from the same file, if they exist")
+    parser.add_argument("--save_images_to", type=str, default="images", help="Set this to the directory you want -o entity_flow_graphs to save the images")
     ### Not implemented
     # parser.add_argument("--highlight_orphans", action="store_true", help="Will highlight entities that are never called (possible dead code).  Only does anything in with 'dot' output")
     
     args = parser.parse_args()
 
     # Make copy of args for future mod:
     args_cp = vars(args).copy()
@@ -61,14 +63,29 @@
     with cf_data.getSqliteConnection() as conn:
         if args.output == "entity_list":
             results = getEntityList(conn)
             entity_list_output(results)
         elif args.output == "dot":
             results = generateEntityResults_selectID_object(conn, select_entity_id=args.select_entity_id)
             pydot_output().output(results, **args_cp)
+        elif args.output == "entity_flow_graphs":
+            try:
+                aef = all_entity_flow(args.save_images_to)
+                aef.generate_all_entity_flows(conn, **args_cp)
+            except FileNotFoundError:
+                
+                print("'entity_flow_graphs' mode requires Graphviz and dot to be installed and on the system path")
+                return
+            except NotADirectoryError:
+                print(f"The {args.save_images_to} directory does not exist, please create it and try again")
+                return
+            except Exception as badnews:
+                # traceback.print_exc()
+                print(f"Unable to complete processing because {badnews}")
+                return
         else:
             results = generateFinalResults_object(conn)
             simpleTextOutput(results)
 
 def collectData( # See argparse list in cli_run()
     target,
     directory = False,
```

### Comparing `pycallflow-0.1.0/pycallflow/cflow_importlib.py` & `pycallflow-0.2.0/pycallflow/cflow_importlib.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/finalResults.py` & `pycallflow-0.2.0/pycallflow/finalResults.py`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pycallflow/output.py` & `pycallflow-0.2.0/pycallflow/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 
 import networkx as nx
 import pydot
 from collections import deque
 from tabulate import tabulate
 import sys
+import subprocess
+import os.path
+import os
+import traceback
+
+from .finalResults import generateEntityResults_selectID_object, getEntityList
 
 from pprint import pprint
 
 def simpleTextOutput(finalOutputDataObject):
     for n, (k, v) in enumerate(finalOutputDataObject.items()):
         print(f"Module: {k}")
         print(f"({v['file_full_path']})")
@@ -60,14 +66,15 @@
         edge_color,
         suppress_recursive_calls,
         combine_calls,
         suppress_class_references,
         suppress_calls_to_init,
         select_entity_id = None,
         graph_name = "Callflow Analysis",
+        output_to_stdout = True,
         **kwargs
     ):
         graph = pydot.Graph(graph_name, compound=True, rankdir=rankdir)
         file_clusters = {}
         class_clusters = {}
         select_entity_id_list = []
         if select_entity_id is not None:
@@ -153,15 +160,18 @@
                         if finalOutputDataObject[to_id]["entity_type"] == "class":
                             # don't draw it
                             continue
                     to_node = finalOutputDataObject[to_id]["node"]
                     graph.add_edge(pydot.Edge(from_node, to_node, style=style, color=color))
                     edge_list.append(edge_id)
 
-        print(graph.to_string())
+        if output_to_stdout:
+            print(graph.to_string())
+        else:
+            return graph.to_string()
 
     def init_x11_colors(self):
         self.x11_colors_d = deque([
             'aquamarine',
             'antiquewhite4',
             'aquamarine3',
             'azure3',
@@ -194,13 +204,56 @@
         ])
 
     def next_X11_color(self):
         color = self.x11_colors_d[0]
         self.x11_colors_d.rotate(1)
         return color
 
+class all_entity_flow:
+
+    def __init__(self, save_images_to) -> None:
+        # Need to test for DOT working
+        try:
+            sp_run_result = subprocess.run(["dot", "--version"], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        except Exception:
+            # traceback.print_exc()
+            raise FileNotFoundError()
+        # Also check to see if the save directory exists
+        if not os.path.isdir(save_images_to):
+            raise NotADirectoryError()
+        else:
+            self.save_images_to = save_images_to
+
+
+    def generate_all_entity_flows(self, db_conn, 
+                                  **kwargs):
+        # Iterate over the entities and create single entity call flows
+        entity_list = getEntityList(db_conn)
+        for entity in entity_list:
+            try:
+                if entity["name"] in ["__init__", "__del__"]:
+                    continue
+                if entity["entity_type"] in ["class"]:
+                    continue
+                import_path = entity["file_import_path"].replace(".","_")
+                filename = f"{self.save_images_to}/{import_path}_{entity['name']}.png"
+                # Generate the dot data
+                # Convert entityID to string because the next call will attempt to split(",") on it
+                kwargs["select_entity_id"] = str(entity["entityID"])
+                this_entity_object = generateEntityResults_selectID_object(db_conn, select_entity_id=kwargs["select_entity_id"])
+                dot_data = pydot_output().output(this_entity_object, output_to_stdout=False,  **kwargs)
+                args = [
+                    "dot",
+                    "-Tpng",
+                    f"-o{filename}"
+                ]
+                p = subprocess.run(args=args, input=dot_data, text=True, capture_output=True)
+            except Exception as badnews:
+                print(f"Unable to make flow graph for {entity['name']} because {badnews}")
+
 
+
```

### Comparing `pycallflow-0.1.0/.gitignore` & `pycallflow-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/LICENSE.txt` & `pycallflow-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/README.md` & `pycallflow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/pyproject.toml` & `pycallflow-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycallflow-0.1.0/PKG-INFO` & `pycallflow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycallflow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Maps function, class, and method calls in python projects, modules, and files
 Project-URL: Documentation, https://github.com/richmr/pycallflow#readme
 Project-URL: Issues, https://github.com/richmr/pycallflow/issues
 Project-URL: Source, https://github.com/richmr/pycallflow
 Author-email: Michael Rich <richmr2174@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

