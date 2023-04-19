# Comparing `tmp/SpaGCN-1.2.5.tar.gz` & `tmp/SpaGCN-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGCN-1.2.5.tar", last modified: Thu May 26 15:13:41 2022, max compression
+gzip compressed data, was "SpaGCN-1.2.6.tar", last modified: Wed Apr 19 20:07:48 2023, max compression
```

## Comparing `SpaGCN-1.2.5.tar` & `SpaGCN-1.2.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 jianhu   (38015) jianhu   (38015)        0 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/
-drwxrwxr-x   0 jianhu   (38015) jianhu   (38015)        0 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN/
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)     4661 2022-05-26 15:13:31.000000 SpaGCN-1.2.5/SpaGCN/SpaGCN.py
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)     2240 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/calculate_moran_I.py
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)     4293 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/calculate_adj.py
--rwxr-xr-x   0 jianhu   (38015) jianhu   (38015)     1295 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/layers.py
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)    17600 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/util.py
--rwxr-xr-x   0 jianhu   (38015) jianhu   (38015)    11045 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/models.py
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)      154 2022-05-26 15:08:32.000000 SpaGCN-1.2.5/SpaGCN/__init__.py
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)     4683 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/SpaGCN/ez_mode.py
-drwxrwxr-x   0 jianhu   (38015) jianhu   (38015)        0 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)        7 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/top_level.txt
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)     2307 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/PKG-INFO
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)      322 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/SOURCES.txt
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)        1 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/dependency_links.txt
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)       76 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/SpaGCN.egg-info/requires.txt
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)     2307 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/PKG-INFO
--rw-rw-r--   0 jianhu   (38015) jianhu   (38015)       38 2022-05-26 15:13:41.000000 SpaGCN-1.2.5/setup.cfg
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)     1675 2021-11-19 00:30:26.000000 SpaGCN-1.2.5/README.md
--rw-r--r--   0 jianhu   (38015) jianhu   (38015)      906 2022-05-26 15:08:20.000000 SpaGCN-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:07:48.739242 SpaGCN-1.2.6/
+-rw-rw-rw-   0        0        0     1068 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/License
+-rw-rw-rw-   0        0        0     2241 2023-04-19 20:07:48.739242 SpaGCN-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1675 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:07:48.708011 SpaGCN-1.2.6/SpaGCN/
+-rw-rw-rw-   0        0        0     4661 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/SpaGCN.py
+-rw-rw-rw-   0        0        0      154 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/__init__.py
+-rw-rw-rw-   0        0        0     4293 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/calculate_adj.py
+-rw-rw-rw-   0        0        0     2240 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/calculate_moran_I.py
+-rw-rw-rw-   0        0        0     4683 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/ez_mode.py
+-rw-rw-rw-   0        0        0     1295 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/layers.py
+-rw-rw-rw-   0        0        0    11045 2023-04-17 13:43:49.000000 SpaGCN-1.2.6/SpaGCN/models.py
+-rw-rw-rw-   0        0        0    17834 2023-04-19 19:06:57.000000 SpaGCN-1.2.6/SpaGCN/util.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:07:48.739242 SpaGCN-1.2.6/SpaGCN.egg-info/
+-rw-rw-rw-   0        0        0     2241 2023-04-19 20:07:48.000000 SpaGCN-1.2.6/SpaGCN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-19 20:07:48.000000 SpaGCN-1.2.6/SpaGCN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:07:48.000000 SpaGCN-1.2.6/SpaGCN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-04-19 20:07:48.000000 SpaGCN-1.2.6/SpaGCN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 20:07:48.000000 SpaGCN-1.2.6/SpaGCN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:07:48.739242 SpaGCN-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-04-19 19:57:26.000000 SpaGCN-1.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SpaGCN-1.2.5/SpaGCN/SpaGCN.py` & `SpaGCN-1.2.6/SpaGCN/SpaGCN.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN/calculate_moran_I.py` & `SpaGCN-1.2.6/SpaGCN/calculate_moran_I.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN/calculate_adj.py` & `SpaGCN-1.2.6/SpaGCN/calculate_adj.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN/layers.py` & `SpaGCN-1.2.6/SpaGCN/layers.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN/util.py` & `SpaGCN-1.2.6/SpaGCN/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,25 +156,29 @@
         y=row["y"]
         tmp_nbr=df[((df["x"]-x)**2+(df["y"]-y)**2)<=(radius**2)]
         #tmp_nbr=df[(df["x"]<x+radius) & (df["x"]>x-radius) & (df["y"]<y+radius) & (df["y"]>y-radius)]
         num_nbr.append(tmp_nbr.shape[0])
         for p in tmp_nbr["pred"]:
             nbr_num[p]=nbr_num.get(p,0)+1
     del nbr_num[target_cluster]
+    nbr_num_back=nbr_num.copy() #Backup
     nbr_num=[(k, v)  for k, v in nbr_num.items() if v>(ratio*cluster_num[k])]
     nbr_num.sort(key=lambda x: -x[1])
     print("radius=", radius, "average number of neighbors for each spot is", np.mean(num_nbr))
     print(" Cluster",target_cluster, "has neighbors:")
     for t in nbr_num:
         print("Dmain ", t[0], ": ",t[1])
     ret=[t[0] for t in nbr_num]
     if len(ret)==0:
-        print("No neighbor domain found, try bigger radius or smaller ratio.")
-    else:
-        return ret
+        nbr_num_back=[(k, v)  for k, v in nbr_num_back.items()]
+        nbr_num_back.sort(key=lambda x: -x[1])
+        ret=[nbr_num_back[0][0]]
+        print("No neighbor domain found, only return one potential neighbor domain:",ret)
+        print("Try bigger radius or smaller ratio.")
+    return ret
 
 
 def rank_genes_groups(input_adata, target_cluster,nbr_list, label_col, adj_nbr=True, log=False):
     if adj_nbr:
         nbr_list=nbr_list+[target_cluster]
         adata=input_adata[input_adata.obs[label_col].isin(nbr_list)]
     else:
```

### Comparing `SpaGCN-1.2.5/SpaGCN/models.py` & `SpaGCN-1.2.6/SpaGCN/models.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN/ez_mode.py` & `SpaGCN-1.2.6/SpaGCN/ez_mode.py`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/SpaGCN.egg-info/PKG-INFO` & `SpaGCN-1.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: SpaGCN
-Version: 1.2.5
-Summary: SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
-Home-page: https://github.com/jianhuupenn/SpaGCN
-Author: Jian Hu
-Author-email: jianhu@pennmedicine.upenn.edu
-License: UNKNOWN
-Description: # SpaGCN
-        
-        ## SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
-        
-        ### Jian Hu,*, Xiangjie Li, Kyle Coleman, Amelia Schroeder, Nan Ma, David J. Irwin, Edward B. Lee, Russell T. Shinohara, Mingyao Li,*
-        
-        SpaGCN is a graph convolutional network to integrate gene expression and histology to identify spatial domains and spatially variable genes. To jointly model all spots in a tissue slide, SpaGCN integrates information from gene expression, spatial locations and histological pixel intensities across spots into an undirected weighted graph. Each vertex in the graph contains gene expression information of a spot and the edge weight between two vertices quantifies their expression similarity that is driven by spatial dependency of their coordinates and the corresponding histology. To aggregate gene expression of each spot from its neighboring spots, SpaGCN utilizes a convolutional layer based on edge weights specified by the graph. The aggregated gene expression is then fed into a deep embedding clustering algorithm to cluster the spots into different spatial domains. After spatial domains are identified, genes that are enriched in each spatial domain can be detected by differential expression analysis between domains. SpaGCN is applicable to both in-situ transcriptomics with single-cell resolution (seqFISH, seqFISH+, MERFISH, STARmap, and FISSEQ) and spatial barcoding based transcriptomics (Spatial Transcriptomics , SLIDE-seq, SLIDE-seqV2, HDST, 10x Visium, DBiT-seq, Stero-seq, and PIXEL-seq) data. 
-        For more info, please go to: 
-        https://github.com/jianhuupenn/SpaGCN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: SpaGCN
+Version: 1.2.6
+Summary: SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
+Home-page: https://github.com/jianhuupenn/SpaGCN
+Author: Jian Hu
+Author-email: jianhu@pennmedicine.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: License
+
+# SpaGCN
+
+## SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
+
+### Jian Hu,*, Xiangjie Li, Kyle Coleman, Amelia Schroeder, Nan Ma, David J. Irwin, Edward B. Lee, Russell T. Shinohara, Mingyao Li,*
+
+SpaGCN is a graph convolutional network to integrate gene expression and histology to identify spatial domains and spatially variable genes. To jointly model all spots in a tissue slide, SpaGCN integrates information from gene expression, spatial locations and histological pixel intensities across spots into an undirected weighted graph. Each vertex in the graph contains gene expression information of a spot and the edge weight between two vertices quantifies their expression similarity that is driven by spatial dependency of their coordinates and the corresponding histology. To aggregate gene expression of each spot from its neighboring spots, SpaGCN utilizes a convolutional layer based on edge weights specified by the graph. The aggregated gene expression is then fed into a deep embedding clustering algorithm to cluster the spots into different spatial domains. After spatial domains are identified, genes that are enriched in each spatial domain can be detected by differential expression analysis between domains. SpaGCN is applicable to both in-situ transcriptomics with single-cell resolution (seqFISH, seqFISH+, MERFISH, STARmap, and FISSEQ) and spatial barcoding based transcriptomics (Spatial Transcriptomics , SLIDE-seq, SLIDE-seqV2, HDST, 10x Visium, DBiT-seq, Stero-seq, and PIXEL-seq) data. 
+For more info, please go to: 
+https://github.com/jianhuupenn/SpaGCN
```

### Comparing `SpaGCN-1.2.5/PKG-INFO` & `SpaGCN-1.2.6/SpaGCN.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: SpaGCN
-Version: 1.2.5
-Summary: SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
-Home-page: https://github.com/jianhuupenn/SpaGCN
-Author: Jian Hu
-Author-email: jianhu@pennmedicine.upenn.edu
-License: UNKNOWN
-Description: # SpaGCN
-        
-        ## SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
-        
-        ### Jian Hu,*, Xiangjie Li, Kyle Coleman, Amelia Schroeder, Nan Ma, David J. Irwin, Edward B. Lee, Russell T. Shinohara, Mingyao Li,*
-        
-        SpaGCN is a graph convolutional network to integrate gene expression and histology to identify spatial domains and spatially variable genes. To jointly model all spots in a tissue slide, SpaGCN integrates information from gene expression, spatial locations and histological pixel intensities across spots into an undirected weighted graph. Each vertex in the graph contains gene expression information of a spot and the edge weight between two vertices quantifies their expression similarity that is driven by spatial dependency of their coordinates and the corresponding histology. To aggregate gene expression of each spot from its neighboring spots, SpaGCN utilizes a convolutional layer based on edge weights specified by the graph. The aggregated gene expression is then fed into a deep embedding clustering algorithm to cluster the spots into different spatial domains. After spatial domains are identified, genes that are enriched in each spatial domain can be detected by differential expression analysis between domains. SpaGCN is applicable to both in-situ transcriptomics with single-cell resolution (seqFISH, seqFISH+, MERFISH, STARmap, and FISSEQ) and spatial barcoding based transcriptomics (Spatial Transcriptomics , SLIDE-seq, SLIDE-seqV2, HDST, 10x Visium, DBiT-seq, Stero-seq, and PIXEL-seq) data. 
-        For more info, please go to: 
-        https://github.com/jianhuupenn/SpaGCN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: SpaGCN
+Version: 1.2.6
+Summary: SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
+Home-page: https://github.com/jianhuupenn/SpaGCN
+Author: Jian Hu
+Author-email: jianhu@pennmedicine.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: License
+
+# SpaGCN
+
+## SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks
+
+### Jian Hu,*, Xiangjie Li, Kyle Coleman, Amelia Schroeder, Nan Ma, David J. Irwin, Edward B. Lee, Russell T. Shinohara, Mingyao Li,*
+
+SpaGCN is a graph convolutional network to integrate gene expression and histology to identify spatial domains and spatially variable genes. To jointly model all spots in a tissue slide, SpaGCN integrates information from gene expression, spatial locations and histological pixel intensities across spots into an undirected weighted graph. Each vertex in the graph contains gene expression information of a spot and the edge weight between two vertices quantifies their expression similarity that is driven by spatial dependency of their coordinates and the corresponding histology. To aggregate gene expression of each spot from its neighboring spots, SpaGCN utilizes a convolutional layer based on edge weights specified by the graph. The aggregated gene expression is then fed into a deep embedding clustering algorithm to cluster the spots into different spatial domains. After spatial domains are identified, genes that are enriched in each spatial domain can be detected by differential expression analysis between domains. SpaGCN is applicable to both in-situ transcriptomics with single-cell resolution (seqFISH, seqFISH+, MERFISH, STARmap, and FISSEQ) and spatial barcoding based transcriptomics (Spatial Transcriptomics , SLIDE-seq, SLIDE-seqV2, HDST, 10x Visium, DBiT-seq, Stero-seq, and PIXEL-seq) data. 
+For more info, please go to: 
+https://github.com/jianhuupenn/SpaGCN
```

### Comparing `SpaGCN-1.2.5/README.md` & `SpaGCN-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `SpaGCN-1.2.5/setup.py` & `SpaGCN-1.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SpaGCN", 
-    version="1.2.5",
+    version="1.2.6",
     author="Jian Hu",
     author_email="jianhu@pennmedicine.upenn.edu",
     description="SpaGCN: Integrating gene expression and histology to identify spatial domains and spatially variable genes using graph convolutional networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jianhuupenn/SpaGCN",
     packages=setuptools.find_packages(),
-    install_requires=["python-igraph","torch","pandas","numpy","scipy","scanpy","anndata","louvain","sklearn", "numba"],
+    install_requires=["python-igraph","torch","pandas","numpy","scipy","scanpy","anndata","louvain","scikit-learn", "numba"],
     #install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

