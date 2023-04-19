# Comparing `tmp/Slpapy-0.1.15.tar.gz` & `tmp/Slpapy-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.15.tar", last modified: Tue Apr 18 09:58:50 2023, max compression
+gzip compressed data, was "Slpapy-0.1.17.tar", last modified: Wed Apr 19 06:20:25 2023, max compression
```

## Comparing `Slpapy-0.1.15.tar` & `Slpapy-0.1.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.626849 Slpapy-0.1.15/
--rw-rw-rw-   0        0        0      160 2023-04-18 09:58:50.625848 Slpapy-0.1.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.594848 Slpapy-0.1.15/Slpapy/
--rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.15/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.15/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.624848 Slpapy-0.1.15/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.1.15/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.1.15/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.1.15/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.1.15/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      259 2023-04-18 08:16:12.000000 Slpapy-0.1.15/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     4983 2023-04-18 08:26:03.000000 Slpapy-0.1.15/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.602849 Slpapy-0.1.15/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 09:58:50.626849 Slpapy-0.1.15/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-18 09:58:38.000000 Slpapy-0.1.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.862725 Slpapy-0.1.17/
+-rw-rw-rw-   0        0        0      160 2023-04-19 06:20:25.861724 Slpapy-0.1.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.825710 Slpapy-0.1.17/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.17/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.17/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.859725 Slpapy-0.1.17/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.1.17/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.1.17/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.1.17/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.1.17/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.1.17/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     4998 2023-04-18 10:22:59.000000 Slpapy-0.1.17/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.834711 Slpapy-0.1.17/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:20:25.862725 Slpapy-0.1.17/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-19 06:20:03.000000 Slpapy-0.1.17/setup.py
```

### Comparing `Slpapy-0.1.15/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.17/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.17/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/beats.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/logging.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.1.17/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.15/Slpapy/processing_analyze.py` & `Slpapy-0.1.17/Slpapy/processing_analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import anndata as ad
 import scanpy as sc
 from scipy.sparse import csr_matrix
 from sklearn import preprocessing
 from sklearn.cluster import KMeans
 import numpy as np
 from typing import Optional
-from Spatial_map import Spatial_map
+from .Spatial_map import Spatial_map
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
 
 
@@ -38,18 +38,18 @@
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
                  save='_total_counts.png')
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
-    sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
-    sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
-    adata.raw = adata
+    # 选择高变异基因
     if onlyhighly==True:
+        sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
+        sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
         adata = adata[:, adata.var.highly_variable]
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
     #保存mz值
     mz=adata.var
     mz.to_csv('mz.csv')
```

### Comparing `Slpapy-0.1.15/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.1.17/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

