# Comparing `tmp/scTAPE-1.1.0.tar.gz` & `tmp/scTAPE-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scTAPE-1.1.0.tar", last modified: Tue Oct 11 03:41:21 2022, max compression
+gzip compressed data, was "scTAPE-1.1.1.tar", last modified: Wed Apr 19 13:59:09 2023, max compression
```

## Comparing `scTAPE-1.1.0.tar` & `scTAPE-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2022-10-11 03:41:21.000000 scTAPE-1.1.0/
--rw-r--r--   0 chan       (501) staff       (20)    35149 2021-10-11 06:27:32.000000 scTAPE-1.1.0/LICENSE
--rw-r--r--   0 chan       (501) staff       (20)      340 2022-10-11 03:41:21.000000 scTAPE-1.1.0/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)     5238 2022-10-11 03:39:28.000000 scTAPE-1.1.0/README.md
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2022-10-11 03:41:21.000000 scTAPE-1.1.0/TAPE/
--rw-r--r--   0 chan       (501) staff       (20)       88 2021-10-11 10:57:17.000000 scTAPE-1.1.0/TAPE/__init__.py
--rw-r--r--   0 chan       (501) staff       (20)     7386 2022-10-11 02:39:40.000000 scTAPE-1.1.0/TAPE/deconvolution.py
--rw-r--r--   0 chan       (501) staff       (20)     7953 2022-09-05 13:17:55.000000 scTAPE-1.1.0/TAPE/model.py
--rw-r--r--   0 chan       (501) staff       (20)     6097 2022-05-05 16:05:47.000000 scTAPE-1.1.0/TAPE/simulation.py
--rw-r--r--   0 chan       (501) staff       (20)     6727 2022-10-11 02:40:35.000000 scTAPE-1.1.0/TAPE/train.py
--rw-r--r--   0 chan       (501) staff       (20)     6995 2022-05-30 16:54:53.000000 scTAPE-1.1.0/TAPE/utils.py
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2022-10-11 03:41:21.000000 scTAPE-1.1.0/scTAPE.egg-info/
--rw-r--r--   0 chan       (501) staff       (20)      340 2022-10-11 03:41:20.000000 scTAPE-1.1.0/scTAPE.egg-info/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)      275 2022-10-11 03:41:21.000000 scTAPE-1.1.0/scTAPE.egg-info/SOURCES.txt
--rw-r--r--   0 chan       (501) staff       (20)        1 2022-10-11 03:41:20.000000 scTAPE-1.1.0/scTAPE.egg-info/dependency_links.txt
--rw-r--r--   0 chan       (501) staff       (20)      113 2022-10-11 03:41:20.000000 scTAPE-1.1.0/scTAPE.egg-info/requires.txt
--rw-r--r--   0 chan       (501) staff       (20)        5 2022-10-11 03:41:20.000000 scTAPE-1.1.0/scTAPE.egg-info/top_level.txt
--rw-r--r--   0 chan       (501) staff       (20)       38 2022-10-11 03:41:21.000000 scTAPE-1.1.0/setup.cfg
--rw-r--r--   0 chan       (501) staff       (20)      671 2022-10-11 03:40:34.000000 scTAPE-1.1.0/setup.py
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.815255 scTAPE-1.1.1/
+-rw-r--r--   0 chan       (501) staff       (20)    35149 2023-04-19 13:46:34.000000 scTAPE-1.1.1/LICENSE
+-rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-19 13:59:09.815113 scTAPE-1.1.1/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)     5180 2023-04-19 13:46:34.000000 scTAPE-1.1.1/README.md
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.814243 scTAPE-1.1.1/TAPE/
+-rw-r--r--   0 chan       (501) staff       (20)       88 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/__init__.py
+-rw-r--r--   0 chan       (501) staff       (20)     7521 2023-04-19 13:52:44.000000 scTAPE-1.1.1/TAPE/deconvolution.py
+-rw-r--r--   0 chan       (501) staff       (20)     7953 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/model.py
+-rw-r--r--   0 chan       (501) staff       (20)     6097 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/simulation.py
+-rw-r--r--   0 chan       (501) staff       (20)     6727 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/train.py
+-rw-r--r--   0 chan       (501) staff       (20)     6421 2023-04-19 13:53:39.000000 scTAPE-1.1.1/TAPE/utils.py
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.814915 scTAPE-1.1.1/scTAPE.egg-info/
+-rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)      275 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/SOURCES.txt
+-rw-r--r--   0 chan       (501) staff       (20)        1 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/dependency_links.txt
+-rw-r--r--   0 chan       (501) staff       (20)      113 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/requires.txt
+-rw-r--r--   0 chan       (501) staff       (20)        5 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/top_level.txt
+-rw-r--r--   0 chan       (501) staff       (20)       38 2023-04-19 13:59:09.815311 scTAPE-1.1.1/setup.cfg
+-rw-r--r--   0 chan       (501) staff       (20)      671 2023-04-19 13:58:02.000000 scTAPE-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scTAPE-1.1.0/LICENSE` & `scTAPE-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.0/README.md` & `scTAPE-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # TAPE: Tissue-AdaPtive autoEncoder for accurate deconvolution and gene expression analysis
 
-![scTAPE](https://img.shields.io/badge/scTAPE-v1.1.0-blue)![GPL](https://img.shields.io/github/license/poseidonchan/TAPE)[![Downloads](https://static.pepy.tech/personalized-badge/sctape?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/sctape)
+![scTAPE](https://img.shields.io/badge/scTAPE-v1.1.0-blue)![GPL](https://img.shields.io/github/license/poseidonchan/TAPE)[![DOI](https://zenodo.org/badge/386163911.svg)](https://zenodo.org/badge/latestdoi/386163911)
 
 **This model is able to accurately deconvolve bulk RNA-seq data into cell fractions and predict cell-type-specific gene expression at cell-type level based on scRNA-seq data**.
 
-related article ***Deep autoencoder for interpretable tissue-adaptive deconvolution and cell-type-specific gene analysis*** is available on [*bioRxiv*](https://doi.org/10.1101/2021.10.26.465846)
-
-## Warning
-The data I uploaded to the tsinghua cloud is not stable and maybe removed in the future since I left Tsinghua University. If you need these files, please contact me (poseidonchan@icloud.com).
+related article ***Deep autoencoder for interpretable tissue-adaptive deconvolution and cell-type-specific gene analysis*** is accepted by *Nature Communications*
 
 ## Setup
 
 TAPE uses PyTorch as its Deep-learning framework, so the suitable version of PyTorch will accelerate the model training process. We recommend users to install PyTorch(>=1.8.0) with ***right*** compute platform (CUDA, CPU or ROCm) from its official [website](https://pytorch.org) in advance.
 
 For example, we used NVIDIA GPU RTX 3090, so we choose the CUDA version 11.1 and the command is:
 
@@ -45,40 +42,51 @@
                   batch_size=128, epochs=128, seed=1)
 ```
 parameters:
 
 1. datatype: use '**TPM**', '**FPKM**' or '**counts**'. Users can choose different normalization method based on your single-cell seq technique, if single-cell data is from 10X Genomics, users should use '**counts**' to maintain a resonable procedure. The explanation could be found from the [webpage](https://kb.10xgenomics.com/hc/en-us/articles/115003684783-Should-I-calculate-TPM-RPKM-or-FPKM-instead-of-counts-for-10x-Genomics-data-).
 2. mode: '**overall**' or '**high-resolution**'. If you need signature matrix for each sample, use 'high-resolution' mode.
 3. adaptive: **True** or **False**. If this is False, then it would not predict signature matrix, the return will be ***None***
-4. variance_threshold: Float number from 0 to 1, it means how many genes you want to keep according to variance from high to low.
+4. variance_threshold: Float number from 0 to 1, it means how many genes you want to keep (in proportion) according to variance from high to low.
 5. batch_size: **int**, related to training result. 32-128 are recommended. Smaller batch_size leads to more time consumption.
 6. epochs: **int**, related to training result. Typically, *5000-10000* iterations are enough for TAPE, the relation is $epochs=\frac{iteration \times batch\_size}{sampleing\_num}$
-7. seed: now, TAPE supports pinning the random seed to make results reproducible.
+7. seed: now, TAPE supports pinning the random seed to make results being reproducible.
 
 Since the original implementation of Scaden [[repository](https://github.com/KevinMenden/scaden)] [[paper](https://www.science.org/doi/10.1126/sciadv.aba2619)] is not easy for us to test, we implemented the PyTorch version of Scaden. If you want to use Scaden to deconvolve bulk RNA-seq data, you can use the following code:
 
 ```python
 from TAPE.deconvolution import ScadenDeconvolution
 Pred = ScadenDeconvolution(sc_ref, bulkdata, sep='\t',
                            batch_size=128, epochs=128)
 ```
 
-The parameters in this function are the same as the parameters in the *Deconvolution* function. 
-
 
 ## Example
 An example is placed in the **Test** directory. Please run the example to get familiar with TAPE.
 
 Run the demo may takes 2 to 3 mins with GPU acceleration or 10 mins with CPU.
 
+
 ## Issues
 If you find any bugs or have problems when you are using scTAPE, feel free to raise issues.
 
 ## Citation
-If you feel TAPE is useful and want to cite TAPE, please use the following format:
-[Bib TeX](https://cloud.tsinghua.edu.cn/f/6351d49841934fa79bc5/?dl=1)
-[EndNote](https://cloud.tsinghua.edu.cn/f/88780d85281c40c0848f/?dl=1)
+```bibtex
+@article{TAPE,
+   author = {Chen, Yanshuo and Wang, Yixuan and Chen, Yuelong and Cheng, Yuqi and Wei, Yumeng and Li, Yunxiang and Wang, Jiuming and Wei, Yingying and Chan, Ting-Fung and Li, Yu},
+   title = {Deep autoencoder for interpretable tissue-adaptive deconvolution and cell-type-specific gene analysis},
+   journal = {Nature Communications},
+   volume = {13},
+   number = {1},
+   pages = {6735},
+   ISSN = {2041-1723},
+   DOI = {10.1038/s41467-022-34550-9},
+   url = {https://doi.org/10.1038/s41467-022-34550-9},
+   year = {2022},
+   type = {Journal Article}
+}
+```
 
 ## Acknowledgement
 Special thanks to [*Mengyue Sun*](https://github.com/sunmy2019), for his help to accelerate the sampling process (in the simulation.py).
 
 Much thanks to [*Yibo Liu*](https://github.com/jedibobo), for his advice on building such a nice repository.
```

### Comparing `scTAPE-1.1.0/TAPE/deconvolution.py` & `scTAPE-1.1.1/TAPE/deconvolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import pandas as pd
 from .simulation import generate_simulated_data
 from .utils import ProcessInputData
 from .train import train_model, predict, reproducibility
 from .model import scaden, AutoEncoder
 
 def Deconvolution(necessary_data, real_bulk, sep='\t', variance_threshold=0.8,
+                  scaler='mms',
                   datatype='counts', genelenfile=None, d_prior=None,
                   mode='overall', adaptive=True,
                   save_model_name=None, sparse=True,
                   batch_size=128, epochs=128, seed=0):
     """
     :param necessary_data: for single-cell data, txt file and dataframe are supported. for simulated data, file location
                            and the h5ad variable are supported. for a trained model, model location(saved with pth) and
                            the model are supported.
     :param real_bulk: an expression file path, index is sample, columns is gene name
     :param variance_threshold: value from 0 to 1. Filter out genes with variance low than this rank.
+    :param scaler: using MinMaxScaler ("mms") or StandardScaler ("ss") to process data.
     :param sep: used to read bulk data, depends on the format
     :param datatype: FPKM or TPM, if bulk RNA-seq normalization type is RPKM, please just use FPKM.
     :param genelenfile: specify the location of gene length file for transforming counts data to TPM or FPKM
                         this file should in txt format and
                         contain three columns: [Gene name,Transcript start (bp),Transcript end (bp)]
     :param d_prior: prior knowledge about cell fractions, used to generate cell fractions, if this param is None, then the
                     fractions is generated as a random way.
@@ -63,15 +65,15 @@
         elif type(necessary_data) is AutoEncoder:
             raise Exception('Do not accept a model as input')
         else:
             raise Exception('Please give the correct input')
 
     train_x, train_y, test_x, genename, celltypes, samplename = \
         ProcessInputData(simudata, real_bulk, sep=sep, datatype=datatype, genelenfile=genelenfile,
-                         variance_threshold=variance_threshold)
+                         variance_threshold=variance_threshold, scaler=scaler)
     print('training data shape is ', train_x.shape, '\ntest data shape is ', test_x.shape)
     if save_model_name is not None:
         reproducibility(seed)
         model = train_model(train_x, train_y, save_model_name, batch_size=batch_size, epochs=epochs)
     else:
         reproducibility(seed)
         model = train_model(train_x, train_y, batch_size=batch_size, epochs=epochs)
```

### Comparing `scTAPE-1.1.0/TAPE/model.py` & `scTAPE-1.1.1/TAPE/model.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.0/TAPE/simulation.py` & `scTAPE-1.1.1/TAPE/simulation.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.0/TAPE/train.py` & `scTAPE-1.1.1/TAPE/train.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.0/TAPE/utils.py` & `scTAPE-1.1.1/TAPE/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 def counts2TPM(counts, genelen):
     fpkm = counts2FPKM(counts, genelen)
     tpm = FPKM2TPM(fpkm)
     return tpm
 
 
 def ProcessInputData(train_data, test_data, sep=None, datatype='TPM', variance_threshold=0.98,
+                     scaler="mms",
                      genelenfile=None):
     ### read train data
     print('Reading training data')
     if type(train_data) is anndata.AnnData:
         pass
     elif type(train_data) is str:
         train_data = anndata.read_h5ad(train_data)
@@ -103,39 +104,30 @@
     fig = plt.figure()
     sns.histplot(data=np.mean(train_x, axis=0), kde=True, color=colors[3],edgecolor=None)
     sns.histplot(data=np.mean(test_x, axis=0), kde=True, color=colors[7],edgecolor=None)
     plt.legend(title='datatype', labels=['trainingdata', 'testdata'])
 
     plt.show()
 
-    mean_trainx = np.mean(train_x, axis=0)
-    top_iv = pd.cut(mean_trainx,
-                    np.linspace(np.min(mean_trainx), np.max(mean_trainx), 100)).value_counts().sort_values()[-5:].index
-    train_mid = [i.mid for i in top_iv]
-    mean_testx = np.mean(test_x, axis=0)
-    top_iv = pd.cut(mean_testx, np.linspace(np.min(mean_testx), np.max(mean_testx), 100)).value_counts().sort_values()[
-             -5:].index
-    test_mid = [i.mid for i in top_iv]
-    if (np.max(train_mid) - np.min(train_mid) > 2 or np.max(test_mid) - np.min(test_mid) > 2):
-        print('The distribution of training data is probably a zero-inflated distribution.\n',
-              'We will use standard scale to deal with low variance noise.')
-
+    if scaler=='ss':
+        print("Using standard scaler...")
         ss = StandardScaler()
         ss_train_x = ss.fit_transform(train_x.T).T
         ss_test_x = ss.fit_transform(test_x.T).T
         fig = plt.figure()
         sns.histplot(data=np.mean(ss_train_x, axis=0), kde=True, color=colors[3],edgecolor=None)
         sns.histplot(data=np.mean(ss_test_x, axis=0), kde=True, color=colors[7],edgecolor=None)
         plt.legend(title='datatype', labels=['trainingdata', 'testdata'])
 
         plt.show()
 
         return ss_train_x, train_y.values, ss_test_x, genename, celltypes, samplename
 
-    else:
+    elif scaler == 'mms':
+        print("Using minmax scaler...")
         mms = MinMaxScaler()
         mms_train_x = mms.fit_transform(train_x.T).T
         mms_test_x = mms.fit_transform(test_x.T).T
         sns.histplot(data=np.mean(mms_train_x, axis=0), kde=True, color=colors[3],edgecolor=None)
         sns.histplot(data=np.mean(mms_test_x, axis=0), kde=True, color=colors[7],edgecolor=None)
         plt.legend(title='datatype', labels=['trainingdata', 'testdata'])
```

### Comparing `scTAPE-1.1.0/setup.py` & `scTAPE-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name = 'scTAPE',
-    version = '1.1.0',
+    version = '1.1.1',
     description = 'deep learning tools for bulk RNA-seq deconvolution and gene expression analysis',
     author = 'Yanshuo Chen',
     author_email = 'poseidonchan@icloud.com',
     url = 'https://github.com/poseidonchan/TAPE',
     license = 'GPL-3.0 License',
     packages = find_packages(),
     python_requires='==3.7',
```

