# Comparing `tmp/pymCADRE-1.2.2.tar.gz` & `tmp/pymCADRE-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymCADRE-1.2.2.tar", last modified: Wed Apr 19 09:37:17 2023, max compression
+gzip compressed data, was "dist/pymCADRE-1.2.3.tar", last modified: Wed Apr 19 09:43:29 2023, max compression
```

## Comparing `pymCADRE-1.2.2.tar` & `pymCADRE-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:37:17.577690 pymCADRE-1.2.2/
--rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     3948 2023-04-19 09:37:17.577322 pymCADRE-1.2.2/PKG-INFO
--rw-rw-r--   0 leonidou   (501) staff       (20)     3278 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:37:17.576775 pymCADRE-1.2.2/pymCADRE.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     3948 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      200 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       33 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/top_level.txt
--rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 09:37:17.577822 pymCADRE-1.2.2/setup.cfg
--rw-rw-r--   0 leonidou   (501) staff       (20)     1008 2023-04-19 09:36:13.000000 pymCADRE-1.2.2/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:43:29.430107 pymCADRE-1.2.3/
+-rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.3/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 09:43:29.429482 pymCADRE-1.2.3/PKG-INFO
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4648 2023-04-19 09:38:15.000000 pymCADRE-1.2.3/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:43:29.428569 pymCADRE-1.2.3/pymCADRE.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)      200 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       28 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/top_level.txt
+-rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.3/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 09:43:29.430441 pymCADRE-1.2.3/setup.cfg
+-rw-rw-r--   0 leonidou   (501) staff       (20)      978 2023-04-19 09:42:53.000000 pymCADRE-1.2.3/setup.py
```

### Comparing `pymCADRE-1.2.2/LICENSE` & `pymCADRE-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.2/PKG-INFO` & `pymCADRE-1.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.2
+Version: 1.2.3
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
@@ -13,20 +13,25 @@
 
 # pymCADRE 
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
 [![Latest version](https://img.shields.io/badge/Latest_version-0.9-brightgreen.svg?style=plastic)](https://github.com/draeger-lab/pymCADRE/releases/)
 ![Code Size](https://img.shields.io/github/languages/code-size/draeger-lab/pymCADRE.svg?style=plastic)
 ![Downloads of all releases](https://img.shields.io/github/downloads/draeger-lab/pymCADRE/total.svg?style=plastic)
-[![DOI](https://zenodo.org/badge/323376678.svg)](https://zenodo.org/badge/latestdoi/323376678)
 
 <img align="right" src="pymCADRE_logo.png" alt="drawing" width="170"/> 
 
 *Authors* : [Nantia Leonidou](https://github.com/NantiaL)
 
+### Publication
+
+When using pymCADRE in a research work, please cite the following work:
+
+Leonidou, N., Renz, A., Mostolizadeh, R., & Dräger, A. (2023). New workflow predicts drug targets against SARS-CoV-2 via metabolic changes in infected cells. PLOS Computational Biology, 19(3), e1010903.
+[![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtab669-blue.svg?style=plastic)](https://doi.org/10.1371/journal.pcbi.1010903)
 
 ### Overview. 
 
 The **pymCADRE** tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation ([mCADRE](https://github.com/jaeddy/mcadre)) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 
 The reactions within the generic global model are being ranked, and the ones with the lowest supporting evidence for the tissue
 of interest are given the highest priority for removal:
@@ -34,19 +39,24 @@
 GM, C, NC, P, Z, model_C = rank_reactions(model, G, U, confidence_scores, C_H_genes, method)
 ```
 If the generic functionality test is passed, the model undergoes pruning, which results in a context-specific reconstruction:
 ```
 PM, cRes = prune_model(GM, P, C, Z, eta, precursorMets, salvage_check, C_H_genes, method)
 ```
 
+### Installation
+```
+pip install pymcadre
+```
+
 ### Prerequisites
 
 This tool has the following dependencies:
 
-python 3.8
+python >=3.8.5
 
 Packages:
 * pandas
 * numpy
 * cobra
 * requests
 * os
@@ -76,10 +86,22 @@
 + `cRes`: result of model checks (consistency/function) during pruning
   
 
 ### Usage
 To run pymCADRE, execute the notebook named main_pymcadre.ipynb or the python script named pymcadre.py. The scripts can be modified to the preferred parameters and input files. Jupyter notebooks with test runs and test scripts are also provided as reference points.
 
 
+### Additional material
+#### PREDICATE (<ins>**Predic**</ins>tion of <ins>**A**</ins>ntiviral <ins>**T**</ins>arg<ins>**e**</ins>ts): 
+<img align="center" src="PREDICATE_overview.png" width="570"/>
+
+Steps: 
+- introduction of mutations in the reference sequence based on the protein sequences 
+- calculation of the necessary stoichiometric coefficients for the final virus biomass functions
+- target detection using two approaches: reaction knock-outs and the host-derived enforcement
+- visualizations that could give insights into the dataset and a better understanding of the results. 
+
+The tool can be applied to either one or more nucleotide sequences and all existing RNA viruses. This makes it particularly advantageous and time-saving when studying multiple variants of a single virus. The number of genomic input sequences equals the number of the calculated VBOF.
 
+To run the tool, set the constant variables to the file pathways where the desired files are stored.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymCADRE-1.2.2/pymCADRE.egg-info/PKG-INFO` & `pymCADRE-1.2.3/pymCADRE.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.2
+Version: 1.2.3
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
@@ -13,20 +13,25 @@
 
 # pymCADRE 
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
 [![Latest version](https://img.shields.io/badge/Latest_version-0.9-brightgreen.svg?style=plastic)](https://github.com/draeger-lab/pymCADRE/releases/)
 ![Code Size](https://img.shields.io/github/languages/code-size/draeger-lab/pymCADRE.svg?style=plastic)
 ![Downloads of all releases](https://img.shields.io/github/downloads/draeger-lab/pymCADRE/total.svg?style=plastic)
-[![DOI](https://zenodo.org/badge/323376678.svg)](https://zenodo.org/badge/latestdoi/323376678)
 
 <img align="right" src="pymCADRE_logo.png" alt="drawing" width="170"/> 
 
 *Authors* : [Nantia Leonidou](https://github.com/NantiaL)
 
+### Publication
+
+When using pymCADRE in a research work, please cite the following work:
+
+Leonidou, N., Renz, A., Mostolizadeh, R., & Dräger, A. (2023). New workflow predicts drug targets against SARS-CoV-2 via metabolic changes in infected cells. PLOS Computational Biology, 19(3), e1010903.
+[![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtab669-blue.svg?style=plastic)](https://doi.org/10.1371/journal.pcbi.1010903)
 
 ### Overview. 
 
 The **pymCADRE** tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation ([mCADRE](https://github.com/jaeddy/mcadre)) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 
 The reactions within the generic global model are being ranked, and the ones with the lowest supporting evidence for the tissue
 of interest are given the highest priority for removal:
@@ -34,19 +39,24 @@
 GM, C, NC, P, Z, model_C = rank_reactions(model, G, U, confidence_scores, C_H_genes, method)
 ```
 If the generic functionality test is passed, the model undergoes pruning, which results in a context-specific reconstruction:
 ```
 PM, cRes = prune_model(GM, P, C, Z, eta, precursorMets, salvage_check, C_H_genes, method)
 ```
 
+### Installation
+```
+pip install pymcadre
+```
+
 ### Prerequisites
 
 This tool has the following dependencies:
 
-python 3.8
+python >=3.8.5
 
 Packages:
 * pandas
 * numpy
 * cobra
 * requests
 * os
@@ -76,10 +86,22 @@
 + `cRes`: result of model checks (consistency/function) during pruning
   
 
 ### Usage
 To run pymCADRE, execute the notebook named main_pymcadre.ipynb or the python script named pymcadre.py. The scripts can be modified to the preferred parameters and input files. Jupyter notebooks with test runs and test scripts are also provided as reference points.
 
 
+### Additional material
+#### PREDICATE (<ins>**Predic**</ins>tion of <ins>**A**</ins>ntiviral <ins>**T**</ins>arg<ins>**e**</ins>ts): 
+<img align="center" src="PREDICATE_overview.png" width="570"/>
+
+Steps: 
+- introduction of mutations in the reference sequence based on the protein sequences 
+- calculation of the necessary stoichiometric coefficients for the final virus biomass functions
+- target detection using two approaches: reaction knock-outs and the host-derived enforcement
+- visualizations that could give insights into the dataset and a better understanding of the results. 
+
+The tool can be applied to either one or more nucleotide sequences and all existing RNA viruses. This makes it particularly advantageous and time-saving when studying multiple variants of a single virus. The number of genomic input sequences equals the number of the calculated VBOF.
 
+To run the tool, set the constant variables to the file pathways where the desired files are stored.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymCADRE-1.2.2/setup.py` & `pymCADRE-1.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymCADRE',
-    version='1.2.2',
+    version='1.2.3',
     description='The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/pymCADRE',
     author='Nantia Leonidou',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
     keywords=['pymCADRE', 'systems biology', 'tissue-specific metabolic models'],
     install_requires=['pandas',
                       'numpy',
-                      'cobrapy',
-                      'requests',
-                      'os']
+                      'cobra',
+                      'requests']
 )
```

