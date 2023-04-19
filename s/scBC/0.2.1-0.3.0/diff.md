# Comparing `tmp/scBC-0.2.1.tar.gz` & `tmp/scBC-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scBC-0.2.1.tar", last modified: Wed Apr 19 05:09:37 2023, max compression
+gzip compressed data, was "scBC-0.3.0.tar", last modified: Wed Apr 19 06:20:33 2023, max compression
```

## Comparing `scBC-0.2.1.tar` & `scBC-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.830209 scBC-0.2.1/
--rw-rw-rw-   0        0        0     1065 2023-04-19 03:17:25.000000 scBC-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    10969 2023-04-19 05:09:37.829207 scBC-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10403 2023-04-19 03:14:30.000000 scBC-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.824207 scBC-0.2.1/scBC/
--rw-rw-rw-   0        0        0     6095 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/DWL.py
--rw-rw-rw-   0        0        0        0 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/__init__.py
--rw-rw-rw-   0        0        0     4240 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/data.py
--rw-rw-rw-   0        0        0    18655 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/model.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.828208 scBC-0.2.1/scBC.egg-info/
--rw-rw-rw-   0        0        0    10969 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 05:09:37.830209 scBC-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      958 2023-04-19 05:09:07.000000 scBC-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:33.512461 scBC-0.3.0/
+-rw-rw-rw-   0        0        0     1065 2023-04-19 03:17:25.000000 scBC-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    11233 2023-04-19 06:20:33.511460 scBC-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10667 2023-04-19 06:12:14.000000 scBC-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:33.506462 scBC-0.3.0/scBC/
+-rw-rw-rw-   0        0        0     6095 2023-04-19 03:14:30.000000 scBC-0.3.0/scBC/DWL.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 03:14:30.000000 scBC-0.3.0/scBC/__init__.py
+-rw-rw-rw-   0        0        0     4240 2023-04-19 03:14:30.000000 scBC-0.3.0/scBC/data.py
+-rw-rw-rw-   0        0        0    18662 2023-04-19 06:16:31.000000 scBC-0.3.0/scBC/model.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:20:33.510460 scBC-0.3.0/scBC.egg-info/
+-rw-rw-rw-   0        0        0    11233 2023-04-19 06:20:33.000000 scBC-0.3.0/scBC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-19 06:20:33.000000 scBC-0.3.0/scBC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:20:33.000000 scBC-0.3.0/scBC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:20:33.000000 scBC-0.3.0/scBC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 06:20:33.000000 scBC-0.3.0/scBC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:20:33.512461 scBC-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      958 2023-04-19 06:18:14.000000 scBC-0.3.0/setup.py
```

### Comparing `scBC-0.2.1/LICENSE` & `scBC-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scBC-0.2.1/PKG-INFO` & `scBC-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBC
-Version: 0.2.1
+Version: 0.3.0
 Summary: a single-cell transcriptome Bayesian biClustering framework
 Home-page: https://github.com/GYQ-form/scBC
 Author: Yuqiao Gong
 Author-email: gyq123@sjtu.edu.cn
 License: MIT
 Keywords: single cell transcriptomics,Biclustering,bioinformatics,variational inference(VI)
 Platform: UNKNOWN
@@ -23,28 +23,31 @@
 
 
 ## Installation
 
 To install our package, run
 
 ```bash
+conda install -c conda-forge scvi-tools #pip install scvi-tools
 pip install scBC
 ```
 
 
 
 ## Quick start
 
 To simply illustrate how one can run our scBC model, here we use the subsampled HEART dataset as an example. We have prepared four subsampled datasets in advance (HEART, PBMC, LUAD and BC), which   can be downloaded locally with simple codes:
 
 ```python
 from scBC import data
 heart = data.load_data("HEART")
 ```
 
+If you can't download the data automatically, you can also download them manually from our [repository](https://github.com/GYQ-form/scBC/tree/main/data) and place them in your working directory.
+
 Now you are ready to set up the scBC model:
 
 ```python
 from scBC.model import scBC
 my_model = scBC(adata=heart,batch_key='cell_source')
 ```
 
@@ -55,15 +58,15 @@
 ```python
 my_model.train_VI()
 ```
 
 Then we can get the reconstructed data, we use 10 posterior samples to estimate the mean expression:
 
 ```python
-my_model.get_reconst_data(n_sample=10)
+my_model.get_reconst_data(n_samples=10)
 ```
 
 Since scBC encourage prior information about genes' co-expression to be provided,  before conducting biclustering, we first generate a prior edge. Thankfully, we have also provide an API for automatically generating prior edge from biomart database, just run with default setting:
 
 ```python
 my_model.get_edge()
 ```
```

### Comparing `scBC-0.2.1/README.md` & `scBC-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 
 
 ## Installation
 
 To install our package, run
 
 ```bash
+conda install -c conda-forge scvi-tools #pip install scvi-tools
 pip install scBC
 ```
 
 
 
 ## Quick start
 
 To simply illustrate how one can run our scBC model, here we use the subsampled HEART dataset as an example. We have prepared four subsampled datasets in advance (HEART, PBMC, LUAD and BC), which   can be downloaded locally with simple codes:
 
 ```python
 from scBC import data
 heart = data.load_data("HEART")
 ```
 
+If you can't download the data automatically, you can also download them manually from our [repository](https://github.com/GYQ-form/scBC/tree/main/data) and place them in your working directory.
+
 Now you are ready to set up the scBC model:
 
 ```python
 from scBC.model import scBC
 my_model = scBC(adata=heart,batch_key='cell_source')
 ```
 
@@ -39,15 +42,15 @@
 ```python
 my_model.train_VI()
 ```
 
 Then we can get the reconstructed data, we use 10 posterior samples to estimate the mean expression:
 
 ```python
-my_model.get_reconst_data(n_sample=10)
+my_model.get_reconst_data(n_samples=10)
 ```
 
 Since scBC encourage prior information about genes' co-expression to be provided,  before conducting biclustering, we first generate a prior edge. Thankfully, we have also provide an API for automatically generating prior edge from biomart database, just run with default setting:
 
 ```python
 my_model.get_edge()
 ```
```

### Comparing `scBC-0.2.1/scBC/DWL.py` & `scBC-0.3.0/scBC/DWL.py`

 * *Files identical despite different names*

### Comparing `scBC-0.2.1/scBC/data.py` & `scBC-0.3.0/scBC/data.py`

 * *Files identical despite different names*

### Comparing `scBC-0.2.1/scBC/model.py` & `scBC-0.3.0/scBC/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                            layer=layer, 
                            batch_key=batch_key, 
                            labels_key=labels_key, 
                            size_factor_key=size_factor_key, 
                            categorical_covariate_keys=categorical_covariate_keys, 
                            continuous_covariate_keys=continuous_covariate_keys)
         
+        self.edge = None
         self.vi_model = None
         self.reconst_data = None
         self.W = None
         self.Z = None
         self.mu = None
         self.convg_trail = None
         self.S = None
@@ -83,15 +84,15 @@
             genes = gene_list
         else:
             genes = self.adata.var_names.to_list()
 
         server = BiomartServer("http://www.ensembl.org/biomart")
 
         # Connect to the biomart server and select the dataset
-        mart = server.datasets['hsapiens_gene_ensembl']
+        mart = server.datasets[dataset]
         filters = {"hgnc_symbol": genes}
         attributes = ["go_id", "hgnc_symbol"]
         response = mart.search({'attributes':attributes, 'filters':filters})
 
         pathway = []
         for line in response.iter_lines():
             line = line.decode('utf-8')
@@ -109,16 +110,16 @@
         # Initialize the edge matrix and pool of genes
         edge = []
         pool = np.array([], dtype=int)
 
         # Select random pathways and add edges between genes in the pathway
         for i in range(intensity):
             path_id = np.random.choice(path_num.index)
-            p = pathway[pathway["go-id"] == path_id]
-            path = np.where(np.isin(topgene, p["gene"]))[0]
+            p = pathway[pathway["go_id"] == path_id]
+            path = np.where(np.isin(genes, p["gene"]))[0]
             if np.intersect1d(pool, path).size:
                 continue
             pool = np.concatenate((pool, path))
             for j in range(len(path)):
                 for k in range(len(path)):
                     if k == j:
                         continue
```

### Comparing `scBC-0.2.1/scBC.egg-info/PKG-INFO` & `scBC-0.3.0/scBC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBC
-Version: 0.2.1
+Version: 0.3.0
 Summary: a single-cell transcriptome Bayesian biClustering framework
 Home-page: https://github.com/GYQ-form/scBC
 Author: Yuqiao Gong
 Author-email: gyq123@sjtu.edu.cn
 License: MIT
 Keywords: single cell transcriptomics,Biclustering,bioinformatics,variational inference(VI)
 Platform: UNKNOWN
@@ -23,28 +23,31 @@
 
 
 ## Installation
 
 To install our package, run
 
 ```bash
+conda install -c conda-forge scvi-tools #pip install scvi-tools
 pip install scBC
 ```
 
 
 
 ## Quick start
 
 To simply illustrate how one can run our scBC model, here we use the subsampled HEART dataset as an example. We have prepared four subsampled datasets in advance (HEART, PBMC, LUAD and BC), which   can be downloaded locally with simple codes:
 
 ```python
 from scBC import data
 heart = data.load_data("HEART")
 ```
 
+If you can't download the data automatically, you can also download them manually from our [repository](https://github.com/GYQ-form/scBC/tree/main/data) and place them in your working directory.
+
 Now you are ready to set up the scBC model:
 
 ```python
 from scBC.model import scBC
 my_model = scBC(adata=heart,batch_key='cell_source')
 ```
 
@@ -55,15 +58,15 @@
 ```python
 my_model.train_VI()
 ```
 
 Then we can get the reconstructed data, we use 10 posterior samples to estimate the mean expression:
 
 ```python
-my_model.get_reconst_data(n_sample=10)
+my_model.get_reconst_data(n_samples=10)
 ```
 
 Since scBC encourage prior information about genes' co-expression to be provided,  before conducting biclustering, we first generate a prior edge. Thankfully, we have also provide an API for automatically generating prior edge from biomart database, just run with default setting:
 
 ```python
 my_model.get_edge()
 ```
```

### Comparing `scBC-0.2.1/setup.py` & `scBC-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="scBC",
     version=__version__,
```

