# Comparing `tmp/clusteval-2.1.6.tar.gz` & `tmp/clusteval-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusteval-2.1.6.tar", last modified: Sun Apr 16 21:42:59 2023, max compression
+gzip compressed data, was "clusteval-2.2.0.tar", last modified: Wed Apr 19 20:57:19 2023, max compression
```

## Comparing `clusteval-2.1.6.tar` & `clusteval-2.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.546082 clusteval-2.1.6/
--rw-rw-rw-   0        0        0     1146 2023-04-10 15:32:29.000000 clusteval-2.1.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7990 2023-04-16 21:42:59.545086 clusteval-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2023-04-10 15:32:29.000000 clusteval-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.498415 clusteval-2.1.6/clusteval/
--rw-rw-rw-   0        0        0     1118 2023-04-16 21:39:47.000000 clusteval-2.1.6/clusteval/__init__.py
--rw-rw-rw-   0        0        0    36815 2023-04-16 21:40:29.000000 clusteval-2.1.6/clusteval/clusteval.py
--rw-rw-rw-   0        0        0     2015 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/coord2density.py
--rw-rw-rw-   0        0        0     8104 2023-04-15 13:48:17.000000 clusteval-2.1.6/clusteval/dbindex.py
--rw-rw-rw-   0        0        0     8604 2023-04-16 14:21:20.000000 clusteval-2.1.6/clusteval/dbscan.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 14:19:24.000000 clusteval-2.1.6/clusteval/derivative.py
--rw-rw-rw-   0        0        0    19051 2023-04-16 18:54:34.000000 clusteval-2.1.6/clusteval/examples.py
--rw-rw-rw-   0        0        0     7479 2023-04-11 18:26:51.000000 clusteval-2.1.6/clusteval/hdbscan.py
--rw-rw-rw-   0        0        0      311 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/image2vec.py
--rw-rw-rw-   0        0        0     2841 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/plot_dendrogram.py
--rw-rw-rw-   0        0        0    14601 2023-04-16 18:33:43.000000 clusteval-2.1.6/clusteval/silhouette.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.544089 clusteval-2.1.6/clusteval/tests/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/tests/__init__.py
--rw-rw-rw-   0        0        0     6418 2023-04-16 18:50:37.000000 clusteval-2.1.6/clusteval/tests/test_clusteval.py
--rw-rw-rw-   0        0        0     2696 2023-04-16 18:40:14.000000 clusteval-2.1.6/clusteval/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.539103 clusteval-2.1.6/clusteval.egg-info/
--rw-rw-rw-   0        0        0     7990 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 21:42:59.546082 clusteval-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-04-16 16:29:41.000000 clusteval-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.646233 clusteval-2.2.0/
+-rw-rw-rw-   0        0        0     1146 2023-04-10 15:32:29.000000 clusteval-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8181 2023-04-19 20:57:19.627646 clusteval-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7628 2023-04-19 20:54:55.000000 clusteval-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.585531 clusteval-2.2.0/clusteval/
+-rw-rw-rw-   0        0        0     1118 2023-04-19 20:52:04.000000 clusteval-2.2.0/clusteval/__init__.py
+-rw-rw-rw-   0        0        0     2361 2023-04-19 11:33:35.000000 clusteval-2.2.0/clusteval/bubblegrid.py
+-rw-rw-rw-   0        0        0    38503 2023-04-19 20:45:55.000000 clusteval-2.2.0/clusteval/clusteval.py
+-rw-rw-rw-   0        0        0     2015 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/coord2density.py
+-rw-rw-rw-   0        0        0     8104 2023-04-15 13:48:17.000000 clusteval-2.2.0/clusteval/dbindex.py
+-rw-rw-rw-   0        0        0     8605 2023-04-17 22:09:35.000000 clusteval-2.2.0/clusteval/dbscan.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 14:19:24.000000 clusteval-2.2.0/clusteval/derivative.py
+-rw-rw-rw-   0        0        0    22922 2023-04-19 20:56:14.000000 clusteval-2.2.0/clusteval/examples.py
+-rw-rw-rw-   0        0        0     7479 2023-04-11 18:26:51.000000 clusteval-2.2.0/clusteval/hdbscan.py
+-rw-rw-rw-   0        0        0     2841 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/plot_dendrogram.py
+-rw-rw-rw-   0        0        0    14608 2023-04-19 20:06:49.000000 clusteval-2.2.0/clusteval/silhouette.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.626650 clusteval-2.2.0/clusteval/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/tests/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-19 20:54:22.000000 clusteval-2.2.0/clusteval/tests/test_clusteval.py
+-rw-rw-rw-   0        0        0     4508 2023-04-18 09:18:54.000000 clusteval-2.2.0/clusteval/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.611223 clusteval-2.2.0/clusteval.egg-info/
+-rw-rw-rw-   0        0        0     8181 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:57:19.646233 clusteval-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-04-16 16:29:41.000000 clusteval-2.2.0/setup.py
```

### Comparing `clusteval-2.1.6/LICENSE` & `clusteval-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/PKG-INFO` & `clusteval-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.1.6
+Version: 2.2.0
 Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.1.6.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.2.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clusteval
+<p align="center">
+  <a href="https://erdogant.github.io/clusteval">
+  <img src="https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png" width="300" />
+  </a>
+</p>
 
 [![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval)
 [![PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE)
 [![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)
 [![Github Forks](https://img.shields.io/github/forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
 [![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/issues)
```

#### html2text {}

```diff
@@ -1,53 +1,55 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.1.6 Summary: clusteval is a
+Metadata-Version: 2.1 Name: clusteval Version: 2.2.0 Summary: clusteval is a
 python package for unsupervised cluster validation. Home-page: https://
 erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
-clusteval/archive/2.1.6.tar.gz Author: Erdogan Taskesen Author-email:
+clusteval/archive/2.2.0.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # clusteval [![Python](https://img.shields.io/pypi/
-pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [!
-[PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/
-project/clusteval/) [![License](https://img.shields.io/badge/license-MIT-
-green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE) [!
-[BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://
-www.buymeacoffee.com/erdogant) [![Github Forks](https://img.shields.io/github/
-forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
-[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
-clusteval.svg)](https://github.com/erdogant/clusteval/issues) [![Project
-Status](http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/clusteval/
-month)](https://pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/
-badge/clusteval)](https://pepy.tech/project/clusteval) [![DOI](https://
-zenodo.org/badge/232915924.svg)](https://zenodo.org/badge/latestdoi/232915924)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/clusteval/) [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
-clusteval/pages/html/Documentation.html#colab-notebook)  ``clusteval`` is a
-python package that is developed to evaluate detected clusters and return the
-cluster labels that have most optimal **clustering tendency**, **Number of
-clusters** and **clustering quality**. Multiple evaluation strategies are
-implemented for the evaluation; **silhouette**, **dbindex**, and
-**derivative**, and four clustering methods can be used: **agglomerative**,
-**kmeans**, **dbscan** and **hdbscan**. # **â­ï¸ Star this repo if you like
-it â­ï¸** # ### Blogs Read the blog to get a structured overview how you can
-use ``clusteval``. * [Medium Blog: A step-by-step guide for clustering images]
-(https://towardsdatascience.com/a-step-by-step-guide-for-clustering-images-
-4b45f9906128) In case you want to detect identical images, you can also use
-hash functionalities. * [Medium Blog: Detection of Duplicate Images Using Image
-Hash Functions](https://towardsdatascience.com/detection-of-duplicate-images-
-using-image-hash-functions-4d9c53f04a75) # ### [Documentation pages](https://
-erdogant.github.io/clusteval/) On the [documentation pages](https://
-erdogant.github.io/clusteval/) you can find detailed information about the
-working of the ``clusteval`` with many examples. # ### Installation ##### It is
-advisable to create a new environment (e.g. with Conda). ```bash conda create -
-n env_clusteval python=3.8 conda activate clusteval ``` ##### Install from PyPI
-```bash pip install clusteval ``` ##### Import library ```python from clusteval
-import clusteval ```
+License-File: LICENSE # clusteval
+[https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png]
+[![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://
+img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
+img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/) [!
+[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
+github.com/erdogant/clusteval/blob/master/LICENSE) [![BuyMeCoffee](https://
+img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/
+erdogant) [![Github Forks](https://img.shields.io/github/forks/erdogant/
+clusteval.svg)](https://github.com/erdogant/clusteval/network) [![GitHub Open
+Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://
+github.com/erdogant/clusteval/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/clusteval/month)](https://
+pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/badge/clusteval)]
+(https://pepy.tech/project/clusteval) [![DOI](https://zenodo.org/badge/
+232915924.svg)](https://zenodo.org/badge/latestdoi/232915924) [![Sphinx](https:
+//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+clusteval/) [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://erdogant.github.io/clusteval/pages/html/
+Documentation.html#colab-notebook)  ``clusteval`` is a python package that is
+developed to evaluate detected clusters and return the cluster labels that have
+most optimal **clustering tendency**, **Number of clusters** and **clustering
+quality**. Multiple evaluation strategies are implemented for the evaluation;
+**silhouette**, **dbindex**, and **derivative**, and four clustering methods
+can be used: **agglomerative**, **kmeans**, **dbscan** and **hdbscan**. #
+**â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read the blog to
+get a structured overview how you can use ``clusteval``. * [Medium Blog: A
+step-by-step guide for clustering images](https://towardsdatascience.com/a-
+step-by-step-guide-for-clustering-images-4b45f9906128) In case you want to
+detect identical images, you can also use hash functionalities. * [Medium Blog:
+Detection of Duplicate Images Using Image Hash Functions](https://
+towardsdatascience.com/detection-of-duplicate-images-using-image-hash-
+functions-4d9c53f04a75) # ### [Documentation pages](https://erdogant.github.io/
+clusteval/) On the [documentation pages](https://erdogant.github.io/clusteval/
+) you can find detailed information about the working of the ``clusteval`` with
+many examples. # ### Installation ##### It is advisable to create a new
+environment (e.g. with Conda). ```bash conda create -n env_clusteval python=3.8
+conda activate clusteval ``` ##### Install from PyPI ```bash pip install
+clusteval ``` ##### Import library ```python from clusteval import clusteval
+```
 ===============================================================================
 ### Examples A structured overview of all examples are now available on the
 [documentation pages](https://erdogant.github.io/clusteval/).
 ===============================================================================
 * [Example: Cluster validation using Silhouette score](https://
 erdogant.github.io/clusteval/pages/html/Examples.html#cluster-evaluation)
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/fig1b_sil.png]
```

### Comparing `clusteval-2.1.6/README.md` & `clusteval-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # clusteval
+<p align="center">
+  <a href="https://erdogant.github.io/clusteval">
+  <img src="https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png" width="300" />
+  </a>
+</p>
 
 [![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval)
 [![PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE)
 [![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)
 [![Github Forks](https://img.shields.io/github/forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
 [![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/issues)
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-# clusteval [![Python](https://img.shields.io/pypi/pyversions/clusteval)]
-(https://img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
+# clusteval
+[https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png]
+[![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://
+img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
 img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/) [!
 [License](https://img.shields.io/badge/license-MIT-green.svg)](https://
 github.com/erdogant/clusteval/blob/master/LICENSE) [![BuyMeCoffee](https://
 img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/
 erdogant) [![Github Forks](https://img.shields.io/github/forks/erdogant/
 clusteval.svg)](https://github.com/erdogant/clusteval/network) [![GitHub Open
 Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://
```

### Comparing `clusteval-2.1.6/clusteval/__init__.py` & `clusteval-2.2.0/clusteval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     dbscan,
     # hdbscan_custom,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.1.6'
+__version__ = '2.2.0'
 
 
 __doc__ = """
 clusteval
 =====================================================================
 
 Description
```

### Comparing `clusteval-2.1.6/clusteval/clusteval.py` & `clusteval-2.2.0/clusteval/clusteval.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """clusteval is a python package to measure the goodness of the unsupervised clustering."""
 
 from scatterd import scatterd
 import clusteval.dbindex as dbindex
 import clusteval.silhouette as silhouette
 import clusteval.derivative as derivative
 import clusteval.dbscan as dbscan
-from clusteval.utils import init_logger, set_logger, compute_embedding
+from clusteval.utils import init_logger, set_logger, compute_embedding, normalize_size
 from clusteval.plot_dendrogram import plot_dendrogram
 import pypickle
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.cluster.hierarchy import linkage as scipy_linkage
 from scipy.cluster.hierarchy import fcluster
+from sklearn.preprocessing import StandardScaler
 from urllib.parse import urlparse
 import requests
 import os
 
 logger = init_logger()
 
 
@@ -55,14 +56,16 @@
             * 'weighted'
             * 'centroid'
             * 'median'
     min_clust : int, (default: 2)
         Number of clusters that is evaluated greater or equals to min_clust.
     max_clust : int, (default: 25)
         Number of clusters that is evaluated smaller or equals to max_clust.
+    normalize : bool (default : False)
+        Normalize data, Z-score
     savemem : bool, (default: False)
         Save memmory when working with large datasets. Note that htis option only in case of KMeans.
     jitter : float, default: None
         Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
     verbose : int, (default: 'info')
         Print progress to screen. The default is 'info'.
         60: None, 40: Error, 30: Warn, 20: Info, 10: Debug
@@ -85,30 +88,30 @@
     >>> # Fit best clusters
     >>> results = ce.fit(X)
     >>>
     >>> # Make plot
     >>> ce.plot()
     >>>
     >>> # silhouette plot
-    >>> ce.plot_silhouette(X)
+    >>> ce.plot_silhouette()
     >>>
     >>> # Scatter plot
-    >>> ce.scatter(X)
+    >>> ce.scatter()
     >>>
     >>> # Dendrogram
     >>> ce.dendrogram()
 
     """
 
-    def __init__(self, cluster='agglomerative', evaluate='silhouette', metric='euclidean', linkage='ward', min_clust=2, max_clust=25, savemem=False, verbose='info', params_dbscan={'eps': None, 'epsres': 50, 'min_samples': 0.01, 'norm': False, 'n_jobs': -1}):
+    def __init__(self, cluster='agglomerative', evaluate='silhouette', metric='euclidean', linkage='ward', min_clust=2, max_clust=25, normalize=False, savemem=False, verbose='info', params_dbscan={'eps': None, 'epsres': 50, 'min_samples': 0.01, 'norm': False, 'n_jobs': -1}):
         """Initialize clusteval with user-defined parameters."""
         if ((min_clust is None) or (min_clust<2)):
             min_clust=2
         if ((max_clust is None) or (max_clust<min_clust)):
-            max_clust=min_clust + 1
+            max_clust = min_clust + 1
 
         if not np.any(np.isin(evaluate, ['silhouette', 'dbindex', 'derivative'])): raise ValueError("evaluate has incorrect input argument [%s]." %(evaluate))
         if not np.any(np.isin(cluster, ['agglomerative', 'kmeans', 'dbscan', 'hdbscan'])): raise ValueError("cluster has incorrect input argument [%s]." %(cluster))
         if cluster=='kmeans' and evaluate=='dbindex':
             logger.error("kmeans can not be combined with dbindex.")
 
         # Set parameters for dbscan
@@ -120,14 +123,15 @@
         self.evaluate = evaluate
         self.cluster = cluster
         self.metric = metric
         self.linkage = linkage
         self.min_clust = min_clust
         self.max_clust = max_clust
         self.savemem = savemem
+        self.normalize = normalize
         self.verbose = verbose
         # Set the logger
         set_logger(verbose=verbose)
 
     # Fit
     def fit(self, X, savemem=False):
         """Cluster validation.
@@ -154,16 +158,23 @@
 
         """
         if self.evaluate=='dbindex' and (self.cluster=='kmeans'):
             logger.warning('Cluster evaluation [%s] can not per performed for [%s] <return>' %(self.evaluate, self.cluster))
             self.results = None
             return None
 
+        # normalize data
+        if self.normalize:
+            logger.info('Normalizing input data per feature (zero mean and unit variance)')
+            scaler = StandardScaler(with_mean=True, with_std=True).fit(X)
+            X = scaler.transform(X)
+
         # Store the input data in self
         if not savemem:
+            logger.info('Saving data in memory.')
             self.X = X.copy()
 
         if isinstance(X, pd.DataFrame): X = X.values
         if 'array' not in str(type(X)): raise ValueError('Input data must be of type numpy array')
         max_d, max_d_lower, max_d_upper = None, None, None
         self.Z = []
 
@@ -173,15 +184,15 @@
         # Compute linkages
         if self.cluster!='kmeans':
             self.Z = scipy_linkage(X, method=self.linkage, metric=self.metric)
 
         # Choosing method
         if (self.cluster=='agglomerative') or (self.cluster=='kmeans'):
             if self.evaluate=='silhouette':
-                self.results = silhouette.fit(X, Z=self.Z, cluster=self.cluster, metric=self.metric, min_clust=self.min_clust, max_clust=self.max_clust, savemem=self.savemem, verbose=self.verbose)
+                self.results = silhouette.fit(X, Z=self.Z, cluster=self.cluster, metric=self.metric, linkage=self.linkage, min_clust=self.min_clust, max_clust=self.max_clust, savemem=self.savemem, verbose=self.verbose)
             elif self.evaluate=='dbindex':
                 self.results = dbindex.fit(X, Z=self.Z, metric=self.metric, min_clust=self.min_clust, max_clust=self.max_clust, savemem=self.savemem, verbose=self.verbose)
             elif self.evaluate=='derivative':
                 self.results = derivative.fit(X, Z=self.Z, cluster=self.cluster, metric=self.metric, min_clust=self.min_clust, max_clust=self.max_clust, verbose=self.verbose)
         elif (self.cluster=='dbscan') and (self.evaluate=='silhouette'):
             self.results = dbscan.fit(X, eps=self.params_dbscan['eps'], epsres=self.params_dbscan['epsres'], min_samples=self.params_dbscan['min_samples'], metric=self.metric, norm=self.params_dbscan['norm'], n_jobs=self.params_dbscan['n_jobs'], min_clust=self.min_clust, max_clust=self.max_clust, verbose=self.verbose)
         elif self.cluster=='hdbscan':
@@ -306,23 +317,23 @@
             fig.savefig(**savefig)
 
         # Return
         return fig, ax
 
     def scatter(self,
                 X=None,
-                s=50,
+                s=25,
                 embedding=None,
                 n_feat=2,
                 legend=False,
                 jitter=None,
                 cmap='tab20c',
                 figsize=(25, 15),
-                fontsize=18,
-                fontcolor=[0,0,0],
+                fontsize=16,
+                fontcolor='k',
                 savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'},
                 showfig=True,
                 ):
         """Scatterplot.
 
         Create a scatterplot for the first two features or with an t-SNE embedding.
         The clusters are colored based on the cluster labels and labeld with the features from the enrichment analysis.
@@ -384,60 +395,64 @@
         """
         # Make some checks
         if not _check_results(self, logger): return None
         X = _check_input_data(self, X, logger)
         if X is None: return None
         if isinstance(X, pd.DataFrame): X = X.values
 
-        # Compute embedding
-        X = compute_embedding(X, embedding, logger)
-
         # Defaults
-        defaults = {'figsize': (25, 15), 'cmap': 'tab20c', 'z': None, 'c': [0, 0, 0], 'marker': None, 'alpha': None, 'gradient': None, 'density': False, 'norm': False, 'xlabel': 'x-axis', 'ylabel': 'y-axis', 'title': '', 'fontsize': 20, 'fontcolor': None, 'axiscolor': '#dddddd', 'jitter': None}
+        defaults = {'figsize': (25, 15), 'cmap': 'tab20c', 'z': None, 'c': [0, 0, 0], 'marker': None, 'alpha': 0.8, 'gradient': None, 'density': False, 'norm': False, 'xlabel': 'x-axis', 'ylabel': 'y-axis', 'title': '', 'fontsize': 20, 'fontcolor': None, 'axiscolor': '#dddddd', 'jitter': None}
         params = {**defaults, **{'jitter': jitter, 'cmap': cmap}, 'figsize': figsize, 'fontsize': fontsize, 'fontcolor': fontcolor}
 
+        # Compute embedding
+        X = compute_embedding(self, X, embedding, logger)
+
         if self.results.get('enrichment') is None:
             labels = self.results['labx']
             scores = np.ones(X.shape[0]) * s
         else:
             # For each cluster, add the most important feature.
             labels = np.repeat('', X.shape[0]).astype('O')
-            scores = np.ones(X.shape[0]) * 25
+            scores = np.ones(X.shape[0]) * s
             for y in self.results['enrichment']['y'].unique():
                 Iloc = self.results['enrichment']['y']==y
                 tmpdf = self.results['enrichment'].loc[Iloc, :].sort_values('logP')[0: n_feat]
                 catname = list(tmpdf['category_name'].values)
                 catlab = list(tmpdf['category_label'].values)
                 label = [catname[i] + ' (' + catlab[i] + ')' for i in range(len(catname))]
+                label = ['cluster ' + str(int(y))] + label
                 label = '\n'.join(label)
                 # Compute maximum
-                score = np.max(tmpdf['logP'].values * -1)
+                # score = np.mean(tmpdf['logP'].values * -1)
                 # Store
                 labels[self.results['labx']==int(y)] = label
-                scores[self.results['labx']==int(y)] = score
+                # scores[self.results['labx']==int(y)] = score
+            # Normalize scores
+            # scores = normalize_size(scores, minscale=25, maxscale=150)
 
         # Scatter
         fig, ax = scatterd(X[:, 0], X[:, 1], labels=labels, s=scores, legend=legend, **params)
         # Save figure
         if (savefig['fname'] is not None) and (fig is not None):
             logger.info('Saving silhouetteplot to [%s]' %(savefig['fname']))
             fig.savefig(**savefig)
 
         # if d3blocks and  _check_import_d3blocks:
         #     from d3blocks import D3Blocks
         #     d3 = D3Blocks()
         #     d3.scatter(X[:, 0], X[:, 1], jitter=jitter, size=scores/10, tooltip=labels, cmap=cmap, color=self.results['labx'].astype(str))
 
         # Return
+        if embedding: self.results['xycoord'] = X
         return fig, ax
 
     # Plot
     def plot_silhouette(self,
                 X=None,
-                dot_size=75,
+                dot_size=25,
                 jitter=None,
                 embedding=None,
                 cmap='tab20c',
                 figsize=(15, 8),
                 savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'},
                 showfig=True,
                 ):
@@ -476,25 +491,29 @@
 
         """
         if not _check_results(self, logger): return None
         X = _check_input_data(self, X, logger)
         if X is None: return None
         if isinstance(X, pd.DataFrame): X = X.values
 
+        # Compute embedding
+        X = compute_embedding(self, X, embedding, logger)
+
         # Make scatterplot
         fig, ax1, ax2 = silhouette.scatter(self.results,
                                            X=X,
                                            dot_size=dot_size,
                                            jitter=jitter,
                                            cmap=cmap,
                                            embedding=embedding,
                                            figsize=figsize,
                                            showfig=showfig,
                                            savefig=savefig)
         # Return
+        if embedding: self.results['xycoord'] = X
         return fig, ax1, ax2
 
     # Plot dendrogram
     def dendrogram(self,
                    X=None,
                    labels=None,
                    leaf_rotation=90,
@@ -502,14 +521,15 @@
                    orientation='top',
                    show_contracted=True,
                    max_d=None,
                    showfig=True,
                    metric=None,
                    linkage=None,
                    truncate_mode=None,
+                   update_results = False,
                    figsize=(15, 10),
                    savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'},
                    ):
         """Plot Dendrogram.
 
         Parameters
         ----------
@@ -556,14 +576,18 @@
             * order_rows : string : Order of the cluster labels as presented in the dendrogram (left-to-right).
             * max_d : float : maximum distance to set the horizontal threshold line.
             * max_d_lower : float : maximum distance lowebound
             * max_d_upper : float : maximum distance upperbound
 
         """
         if not _check_results(self, logger): return None
+        X = _check_input_data(self, X, logger)
+        if X is None: return None
+        if isinstance(X, pd.DataFrame): X = X.values
+
         # Set parameters
         no_plot = False if showfig else True
         max_d_lower, max_d_upper = None, None
 
         # Check whether
         if (metric is not None) and (linkage is not None) and (X is not None):
             logger.warning('Compute dendrogram using metric=%s, linkage=%s' %(metric, linkage))
@@ -590,14 +614,16 @@
             max_d_lower = self.results['max_d_lower']
             max_d_upper = self.results['max_d_upper']
 
         # Make the dendrogram
         if showfig:
             fig, ax = plt.subplots(figsize=figsize)
         annotate_above = max_d
+
+        # Make the dendrogram
         results = plot_dendrogram(Z, labels=labels, leaf_rotation=leaf_rotation, leaf_font_size=leaf_font_size, orientation=orientation, show_contracted=show_contracted, annotate_above=annotate_above, max_d=max_d, truncate_mode=truncate_mode, ax=ax, no_plot=no_plot)
 
         # Compute cluster labels
         logger.info('Compute cluster labels.')
         labx = fcluster(Z, max_d, criterion='distance')
 
         # Store results
@@ -609,14 +635,23 @@
         results['ax'] = ax
 
         # Save figure
         if (savefig['fname'] is not None) and (fig is not None):
             logger.info('Saving dendrogram: [%s]' %(savefig['fname']))
             fig.savefig(**savefig)
 
+        if update_results:
+            logger.info('Updating results.')
+            self.results['order_rows'] = results['order_rows']
+            self.results['labx'] = results['labx']
+            self.results['max_d'] = results['max_d']
+            self.results['max_d_lower'] = results['max_d_lower']
+            self.results['max_d_upper'] = results['max_d_upper']
+            self.results['ax'] = results['ax']
+
         return results
 
     def save(self, filepath='clusteval.pkl', overwrite=False):
         """Save model in pickle file.
 
         Parameters
         ----------
@@ -673,24 +708,24 @@
         """Import example dataset from github source.
 
         Import one of the few datasets from github source or specify your own download url link.
 
         Parameters
         ----------
         data : str
-            * 'blobs'
-            * 'moons'
-            * 'circles'
-            * 'anisotropic'
-            * 'globular'
-            * 'uniform'
-            * 'densities'
-            * 'sprinkler'
-            * 'titanic'
-            * 'student'
+            * 'blobs' (numeric)
+            * 'moons' (numeric)
+            * 'circles' (numeric)
+            * 'anisotropic' (numeric)
+            * 'globular' (numeric)
+            * 'uniform' (numeric)
+            * 'densities' (numeric)
+            * 'sprinkler' (categorical)
+            * 'titanic' (mixed)
+            * 'student' (categorical)
             * 'fifa'
             * 'cancer'
             * 'waterpump'
             * 'retail'
             * 'breast'
             * 'iris'
         url : str
@@ -864,14 +899,15 @@
         with open(writepath, "wb") as fd:
             for chunk in r.iter_content(chunk_size=1024):
                 fd.write(chunk)
 
 
 def _check_input_data(self, X, logger):
     if X is None and hasattr(self, 'X'):
+        logger.info('Retrieving input data set.')
         X = self.X.copy()
     elif X is None and not hasattr(self, 'X'):
         logger.error('Input data set is required <return>')
         X = None
     return X
```

### Comparing `clusteval-2.1.6/clusteval/coord2density.py` & `clusteval-2.2.0/clusteval/coord2density.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/clusteval/dbindex.py` & `clusteval-2.2.0/clusteval/dbindex.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/clusteval/dbscan.py` & `clusteval-2.2.0/clusteval/dbscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,14 @@
         ax2.axvline(x=results['fig']['eps'][idx], ymin=0, ymax=results['fig']['sillclust'][idx], linewidth=1, color='r', linestyle='--')
         ax2.axhline(y=len(np.unique(results['labx'])), xmin=0, xmax=1, linewidth=1.5, color='r', linestyle='--')
 
     ax2.tick_params(axis='x', labelsize=font_properties['size_x_axis'])
     ax2.tick_params(axis='y', labelsize=font_properties['size_y_axis'], labelcolor='b')
     ax2.plot(results['fig']['eps'], results['fig']['sillclust'], color='b')
     ax2.set_ylabel('Nr. Clusters', fontsize=font_properties['size_y_axis'], color='b')
-    title2 = "Gridsearch on Epsilon. Optimal nr. clusters: %d" %(len(np.unique(results['labx'])))
-    ax2.set_title(title2, fontsize=font_properties['size_title'])
+    # title2 = "Gridsearch on Epsilon. Optimal nr. clusters: %d" %(len(np.unique(results['labx'])))
+    ax2.set_title(title, fontsize=font_properties['size_title'])
 
     if showfig:
         plt.show()
     # Return
     return (fig, (ax, ax2))
```

### Comparing `clusteval-2.1.6/clusteval/derivative.py` & `clusteval-2.2.0/clusteval/derivative.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/clusteval/examples.py` & `clusteval-2.2.0/clusteval/examples.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,126 @@
 # EXAMPLE
+# import sys
+# sys.path.insert(1, 'D:/REPOS/clusteval/clusteval/')
 from sklearn.datasets import make_blobs
 import matplotlib.pyplot as plt
 from clusteval import clusteval
 
 # import clusteval
 # print(clusteval.__version__)
 # print(dir(clusteval))
 
+# %%
+from df2onehot import df2onehot
+from clusteval import clusteval
+
+# url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/00519/heart_failure_clinical_records_dataset.csv'
+url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/00468/online_shoppers_intention.csv'
+ce = clusteval()
+df = ce.import_example(url=url)
+# df = ce.import_example(data='waterpump')
+
+# Set the following columns as floating type
+# df.drop(labels=['id', 'date_recorded'], axis=1, inplace=True)
+# cols_as_float = ['ProductRelated', 'Administrative']
+# df[cols_as_float]=df[cols_as_float].astype(float)
+dfhot = df2onehot(df,
+                  excl_background=['0.0', 'None', '?', 'False'],
+                  y_min=50,
+                  perc_min_num=0.8,
+                  remove_mutual_exclusive=True,
+                  verbose=4)['onehot']
+
+ce = clusteval(evaluate='silhouette',
+               cluster='agglomerative',
+               metric='hamming',
+               linkage='complete',
+               min_clust=2,
+               normalize=False,
+               verbose='info')
+# ce = clusteval(cluster='dbscan', metric='hamming', linkage='complete', min_clust=2, verbose='info')
+
+ce.fit(dfhot)
+ce.plot()
+ce.plot_silhouette()
+ce.plot_silhouette(embedding='tsne')
+ce.scatter(embedding='tsne', fontsize=26)
+ce.dendrogram()
+
+ce.enrichment(df)
+ce.scatter(embedding='tsne', n_feat=3, fontcolor=None, fontsize=12)
+ce.scatter(embedding='tsne', n_feat=3, fontcolor='k', fontsize=12)
+# scatterd(ce.results['xycoord'][:,0], ce.results['xycoord'][:,1], labels=df['Browser'], fontcolor='k', cmap='tab20c')
+
+
+from sklearn.manifold import TSNE
+xycoord = TSNE(n_components=2, init='random', perplexity=30).fit_transform(dfhot.values)
+# ce = clusteval(cluster='dbscan', min_clust=2, verbose='info')
+ce = clusteval(evaluate='silhouette', cluster='agglomerative', linkage='complete', min_clust=5, max_clust=30, verbose='info')
+ce.fit(xycoord)
+
+ce.plot()
+ce.plot_silhouette()
+ce.scatter()
+ce.enrichment(df)
+ce.scatter(fontcolor='k', n_feat=2)
+
+from scatterd import scatterd
+# scatterd(xycoord[:,0], xycoord[:,1], labels=ce.results['labx'], cmap='tab20c')
+scatterd(xycoord[:,0], xycoord[:,1], labels=df['Browser'], fontcolor='k', cmap='tab20c')
+scatterd(xycoord[:,0], xycoord[:,1], labels=dfhot['TrafficType_11.0'], fontcolor='k', cmap='tab20c')
+scatterd(xycoord[:,0], xycoord[:,1], labels=dfhot['Browser_2.0'], fontcolor='k', cmap='tab20c')
+
+
 # %% Imort own data 
 from df2onehot import df2onehot
 from clusteval import clusteval
 ce = clusteval()
 
 url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
 df = ce.import_example(url=url)
+df = df.iloc[0:1000, :]
+
 # Add column names
 df.columns=['age','workclass','fnlwgt','education','education-num','marital-status','occupation','relationship','race','sex','capital-gain','capital-loss','hours-per-week','native-country','earnings']
 # Set the following columns as floating type
-cols_as_float = ['age','hours-per-week','capital-loss','capital-gain', 'fnlwgt']
+df.drop(labels=['fnlwgt', 'marital-status', 'education-num'], axis=1, inplace=True)
+cols_as_float = ['age','hours-per-week','capital-loss','capital-gain']
 df[cols_as_float]=df[cols_as_float].astype(float)
-dfhot = df2onehot(df, excl_background=['0.0', 'None'], verbose=4)['onehot']
+dfhot = df2onehot(df, hot_only=True, excl_background=['0.0', 'None', '?', 'False'], perc_min_num=0.8, remove_mutual_exclusive=True, verbose=4)['onehot']
+
+ce = clusteval(cluster='agglomerative', metric='hamming', linkage='complete', min_clust=10, max_clust=25, verbose='info')
+ce = clusteval(cluster='agglomerative', metric='euclidean', linkage='complete', min_clust=7, normalize=True, verbose='info')
+ce = clusteval(cluster='dbscan', metric='euclidean', linkage='complete', min_clust=7, normalize=True, verbose='info')
+ce = clusteval(evaluate='dbindex', cluster='agglomerative', metric='hamming', linkage='complete', min_clust=7, normalize=False, verbose='info')
+ce = clusteval(evaluate='dbindex', cluster='agglomerative', metric='euclidean', linkage='complete', min_clust=7, normalize=True, verbose='info')
+
+# fig, axs = plt.subplots(2,4, figsize=(25,10))
 
-ce = clusteval(cluster='agglomerative', metric='hamming', linkage='complete', min_clust=7, verbose='info')
 ce.fit(dfhot);
 ce.plot()
-ce.scatter(jitter=0.01)
+ce.plot_silhouette(embedding='tsne')
+ce.scatter(embedding='tsne', fontcolor='k')
+ce.dendrogram()
+ce.dendrogram(max_d=0.125)
+ce.scatter(embedding='tsne')
+
+
+ce.enrichment(df)
+ce.scatter(embedding='tsne', fontcolor='k')
 
 from pca import pca
 model = pca()
 xycoord = model.fit_transform(dfhot)['PC'].values
-ce.scatter(xycoord, jitter=0.05)
-
-from sklearn.manifold import TSNE
-xycoord = TSNE(n_components=2, init='random').fit_transform(dfhot)
 ce.scatter(xycoord)
-ce.enrichment()
+
+from scatterd import scatterd
+scatterd(xycoord[:,0], xycoord[:,1], labels=ce.results['labx']==16)
+scatterd(xycoord[:,0], xycoord[:,1], labels=dfhot['Sex_female'])
+
 
 # %% Enrichment analysis
 
 from df2onehot import df2onehot
 from clusteval import clusteval
 
 ce = clusteval()
@@ -47,27 +129,29 @@
 df.drop(labels=['Survived', 'Name', 'Age', 'PassengerId', 'Ticket', 'Fare', 'Cabin'], axis=1, inplace=True)
 dfhot = df2onehot(df, excl_background=['0.0', 'None'], verbose=4)['onehot']
 X = dfhot.values
 
 ce = clusteval(cluster='agglomerative', metric='hamming', linkage='complete', min_clust=7, verbose='info')
 # ce = clusteval(cluster='agglomerative', linkage='complete', min_clust=7, max_clust=40, verbose='info')
 # ce = clusteval(cluster='dbscan', linkage='complete', min_clust=7, max_clust=40, verbose='info')
-# ce = clusteval(cluster='dbscan', metric='hamming', linkage='complete', min_clust=7, verbose='info')
+# ce = clusteval(cluster='dbscan', linkage='complete', min_clust=7, verbose='info')
 ce.fit(dfhot);
 ce.plot()
 ce.scatter()
 ce.scatter(embedding='tsne')
 ce.enrichment(df)
-ce.scatter(embedding='tsne')
+ce.scatter(embedding='tsne', fontcolor='k')
 
 from pca import pca
 model = pca()
 xycoord = model.fit_transform(X)['PC'].values
 ce.scatter(X=xycoord)
 
+from scatterd import scatterd
+scatterd(ce.results['xycoord'][:,0], ce.results['xycoord'][:,1], labels=df['Embarked'].astype(str))
 
 from scatterd import scatterd
 scatterd(xycoord[:,0], xycoord[:,1], labels=ce.results['labx']==16)
 scatterd(xycoord[:,0], xycoord[:,1], labels=dfhot['Sex_female'])
 
 # %%
 # Import library
@@ -124,44 +208,41 @@
 
 # %%
 import clusteval
 from scatterd import scatterd
 import numpy as np
 
 X, y = ce.import_example(data='blobs', params={'random_state': 1})
+# X, y = datasets.make_circles(n_samples=n_samples, factor=0.5, noise=0.05)
 
 plt.figure(figsize=(15,10))
-plt.scatter(X[:,0], X[:,1])
 plt.grid(True); plt.xlabel('Feature 1'); plt.ylabel('Feature 2')
 
-# X, y = datasets.make_circles(n_samples=n_samples, factor=0.5, noise=0.05)
-
-scatterd(X[:,0], X[:,1],labels=y, figsize=(15, 10))
-
 plt.figure()
 fig, axs = plt.subplots(2,4, figsize=(25,10))
+font_properties={'size_x_axis': 12, 'size_y_axis': 12}
 
 # dbindex
-results = clusteval.dbindex.fit(X)
-_ = clusteval.dbindex.plot(results, title='dbindex', ax=axs[0][0], showfig=False)
+results = clusteval.dbindex.fit(X, max_clust=10)
+_ = clusteval.dbindex.plot(results, title='dbindex', ax=axs[0][0], showfig=False, font_properties=font_properties)
 axs[1][0].scatter(X[:,0], X[:,1],c=results['labx']);axs[1][0].grid(True)
 
 # silhouette
 results = clusteval.silhouette.fit(X)
-_ = clusteval.silhouette.plot(results, title='silhouette', ax=axs[0][1], showfig=False)
+_ = clusteval.silhouette.plot(results, title='silhouette', ax=axs[0][1], showfig=False, font_properties=font_properties)
 axs[1][1].scatter(X[:,0], X[:,1],c=results['labx']);axs[1][1].grid(True)
 
 # derivative
 results = clusteval.derivative.fit(X)
-_ = clusteval.derivative.plot(results, title='derivative', ax=axs[0][2], showfig=False)
+_ = clusteval.derivative.plot(results, title='derivative', ax=axs[0][2], showfig=False, font_properties=font_properties)
 axs[1][2].scatter(X[:,0], X[:,1],c=results['labx']);axs[1][2].grid(True)
 
 # dbscan
 results = clusteval.dbscan.fit(X)
-_ = clusteval.dbscan.plot(results, title='dbscan', ax=axs[0][3], showfig=False)
+_ = clusteval.dbscan.plot(results, title='dbscan', ax=axs[0][3], showfig=False, font_properties=font_properties)
 axs[1][3].scatter(X[:,0], X[:,1],c=results['labx']);axs[1][3].grid(True)
 
 # results = clusteval.hdbscan.fit(X)
 # _ = clusteval.dbscan.plot(results, title='dbscan', ax=axs[0][3], showfig=False)
 # axs[1][3].scatter(X[:,0], X[:,1],c=results['labx']);axs[1][3].grid(True)
 
 
@@ -225,27 +306,27 @@
 df.drop(labels=['Fouls Committed', 'Date', 'Passes', 'Ball Possession %', 'Distance Covered (Kms)', 'Pass Accuracy %', 'Free Kicks', 'Attempts'], axis=1, inplace=True)
 X = df2onehot(df, excl_background=['0.0', 'NaN', 'nan'], verbose=4)['onehot'].values
 
 df = ce.import_example(data='retail')
 df.drop(labels=['CustomerID', 'InvoiceNo', 'StockCode', 'Country', 'InvoiceDate', 'UnitPrice'], axis=1, inplace=True)
 X = df2onehot(df, excl_background=['0.0', 'NaN', 'nan'], verbose=4)['onehot'].values
 
-
 df = ce.import_example(data='titanic')
 df.drop(labels=['Name', 'Age', 'PassengerId', 'Ticket', 'Fare', 'Cabin'], axis=1, inplace=True)
 X = df2onehot(df, excl_background=['0.0', 'NaN', 'nan'], verbose=4)['onehot'].values
 
 from clusteval import clusteval
 ce = clusteval(cluster='agglomerative', metric='hamming', linkage='complete', min_clust=7, verbose=3)
 ce = clusteval(cluster='agglomerative', metric='euclidean', linkage='complete', min_clust=7, verbose=3)
-# ce = clusteval(cluster='dbscan', metric='hamming', linkage='complete', min_clust=7, verbose=3)
+ce = clusteval(cluster='dbscan', metric='euclidean', linkage='complete', min_clust=7, verbose=3)
 results = ce.fit(X)
 ce.plot()
 ce.scatter(embedding='tsne')
-ce.plot_silhouette(jitter=0.01)
+ce.plot_silhouette(embedding='tsne')
+ce.enrichment(df)
 
 from pca import pca
 model = pca()
 xycoord = model.fit_transform(X)['PC'].values
 ce.scatter(xycoord[:, :2], jitter=0.01)
 
 # %%
@@ -392,15 +473,16 @@
 lsa = make_pipeline(svd, normalizer)
 X = lsa.fit_transform(X)
 
 from clusteval import clusteval
 ce = clusteval(cluster='dbscan')
 ce.fit(X)
 ce.plot()
-ce.scatter(X)
+ce.plot_silhouette(embedding='tsne')
+ce.scatter(embedding='tsne')
 ce.dendrogram(labels=corpus)
 
 # %% Generate dataset
 X, labels_true = make_blobs(n_samples=50, centers=[[1, 1], [-1, -1], [1, -1]], cluster_std=0.4,random_state=0)
 # [X, labels_true] = make_blobs(n_samples=750, centers=[[1, 1], [-1, -1], [1, -1], [-1, 1]], cluster_std=0.4,random_state=0)
 # X, labels_true = make_blobs(n_samples=750, centers=4, n_features=6, cluster_std=0.5)
 # X, labels_true = make_blobs(n_samples=750, centers=6, n_features=10)
@@ -486,14 +568,15 @@
 # for i in zip(results['labx'], results_dendro['labx']):
 #     assert np.all(np.logical_and(np.where(results['labx']==i[0])[0]+1, np.where(results_dendro['labx']==i[1])[0]+1))
 
 # %% Directly use the dbindex method
 import clusteval
 from sklearn.datasets import make_blobs
 import matplotlib.pyplot as plt
+
 X, labels_true = make_blobs(n_samples=750, centers=4, n_features=10)
 
 
 X, labx = make_blobs(n_samples=200, n_features=2, centers=2, random_state=1)
 c = np.random.multivariate_normal([40, 40], [[20, 1], [1, 30]], size=[200,])
 d = np.random.multivariate_normal([80, 80], [[30, 1], [1, 30]], size=[200,])
 e = np.random.multivariate_normal([0, 100], [[200, 1], [1, 100]], size=[200,])
```

### Comparing `clusteval-2.1.6/clusteval/hdbscan.py` & `clusteval-2.2.0/clusteval/hdbscan.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/clusteval/plot_dendrogram.py` & `clusteval-2.2.0/clusteval/plot_dendrogram.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.6/clusteval/silhouette.py` & `clusteval-2.2.0/clusteval/silhouette.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,16 +274,16 @@
     """
     font_properties = set_font_properties(font_properties)
     fig, ax1, ax2 = None, None, None
     if X is None:
         logger.warning('Input data X is required for the scatterplot.')
         return None
 
-    # Compute embedding
-    X = compute_embedding(X, embedding, logger)
+    # # Compute embedding
+    # X = compute_embedding(y, X, embedding, logger)
 
     if X.shape[1]>2:
         logger.info('Scatterplot is performed on the first two dimensions of input data X.')
         X = X[:, :2]
 
     # Extract label from dict
     if isinstance(y, dict):
```

### Comparing `clusteval-2.1.6/clusteval/tests/test_clusteval.py` & `clusteval-2.2.0/clusteval/tests/test_clusteval.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import unittest
 import matplotlib.pyplot as plt
 
 
 class TestCLUSTEVAL(unittest.TestCase):
 
-    def test_different_X():
+    def test_different_X(self):
         ce = clusteval()
         
         # Generate random data
         X1, y1 = ce.import_example(data='circles')
         X2, y2 = ce.import_example(data='moons')
         X3, y3 = ce.import_example(data='anisotropic')
         X4, y4 = ce.import_example(data='densities')
@@ -89,40 +89,40 @@
 
     for cluster in clusters:
         for evaluate in evaluates:
             for metric in metrics:
                 for linkage in linkages:
                     for min_clust in min_clusts:
                         for max_clust in max_clusts:
-                            print(cluster)
-                            print(evaluate)
-                            print(metric)
-                            print(linkage)
-                            print(min_clust)
-                            print(max_clust)
+                            # print(cluster)
+                            # print(evaluate)
+                            # print(metric)
+                            # print(linkage)
+                            # print(min_clust)
+                            # print(max_clust)
 
                             # cluster='agglomerative'
                             # evaluate='dbindex'
                             # metric='euclidean'
                             # linkage='complete'
                             # min_clust=1
                             # max_clust=10
 
                             try:
                                 status = 'OK'
-                                ce = clusteval(evaluate=evaluate, cluster=cluster, metric=metric, linkage=linkage, min_clust=min_clust, max_clust=max_clust, verbose=3)
+                                ce = clusteval(evaluate=evaluate, cluster=cluster, metric=metric, linkage=linkage, min_clust=min_clust, max_clust=max_clust, verbose=2)
                                 results = ce.fit(X)
                                 # print('Clusters: %s' %(str(np.unique(results['labx']))))
                                 # assert ce.plot()
                                 # assert ce.scatter(X)
                                 # assert ce.dendrogram()
 
                                 if (ce.results is not None) and (ce.results['labx'] is not None) and (linkage!='single') and (min_clust < len(np.unique(y_true))) and (max_clust > len(np.unique(y_true))) and (metric=='euclidean'):
-                                    print(len(np.unique(results['labx'])))
-                                    print(len(np.unique(y_true)))
+                                    # print(len(np.unique(results['labx'])))
+                                    # print(len(np.unique(y_true)))
                                     assert len(np.unique(results['labx']))==len(np.unique(y_true))
 
                             except ValueError as err:
                                 assert not 'clusteval' in err.args
                                 status = err.args
                                 print(err.args)
                                 # ce.results=None
```

### Comparing `clusteval-2.1.6/clusteval.egg-info/PKG-INFO` & `clusteval-2.2.0/clusteval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.1.6
+Version: 2.2.0
 Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.1.6.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.2.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clusteval
+<p align="center">
+  <a href="https://erdogant.github.io/clusteval">
+  <img src="https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png" width="300" />
+  </a>
+</p>
 
 [![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval)
 [![PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE)
 [![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)
 [![Github Forks](https://img.shields.io/github/forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
 [![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/issues)
```

#### html2text {}

```diff
@@ -1,53 +1,55 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.1.6 Summary: clusteval is a
+Metadata-Version: 2.1 Name: clusteval Version: 2.2.0 Summary: clusteval is a
 python package for unsupervised cluster validation. Home-page: https://
 erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
-clusteval/archive/2.1.6.tar.gz Author: Erdogan Taskesen Author-email:
+clusteval/archive/2.2.0.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # clusteval [![Python](https://img.shields.io/pypi/
-pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [!
-[PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/
-project/clusteval/) [![License](https://img.shields.io/badge/license-MIT-
-green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE) [!
-[BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://
-www.buymeacoffee.com/erdogant) [![Github Forks](https://img.shields.io/github/
-forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
-[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
-clusteval.svg)](https://github.com/erdogant/clusteval/issues) [![Project
-Status](http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/clusteval/
-month)](https://pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/
-badge/clusteval)](https://pepy.tech/project/clusteval) [![DOI](https://
-zenodo.org/badge/232915924.svg)](https://zenodo.org/badge/latestdoi/232915924)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/clusteval/) [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
-clusteval/pages/html/Documentation.html#colab-notebook)  ``clusteval`` is a
-python package that is developed to evaluate detected clusters and return the
-cluster labels that have most optimal **clustering tendency**, **Number of
-clusters** and **clustering quality**. Multiple evaluation strategies are
-implemented for the evaluation; **silhouette**, **dbindex**, and
-**derivative**, and four clustering methods can be used: **agglomerative**,
-**kmeans**, **dbscan** and **hdbscan**. # **â­ï¸ Star this repo if you like
-it â­ï¸** # ### Blogs Read the blog to get a structured overview how you can
-use ``clusteval``. * [Medium Blog: A step-by-step guide for clustering images]
-(https://towardsdatascience.com/a-step-by-step-guide-for-clustering-images-
-4b45f9906128) In case you want to detect identical images, you can also use
-hash functionalities. * [Medium Blog: Detection of Duplicate Images Using Image
-Hash Functions](https://towardsdatascience.com/detection-of-duplicate-images-
-using-image-hash-functions-4d9c53f04a75) # ### [Documentation pages](https://
-erdogant.github.io/clusteval/) On the [documentation pages](https://
-erdogant.github.io/clusteval/) you can find detailed information about the
-working of the ``clusteval`` with many examples. # ### Installation ##### It is
-advisable to create a new environment (e.g. with Conda). ```bash conda create -
-n env_clusteval python=3.8 conda activate clusteval ``` ##### Install from PyPI
-```bash pip install clusteval ``` ##### Import library ```python from clusteval
-import clusteval ```
+License-File: LICENSE # clusteval
+[https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png]
+[![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://
+img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
+img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/) [!
+[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
+github.com/erdogant/clusteval/blob/master/LICENSE) [![BuyMeCoffee](https://
+img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/
+erdogant) [![Github Forks](https://img.shields.io/github/forks/erdogant/
+clusteval.svg)](https://github.com/erdogant/clusteval/network) [![GitHub Open
+Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://
+github.com/erdogant/clusteval/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/clusteval/month)](https://
+pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/badge/clusteval)]
+(https://pepy.tech/project/clusteval) [![DOI](https://zenodo.org/badge/
+232915924.svg)](https://zenodo.org/badge/latestdoi/232915924) [![Sphinx](https:
+//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+clusteval/) [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://erdogant.github.io/clusteval/pages/html/
+Documentation.html#colab-notebook)  ``clusteval`` is a python package that is
+developed to evaluate detected clusters and return the cluster labels that have
+most optimal **clustering tendency**, **Number of clusters** and **clustering
+quality**. Multiple evaluation strategies are implemented for the evaluation;
+**silhouette**, **dbindex**, and **derivative**, and four clustering methods
+can be used: **agglomerative**, **kmeans**, **dbscan** and **hdbscan**. #
+**â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read the blog to
+get a structured overview how you can use ``clusteval``. * [Medium Blog: A
+step-by-step guide for clustering images](https://towardsdatascience.com/a-
+step-by-step-guide-for-clustering-images-4b45f9906128) In case you want to
+detect identical images, you can also use hash functionalities. * [Medium Blog:
+Detection of Duplicate Images Using Image Hash Functions](https://
+towardsdatascience.com/detection-of-duplicate-images-using-image-hash-
+functions-4d9c53f04a75) # ### [Documentation pages](https://erdogant.github.io/
+clusteval/) On the [documentation pages](https://erdogant.github.io/clusteval/
+) you can find detailed information about the working of the ``clusteval`` with
+many examples. # ### Installation ##### It is advisable to create a new
+environment (e.g. with Conda). ```bash conda create -n env_clusteval python=3.8
+conda activate clusteval ``` ##### Install from PyPI ```bash pip install
+clusteval ``` ##### Import library ```python from clusteval import clusteval
+```
 ===============================================================================
 ### Examples A structured overview of all examples are now available on the
 [documentation pages](https://erdogant.github.io/clusteval/).
 ===============================================================================
 * [Example: Cluster validation using Silhouette score](https://
 erdogant.github.io/clusteval/pages/html/Examples.html#cluster-evaluation)
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/fig1b_sil.png]
```

### Comparing `clusteval-2.1.6/clusteval.egg-info/SOURCES.txt` & `clusteval-2.2.0/clusteval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 clusteval/__init__.py
+clusteval/bubblegrid.py
 clusteval/clusteval.py
 clusteval/coord2density.py
 clusteval/dbindex.py
 clusteval/dbscan.py
 clusteval/derivative.py
 clusteval/examples.py
 clusteval/hdbscan.py
-clusteval/image2vec.py
 clusteval/plot_dendrogram.py
 clusteval/silhouette.py
 clusteval/utils.py
 clusteval.egg-info/PKG-INFO
 clusteval.egg-info/SOURCES.txt
 clusteval.egg-info/dependency_links.txt
 clusteval.egg-info/requires.txt
```

### Comparing `clusteval-2.1.6/setup.py` & `clusteval-2.2.0/setup.py`

 * *Files identical despite different names*

