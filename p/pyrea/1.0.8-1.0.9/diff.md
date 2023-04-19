# Comparing `tmp/pyrea-1.0.8.tar.gz` & `tmp/pyrea-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrea-1.0.8.tar", last modified: Wed Feb 22 10:59:00 2023, max compression
+gzip compressed data, was "pyrea-1.0.9.tar", last modified: Wed Feb 22 15:39:43 2023, max compression
```

## Comparing `pyrea-1.0.8.tar` & `pyrea-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 10:59:00.958140 pyrea-1.0.8/
--rw-rw-r--   0 mblo      (1000) mblo      (1000)     1103 2022-08-16 09:39:49.000000 pyrea-1.0.8/LICENSE
--rw-rw-r--   0 mblo      (1000) mblo      (1000)    12600 2023-02-22 10:59:00.954139 pyrea-1.0.8/PKG-INFO
--rw-rw-r--   0 mblo      (1000) mblo      (1000)    11375 2023-02-09 10:34:19.000000 pyrea-1.0.8/README.md
-drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 10:59:00.954139 pyrea-1.0.8/pyrea/
--rw-r--r--   0 mblo      (1000) mblo      (1000)       43 2023-02-22 10:55:35.000000 pyrea-1.0.8/pyrea/__init__.py
--rw-rw-r--   0 mblo      (1000) mblo      (1000)     1480 2023-02-01 09:43:41.000000 pyrea-1.0.8/pyrea/call_c.py
--rw-r--r--   0 mblo      (1000) mblo      (1000)    25997 2023-02-22 10:51:05.000000 pyrea-1.0.8/pyrea/core.py
--rw-r--r--   0 mblo      (1000) mblo      (1000)      791 2022-09-30 11:01:28.000000 pyrea-1.0.8/pyrea/debug.py
--rw-r--r--   0 mblo      (1000) mblo      (1000)    19534 2023-02-22 09:45:02.000000 pyrea-1.0.8/pyrea/structure.py
-drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 10:59:00.954139 pyrea-1.0.8/pyrea.egg-info/
--rw-r--r--   0 mblo      (1000) mblo      (1000)    12600 2023-02-22 10:59:00.000000 pyrea-1.0.8/pyrea.egg-info/PKG-INFO
--rw-r--r--   0 mblo      (1000) mblo      (1000)      252 2023-02-22 10:59:00.000000 pyrea-1.0.8/pyrea.egg-info/SOURCES.txt
--rw-rw-r--   0 mblo      (1000) mblo      (1000)        1 2023-02-22 10:59:00.000000 pyrea-1.0.8/pyrea.egg-info/dependency_links.txt
--rw-rw-r--   0 mblo      (1000) mblo      (1000)       68 2023-02-22 10:59:00.000000 pyrea-1.0.8/pyrea.egg-info/requires.txt
--rw-rw-r--   0 mblo      (1000) mblo      (1000)        6 2023-02-22 10:59:00.000000 pyrea-1.0.8/pyrea.egg-info/top_level.txt
--rw-rw-r--   0 mblo      (1000) mblo      (1000)       38 2023-02-22 10:59:00.958140 pyrea-1.0.8/setup.cfg
--rw-r--r--   0 mblo      (1000) mblo      (1000)     1790 2023-02-22 10:55:29.000000 pyrea-1.0.8/setup.py
+drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 15:39:43.222872 pyrea-1.0.9/
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)     1103 2022-08-16 09:39:49.000000 pyrea-1.0.9/LICENSE
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)    13327 2023-02-22 15:39:43.222872 pyrea-1.0.9/PKG-INFO
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)    12102 2023-02-22 15:33:05.000000 pyrea-1.0.9/README.md
+drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 15:39:43.218872 pyrea-1.0.9/pyrea/
+-rw-r--r--   0 mblo      (1000) mblo      (1000)       43 2023-02-22 15:37:07.000000 pyrea-1.0.9/pyrea/__init__.py
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)     1480 2023-02-01 09:43:41.000000 pyrea-1.0.9/pyrea/call_c.py
+-rw-r--r--   0 mblo      (1000) mblo      (1000)    28265 2023-02-22 15:35:36.000000 pyrea-1.0.9/pyrea/core.py
+-rw-r--r--   0 mblo      (1000) mblo      (1000)      791 2022-09-30 11:01:28.000000 pyrea-1.0.9/pyrea/debug.py
+-rw-r--r--   0 mblo      (1000) mblo      (1000)    19534 2023-02-22 09:45:02.000000 pyrea-1.0.9/pyrea/structure.py
+drwxrwxr-x   0 mblo      (1000) mblo      (1000)        0 2023-02-22 15:39:43.222872 pyrea-1.0.9/pyrea.egg-info/
+-rw-r--r--   0 mblo      (1000) mblo      (1000)    13327 2023-02-22 15:39:43.000000 pyrea-1.0.9/pyrea.egg-info/PKG-INFO
+-rw-r--r--   0 mblo      (1000) mblo      (1000)      252 2023-02-22 15:39:43.000000 pyrea-1.0.9/pyrea.egg-info/SOURCES.txt
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)        1 2023-02-22 15:39:43.000000 pyrea-1.0.9/pyrea.egg-info/dependency_links.txt
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)       68 2023-02-22 15:39:43.000000 pyrea-1.0.9/pyrea.egg-info/requires.txt
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)        6 2023-02-22 15:39:43.000000 pyrea-1.0.9/pyrea.egg-info/top_level.txt
+-rw-rw-r--   0 mblo      (1000) mblo      (1000)       38 2023-02-22 15:39:43.222872 pyrea-1.0.9/setup.cfg
+-rw-r--r--   0 mblo      (1000) mblo      (1000)     1790 2023-02-22 15:37:25.000000 pyrea-1.0.9/setup.py
```

### Comparing `pyrea-1.0.8/LICENSE` & `pyrea-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrea-1.0.8/PKG-INFO` & `pyrea-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrea
-Version: 1.0.8
+Version: 1.0.9
 Summary: Multi-view clustering with deep ensemble structures.
 Home-page: https://github.com/mdbloice/Pyrea
 Author: Marcus D. Bloice, Bastian Pfeifer
 Author-email: marcus.bloice@medunigraz.at
 License: MIT
 Keywords: multi-view,clustering,ensemble clustering
 Platform: UNKNOWN
@@ -49,19 +49,21 @@
 ```bash
 pip install pyrea
 ```
 
 This will install the latest version of Pyrea from PyPI.
 
 ## Usage
-The Pyrea software package is the accompanying software for our paper: *Parea: multi-view ensemble clustering for cancer subtype discovery*[^1].
+The Pyrea software package is the accompanying software for our paper:
+
+Pfeifer, B., Bloice, M.D., & Schimek, M.G. (2022). *Parea: multi-view ensemble clustering for cancer subtype discovery*. arXiv. <https://arxiv.org/abs/2209.15399>
 
 While Pyrea allows for flexible and custom architectures to be built, two structures are discussed specifically in the paper cited above, namely Parea 1 and Parea 2.
 
-Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows
+Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows:
 
 ```python
 import pyrea
 import numpy as np
 
 # Create sample data:
 d1 = np.random.rand(100,10)
@@ -71,15 +73,15 @@
 data = [d1,d2, d3]
 
 labels = pyrea.parea_2(data)
 ```
 
 which executes Parea 2.
 
-Default parameters are used which match those used in our experiments discussed in the paper above. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
+Default parameters are used which match those used in our experiments discussed in the paper[^1]. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
 
 ### Genetic Algorithm
 
 The Parea 1 and Parea 2 structures can be optimised using a genetic algorithm in order to find the best combinations of clustering methods, fusion methods, and number of clusters.
 
 For example, to find optimal parameters for Parea 2:
 
@@ -90,33 +92,71 @@
 
 d1 = datasets.load_iris().data
 d2 = datasets.load_iris().data
 d3 = datasets.load_iris().data
 
 data = [d1,d2,d3]
 
-params = pyrea.parea_2_genetic(data, max_k=5)
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5)
 ```
 
-where `max_k` refers to the maximum number of clusters to attempt for each layer.
+where `k_min` and `k_max` refer to the minimum and maximum number of clusters to attempt for each layer, respectively.
 
-Note that `params` contains the optimal parameters found by the genetic algorithm. To get the labels, run `parea_2()` using these parameters and your data:
+Note that `params` contains the optimal parameters found by the genetic algorithm:
+
+```python
+print(params)
+
+['hierarchical',
+ 'ward',
+ 2,
+ 'hierarchical',
+ 'ward2',
+ 4,
+ 'hierarchical',
+ 'single',
+ 3,
+ 'hierarchical',
+ 'ward',
+ 4,
+ 'hierarchical',
+ 'single',
+ 5,
+ 'hierarchical',
+ 'complete',
+ 3,
+ 'disagreement']
+```
+
+To get the labels, run `parea_2()` using these parameters and your data:
 
 ```python
 pyrea.parea_2(data, *params)
 ```
 
 which will return the cluster labels for your data.
 
-**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these to be customised.
+Also, you may choose to define the **final** number of clusters returned by the algorithm (but allowing it to optimise intermediate numbers of clusters) by defining `k_final`, e.g:
+
+```python
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5, k_final=3)
+```
+
+and calling `pyrea_2()` as follows:
+
+```python
+pyrea.parea_2(data, params, k_final=3)
+```
+
+**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these parameters to be customised in the near future.
 
 ### API
 
 **Please note that Pyrea is work in progress. The API may change from version
-to version in the coming weeks, which could introduce breaking changes.**
+to version and introduce breaking changes.**
 
 In Pyrea, your data are organised in to views. A view consists of the data in
 the form of a 2D matrix, and an associated clustering algorithm (a *clusterer*).
 
 To create a view you must have some data, and a clusterer:
 
 ```python
```

### Comparing `pyrea-1.0.8/README.md` & `pyrea-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 ```bash
 pip install pyrea
 ```
 
 This will install the latest version of Pyrea from PyPI.
 
 ## Usage
-The Pyrea software package is the accompanying software for our paper: *Parea: multi-view ensemble clustering for cancer subtype discovery*[^1].
+The Pyrea software package is the accompanying software for our paper:
+
+Pfeifer, B., Bloice, M.D., & Schimek, M.G. (2022). *Parea: multi-view ensemble clustering for cancer subtype discovery*. arXiv. <https://arxiv.org/abs/2209.15399>
 
 While Pyrea allows for flexible and custom architectures to be built, two structures are discussed specifically in the paper cited above, namely Parea 1 and Parea 2.
 
-Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows
+Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows:
 
 ```python
 import pyrea
 import numpy as np
 
 # Create sample data:
 d1 = np.random.rand(100,10)
@@ -40,15 +42,15 @@
 data = [d1,d2, d3]
 
 labels = pyrea.parea_2(data)
 ```
 
 which executes Parea 2.
 
-Default parameters are used which match those used in our experiments discussed in the paper above. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
+Default parameters are used which match those used in our experiments discussed in the paper[^1]. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
 
 ### Genetic Algorithm
 
 The Parea 1 and Parea 2 structures can be optimised using a genetic algorithm in order to find the best combinations of clustering methods, fusion methods, and number of clusters.
 
 For example, to find optimal parameters for Parea 2:
 
@@ -59,33 +61,71 @@
 
 d1 = datasets.load_iris().data
 d2 = datasets.load_iris().data
 d3 = datasets.load_iris().data
 
 data = [d1,d2,d3]
 
-params = pyrea.parea_2_genetic(data, max_k=5)
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5)
 ```
 
-where `max_k` refers to the maximum number of clusters to attempt for each layer.
+where `k_min` and `k_max` refer to the minimum and maximum number of clusters to attempt for each layer, respectively.
 
-Note that `params` contains the optimal parameters found by the genetic algorithm. To get the labels, run `parea_2()` using these parameters and your data:
+Note that `params` contains the optimal parameters found by the genetic algorithm:
+
+```python
+print(params)
+
+['hierarchical',
+ 'ward',
+ 2,
+ 'hierarchical',
+ 'ward2',
+ 4,
+ 'hierarchical',
+ 'single',
+ 3,
+ 'hierarchical',
+ 'ward',
+ 4,
+ 'hierarchical',
+ 'single',
+ 5,
+ 'hierarchical',
+ 'complete',
+ 3,
+ 'disagreement']
+```
+
+To get the labels, run `parea_2()` using these parameters and your data:
 
 ```python
 pyrea.parea_2(data, *params)
 ```
 
 which will return the cluster labels for your data.
 
-**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these to be customised.
+Also, you may choose to define the **final** number of clusters returned by the algorithm (but allowing it to optimise intermediate numbers of clusters) by defining `k_final`, e.g:
+
+```python
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5, k_final=3)
+```
+
+and calling `pyrea_2()` as follows:
+
+```python
+pyrea.parea_2(data, params, k_final=3)
+```
+
+**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these parameters to be customised in the near future.
 
 ### API
 
 **Please note that Pyrea is work in progress. The API may change from version
-to version in the coming weeks, which could introduce breaking changes.**
+to version and introduce breaking changes.**
 
 In Pyrea, your data are organised in to views. A view consists of the data in
 the form of a 2D matrix, and an associated clustering algorithm (a *clusterer*).
 
 To create a view you must have some data, and a clusterer:
 
 ```python
```

### Comparing `pyrea-1.0.8/pyrea/call_c.py` & `pyrea-1.0.9/pyrea/call_c.py`

 * *Files identical despite different names*

### Comparing `pyrea-1.0.8/pyrea/core.py` & `pyrea-1.0.9/pyrea/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 Developers, especially those who wish to extend Pyrea, may want to look at the
 classes and functions defined in the :py:mod:`pyrea.structure` module.
 """
 import random
 from array import array
 from cmath import exp
-from typing import List
+from typing import List, Union
 import numpy as np
+import warnings
 from sklearn.metrics import silhouette_score
 
 # Genetic algorithm imports
 from deap import base
 from deap import creator
 from deap import tools
 from deap import algorithms
@@ -171,15 +172,14 @@
     if fuser == "disagreement":
         return Disagreement()
     elif fuser == "agreement":
         return Agreement()
     elif fuser == "consensus":
         return Consensus()
 
-
 def execute_ensemble(views: List[View], fuser: Fusion) -> list:
     """
     Executes an ensemble and returns a new :class:`View` object.
 
     :param views: The ensemble's views.
     :param fuser: The fusion algorithm used to fuse the clustered data.
     :param clusterers: A clustering algorithm or list of clustering algorithms
@@ -264,15 +264,15 @@
 
     return silhouette_score
 
 def parea_1(data: list, c_1_type='hierarchical', c_1_method='ward', c_1_k=2,
             c_2_type='hierarchical', c_2_method='complete', c_2_k=2,
             c_1_pre_type='hierarchical', c_1_pre_method='ward', c_1_pre_k=2,
             c_2_pre_type='hierarchical', c_2_pre_method='complete', c_2_pre_k=2,
-            fusion_method='disagreement', fitness=False):
+            fusion_method='disagreement', fitness=False, k_final=None):
     """
     Implements the PAREA-1 algorithm.
 
     The function accepts a list of parameters for the Parea 1 algorithm.
 
     The default values are those described in the package's paper and README
     documentation regarding the PAREA-1 structure.
@@ -327,69 +327,72 @@
     # Execute our second ensemble, and retreive a new view:
     v_ensemble_2 = view(execute_ensemble(views2, f), c2_pre)
 
     # Now we can execute a further ensemble, using the views generated from the
     # two previous ensemble methods:
     v_res  = execute_ensemble([v_ensemble_1, v_ensemble_2], f)
 
-    # The returned distance matrix is now used as an input for the two clustering methods (hc1 and hc2)
-    v1_res = view(v_res, c1_pre)
-    v2_res = view(v_res, c2_pre)
+    # TODO: allow for type and method to be passed in as parameters
+    if k_final:
+        c_final = clusterer(c_1_pre_type, method=c_1_pre_method, n_clusters=k_final, precomputed=True)
+        v_res_final = view(v_res, c_final)
+        labels = v_res_final.execute()
+
+        labels = labels[:,0]
+    else:
+        # The returned distance matrix is now used as an input for the two clustering methods (hc1 and hc2)
+        v1_res = view(v_res, c1_pre)
+        v2_res = view(v_res, c2_pre)
 
-    # and the cluster solutions are combined
-    labels = consensus([v1_res.execute(), v2_res.execute()])
+        # and the cluster solutions are combined
+        labels = consensus([v1_res.execute(), v2_res.execute()])
 
     if fitness:
         return silhouette_score(v_res, labels, metric='precomputed')
     else:
         return labels
 
-
-def parea_1_genetic(data: list, max_k: int):
+def parea_1_genetic(data: list, k_min: int, k_max: int, k_final: Union[int, None] = None):
     """
     Genetic algorithm optimised implementation of Parea 1.
     """
     # Check if creator has been initialised
     if not hasattr(creator, "FitnessMax"):
         creator.create("FitnessMax", base.Fitness, weights=(1.0,))
 
     if not hasattr(creator, "Individual"):
         creator.create("Individual", list, fitness=creator.FitnessMax)
 
     toolbox = base.Toolbox()
 
-    # Cluster size range
-    k_low, k_high = 2, max_k
-
     # Define possible parameters
     # TODO: Replace these with the global variables
     cluster_methods = ['spectral', 'hierarchical', 'dbscan', 'optics']
     fusion_methods = ['agreement', 'consensus', 'disagreement']
     linkages = ['single', 'complete', 'average', 'weighted', 'centroid', 'median', 'ward', 'ward2']
 
     # Overwrite the cluster and fusion methods temporarily
     cluster_methods = ['hierarchical']
     fusion_methods = ['disagreement']
 
     # Set up parameters for the genetic algorithm                       Index
     toolbox.register("c_1_type", random.choice, cluster_methods)        # 0
     toolbox.register("c_1_method", random.choice, linkages)             # 1
-    toolbox.register("c_1_k", random.randint, k_low, k_high)            # 2
+    toolbox.register("c_1_k", random.randint, k_min, k_max)             # 2
     toolbox.register("c_2_type", random.choice, cluster_methods)        # 3
     toolbox.register("c_2_method", random.choice, linkages)             # 4
-    toolbox.register("c_2_k", random.randint, k_low, k_high)            # 5
+    toolbox.register("c_2_k", random.randint, k_min, k_max)             # 5
     toolbox.register("c_1_pre_type", random.choice, cluster_methods)    # 6
     toolbox.register("c_1_pre_method", random.choice, linkages)         # 7
-    toolbox.register("c_1_pre_k", random.randint, k_low, k_high)        # 8
+    toolbox.register("c_1_pre_k", random.randint, k_min, k_max)         # 8
     toolbox.register("c_2_pre_type", random.choice, cluster_methods)    # 9
     toolbox.register("c_2_pre_method", random.choice, linkages)         # 10
-    toolbox.register("c_2_pre_k", random.randint, k_low, k_high)        # 11
+    toolbox.register("c_2_pre_k", random.randint, k_min, k_max)         # 11
     toolbox.register("fusion_method", random.choice, fusion_methods)    # 12
 
-
     # Chromosomes
     # TODO: Add user parameter for N_CYCLES
     N_CYCLES = 1
     toolbox.register("individual", tools.initCycle, creator.Individual,
                      (toolbox.c_1_type, toolbox.c_1_method, toolbox.c_1_k,
                       toolbox.c_2_type, toolbox.c_2_method, toolbox.c_2_k,
                       toolbox.c_1_pre_type, toolbox.c_1_pre_method, toolbox.c_1_pre_k,
@@ -397,40 +400,58 @@
                       toolbox.fusion_method), n=N_CYCLES)
 
     # How the population is created
     toolbox.register("population", tools.initRepeat, list, toolbox.individual)
 
     def mutate(individual):
         """ Mutate an individual. """
-        # Choose a random parameter to mutate
+        # Choose a random parameter to mutate, and select the gene
         index = random.randint(0, len(individual) - 1)
-
-        # Get the gene to be mutated
         gene = individual[index]
 
         # Mutate the parameter. Remember that:
         # 0, 3, 6, 9, are cluster methods
         # 1, 4, 7, 10, are linkages
         # 2, 5, 8, 11, are cluster sizes
         # 12 is the fusion method
 
         if gene in [0, 3, 6, 9]:
             individual[gene] = random.choice(cluster_methods)
         elif gene in [1, 4, 7, 10]:
             individual[gene] = random.choice(linkages)
         elif gene in [2, 5, 8, 11]:
-            individual[gene] = random.randint(k_low, k_high)
+            individual[gene] = random.randint(k_min, k_max)
         elif gene == 12:
             individual[gene] = random.choice(fusion_methods)
 
         return individual,
 
     def evaluate(individual):
         """ Evaluate an individual. """
-        sil = parea_1(data, individual[0], individual[1], individual[2], individual[3], individual[4], individual[5], individual[6], individual[7], individual[8], individual[9], individual[10], individual[11], individual[12], fitness=True)
+
+        # sklearn uses np.matrix which throws a warning as it is deprecated
+        # Use this to silence the warning
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            sil = parea_1(data,
+                          individual[0],
+                          individual[1],
+                          individual[2],
+                          individual[3],
+                          individual[4],
+                          individual[5],
+                          individual[6],
+                          individual[7],
+                          individual[8],
+                          individual[9],
+                          individual[10],
+                          individual[11],
+                          individual[12],
+                          fitness=True, k_final=k_final)
 
         print("Silhouette score: %s" % sil)
 
         return sil,
 
     # Register the functions
     # TODO: Try other crossover methods and tournament sizes, etc.
@@ -446,15 +467,17 @@
 
     stats.register("avg", np.mean)
     stats.register("std", np.std)
     stats.register("min", np.min)
     stats.register("max", np.max)
 
     # Run the genetic algorithm
-    x, y = algorithms.eaSimple(population, toolbox, cxpb=0.7, mutpb=0.2, ngen=10, stats=stats, halloffame=hall_of_fame, verbose=True)
+    pop, log = algorithms.eaSimple(population, toolbox, cxpb=0.7, mutpb=0.2, ngen=10, stats=stats, halloffame=hall_of_fame, verbose=True)
+
+    print(f"\nSummary:\n{log}")
 
     return hall_of_fame[0]
 
 def cluster_silhoutte_score(data: list, type: str, method: str, k: int, precomputed: bool=False):
 
     # Cluster the data and get the labels
     c = clusterer(type, precomputed=precomputed, method=method, n_clusters=k)
@@ -465,15 +488,15 @@
 
 def parea_2(data: list, c_1_type='hierarchical', c_1_method='ward', c_1_k=2,
             c_2_type='hierarchical', c_2_method='complete', c_2_k=2,
             c_3_type='hierarchical', c_3_method='single', c_3_k=2,
             c_1_pre_type='hierarchical', c_1_pre_method='ward', c_1_pre_k=2,
             c_2_pre_type='hierarchical', c_2_pre_method='complete', c_2_pre_k=2,
             c_3_pre_type='hierarchical', c_3_pre_method='single', c_3_pre_k=2,
-            fusion_method='disagreement', fitness=False):
+            fusion_method='disagreement', fitness=False, k_final=None):
     """
     Implements the PAREA-2 algorithm.
 
     :param views: A list of views to be used in the ensemble.
     :param c_1_type: The type of clustering algorithm to use for the first clustering step.
     :param c_1_method: The method of clustering algorithm to use for the first clustering step.
     :param c_2_type: The type of clustering algorithm to use for the second clustering step.
@@ -512,28 +535,36 @@
 
     # Fusion algorithm
     f = fuser(fusion_method)
 
     # Create the ensemble and define new views based on the returned disagreement matrix v_res
     v_res  = execute_ensemble(views, f)
 
-    v1_res = view(v_res, c1_pre)
-    v2_res = view(v_res, c2_pre)
-    v3_res = view(v_res, c3_pre)
+    # TODO: allow for type and method to be passed in as parameters
+    if k_final:
+        c_final = clusterer(c_1_pre_type, method=c_1_pre_method, n_clusters=k_final, precomputed=True)
+        v_res_final = view(v_res, c_final)
+        labels = v_res_final.execute()
+
+        # Remove the last dimension of the labels, could also use np.squeeze, but requires 1.7 or higher
+        labels = labels[:,0]
+    else:
+        v1_res = view(v_res, c1_pre)
+        v2_res = view(v_res, c2_pre)
+        v3_res = view(v_res, c3_pre)
 
-    # Get the final cluster solution
-    labels = consensus([v1_res.execute(), v2_res.execute(), v3_res.execute()])
+        # Get the final cluster solution
+        labels = consensus([v1_res.execute(), v2_res.execute(), v3_res.execute()])
 
     if fitness:
         return silhouette_score(v_res, labels, metric='precomputed')
     else:
         return labels
 
-
-def parea_2_genetic(data: list, max_k: int):
+def parea_2_genetic(data: list, k_min: int, k_max: int, k_final: Union[int, None] = None):
     """
     Genetic algorithm optimised implementation of Parea 2.
     """
     # Create FitnesssMax and Individual classes/types.
     # Maybe place this outside of this function as it will be called
     # in the parea_1_genetic function also... and will be identical
 
@@ -542,46 +573,43 @@
 
     if not hasattr(creator, "Individual"):
         creator.create("Individual", list, fitness=creator.FitnessMax)
 
     # Create the toolbox
     toolbox = base.Toolbox()
 
-    # Cluster size range
-    k_low, k_high = 2, max_k
-
     # Define possible parameters
     # TODO: Replace these with the global variables
     cluster_methods = ['spectral', 'hierarchical', 'dbscan', 'optics']
     fusion_methods = ['agreement', 'consensus', 'disagreement']
     linkages = ['single', 'complete', 'average', 'weighted', 'centroid', 'median', 'ward', 'ward2']
 
     # Overwrite the cluster and fusion methods temporarily
     cluster_methods = ['hierarchical']
     fusion_methods = ['disagreement']
 
     # Set up our parameters for the genetic algorithm                   Index
     toolbox.register("c_1_type", random.choice, cluster_methods)        # 0
     toolbox.register("c_1_method", random.choice, linkages)             # 1
-    toolbox.register("c_1_k", random.randint, k_low, k_high)            # 2
+    toolbox.register("c_1_k", random.randint, k_min, k_max)             # 2
     toolbox.register("c_2_type", random.choice, cluster_methods)        # 3
     toolbox.register("c_2_method", random.choice, linkages)             # 4
-    toolbox.register("c_2_k", random.randint, k_low, k_high)            # 5
+    toolbox.register("c_2_k", random.randint, k_min, k_max)             # 5
     toolbox.register("c_3_type", random.choice, cluster_methods)        # 6
     toolbox.register("c_3_method", random.choice, linkages)             # 7
-    toolbox.register("c_3_k", random.randint, k_low, k_high)            # 8
+    toolbox.register("c_3_k", random.randint, k_min, k_max)             # 8
     toolbox.register("c_1_pre_type", random.choice, cluster_methods)    # 9
     toolbox.register("c_1_pre_method", random.choice, linkages)         # 10
-    toolbox.register("c_1_pre_k", random.randint, k_low, k_high)        # 11
+    toolbox.register("c_1_pre_k", random.randint, k_min, k_max)         # 11
     toolbox.register("c_2_pre_type", random.choice, cluster_methods)    # 12
     toolbox.register("c_2_pre_method", random.choice, linkages)         # 13
-    toolbox.register("c_2_pre_k", random.randint, k_low, k_high)        # 14
+    toolbox.register("c_2_pre_k", random.randint, k_min, k_max)         # 14
     toolbox.register("c_3_pre_type", random.choice, cluster_methods)    # 15
     toolbox.register("c_3_pre_method", random.choice, linkages)         # 16
-    toolbox.register("c_3_pre_k", random.randint, k_low, k_high)        # 17
+    toolbox.register("c_3_pre_k", random.randint, k_min, k_max)         # 17
     toolbox.register("fusion_method", random.choice, fusion_methods)    # 18
 
     # How the chromosomes are created
     N_CYCLES = 1
     # TODO: Add user parameter for N_CYCLES
     toolbox.register("individual", tools.initCycle, creator.Individual,
     (toolbox.c_1_type, toolbox.c_1_method, toolbox.c_1_k, toolbox.c_2_type,
@@ -591,33 +619,58 @@
     toolbox.c_3_pre_type, toolbox.c_3_pre_method, toolbox.c_3_pre_k,
     toolbox.fusion_method), n=N_CYCLES)
 
     # How the population is created
     toolbox.register("population", tools.initRepeat, list, toolbox.individual)
 
     # Define how to mutate the chromosomes
-    def mutate(inidividual):
-        # Mutate one parameter randomly
-
-        gene = random.randint(0, 19)
+    def mutate(individual):
+        # Choose a random parameter to mutate, and select the gene
+        index = random.randint(0, len(individual) - 1)
+        gene = individual[index]
 
         if gene in [0, 3, 6, 9, 12, 15]:
-            inidividual[gene] = random.choice(cluster_methods)
+            individual[gene] = random.choice(cluster_methods)
         elif gene in [1, 4, 7, 10, 13, 16]:
-            inidividual[gene] = random.choice(linkages)
+            individual[gene] = random.choice(linkages)
         elif gene in [2, 5, 8, 11, 14, 17]:
-            inidividual[gene] = random.randint(k_low, k_high)
+            individual[gene] = random.randint(k_min, k_max)
         elif gene == 18:
-            inidividual[gene] = random.choice(fusion_methods)
+            individual[gene] = random.choice(fusion_methods)
 
-        return inidividual,
+        return individual,
 
     def evaluate(individual):
 
-        sil = parea_2(data, individual[0], individual[1], individual[2], individual[3], individual[4], individual[5], individual[6], individual[7], individual[8], individual[9], individual[10], individual[11], individual[12], individual[13], individual[14], individual[15], individual[16], individual[17], individual[18], fitness=True)
+        # sklearn uses np.matrix which throws a warning as it is deprecated
+        # Use this to silence the warning
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            sil = parea_2(data,
+                          individual[0],
+                          individual[1],
+                          individual[2],
+                          individual[3],
+                          individual[4],
+                          individual[5],
+                          individual[6],
+                          individual[7],
+                          individual[8],
+                          individual[9],
+                          individual[10],
+                          individual[11],
+                          individual[12],
+                          individual[13],
+                          individual[14],
+                          individual[15],
+                          individual[16],
+                          individual[17],
+                          individual[18],
+                          fitness=True, k_final=k_final)
 
         print("Silhouette score: %s" % sil)
 
         return sil,
 
     # Register the functions
     # TODO: Try other crossover methods and tournament sizes, etc.
@@ -632,11 +685,13 @@
     stats = tools.Statistics(lambda ind: ind.fitness.values)
 
     stats.register("avg", np.mean)
     stats.register("std", np.std)
     stats.register("min", np.min)
     stats.register("max", np.max)
 
-    # TODO: Check what pop and log are
+    # TODO: Work out if pop and log should also be returned
     pop, log = algorithms.eaSimple(population, toolbox, cxpb=0.7, mutpb=0.2, ngen=10, stats=stats, halloffame=hall_of_fame, verbose=True)
 
+    print(f"\nSummary:\n{log}")
+
     return hall_of_fame[0]
```

### Comparing `pyrea-1.0.8/pyrea/debug.py` & `pyrea-1.0.9/pyrea/debug.py`

 * *Files identical despite different names*

### Comparing `pyrea-1.0.8/pyrea/structure.py` & `pyrea-1.0.9/pyrea/structure.py`

 * *Files identical despite different names*

### Comparing `pyrea-1.0.8/pyrea.egg-info/PKG-INFO` & `pyrea-1.0.9/pyrea.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrea
-Version: 1.0.8
+Version: 1.0.9
 Summary: Multi-view clustering with deep ensemble structures.
 Home-page: https://github.com/mdbloice/Pyrea
 Author: Marcus D. Bloice, Bastian Pfeifer
 Author-email: marcus.bloice@medunigraz.at
 License: MIT
 Keywords: multi-view,clustering,ensemble clustering
 Platform: UNKNOWN
@@ -49,19 +49,21 @@
 ```bash
 pip install pyrea
 ```
 
 This will install the latest version of Pyrea from PyPI.
 
 ## Usage
-The Pyrea software package is the accompanying software for our paper: *Parea: multi-view ensemble clustering for cancer subtype discovery*[^1].
+The Pyrea software package is the accompanying software for our paper:
+
+Pfeifer, B., Bloice, M.D., & Schimek, M.G. (2022). *Parea: multi-view ensemble clustering for cancer subtype discovery*. arXiv. <https://arxiv.org/abs/2209.15399>
 
 While Pyrea allows for flexible and custom architectures to be built, two structures are discussed specifically in the paper cited above, namely Parea 1 and Parea 2.
 
-Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows
+Both the structures, which are described in detail below as well as in the paper mentioned above, can be quickly generated and applied to your data using two helper functions, `parea_1()` and `parea_2()`, and can be quickly run as follows:
 
 ```python
 import pyrea
 import numpy as np
 
 # Create sample data:
 d1 = np.random.rand(100,10)
@@ -71,15 +73,15 @@
 data = [d1,d2, d3]
 
 labels = pyrea.parea_2(data)
 ```
 
 which executes Parea 2.
 
-Default parameters are used which match those used in our experiments discussed in the paper above. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
+Default parameters are used which match those used in our experiments discussed in the paper[^1]. These default parameters can of course be overridden. As there are many combinations of parameters that could be used, a genetic algorithm can be utilised to find the optimum parameters, as shown in the next section.
 
 ### Genetic Algorithm
 
 The Parea 1 and Parea 2 structures can be optimised using a genetic algorithm in order to find the best combinations of clustering methods, fusion methods, and number of clusters.
 
 For example, to find optimal parameters for Parea 2:
 
@@ -90,33 +92,71 @@
 
 d1 = datasets.load_iris().data
 d2 = datasets.load_iris().data
 d3 = datasets.load_iris().data
 
 data = [d1,d2,d3]
 
-params = pyrea.parea_2_genetic(data, max_k=5)
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5)
 ```
 
-where `max_k` refers to the maximum number of clusters to attempt for each layer.
+where `k_min` and `k_max` refer to the minimum and maximum number of clusters to attempt for each layer, respectively.
 
-Note that `params` contains the optimal parameters found by the genetic algorithm. To get the labels, run `parea_2()` using these parameters and your data:
+Note that `params` contains the optimal parameters found by the genetic algorithm:
+
+```python
+print(params)
+
+['hierarchical',
+ 'ward',
+ 2,
+ 'hierarchical',
+ 'ward2',
+ 4,
+ 'hierarchical',
+ 'single',
+ 3,
+ 'hierarchical',
+ 'ward',
+ 4,
+ 'hierarchical',
+ 'single',
+ 5,
+ 'hierarchical',
+ 'complete',
+ 3,
+ 'disagreement']
+```
+
+To get the labels, run `parea_2()` using these parameters and your data:
 
 ```python
 pyrea.parea_2(data, *params)
 ```
 
 which will return the cluster labels for your data.
 
-**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these to be customised.
+Also, you may choose to define the **final** number of clusters returned by the algorithm (but allowing it to optimise intermediate numbers of clusters) by defining `k_final`, e.g:
+
+```python
+params = pyrea.parea_2_genetic(data, k_min=2, k_max=5, k_final=3)
+```
+
+and calling `pyrea_2()` as follows:
+
+```python
+pyrea.parea_2(data, params, k_final=3)
+```
+
+**Note**: Currently the genetic algorithm uses a population size of 100 and runs for 10 generations. This function will be updated to allow these parameters to be customised in the near future.
 
 ### API
 
 **Please note that Pyrea is work in progress. The API may change from version
-to version in the coming weeks, which could introduce breaking changes.**
+to version and introduce breaking changes.**
 
 In Pyrea, your data are organised in to views. A view consists of the data in
 the form of a 2D matrix, and an associated clustering algorithm (a *clusterer*).
 
 To create a view you must have some data, and a clusterer:
 
 ```python
```

### Comparing `pyrea-1.0.8/setup.py` & `pyrea-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='pyrea',
-    version='1.0.8',
+    version='1.0.9',
     author='Marcus D. Bloice, Bastian Pfeifer',
     license='MIT',
     author_email='marcus.bloice@medunigraz.at',
     description='Multi-view clustering with deep ensemble structures.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdbloice/Pyrea',
```

