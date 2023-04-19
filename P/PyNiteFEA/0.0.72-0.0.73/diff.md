# Comparing `tmp/PyNiteFEA-0.0.72.tar.gz` & `tmp/PyNiteFEA-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.72.tar", last modified: Tue Apr 11 00:38:16 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.73.tar", last modified: Wed Apr 19 15:07:44 2023, max compression
```

## Comparing `PyNiteFEA-0.0.72.tar` & `PyNiteFEA-0.0.73.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   152209 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    66665 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152624 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66986 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/setup.py
```

### Comparing `PyNiteFEA-0.0.72/LICENSE` & `PyNiteFEA-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PKG-INFO` & `PyNiteFEA-0.0.73/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.72
+Version: 0.0.73
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.73
+* Bug fix for merging duplicated plate names when using models with multiple meshes.
+
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
 
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
```

### Comparing `PyNiteFEA-0.0.72/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.73/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.73/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.73/PyNite/FEModel3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # %%
 from os import rename
 import warnings
+from math import isclose
+
 from matplotlib.pyplot import get
 
 from numpy import array, zeros, matmul, divide, subtract, atleast_2d, nanmax
 from numpy import seterr
 from numpy.linalg import solve
 
 from PyNite.Node3D import Node3D
@@ -737,17 +739,14 @@
 
         Returns
         -------
         remove_list : list
             A list of th enames of the nodes that were removed.
         """
 
-        # Initialize a list of nodes to be removed from the `Nodes` dictionary
-        node_remove_list = []
-
         # Initialize a dictionary marking where each node is used
         node_lookup = {node_name: [] for node_name in self.Nodes.keys()}
         element_dicts = ('Springs', 'Members', 'Plates', 'Quads')
         node_types = ('i_node', 'j_node', 'm_node', 'n_node')
 
         # Step through each dictionary of elements in the model (springs, members, plates, quads)
         for element_dict in element_dicts:
@@ -763,80 +762,87 @@
                     node = getattr(element, node_type, None)
 
                     # Determine if the node exists on the element
                     if node is not None:
                         # Add the element to the list of elements attached to the node
                         node_lookup[node.name].append((element, node_type))
 
-        # Make a copy of the `Nodes` dictionary
-        temp = list(self.Nodes.values())
+        # Make a list of the names of each node in the model
+        node_names = list(self.Nodes.keys())
+
+        # Make a list of nodes to be removed from the model
+        remove_list = []
 
         # Step through each node in the copy of the `Nodes` dictionary
-        for i, node_1 in enumerate(temp):
+        for i, node_1_name in enumerate(node_names):
 
             # Skip iteration if `node_1` has already been removed
-            if node_lookup[node_1.name] is None:
+            if node_lookup[node_1_name] is None:
                 continue
 
             # There is no need to check `node_1` against itself
-            for node_2 in temp[i + 1:]:
+            for node_2_name in node_names[i + 1:]:
 
                 # Skip iteration if node_2 has already been removed
-                if node_lookup[node_2.name] is None:
+                if node_lookup[node_2_name] is None:
                     continue
 
                 # Calculate the distance between nodes
-                if self.Nodes[node_1.name].distance(self.Nodes[node_2.name]) > tolerance:
+                if self.Nodes[node_1_name].distance(self.Nodes[node_2_name]) > tolerance:
                     continue
 
                 # Replace references to `node_2` in each element with references to `node_1`
-                for element, node_type in node_lookup[node_2.name]:
-                    setattr(element, node_type, node_1)
-
-                # Replace references to `node_2` in each mesh with references to `node_1`
-                for mesh in self.Meshes.values():
-
-                    if node_2.name in mesh.nodes.keys():
-                        mesh.nodes[node_2.name] = node_1
-
-                    for element in mesh.elements.values():
-                        if element.i_node is node_2: element.i_node = node_1
-                        if element.j_node is node_2: element.j_node = node_1
-                        if element.m_node is node_2: element.m_node = node_1
-                        if element.n_node is node_2: element.n_node = node_1
+                for element, node_type in node_lookup[node_2_name]:
+                    setattr(element, node_type, self.Nodes[node_1_name])
 
-                # Mark `node_2` for removal from the `Nodes` dictionary
-                node_remove_list.append(node_2.name)
-
-                # Flag `node_2` as not used
-                node_lookup[node_2.name] = None
+                # Flag `node_2` as no longer used
+                node_lookup[node_2_name] = None
 
                 # Merge any boundary conditions
                 support_cond = ('support_DX', 'support_DY', 'support_DZ', 'support_RX', 'support_RY', 'support_RZ')
                 for dof in support_cond:
-                    if getattr(node_2, dof) == True:
-                        setattr(node_1, dof, True)
+                    if getattr(self.Nodes[node_2_name], dof) == True:
+                        setattr(self.Nodes[node_1_name], dof, True)
                 
                 # Merge any spring supports
                 spring_cond = ('spring_DX', 'spring_DY', 'spring_DZ', 'spring_RX', 'spring_RY', 'spring_RZ')
                 for dof in spring_cond:
-                    value = getattr(node_2, dof)
+                    value = getattr(self.Nodes[node_2_name], dof)
                     if value != [None, None, None]:
-                        setattr(node_1, dof, value)
+                        setattr(self.Nodes[node_1_name], dof, value)
+                
+                # Fix the mesh labels
+                for mesh in self.Meshes.values():
+
+                    # Fix the nodes in the mesh
+                    if node_2_name in mesh.nodes.keys():
 
-        # Delete the duplicate nodes from the model
-        for name in node_remove_list:
-            self.Nodes.pop(name)
+                        # Attach the correct node to the mesh
+                        mesh.nodes[node_2_name] = self.Nodes[node_1_name]
+
+                        # Fix the dictionary key
+                        mesh.nodes[node_1_name] = mesh.nodes.pop(node_2_name)
+
+                    # Fix the elements in the mesh
+                    for element in mesh.elements.values():
+                        if node_2_name == element.i_node.name: element.i_node = self.Nodes[node_1_name]
+                        if node_2_name == element.j_node.name: element.j_node = self.Nodes[node_1_name]
+                        if node_2_name == element.m_node.name: element.m_node = self.Nodes[node_1_name]
+                        if node_2_name == element.n_node.name: element.n_node = self.Nodes[node_1_name]
+                    
+                # Add the node to the `remove` list
+                remove_list.append(node_2_name)
+
+        # Remove `node_2` from the model's `Nodes` dictionary
+        for node_name in remove_list:
+            self.Nodes.pop(node_name)
         
         # Flag the model as unsolved
         self.solution = None
 
-        # Return a list of the names of nodes that were removed from the model
-        return node_remove_list
-
     def delete_node(self, node_name):
         '''
         Removes a node from the model. All nodal loads associated with the
         node and elements attached to the node will also be removed.
         
         Parameters
         ----------
@@ -3074,29 +3080,29 @@
                 supported = node.support_RX
             elif dof == 4:
                 supported = node.support_RY
             elif dof == 5:
                 supported = node.support_RZ
 
             # Check if the degree of freedom on this diagonal is unstable
-            if K[i, i] == 0 and not supported:
+            if isclose(K[i, i], 0) and not supported:
 
                 # Flag the model as unstable
                 unstable = True
 
                 # Identify which direction this instability effects
                 if i%6 == 0: direction = 'for translation in the global X direction.'
                 if i%6 == 1: direction = 'for translation in the global Y direction.'
                 if i%6 == 2: direction = 'for translation in the global Z direction.'
                 if i%6 == 3: direction = 'for rotation about the global X axis.'
                 if i%6 == 4: direction = 'for rotation about the global Y axis.'
                 if i%6 == 5: direction = 'for rotation about the global Z axis.'
 
                 # Print a message to the console
-                print('* Nodal instability detected: node' + node.name + 'is unstable for' + direction)
+                print('* Nodal instability detected: node ' + node.name + ' is unstable ' + direction)
 
         if unstable:
             raise Exception('Unstable node(s). See console output for details.')
 
         return
     
     def _check_statics(self):
@@ -3224,15 +3230,15 @@
         :type prefix: str
         :return: A unique name for the dictionary.
         :rtype: str
         """
 
         # Select a trial value for the next available name
         name = prefix + str(len(dictionary) + 1)
-        i = 1
+        i = 2
         while name in dictionary.keys():
             name = prefix + str(len(dictionary) + i)
             i += 1
         
         # Return the next available name
         return name
```

### Comparing `PyNiteFEA-0.0.72/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.73/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/LoadCombo.py` & `PyNiteFEA-0.0.73/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.73/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Member3D.py` & `PyNiteFEA-0.0.73/PyNite/Member3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Mesh.py` & `PyNiteFEA-0.0.73/PyNite/Mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,41 +42,47 @@
 
             # Check if this node name is already being used in the model's `Nodes` dictionary
             if node.name in self.model.Nodes.keys():
 
                 # Come up with a new node name
                 node.name = self.model.unique_name(self.model.Nodes, 'N')
             
-            # Save the element to the model
+            # Save the node to the model
             self.model.Nodes[node.name] = node
 
-            # Prepare to save the element to the mesh
+            # Add this node to the mesh's new/replacement `nodes` dictionary
             revised_nodes[node.name] = node
             
         # Step through each element in the mesh
         for element in self.elements.values():
 
-            # Check if this element name is already being used in the model's `Plates` dictionary
-            if element.name in self.model.Plates.keys():
+            # Check which type of element this is
+            if element.type == 'Rect':
+
+                # Check if this element name is already being used in the model's `Plates` dictionary
+                if element.name in self.model.Plates.keys():
 
-                # Come up with a new element name
-                element.name = self.model.unique_name(self.model.Plates, 'R')
+                    # Come up with a new element name
+                    element.name = self.model.unique_name(self.model.Plates, 'R')
 
                 # Save the element to the model
                 self.model.Plates[element.name] = element
 
-            # Check if this element name is already being used in the model's `Quads` dictionary
-            elif element.name in self.model.Quads.keys():
+            elif element.type == 'Quad':
+
+                # Check if this element name is already being used in the model's `Quads` dictionary
+                if element.name in self.model.Quads.keys():
 
-                # Come up with a new element name
-                element.name = self.model.unique_name(self.model.Quads, prefix='Q')
+                    # Come up with a new element name
+                    element.name = self.model.unique_name(self.model.Quads, prefix='Q')
 
                 # Save the element to the model
                 self.model.Quads[element.name] = element
             
+            # Add this element to the mesh's new/replacement `elements` dictionary
             revised_elements[element.name] = element
         
         # Replace the old dictionaries of nodes and elements with the revised dictionaries
         self.nodes = revised_nodes
         self.elements = revised_elements
             
     def generate(self):
@@ -642,37 +648,28 @@
         for node_name in node_del_list:
             del self.nodes[node_name]
 
         # Identify the last node and last element in the mesh
         self.last_node = list(self.nodes.values())[-1]
         self.last_element = list(self.elements.values())[-1]
 
-        print(' ')
-        print('Mesh Check Before Renaming:')
-        print('***************************')
-        print(check_mesh_integrity(self))
-
         # At this point we have a mesh, but some of the element or node names may already be
         # being used in the model. Rename any names that are already being used.
         self._rename_duplicates()
 
         # Add the nodes to the model
         for key, node in self.nodes.items():
             self.model.Nodes[key] = node
         
         # Add the elements to the model
         for key, element in self.elements.items():
             if element.type == 'Quad':
                 self.model.Quads[key] = element
             elif element.type == 'Rect':
                 self.model.Plates[key] = element
-        
-        print('Mesh Check After Renaming:')
-        print('**************************')
-        print(check_mesh_integrity(self))
 
         # Flag the mesh as generated
         self._is_generated = True
 
     def node_local_coords(self, node):
         """
         Calculates a node's position in the mesh's local coordinate system
@@ -1599,24 +1596,33 @@
             if element.name not in mesh.model.Quads.keys() or mesh.elements[element.name] is not mesh.model.Quads[element.name]:
                 count += 1
     
     # Prepare the error message
     if count != 0:
         errors.append(str(count) + ' elements in the mesh do not match their respective elements in the model.')
     
-    # Check that each node in the mesh matches its corresponding node in the model
+    # Check that the mesh's key for each node matches the node's name
     count = 0
     for node in mesh.nodes.values():
-
-        if node.name not in mesh.model.Nodes.keys() or mesh.nodes[node.name] is not mesh.model.Nodes[node.name]:
+        if node.name not in mesh.nodes.keys():
             count += 1
     
-    # Prepare the error message
     if count != 0:
-        errors.append(str(count) + ' nodes in the mesh do not match their respective nodes in the model.')
+        errors.append(str(count) + ' node names in the mesh do not match the mesh\'s `nodes` dictionary\'s keys.')
+
+    # # Check that each node in the mesh matches its corresponding node in the model
+    # count = 0
+    # for node in mesh.nodes.values():
+
+    #     if node.name not in mesh.model.Nodes.keys() or mesh.nodes[node.name] is not mesh.model.Nodes[node.name]:
+    #         count += 1
+    
+    # # Prepare the error message
+    # if count != 0:
+    #     errors.append(str(count) + ' nodes in the mesh do not match their respective nodes in the model.')
 
     # TODO: Add more integrity checks and error messages
 
     # Report if no errors were found
     if errors == []:
         errors = ['No errors detected.']
```

### Comparing `PyNiteFEA-0.0.72/PyNite/Node3D.py` & `PyNiteFEA-0.0.73/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/PhysMember.py` & `PyNiteFEA-0.0.73/PyNite/PhysMember.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Plate3D.py` & `PyNiteFEA-0.0.73/PyNite/Plate3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Quad3D.py` & `PyNiteFEA-0.0.73/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Report_Template.html` & `PyNiteFEA-0.0.73/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Reporting.py` & `PyNiteFEA-0.0.73/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Spring3D.py` & `PyNiteFEA-0.0.73/PyNite/Spring3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNite/Visualization.py` & `PyNiteFEA-0.0.73/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.73/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.72
+Version: 0.0.73
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.73
+* Bug fix for merging duplicated plate names when using models with multiple meshes.
+
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
 
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
```

### Comparing `PyNiteFEA-0.0.72/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.73/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.72/README.md` & `PyNiteFEA-0.0.73/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.73
+* Bug fix for merging duplicated plate names when using models with multiple meshes.
+
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
 
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
```

### Comparing `PyNiteFEA-0.0.72/setup.py` & `PyNiteFEA-0.0.73/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.72",
+    version="0.0.73",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
```

