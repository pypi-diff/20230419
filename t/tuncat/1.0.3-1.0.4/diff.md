# Comparing `tmp/tuncat-1.0.3.tar.gz` & `tmp/tuncat-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\baoyi\Documents\GitHub\TUnCaT\dist\tmp74bsdu6t\tuncat-1.0.3.tar", last modified: Wed Jan 12 02:11:58 2022, max compression
+gzip compressed data, was "dist\tuncat-1.0.4.tar", last modified: Wed Apr 19 01:11:44 2023, max compression
```

## Comparing `tuncat-1.0.3.tar` & `tuncat-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-01-12 02:11:58.004526 tuncat-1.0.3/
--rw-rw-rw-   0        0        0    18411 2021-08-17 00:24:35.000000 tuncat-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    13647 2022-01-12 02:11:58.004526 tuncat-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12569 2021-12-16 05:35:29.000000 tuncat-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-01-12 02:11:58.005527 tuncat-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1557 2022-01-12 01:37:26.000000 tuncat-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-12 02:11:57.976527 tuncat-1.0.3/tuncat/
--rw-rw-rw-   0        0        0        0 2020-08-12 00:06:25.000000 tuncat-1.0.3/tuncat/__init__.py
--rw-rw-rw-   0        0        0     3355 2021-09-21 22:02:49.000000 tuncat-1.0.3/tuncat/bin_trace_video.py
-drwxrwxrwx   0        0        0        0 2022-01-12 02:11:58.000528 tuncat-1.0.3/tuncat/more_options/
--rw-rw-rw-   0        0        0        0 2020-08-12 00:06:25.000000 tuncat-1.0.3/tuncat/more_options/__init__.py
--rw-rw-rw-   0        0        0     8772 2021-12-07 03:38:15.000000 tuncat-1.0.3/tuncat/more_options/nmfunmix1_pertmin_res_MSE_novideo_2side.py
--rw-rw-rw-   0        0        0     7924 2021-12-05 23:20:03.000000 tuncat-1.0.3/tuncat/more_options/nmfunmix_MSE_allow0.py
--rw-rw-rw-   0        0        0     7563 2021-12-16 04:43:30.000000 tuncat-1.0.3/tuncat/nmfunmix1_pertmin_res_MSE_novideo.py
--rw-rw-rw-   0        0        0     7826 2021-12-16 04:43:27.000000 tuncat-1.0.3/tuncat/nmfunmix_MSE.py
--rw-rw-rw-   0        0        0    13651 2022-01-12 02:07:43.000000 tuncat-1.0.3/tuncat/run_TUnCaT.py
--rw-rw-rw-   0        0        0     7888 2021-09-22 20:02:15.000000 tuncat-1.0.3/tuncat/traces_from_masks_mp_mmap_fn_neighbors.py
--rw-rw-rw-   0        0        0     7879 2021-09-22 19:58:21.000000 tuncat-1.0.3/tuncat/traces_from_masks_mp_shm_neighbors.py
--rw-rw-rw-   0        0        0     6495 2021-09-22 00:39:18.000000 tuncat-1.0.3/tuncat/traces_from_masks_numba_neighbors.py
--rw-rw-rw-   0        0        0     5884 2021-12-16 04:44:03.000000 tuncat-1.0.3/tuncat/use_nmfunmix_mp_MSE_novideo.py
--rw-rw-rw-   0        0        0      943 2021-12-16 04:44:07.000000 tuncat-1.0.3/tuncat/utils.py
-drwxrwxrwx   0        0        0        0 2022-01-12 02:11:57.991531 tuncat-1.0.3/tuncat.egg-info/
--rw-rw-rw-   0        0        0    13647 2022-01-12 02:11:57.000000 tuncat-1.0.3/tuncat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2022-01-12 02:11:57.000000 tuncat-1.0.3/tuncat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-12 02:11:57.000000 tuncat-1.0.3/tuncat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2022-01-12 02:11:57.000000 tuncat-1.0.3/tuncat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-01-12 02:11:57.000000 tuncat-1.0.3/tuncat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 01:11:44.000000 tuncat-1.0.4/
+-rw-rw-rw-   0        0        0    18411 2021-08-17 00:24:35.000000 tuncat-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    14505 2023-04-19 01:11:44.000000 tuncat-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12569 2021-12-16 05:35:29.000000 tuncat-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:11:44.000000 tuncat-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1562 2023-04-19 01:11:35.000000 tuncat-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat/
+-rw-rw-rw-   0        0        0        0 2020-08-12 00:06:25.000000 tuncat-1.0.4/tuncat/__init__.py
+-rw-rw-rw-   0        0        0     3355 2021-09-21 22:02:49.000000 tuncat-1.0.4/tuncat/bin_trace_video.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat/more_options/
+-rw-rw-rw-   0        0        0        0 2020-08-12 00:06:25.000000 tuncat-1.0.4/tuncat/more_options/__init__.py
+-rw-rw-rw-   0        0        0     8772 2021-12-07 03:38:15.000000 tuncat-1.0.4/tuncat/more_options/nmfunmix1_pertmin_res_MSE_novideo_2side.py
+-rw-rw-rw-   0        0        0     7924 2021-12-05 23:20:03.000000 tuncat-1.0.4/tuncat/more_options/nmfunmix_MSE_allow0.py
+-rw-rw-rw-   0        0        0     7563 2021-12-16 04:43:30.000000 tuncat-1.0.4/tuncat/nmfunmix1_pertmin_res_MSE_novideo.py
+-rw-rw-rw-   0        0        0     7826 2021-12-16 04:43:27.000000 tuncat-1.0.4/tuncat/nmfunmix_MSE.py
+-rw-rw-rw-   0        0        0    14181 2023-04-19 01:09:41.000000 tuncat-1.0.4/tuncat/run_TUnCaT.py
+-rw-rw-rw-   0        0        0     7888 2021-09-22 20:02:15.000000 tuncat-1.0.4/tuncat/traces_from_masks_mp_mmap_fn_neighbors.py
+-rw-rw-rw-   0        0        0     8111 2023-04-19 01:09:41.000000 tuncat-1.0.4/tuncat/traces_from_masks_mp_shm_neighbors.py
+-rw-rw-rw-   0        0        0     6495 2021-09-22 00:39:18.000000 tuncat-1.0.4/tuncat/traces_from_masks_numba_neighbors.py
+-rw-rw-rw-   0        0        0     5884 2021-12-16 04:44:03.000000 tuncat-1.0.4/tuncat/use_nmfunmix_mp_MSE_novideo.py
+-rw-rw-rw-   0        0        0      943 2021-12-16 04:44:07.000000 tuncat-1.0.4/tuncat/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/
+-rw-rw-rw-   0        0        0    14505 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 01:11:44.000000 tuncat-1.0.4/tuncat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tuncat-1.0.3/LICENSE` & `tuncat-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/PKG-INFO` & `tuncat-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: tuncat
-Version: 1.0.3
-Summary: Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. 
-Home-page: https://github.com/YijunBao/TUnCaT
-Author: Yijun Bao
-Author-email: yijun.bao@duke.edu
-Maintainer: Yijun Bao
-Maintainer-email: yijun.bao@duke.edu
-License: the GNU License, Version 2.0
-Project-URL: Source Code, https://github.com/YijunBao/TUnCaT
-Project-URL: Citation, https://doi.org/10.5281/zenodo.5764576
-Project-URL: Paper, https://doi.org/10.3389/fnins.2021.797421
-Platform: all
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![NeuroToolbox logo](readme/neurotoolbox-logo.svg)
 
 [![DOI](https://zenodo.org/badge/397026426.svg)](https://zenodo.org/badge/latestdoi/397026426)
 
 # TUnCaT
 Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. TUnCaT removed false transients caused by large-scale background fluctuation using background subtraction; TUnCaT removed false transients caused by neighboring neurons, axons, and dendrites using nonnegative matrix factorization (NMF).
 
@@ -127,9 +103,7 @@
 TUnCaT is released under [the GNU License, Version 2.0](LICENSE).
 
 
 # Sponsors
 <img src="readme/NSFBRAIN.png" height="100"/><img src="readme/BRF.png" height="100"/><img src="readme/Beckmanlogo.png" height="100"/>
 <br>
 <img src="readme/valleelogo.png" height="100"/><img src="readme/dibslogo.png" height="100"/><img src="readme/sloan_logo_new.jpg" height="100"/>
-
-
```

### Comparing `tuncat-1.0.3/README.md` & `tuncat-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,109 +1,132 @@
-![NeuroToolbox logo](readme/neurotoolbox-logo.svg)
-
-[![DOI](https://zenodo.org/badge/397026426.svg)](https://zenodo.org/badge/latestdoi/397026426)
-
-# TUnCaT
-Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. TUnCaT removed false transients caused by large-scale background fluctuation using background subtraction; TUnCaT removed false transients caused by neighboring neurons, axons, and dendrites using nonnegative matrix factorization (NMF).
-
-Copyright (C) 2021 Duke University NeuroToolbox
-
-This repo contains the code of TUnCaT. If you want to reproduce the results in our paper, please visit the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) or [figshare](https://figshare.com/articles/dataset/TUnCaT_paper_reproduction/17132069) to find the data, results, and code to analyze the results. 
-
-- [TUnCaT](#tuncat)
-- [Installation on Windows or Linux](#installation-on-windows-or-linux)
-- [Demo](#demo)
-- [Input, Output, and Intermediate Files](#input-output-and-intermediate-files)
-  - [Input files](#input-files)
-  - [Intermediate and Output files](#intermediate-and-output-files)
-- [Use your own data](#use-your-own-data)
-  - [Use your own videos](#use-your-own-videos)
-  - [Use your own neuron masks](#use-your-own-neuron-masks)
-  - [Set the unmixing parameters](#set-the-unmixing-parameters)
-    - [Set alpha as a user-defined value or using cross-validation](#set-alpha-as-a-user-defined-value-or-using-cross-validation)
-- [Citation](#citation)
-- [Licensing and Copyright](#licensing-and-copyright)
-- [Sponsors](#sponsors)
-
-
-# Installation on Windows or Linux 
-* First, install Python from the [official website](https://www.python.org/downloads/) or any other distribution like [Anaconda](https://www.anaconda.com/). 
-* Launch Windows/Linux terminal or Anaconda prompt, and install TUnCaT using pip:
-```bat
-python -m pip install tuncat
-```
-* Please be aware that the speed of TUnCaT in the Anaconda installation may be significantly slower than the speed in the offical python installation in Windows.
-
-
-# Demo
-We provided a demo for all users to get familiar with TUnCaT. To run the demo, please download the code from our GitHub repository. We provided a one-photon imaging video `c28_163_244.h5` as well as its manually labeled neurons `FinalMasks_c28_163_244.mat`. The demo will calculate the raw traces and background traces of all neurons, calculate the unmixed traces using TUnCaT, and export them to the folder `unmixed_traces`. The input, output, and intermediate files will be explained in [Input, Output, and Intermediate Files](#input-output-and-intermediate-files). 
-
-To run the demo python script, launch system terminal or Anaconda prompt, and type the following script 
-```bat
-cd {TUnCaT_root_path}
-python demo_TUnCaT.py
-```
-You can also run the demo `demo_TUnCaT.ipynb` interactively using Jupyter Notebook. This notebook contains the expected figure of the background-subtracted trace and the unmixed trace of the first neuron. The saved processing time is recorded in a laptop with an AMD Ryzen 5 3500U quad-core CPU.
-
-
-# Input, Output, and Intermediate Files
-By default, all the input, output, and intermediate files are saved under the `TUnCaT` folder. 
-
-## Input files
-* A .h5 file `{name}.h5` contains the input video. This is a 3D dataset with shape = (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The demo video has (T, Lx, Ly) = (6000, 50, 50). 
-* A .mat file `FinalMasks_{name}.mat` contains the nueron masks of the video. This is a 3D array with shape = (Ly, Lx, n) in MATLAB, where Ly and Lx should match the lateral dimensions of the video, and n is the number of neurons. The demo mask has (Ly, Lx, n) = (50, 50, 45). 
-* Important notice: The default dimension order for multi-dimensional array is reversed in MATLAB and python. When you save a dataset with shape = (L1, L2, L3) in MATLAB to an .h5 file or a .mat file with version 7.3 or newer (requiring h5py.File to load in python workspace), and then load it in python, the shape will become (L3, L2, L1). However, if you save the dataset as a .mat file with version 7 or earlier (requiring scipy.loadmat to load in python workspace), the dimensions will preserve and still be (L1, L2, L3). In this document, we will use the python default order to describe the datasets in python workspace or saved in .h5, and use the MATLAB default order to describe the datasets saved in .mat. Sometimes you need to transpose the dimensions to make them consistent. In python, you can transpose the dimensions using `Masks = Masks.transpose((2,1,0))`. In MATLAB, you can transpose the dimensions using `Masks = permute(Masks,[3,2,1])`.
-
-## Intermediate and Output files
-After running TUnCaT on the demo video, the intermediate and output files will be under a new folder `unmixed_traces`. 
-* Intermediate file: `unmixed_traces/raw/{name}.mat` stores the raw neuron traces (`traces`) and the background traces (`bgtraces`). Each trace variable is 2D matrix with shape = (T, n), where T is the number of frames, and n is the number of neurons. 
-* Output file: `unmixed_traces/alpha={}/{name}.mat` or `unmixed_traces/list_alpha={}/{name}.mat` stores the unmixed traces of the neurons (`traces_nmfdemix`), as well as other quantities characterizing the NMF unmixing process of each neuron, including the mixing matrix (`list_mixout`), final alpha (`list_alpha_final`), reconstruction residual (`list_MSE`), and number of iterations (`list_n_iter`). See the function descriptions for the detailed meanings of these quantities.
-
-
-# Use your own data
-Of course, you can modify the demo scripts to process other videos. You need to set the folders of the videos and neuron masks, and change some parameters in the python scripts to correspond to your videos. 
-
-## Use your own videos
-* Set the folder and file names of your video correctly. You need to change the variables `dir_video` and `list_Exp_ID`. The variable `dir_video` is the folder containing the input videos. For example, if your videos are stored in `C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data`, set `dir_video = 'C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data'`. You can also use relative path, such as `dir_video = './data'`. The variable `list_Exp_ID` is the list of the file names (without extension) of the input videos (e.g., `list_Exp_ID = ['c28_163_244']` in the demo referes to the input file `{TUnCaT_root_path}/data/c28_163_244.h5`). 
-* Currently, we only support .h5 files as the input video, so you need to convert the format of your data to .h5. You can save the video in a dataset with any name, but don't save the video under any group. The video should have a shape of (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The support to more video formats will come soon. When doing format conversion, make sure the dimension is in the correct order. For example, if you save save the .h5 files from MATLAB, the shape of the dataset should be (Ly, Lx, T) in MATLAB. See [Input files](#input-files) for more explanation of the dimension order.
-
-## Use your own neuron masks
-* Set the folder and file names of your mask files correctly. You need to change variable `dir_mask` to the folder containing the mask files. 
-* Currently, we only support .mat files as the neuron masks, so you need to convert the format of your neuron masks to .mat, and save the neuron masks in dataset 'FinalMasks'. The name of the masks file should be `FinalMasks_{Exp_ID}.mat`, where the `{Exp_ID}` is the name of the corresponding video. The neuron masks should be saved as a 3D array named `FinalMasks`, and the dimension should be (Ly, Lx, n) in MATLAB, where Ly and Lx are the same as the lateral dimension of the video, and n is the number of neurons.
-* The masks created by some manual labeling software may contain an empty (all zero) image as the first frame. You need to remove the empty frame before saving them.
-
-## Set the unmixing parameters
-* The list of video names (e.g., `list_Exp_ID = ['c28_163_244']`)
-* The folder of the video (e.g., `dir_video='./data'`);
-* The folder of the neuron masks (e.g., `dir_masks='./data'`);
-* The folder of the output traces (e.g., `dir_traces='./data/unmixed_traces'`);
-* `list_alpha` is the list of tested alpha;
-* `multi_alpha` determines the option to deal with multiple elements in `list_alpha`. False means the largest element providing non-trivial output traces will be used, which can be differnt for different neurons. True means each element will be tested and saved independently. These options are equivalent when there is only one element in `list_alpha`;
-* `Qclip` is clipping quantile. Traces lower than this quantile are clipped to this quantile value;
-* `th_pertmin` is maximum pertentage of unmixed traces equaling to the trace minimum;
-* `epsilon` is the minimum value of the input traces after scaling and shifting;
-* `th_residual` is the maximum factorization residual if this value is not zero;
-* `nbin` is the temporal downsampling ratio;
-* `bin_option` determines the temporal downsampling option. It can be 'downsample', 'sum', or 'mean'. It is not used when nbin == 1;
-* `flexible_alpha` determines whether a flexible alpha strategy is used when the smallest alpha in "list_alpha" already caused over-regularization.
-
-### Set alpha as a user-defined value or using cross-validation
-Among the above parameters, we think most parameters do not need to be changed, but an optimized `list_alpha` can improve the unmixing accuracy. In our paper, we optimized the alpha using cross-validation, but it requires manual labeling of many traces, which is time consuming. Users can start with `list_alpha = [1]`, because we showed that most of our optimized alpha are close to 1, and using a user-defined initial alpha=1 can give nearly the same accuracy for most videos without extreme conditions. 
-
-However, if the experimental conditions are very different from our test datasets, using cross-validation to optimize alpha will potentially be more reliable. Because cross-validation requires multiple videos, we don't provide demo for cross-validation, but users can run through our paper reproduction code in the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) to see how cross-validation can be done. Here, we will briefly introduce how to perform cross-validation, and use our ABO dataset as an example. The following folders will refer to the folder in the paper reproduction repo. 
-
-(1) Find a dataset containing multiple videos with similar experimental conditions. The three major datasets in our paper, ABO, NAOMi, 1p, are all qualified. (2) Manually label ground truth transients using the MATLAB GUI in the folder `TemporalLabelingGUI` (We already provided the ground truth transients for the paper reproduction datasets). (3) Run TUnCaT with multiple alpha in `list_alpha` using `TUnCaT_multi_ABO.py`. For a new dataset, you can also start with `demo_TUnCaT.py`, and set `list_alpha = [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10]`. Make sure `multi_alpha = True`. (4) Calculate the F1 scores of all videos with different alpha using `evaluation/eval_ABO_ours.m`. (5) Find the optimal alpha for each cross-validation round using `evaluation/cross_validation.m`. You can load the file storing the calculated F1 scores, or run `cross_validation.m` immediately after `eval_ABO_ours.m` to avoid reloading the F1 scores.
-
-
-# Citation 
-If you use any part of this software in your work, please cite our paper:
-Bao, Y., E. Redington, A. Agarwal, and Y. Gong, Decontaminate traces from fluorescence calcium imaging videos using targeted nonnegative matrix factorization. Frontiers in Neuroscience (2021 (in press)). doi: [10.3389/fnins.2021.797421](https://www.frontiersin.org/articles/10.3389/fnins.2021.797421/abstract).
-
-
-# Licensing and Copyright
-TUnCaT is released under [the GNU License, Version 2.0](LICENSE).
-
-
-# Sponsors
-<img src="readme/NSFBRAIN.png" height="100"/><img src="readme/BRF.png" height="100"/><img src="readme/Beckmanlogo.png" height="100"/>
-<br>
-<img src="readme/valleelogo.png" height="100"/><img src="readme/dibslogo.png" height="100"/><img src="readme/sloan_logo_new.jpg" height="100"/>
+Metadata-Version: 2.1
+Name: tuncat
+Version: 1.0.4
+Summary: Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. 
+Home-page: https://github.com/YijunBao/TUnCaT
+Author: Yijun Bao
+Author-email: yijun.bao@duke.edu
+Maintainer: Yijun Bao
+Maintainer-email: yijun.bao@duke.edu
+License: the GNU License, Version 2.0
+Project-URL: Source Code, https://github.com/YijunBao/TUnCaT
+Project-URL: Citation, https://doi.org/10.5281/zenodo.5764576
+Project-URL: Paper, https://doi.org/10.3389/fnins.2021.797421
+Description: ![NeuroToolbox logo](readme/neurotoolbox-logo.svg)
+        
+        [![DOI](https://zenodo.org/badge/397026426.svg)](https://zenodo.org/badge/latestdoi/397026426)
+        
+        # TUnCaT
+        Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. TUnCaT removed false transients caused by large-scale background fluctuation using background subtraction; TUnCaT removed false transients caused by neighboring neurons, axons, and dendrites using nonnegative matrix factorization (NMF).
+        
+        Copyright (C) 2021 Duke University NeuroToolbox
+        
+        This repo contains the code of TUnCaT. If you want to reproduce the results in our paper, please visit the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) or [figshare](https://figshare.com/articles/dataset/TUnCaT_paper_reproduction/17132069) to find the data, results, and code to analyze the results. 
+        
+        - [TUnCaT](#tuncat)
+        - [Installation on Windows or Linux](#installation-on-windows-or-linux)
+        - [Demo](#demo)
+        - [Input, Output, and Intermediate Files](#input-output-and-intermediate-files)
+          - [Input files](#input-files)
+          - [Intermediate and Output files](#intermediate-and-output-files)
+        - [Use your own data](#use-your-own-data)
+          - [Use your own videos](#use-your-own-videos)
+          - [Use your own neuron masks](#use-your-own-neuron-masks)
+          - [Set the unmixing parameters](#set-the-unmixing-parameters)
+            - [Set alpha as a user-defined value or using cross-validation](#set-alpha-as-a-user-defined-value-or-using-cross-validation)
+        - [Citation](#citation)
+        - [Licensing and Copyright](#licensing-and-copyright)
+        - [Sponsors](#sponsors)
+        
+        
+        # Installation on Windows or Linux 
+        * First, install Python from the [official website](https://www.python.org/downloads/) or any other distribution like [Anaconda](https://www.anaconda.com/). 
+        * Launch Windows/Linux terminal or Anaconda prompt, and install TUnCaT using pip:
+        ```bat
+        python -m pip install tuncat
+        ```
+        * Please be aware that the speed of TUnCaT in the Anaconda installation may be significantly slower than the speed in the offical python installation in Windows.
+        
+        
+        # Demo
+        We provided a demo for all users to get familiar with TUnCaT. To run the demo, please download the code from our GitHub repository. We provided a one-photon imaging video `c28_163_244.h5` as well as its manually labeled neurons `FinalMasks_c28_163_244.mat`. The demo will calculate the raw traces and background traces of all neurons, calculate the unmixed traces using TUnCaT, and export them to the folder `unmixed_traces`. The input, output, and intermediate files will be explained in [Input, Output, and Intermediate Files](#input-output-and-intermediate-files). 
+        
+        To run the demo python script, launch system terminal or Anaconda prompt, and type the following script 
+        ```bat
+        cd {TUnCaT_root_path}
+        python demo_TUnCaT.py
+        ```
+        You can also run the demo `demo_TUnCaT.ipynb` interactively using Jupyter Notebook. This notebook contains the expected figure of the background-subtracted trace and the unmixed trace of the first neuron. The saved processing time is recorded in a laptop with an AMD Ryzen 5 3500U quad-core CPU.
+        
+        
+        # Input, Output, and Intermediate Files
+        By default, all the input, output, and intermediate files are saved under the `TUnCaT` folder. 
+        
+        ## Input files
+        * A .h5 file `{name}.h5` contains the input video. This is a 3D dataset with shape = (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The demo video has (T, Lx, Ly) = (6000, 50, 50). 
+        * A .mat file `FinalMasks_{name}.mat` contains the nueron masks of the video. This is a 3D array with shape = (Ly, Lx, n) in MATLAB, where Ly and Lx should match the lateral dimensions of the video, and n is the number of neurons. The demo mask has (Ly, Lx, n) = (50, 50, 45). 
+        * Important notice: The default dimension order for multi-dimensional array is reversed in MATLAB and python. When you save a dataset with shape = (L1, L2, L3) in MATLAB to an .h5 file or a .mat file with version 7.3 or newer (requiring h5py.File to load in python workspace), and then load it in python, the shape will become (L3, L2, L1). However, if you save the dataset as a .mat file with version 7 or earlier (requiring scipy.loadmat to load in python workspace), the dimensions will preserve and still be (L1, L2, L3). In this document, we will use the python default order to describe the datasets in python workspace or saved in .h5, and use the MATLAB default order to describe the datasets saved in .mat. Sometimes you need to transpose the dimensions to make them consistent. In python, you can transpose the dimensions using `Masks = Masks.transpose((2,1,0))`. In MATLAB, you can transpose the dimensions using `Masks = permute(Masks,[3,2,1])`.
+        
+        ## Intermediate and Output files
+        After running TUnCaT on the demo video, the intermediate and output files will be under a new folder `unmixed_traces`. 
+        * Intermediate file: `unmixed_traces/raw/{name}.mat` stores the raw neuron traces (`traces`) and the background traces (`bgtraces`). Each trace variable is 2D matrix with shape = (T, n), where T is the number of frames, and n is the number of neurons. 
+        * Output file: `unmixed_traces/alpha={}/{name}.mat` or `unmixed_traces/list_alpha={}/{name}.mat` stores the unmixed traces of the neurons (`traces_nmfdemix`), as well as other quantities characterizing the NMF unmixing process of each neuron, including the mixing matrix (`list_mixout`), final alpha (`list_alpha_final`), reconstruction residual (`list_MSE`), and number of iterations (`list_n_iter`). See the function descriptions for the detailed meanings of these quantities.
+        
+        
+        # Use your own data
+        Of course, you can modify the demo scripts to process other videos. You need to set the folders of the videos and neuron masks, and change some parameters in the python scripts to correspond to your videos. 
+        
+        ## Use your own videos
+        * Set the folder and file names of your video correctly. You need to change the variables `dir_video` and `list_Exp_ID`. The variable `dir_video` is the folder containing the input videos. For example, if your videos are stored in `C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data`, set `dir_video = 'C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data'`. You can also use relative path, such as `dir_video = './data'`. The variable `list_Exp_ID` is the list of the file names (without extension) of the input videos (e.g., `list_Exp_ID = ['c28_163_244']` in the demo referes to the input file `{TUnCaT_root_path}/data/c28_163_244.h5`). 
+        * Currently, we only support .h5 files as the input video, so you need to convert the format of your data to .h5. You can save the video in a dataset with any name, but don't save the video under any group. The video should have a shape of (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The support to more video formats will come soon. When doing format conversion, make sure the dimension is in the correct order. For example, if you save save the .h5 files from MATLAB, the shape of the dataset should be (Ly, Lx, T) in MATLAB. See [Input files](#input-files) for more explanation of the dimension order.
+        
+        ## Use your own neuron masks
+        * Set the folder and file names of your mask files correctly. You need to change variable `dir_mask` to the folder containing the mask files. 
+        * Currently, we only support .mat files as the neuron masks, so you need to convert the format of your neuron masks to .mat, and save the neuron masks in dataset 'FinalMasks'. The name of the masks file should be `FinalMasks_{Exp_ID}.mat`, where the `{Exp_ID}` is the name of the corresponding video. The neuron masks should be saved as a 3D array named `FinalMasks`, and the dimension should be (Ly, Lx, n) in MATLAB, where Ly and Lx are the same as the lateral dimension of the video, and n is the number of neurons.
+        * The masks created by some manual labeling software may contain an empty (all zero) image as the first frame. You need to remove the empty frame before saving them.
+        
+        ## Set the unmixing parameters
+        * The list of video names (e.g., `list_Exp_ID = ['c28_163_244']`)
+        * The folder of the video (e.g., `dir_video='./data'`);
+        * The folder of the neuron masks (e.g., `dir_masks='./data'`);
+        * The folder of the output traces (e.g., `dir_traces='./data/unmixed_traces'`);
+        * `list_alpha` is the list of tested alpha;
+        * `multi_alpha` determines the option to deal with multiple elements in `list_alpha`. False means the largest element providing non-trivial output traces will be used, which can be differnt for different neurons. True means each element will be tested and saved independently. These options are equivalent when there is only one element in `list_alpha`;
+        * `Qclip` is clipping quantile. Traces lower than this quantile are clipped to this quantile value;
+        * `th_pertmin` is maximum pertentage of unmixed traces equaling to the trace minimum;
+        * `epsilon` is the minimum value of the input traces after scaling and shifting;
+        * `th_residual` is the maximum factorization residual if this value is not zero;
+        * `nbin` is the temporal downsampling ratio;
+        * `bin_option` determines the temporal downsampling option. It can be 'downsample', 'sum', or 'mean'. It is not used when nbin == 1;
+        * `flexible_alpha` determines whether a flexible alpha strategy is used when the smallest alpha in "list_alpha" already caused over-regularization.
+        
+        ### Set alpha as a user-defined value or using cross-validation
+        Among the above parameters, we think most parameters do not need to be changed, but an optimized `list_alpha` can improve the unmixing accuracy. In our paper, we optimized the alpha using cross-validation, but it requires manual labeling of many traces, which is time consuming. Users can start with `list_alpha = [1]`, because we showed that most of our optimized alpha are close to 1, and using a user-defined initial alpha=1 can give nearly the same accuracy for most videos without extreme conditions. 
+        
+        However, if the experimental conditions are very different from our test datasets, using cross-validation to optimize alpha will potentially be more reliable. Because cross-validation requires multiple videos, we don't provide demo for cross-validation, but users can run through our paper reproduction code in the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) to see how cross-validation can be done. Here, we will briefly introduce how to perform cross-validation, and use our ABO dataset as an example. The following folders will refer to the folder in the paper reproduction repo. 
+        
+        (1) Find a dataset containing multiple videos with similar experimental conditions. The three major datasets in our paper, ABO, NAOMi, 1p, are all qualified. (2) Manually label ground truth transients using the MATLAB GUI in the folder `TemporalLabelingGUI` (We already provided the ground truth transients for the paper reproduction datasets). (3) Run TUnCaT with multiple alpha in `list_alpha` using `TUnCaT_multi_ABO.py`. For a new dataset, you can also start with `demo_TUnCaT.py`, and set `list_alpha = [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10]`. Make sure `multi_alpha = True`. (4) Calculate the F1 scores of all videos with different alpha using `evaluation/eval_ABO_ours.m`. (5) Find the optimal alpha for each cross-validation round using `evaluation/cross_validation.m`. You can load the file storing the calculated F1 scores, or run `cross_validation.m` immediately after `eval_ABO_ours.m` to avoid reloading the F1 scores.
+        
+        
+        # Citation 
+        If you use any part of this software in your work, please cite our paper:
+        Bao, Y., E. Redington, A. Agarwal, and Y. Gong, Decontaminate traces from fluorescence calcium imaging videos using targeted nonnegative matrix factorization. Frontiers in Neuroscience (2021 (in press)). doi: [10.3389/fnins.2021.797421](https://www.frontiersin.org/articles/10.3389/fnins.2021.797421/abstract).
+        
+        
+        # Licensing and Copyright
+        TUnCaT is released under [the GNU License, Version 2.0](LICENSE).
+        
+        
+        # Sponsors
+        <img src="readme/NSFBRAIN.png" height="100"/><img src="readme/BRF.png" height="100"/><img src="readme/Beckmanlogo.png" height="100"/>
+        <br>
+        <img src="readme/valleelogo.png" height="100"/><img src="readme/dibslogo.png" height="100"/><img src="readme/sloan_logo_new.jpg" height="100"/>
+        
+Platform: all
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3
+Description-Content-Type: text/markdown
```

### Comparing `tuncat-1.0.3/setup.py` & `tuncat-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='tuncat',
-    version='1.0.3',
+    version='1.0.4',
     description=(
         'Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. '
     ),
     long_description=open('README.md').read(),
     # long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yijun Bao',
@@ -32,14 +32,14 @@
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Bio-Informatics'
     ],
     install_requires=[
         'numpy',
         'scipy',
-        'scikit-learn',
+        'scikit-learn <1.2',
         'numba',
         'h5py',
         'matplotlib'
     ],
     python_requires='>=3'
     )
```

### Comparing `tuncat-1.0.3/tuncat/bin_trace_video.py` & `tuncat-1.0.4/tuncat/bin_trace_video.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/more_options/nmfunmix1_pertmin_res_MSE_novideo_2side.py` & `tuncat-1.0.4/tuncat/more_options/nmfunmix1_pertmin_res_MSE_novideo_2side.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/more_options/nmfunmix_MSE_allow0.py` & `tuncat-1.0.4/tuncat/more_options/nmfunmix_MSE_allow0.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/nmfunmix1_pertmin_res_MSE_novideo.py` & `tuncat-1.0.4/tuncat/nmfunmix1_pertmin_res_MSE_novideo.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/nmfunmix_MSE.py` & `tuncat-1.0.4/tuncat/nmfunmix_MSE.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/run_TUnCaT.py` & `tuncat-1.0.4/tuncat/run_TUnCaT.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,29 +130,35 @@
             print('Using memory mapping for trace calculation.')
         
     if trace_method == 'shm':
         # Create the shared memory object for the video
         if isinstance(filename_video, str):
             nbytes_video = int(video_dtype.itemsize * file_video[varname].size)
             shm_video = SharedMemory(create=True, size=nbytes_video)
-            video = np.frombuffer(shm_video.buf, dtype = video_dtype)
-            video[:] = file_video[varname][()].ravel()
-            video = video.reshape(file_video[varname].shape)
+            video = np.ndarray(video_shape, dtype = video_dtype, buffer=shm_video.buf)
+            video[:] = file_video[varname][:]
+            # video = np.frombuffer(shm_video.buf, dtype = video_dtype)
+            # video[:] = file_video[varname][()].ravel()
+            # video = video.reshape(file_video[varname].shape)
         else:
             nbytes_video = int(video_dtype.itemsize * filename_video.size)
             shm_video = SharedMemory(create=True, size=nbytes_video)
-            video = np.frombuffer(shm_video.buf, dtype = video_dtype)
-            video[:] = filename_video[()].ravel()
-            video = video.reshape(filename_video.shape)
+            video = np.ndarray(video_shape, dtype = video_dtype, buffer=shm_video.buf)
+            video[:] = filename_video[:]
+            # video = np.frombuffer(shm_video.buf, dtype = video_dtype)
+            # video[:] = filename_video[()].ravel()
+            # video = video.reshape(filename_video.shape)
 
         # Create the shared memory object for the masks
         shm_masks = SharedMemory(create=True, size=Masks.nbytes)
-        FinalMasks = np.frombuffer(shm_masks.buf, dtype = 'bool')
-        FinalMasks[:] = Masks.ravel()
-        FinalMasks = FinalMasks.reshape(Masks.shape)
+        FinalMasks = np.ndarray(masks_shape, dtype = 'bool', buffer=shm_masks.buf)
+        FinalMasks[:] = Masks[:]
+        # FinalMasks = np.frombuffer(shm_masks.buf, dtype = 'bool')
+        # FinalMasks[:] = Masks.ravel()
+        # FinalMasks = FinalMasks.reshape(Masks.shape)
         del Masks
 
     elif trace_method == 'memmap':
         name_mmap = Exp_ID
         # Create the memory mapping file for the video
         fn_video = name_mmap + 'video.dat'
         fp_video = np.memmap(fn_video, dtype=video_dtype, mode='w+', shape=(T,Lx*Ly))
@@ -241,22 +247,28 @@
             os.makedirs(dir_trace_unmix)        
         savemat(os.path.join(dir_trace_unmix, Exp_ID+".mat"), {"traces_nmfdemix": traces_nmfdemix,\
             "list_mixout":list_mixout, "list_MSE":list_MSE, "list_final_alpha":list_final_alpha, "list_n_iter":list_n_iter})
 
 
     if trace_method == 'shm':
         # Unlink shared memory objects
+        del video
         shm_video.close()
         shm_video.unlink()
+        del FinalMasks
         shm_masks.close()
         shm_masks.unlink()
     elif trace_method == 'memmap':
         # Delete memory mapping files
         fp_masks._mmap.close()
         del fp_masks
         os.remove(fn_masks)
         fp_video._mmap.close()
         del fp_video
         os.remove(fn_video)
 
+    if len(list_alpha) == 0:
+        traces_nmfdemix = 0
+        list_mixout = 0
+
     return traces_nmfdemix, list_mixout, traces, bgtraces
```

### Comparing `tuncat-1.0.3/tuncat/traces_from_masks_mp_mmap_fn_neighbors.py` & `tuncat-1.0.4/tuncat/traces_from_masks_mp_mmap_fn_neighbors.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/traces_from_masks_mp_shm_neighbors.py` & `tuncat-1.0.4/tuncat/traces_from_masks_mp_shm_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,20 +84,24 @@
     # Find the neighboring neurons of all neurons. 
     (list_neighbors, comx, comy, area, r_bg) = find_neighbors(FinalMasks)
 
     # Create shared memory objects for x and y coordinates
     [xx, yy] = np.meshgrid(np.arange(Ly), np.arange(Lx))
     xx = xx.astype('uint16')
     shm_xx = SharedMemory(create=True, size=xx.nbytes)
-    xx_temp = np.frombuffer(shm_xx.buf, dtype='uint16')
-    xx_temp[:] = xx.ravel()
+    xx_temp = np.ndarray(xx.shape, dtype='uint16', buffer=shm_xx.buf)
+    xx_temp[:] = xx[:]
+    # xx_temp = np.frombuffer(shm_xx.buf, dtype='uint16')
+    # xx_temp[:] = xx.ravel()
     yy = yy.astype('uint16')
     shm_yy = SharedMemory(create=True, size=yy.nbytes)
-    yy_temp = np.frombuffer(shm_yy.buf, dtype='uint16')
-    yy_temp[:] = yy.ravel()
+    yy_temp = np.ndarray(yy.shape, dtype='uint16', buffer=shm_yy.buf)
+    yy_temp[:] = yy[:]
+    # yy_temp = np.frombuffer(shm_yy.buf, dtype='uint16')
+    # yy_temp[:] = yy.ravel()
     
     # results = []
     # for nn in range(ncells):
     #     results.append(mean_median_out_trace(nn, shm_video, video_dtype, video_shape, \
     #         shm_masks, shm_xx, shm_yy, r_bg, comx, comy, area[nn], list_neighbors[nn]))
 
     # Calculate the traces of the neuron, background, and outside region for each neuron. 
@@ -107,16 +111,18 @@
     p.close()
 
     traces = np.vstack([x[0] for x in results]).T
     bgtraces = np.vstack([x[1] for x in results]).T
     outtraces = np.array([x[2] for x in results]).T
 
     # Unlink shared memory objects
+    del xx_temp
     shm_xx.close()
     shm_xx.unlink()
+    del yy_temp
     shm_yy.close()
     shm_yy.unlink()
 
     return traces, bgtraces, outtraces, list_neighbors
 
 
 def find_neighbors(FinalMasks):
```

### Comparing `tuncat-1.0.3/tuncat/traces_from_masks_numba_neighbors.py` & `tuncat-1.0.4/tuncat/traces_from_masks_numba_neighbors.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/use_nmfunmix_mp_MSE_novideo.py` & `tuncat-1.0.4/tuncat/use_nmfunmix_mp_MSE_novideo.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat/utils.py` & `tuncat-1.0.4/tuncat/utils.py`

 * *Files identical despite different names*

### Comparing `tuncat-1.0.3/tuncat.egg-info/PKG-INFO` & `tuncat-1.0.4/tuncat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,132 @@
 Metadata-Version: 2.1
 Name: tuncat
-Version: 1.0.3
+Version: 1.0.4
 Summary: Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. 
 Home-page: https://github.com/YijunBao/TUnCaT
 Author: Yijun Bao
 Author-email: yijun.bao@duke.edu
 Maintainer: Yijun Bao
 Maintainer-email: yijun.bao@duke.edu
 License: the GNU License, Version 2.0
 Project-URL: Source Code, https://github.com/YijunBao/TUnCaT
 Project-URL: Citation, https://doi.org/10.5281/zenodo.5764576
 Project-URL: Paper, https://doi.org/10.3389/fnins.2021.797421
+Description: ![NeuroToolbox logo](readme/neurotoolbox-logo.svg)
+        
+        [![DOI](https://zenodo.org/badge/397026426.svg)](https://zenodo.org/badge/latestdoi/397026426)
+        
+        # TUnCaT
+        Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. TUnCaT removed false transients caused by large-scale background fluctuation using background subtraction; TUnCaT removed false transients caused by neighboring neurons, axons, and dendrites using nonnegative matrix factorization (NMF).
+        
+        Copyright (C) 2021 Duke University NeuroToolbox
+        
+        This repo contains the code of TUnCaT. If you want to reproduce the results in our paper, please visit the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) or [figshare](https://figshare.com/articles/dataset/TUnCaT_paper_reproduction/17132069) to find the data, results, and code to analyze the results. 
+        
+        - [TUnCaT](#tuncat)
+        - [Installation on Windows or Linux](#installation-on-windows-or-linux)
+        - [Demo](#demo)
+        - [Input, Output, and Intermediate Files](#input-output-and-intermediate-files)
+          - [Input files](#input-files)
+          - [Intermediate and Output files](#intermediate-and-output-files)
+        - [Use your own data](#use-your-own-data)
+          - [Use your own videos](#use-your-own-videos)
+          - [Use your own neuron masks](#use-your-own-neuron-masks)
+          - [Set the unmixing parameters](#set-the-unmixing-parameters)
+            - [Set alpha as a user-defined value or using cross-validation](#set-alpha-as-a-user-defined-value-or-using-cross-validation)
+        - [Citation](#citation)
+        - [Licensing and Copyright](#licensing-and-copyright)
+        - [Sponsors](#sponsors)
+        
+        
+        # Installation on Windows or Linux 
+        * First, install Python from the [official website](https://www.python.org/downloads/) or any other distribution like [Anaconda](https://www.anaconda.com/). 
+        * Launch Windows/Linux terminal or Anaconda prompt, and install TUnCaT using pip:
+        ```bat
+        python -m pip install tuncat
+        ```
+        * Please be aware that the speed of TUnCaT in the Anaconda installation may be significantly slower than the speed in the offical python installation in Windows.
+        
+        
+        # Demo
+        We provided a demo for all users to get familiar with TUnCaT. To run the demo, please download the code from our GitHub repository. We provided a one-photon imaging video `c28_163_244.h5` as well as its manually labeled neurons `FinalMasks_c28_163_244.mat`. The demo will calculate the raw traces and background traces of all neurons, calculate the unmixed traces using TUnCaT, and export them to the folder `unmixed_traces`. The input, output, and intermediate files will be explained in [Input, Output, and Intermediate Files](#input-output-and-intermediate-files). 
+        
+        To run the demo python script, launch system terminal or Anaconda prompt, and type the following script 
+        ```bat
+        cd {TUnCaT_root_path}
+        python demo_TUnCaT.py
+        ```
+        You can also run the demo `demo_TUnCaT.ipynb` interactively using Jupyter Notebook. This notebook contains the expected figure of the background-subtracted trace and the unmixed trace of the first neuron. The saved processing time is recorded in a laptop with an AMD Ryzen 5 3500U quad-core CPU.
+        
+        
+        # Input, Output, and Intermediate Files
+        By default, all the input, output, and intermediate files are saved under the `TUnCaT` folder. 
+        
+        ## Input files
+        * A .h5 file `{name}.h5` contains the input video. This is a 3D dataset with shape = (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The demo video has (T, Lx, Ly) = (6000, 50, 50). 
+        * A .mat file `FinalMasks_{name}.mat` contains the nueron masks of the video. This is a 3D array with shape = (Ly, Lx, n) in MATLAB, where Ly and Lx should match the lateral dimensions of the video, and n is the number of neurons. The demo mask has (Ly, Lx, n) = (50, 50, 45). 
+        * Important notice: The default dimension order for multi-dimensional array is reversed in MATLAB and python. When you save a dataset with shape = (L1, L2, L3) in MATLAB to an .h5 file or a .mat file with version 7.3 or newer (requiring h5py.File to load in python workspace), and then load it in python, the shape will become (L3, L2, L1). However, if you save the dataset as a .mat file with version 7 or earlier (requiring scipy.loadmat to load in python workspace), the dimensions will preserve and still be (L1, L2, L3). In this document, we will use the python default order to describe the datasets in python workspace or saved in .h5, and use the MATLAB default order to describe the datasets saved in .mat. Sometimes you need to transpose the dimensions to make them consistent. In python, you can transpose the dimensions using `Masks = Masks.transpose((2,1,0))`. In MATLAB, you can transpose the dimensions using `Masks = permute(Masks,[3,2,1])`.
+        
+        ## Intermediate and Output files
+        After running TUnCaT on the demo video, the intermediate and output files will be under a new folder `unmixed_traces`. 
+        * Intermediate file: `unmixed_traces/raw/{name}.mat` stores the raw neuron traces (`traces`) and the background traces (`bgtraces`). Each trace variable is 2D matrix with shape = (T, n), where T is the number of frames, and n is the number of neurons. 
+        * Output file: `unmixed_traces/alpha={}/{name}.mat` or `unmixed_traces/list_alpha={}/{name}.mat` stores the unmixed traces of the neurons (`traces_nmfdemix`), as well as other quantities characterizing the NMF unmixing process of each neuron, including the mixing matrix (`list_mixout`), final alpha (`list_alpha_final`), reconstruction residual (`list_MSE`), and number of iterations (`list_n_iter`). See the function descriptions for the detailed meanings of these quantities.
+        
+        
+        # Use your own data
+        Of course, you can modify the demo scripts to process other videos. You need to set the folders of the videos and neuron masks, and change some parameters in the python scripts to correspond to your videos. 
+        
+        ## Use your own videos
+        * Set the folder and file names of your video correctly. You need to change the variables `dir_video` and `list_Exp_ID`. The variable `dir_video` is the folder containing the input videos. For example, if your videos are stored in `C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data`, set `dir_video = 'C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data'`. You can also use relative path, such as `dir_video = './data'`. The variable `list_Exp_ID` is the list of the file names (without extension) of the input videos (e.g., `list_Exp_ID = ['c28_163_244']` in the demo referes to the input file `{TUnCaT_root_path}/data/c28_163_244.h5`). 
+        * Currently, we only support .h5 files as the input video, so you need to convert the format of your data to .h5. You can save the video in a dataset with any name, but don't save the video under any group. The video should have a shape of (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The support to more video formats will come soon. When doing format conversion, make sure the dimension is in the correct order. For example, if you save save the .h5 files from MATLAB, the shape of the dataset should be (Ly, Lx, T) in MATLAB. See [Input files](#input-files) for more explanation of the dimension order.
+        
+        ## Use your own neuron masks
+        * Set the folder and file names of your mask files correctly. You need to change variable `dir_mask` to the folder containing the mask files. 
+        * Currently, we only support .mat files as the neuron masks, so you need to convert the format of your neuron masks to .mat, and save the neuron masks in dataset 'FinalMasks'. The name of the masks file should be `FinalMasks_{Exp_ID}.mat`, where the `{Exp_ID}` is the name of the corresponding video. The neuron masks should be saved as a 3D array named `FinalMasks`, and the dimension should be (Ly, Lx, n) in MATLAB, where Ly and Lx are the same as the lateral dimension of the video, and n is the number of neurons.
+        * The masks created by some manual labeling software may contain an empty (all zero) image as the first frame. You need to remove the empty frame before saving them.
+        
+        ## Set the unmixing parameters
+        * The list of video names (e.g., `list_Exp_ID = ['c28_163_244']`)
+        * The folder of the video (e.g., `dir_video='./data'`);
+        * The folder of the neuron masks (e.g., `dir_masks='./data'`);
+        * The folder of the output traces (e.g., `dir_traces='./data/unmixed_traces'`);
+        * `list_alpha` is the list of tested alpha;
+        * `multi_alpha` determines the option to deal with multiple elements in `list_alpha`. False means the largest element providing non-trivial output traces will be used, which can be differnt for different neurons. True means each element will be tested and saved independently. These options are equivalent when there is only one element in `list_alpha`;
+        * `Qclip` is clipping quantile. Traces lower than this quantile are clipped to this quantile value;
+        * `th_pertmin` is maximum pertentage of unmixed traces equaling to the trace minimum;
+        * `epsilon` is the minimum value of the input traces after scaling and shifting;
+        * `th_residual` is the maximum factorization residual if this value is not zero;
+        * `nbin` is the temporal downsampling ratio;
+        * `bin_option` determines the temporal downsampling option. It can be 'downsample', 'sum', or 'mean'. It is not used when nbin == 1;
+        * `flexible_alpha` determines whether a flexible alpha strategy is used when the smallest alpha in "list_alpha" already caused over-regularization.
+        
+        ### Set alpha as a user-defined value or using cross-validation
+        Among the above parameters, we think most parameters do not need to be changed, but an optimized `list_alpha` can improve the unmixing accuracy. In our paper, we optimized the alpha using cross-validation, but it requires manual labeling of many traces, which is time consuming. Users can start with `list_alpha = [1]`, because we showed that most of our optimized alpha are close to 1, and using a user-defined initial alpha=1 can give nearly the same accuracy for most videos without extreme conditions. 
+        
+        However, if the experimental conditions are very different from our test datasets, using cross-validation to optimize alpha will potentially be more reliable. Because cross-validation requires multiple videos, we don't provide demo for cross-validation, but users can run through our paper reproduction code in the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) to see how cross-validation can be done. Here, we will briefly introduce how to perform cross-validation, and use our ABO dataset as an example. The following folders will refer to the folder in the paper reproduction repo. 
+        
+        (1) Find a dataset containing multiple videos with similar experimental conditions. The three major datasets in our paper, ABO, NAOMi, 1p, are all qualified. (2) Manually label ground truth transients using the MATLAB GUI in the folder `TemporalLabelingGUI` (We already provided the ground truth transients for the paper reproduction datasets). (3) Run TUnCaT with multiple alpha in `list_alpha` using `TUnCaT_multi_ABO.py`. For a new dataset, you can also start with `demo_TUnCaT.py`, and set `list_alpha = [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10]`. Make sure `multi_alpha = True`. (4) Calculate the F1 scores of all videos with different alpha using `evaluation/eval_ABO_ours.m`. (5) Find the optimal alpha for each cross-validation round using `evaluation/cross_validation.m`. You can load the file storing the calculated F1 scores, or run `cross_validation.m` immediately after `eval_ABO_ours.m` to avoid reloading the F1 scores.
+        
+        
+        # Citation 
+        If you use any part of this software in your work, please cite our paper:
+        Bao, Y., E. Redington, A. Agarwal, and Y. Gong, Decontaminate traces from fluorescence calcium imaging videos using targeted nonnegative matrix factorization. Frontiers in Neuroscience (2021 (in press)). doi: [10.3389/fnins.2021.797421](https://www.frontiersin.org/articles/10.3389/fnins.2021.797421/abstract).
+        
+        
+        # Licensing and Copyright
+        TUnCaT is released under [the GNU License, Version 2.0](LICENSE).
+        
+        
+        # Sponsors
+        <img src="readme/NSFBRAIN.png" height="100"/><img src="readme/BRF.png" height="100"/><img src="readme/Beckmanlogo.png" height="100"/>
+        <br>
+        <img src="readme/valleelogo.png" height="100"/><img src="readme/dibslogo.png" height="100"/><img src="readme/sloan_logo_new.jpg" height="100"/>
+        
 Platform: all
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![NeuroToolbox logo](readme/neurotoolbox-logo.svg)
-
-[![DOI](https://zenodo.org/badge/397026426.svg)](https://zenodo.org/badge/latestdoi/397026426)
-
-# TUnCaT
-Temporal Unmixing of Calcium Traces (TUnCaT) is an automatic algorithm to decontaminate false transients from temporal traces generated from fluorescent calcium imaging videos. TUnCaT removed false transients caused by large-scale background fluctuation using background subtraction; TUnCaT removed false transients caused by neighboring neurons, axons, and dendrites using nonnegative matrix factorization (NMF).
-
-Copyright (C) 2021 Duke University NeuroToolbox
-
-This repo contains the code of TUnCaT. If you want to reproduce the results in our paper, please visit the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) or [figshare](https://figshare.com/articles/dataset/TUnCaT_paper_reproduction/17132069) to find the data, results, and code to analyze the results. 
-
-- [TUnCaT](#tuncat)
-- [Installation on Windows or Linux](#installation-on-windows-or-linux)
-- [Demo](#demo)
-- [Input, Output, and Intermediate Files](#input-output-and-intermediate-files)
-  - [Input files](#input-files)
-  - [Intermediate and Output files](#intermediate-and-output-files)
-- [Use your own data](#use-your-own-data)
-  - [Use your own videos](#use-your-own-videos)
-  - [Use your own neuron masks](#use-your-own-neuron-masks)
-  - [Set the unmixing parameters](#set-the-unmixing-parameters)
-    - [Set alpha as a user-defined value or using cross-validation](#set-alpha-as-a-user-defined-value-or-using-cross-validation)
-- [Citation](#citation)
-- [Licensing and Copyright](#licensing-and-copyright)
-- [Sponsors](#sponsors)
-
-
-# Installation on Windows or Linux 
-* First, install Python from the [official website](https://www.python.org/downloads/) or any other distribution like [Anaconda](https://www.anaconda.com/). 
-* Launch Windows/Linux terminal or Anaconda prompt, and install TUnCaT using pip:
-```bat
-python -m pip install tuncat
-```
-* Please be aware that the speed of TUnCaT in the Anaconda installation may be significantly slower than the speed in the offical python installation in Windows.
-
-
-# Demo
-We provided a demo for all users to get familiar with TUnCaT. To run the demo, please download the code from our GitHub repository. We provided a one-photon imaging video `c28_163_244.h5` as well as its manually labeled neurons `FinalMasks_c28_163_244.mat`. The demo will calculate the raw traces and background traces of all neurons, calculate the unmixed traces using TUnCaT, and export them to the folder `unmixed_traces`. The input, output, and intermediate files will be explained in [Input, Output, and Intermediate Files](#input-output-and-intermediate-files). 
-
-To run the demo python script, launch system terminal or Anaconda prompt, and type the following script 
-```bat
-cd {TUnCaT_root_path}
-python demo_TUnCaT.py
-```
-You can also run the demo `demo_TUnCaT.ipynb` interactively using Jupyter Notebook. This notebook contains the expected figure of the background-subtracted trace and the unmixed trace of the first neuron. The saved processing time is recorded in a laptop with an AMD Ryzen 5 3500U quad-core CPU.
-
-
-# Input, Output, and Intermediate Files
-By default, all the input, output, and intermediate files are saved under the `TUnCaT` folder. 
-
-## Input files
-* A .h5 file `{name}.h5` contains the input video. This is a 3D dataset with shape = (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The demo video has (T, Lx, Ly) = (6000, 50, 50). 
-* A .mat file `FinalMasks_{name}.mat` contains the nueron masks of the video. This is a 3D array with shape = (Ly, Lx, n) in MATLAB, where Ly and Lx should match the lateral dimensions of the video, and n is the number of neurons. The demo mask has (Ly, Lx, n) = (50, 50, 45). 
-* Important notice: The default dimension order for multi-dimensional array is reversed in MATLAB and python. When you save a dataset with shape = (L1, L2, L3) in MATLAB to an .h5 file or a .mat file with version 7.3 or newer (requiring h5py.File to load in python workspace), and then load it in python, the shape will become (L3, L2, L1). However, if you save the dataset as a .mat file with version 7 or earlier (requiring scipy.loadmat to load in python workspace), the dimensions will preserve and still be (L1, L2, L3). In this document, we will use the python default order to describe the datasets in python workspace or saved in .h5, and use the MATLAB default order to describe the datasets saved in .mat. Sometimes you need to transpose the dimensions to make them consistent. In python, you can transpose the dimensions using `Masks = Masks.transpose((2,1,0))`. In MATLAB, you can transpose the dimensions using `Masks = permute(Masks,[3,2,1])`.
-
-## Intermediate and Output files
-After running TUnCaT on the demo video, the intermediate and output files will be under a new folder `unmixed_traces`. 
-* Intermediate file: `unmixed_traces/raw/{name}.mat` stores the raw neuron traces (`traces`) and the background traces (`bgtraces`). Each trace variable is 2D matrix with shape = (T, n), where T is the number of frames, and n is the number of neurons. 
-* Output file: `unmixed_traces/alpha={}/{name}.mat` or `unmixed_traces/list_alpha={}/{name}.mat` stores the unmixed traces of the neurons (`traces_nmfdemix`), as well as other quantities characterizing the NMF unmixing process of each neuron, including the mixing matrix (`list_mixout`), final alpha (`list_alpha_final`), reconstruction residual (`list_MSE`), and number of iterations (`list_n_iter`). See the function descriptions for the detailed meanings of these quantities.
-
-
-# Use your own data
-Of course, you can modify the demo scripts to process other videos. You need to set the folders of the videos and neuron masks, and change some parameters in the python scripts to correspond to your videos. 
-
-## Use your own videos
-* Set the folder and file names of your video correctly. You need to change the variables `dir_video` and `list_Exp_ID`. The variable `dir_video` is the folder containing the input videos. For example, if your videos are stored in `C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data`, set `dir_video = 'C:/Users/{username}/Documents/GitHub/TUnCaT_paper_reproduction/TUnCaT/data'`. You can also use relative path, such as `dir_video = './data'`. The variable `list_Exp_ID` is the list of the file names (without extension) of the input videos (e.g., `list_Exp_ID = ['c28_163_244']` in the demo referes to the input file `{TUnCaT_root_path}/data/c28_163_244.h5`). 
-* Currently, we only support .h5 files as the input video, so you need to convert the format of your data to .h5. You can save the video in a dataset with any name, but don't save the video under any group. The video should have a shape of (T, Lx, Ly), where T is the number of frames, and (Lx, Ly) is the lateral dimension of each frame. The support to more video formats will come soon. When doing format conversion, make sure the dimension is in the correct order. For example, if you save save the .h5 files from MATLAB, the shape of the dataset should be (Ly, Lx, T) in MATLAB. See [Input files](#input-files) for more explanation of the dimension order.
-
-## Use your own neuron masks
-* Set the folder and file names of your mask files correctly. You need to change variable `dir_mask` to the folder containing the mask files. 
-* Currently, we only support .mat files as the neuron masks, so you need to convert the format of your neuron masks to .mat, and save the neuron masks in dataset 'FinalMasks'. The name of the masks file should be `FinalMasks_{Exp_ID}.mat`, where the `{Exp_ID}` is the name of the corresponding video. The neuron masks should be saved as a 3D array named `FinalMasks`, and the dimension should be (Ly, Lx, n) in MATLAB, where Ly and Lx are the same as the lateral dimension of the video, and n is the number of neurons.
-* The masks created by some manual labeling software may contain an empty (all zero) image as the first frame. You need to remove the empty frame before saving them.
-
-## Set the unmixing parameters
-* The list of video names (e.g., `list_Exp_ID = ['c28_163_244']`)
-* The folder of the video (e.g., `dir_video='./data'`);
-* The folder of the neuron masks (e.g., `dir_masks='./data'`);
-* The folder of the output traces (e.g., `dir_traces='./data/unmixed_traces'`);
-* `list_alpha` is the list of tested alpha;
-* `multi_alpha` determines the option to deal with multiple elements in `list_alpha`. False means the largest element providing non-trivial output traces will be used, which can be differnt for different neurons. True means each element will be tested and saved independently. These options are equivalent when there is only one element in `list_alpha`;
-* `Qclip` is clipping quantile. Traces lower than this quantile are clipped to this quantile value;
-* `th_pertmin` is maximum pertentage of unmixed traces equaling to the trace minimum;
-* `epsilon` is the minimum value of the input traces after scaling and shifting;
-* `th_residual` is the maximum factorization residual if this value is not zero;
-* `nbin` is the temporal downsampling ratio;
-* `bin_option` determines the temporal downsampling option. It can be 'downsample', 'sum', or 'mean'. It is not used when nbin == 1;
-* `flexible_alpha` determines whether a flexible alpha strategy is used when the smallest alpha in "list_alpha" already caused over-regularization.
-
-### Set alpha as a user-defined value or using cross-validation
-Among the above parameters, we think most parameters do not need to be changed, but an optimized `list_alpha` can improve the unmixing accuracy. In our paper, we optimized the alpha using cross-validation, but it requires manual labeling of many traces, which is time consuming. Users can start with `list_alpha = [1]`, because we showed that most of our optimized alpha are close to 1, and using a user-defined initial alpha=1 can give nearly the same accuracy for most videos without extreme conditions. 
-
-However, if the experimental conditions are very different from our test datasets, using cross-validation to optimize alpha will potentially be more reliable. Because cross-validation requires multiple videos, we don't provide demo for cross-validation, but users can run through our paper reproduction code in the [paper reproduction repo](https://github.com/YijunBao/TUnCaT_paper_reproduction) to see how cross-validation can be done. Here, we will briefly introduce how to perform cross-validation, and use our ABO dataset as an example. The following folders will refer to the folder in the paper reproduction repo. 
-
-(1) Find a dataset containing multiple videos with similar experimental conditions. The three major datasets in our paper, ABO, NAOMi, 1p, are all qualified. (2) Manually label ground truth transients using the MATLAB GUI in the folder `TemporalLabelingGUI` (We already provided the ground truth transients for the paper reproduction datasets). (3) Run TUnCaT with multiple alpha in `list_alpha` using `TUnCaT_multi_ABO.py`. For a new dataset, you can also start with `demo_TUnCaT.py`, and set `list_alpha = [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10]`. Make sure `multi_alpha = True`. (4) Calculate the F1 scores of all videos with different alpha using `evaluation/eval_ABO_ours.m`. (5) Find the optimal alpha for each cross-validation round using `evaluation/cross_validation.m`. You can load the file storing the calculated F1 scores, or run `cross_validation.m` immediately after `eval_ABO_ours.m` to avoid reloading the F1 scores.
-
-
-# Citation 
-If you use any part of this software in your work, please cite our paper:
-Bao, Y., E. Redington, A. Agarwal, and Y. Gong, Decontaminate traces from fluorescence calcium imaging videos using targeted nonnegative matrix factorization. Frontiers in Neuroscience (2021 (in press)). doi: [10.3389/fnins.2021.797421](https://www.frontiersin.org/articles/10.3389/fnins.2021.797421/abstract).
-
-
-# Licensing and Copyright
-TUnCaT is released under [the GNU License, Version 2.0](LICENSE).
-
-
-# Sponsors
-<img src="readme/NSFBRAIN.png" height="100"/><img src="readme/BRF.png" height="100"/><img src="readme/Beckmanlogo.png" height="100"/>
-<br>
-<img src="readme/valleelogo.png" height="100"/><img src="readme/dibslogo.png" height="100"/><img src="readme/sloan_logo_new.jpg" height="100"/>
-
-
```

### Comparing `tuncat-1.0.3/tuncat.egg-info/SOURCES.txt` & `tuncat-1.0.4/tuncat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

