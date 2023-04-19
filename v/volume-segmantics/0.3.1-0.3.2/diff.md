# Comparing `tmp/volume_segmantics-0.3.1.tar.gz` & `tmp/volume_segmantics-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volume_segmantics-0.3.1.tar", max compression
+gzip compressed data, was "volume_segmantics-0.3.2.tar", max compression
```

## Comparing `volume_segmantics-0.3.1.tar` & `volume_segmantics-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-02-09 12:36:02.634874 volume_segmantics-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     7861 2023-02-09 12:36:02.634874 volume_segmantics-0.3.1/README.md
--rw-r--r--   0        0        0     1622 2023-02-09 12:36:02.634874 volume_segmantics-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/__init__.py
--rw-r--r--   0        0        0      184 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/data/__init__.py
--rw-r--r--   0        0        0     3219 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/data/augmentations.py
--rw-r--r--   0        0        0     1611 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/data/base_data_manager.py
--rw-r--r--   0        0        0     2564 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/data/dataloaders.py
--rw-r--r--   0        0        0     5532 2023-02-09 12:36:02.662874 volume_segmantics-0.3.1/volume_segmantics/data/datasets.py
--rw-r--r--   0        0        0    13578 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/data/pytorch3dunet_losses.py
--rw-r--r--   0        0        0     5315 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/data/pytorch3dunet_metrics.py
--rw-r--r--   0        0        0      882 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/data/settings_data.py
--rw-r--r--   0        0        0     5947 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/data/slicers.py
--rw-r--r--   0        0        0      251 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/model/__init__.py
--rw-r--r--   0        0        0     2464 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/model/model_2d.py
--rw-r--r--   0        0        0     6416 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_2d_predictor.py
--rw-r--r--   0        0        0    22077 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_2d_trainer.py
--rw-r--r--   0        0        0     4128 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_prediction_manager.py
--rw-r--r--   0        0        0     1419 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/scripts/predict_2d_model.py
--rw-r--r--   0        0        0     3107 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/scripts/train_2d_model.py
--rw-r--r--   0        0        0      256 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/__init__.py
--rw-r--r--   0        0        0     4339 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/arg_parsing.py
--rw-r--r--   0        0        0    11231 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/base_data_utils.py
--rw-r--r--   0        0        0     1821 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/config.py
--rw-r--r--   0        0        0     2537 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/early_stopping.py
--rw-r--r--   0        0        0     1903 2023-02-09 12:36:02.666874 volume_segmantics-0.3.1/volume_segmantics/utilities/pytorch3dunet_utils.py
--rw-r--r--   0        0        0     9364 1970-01-01 00:00:00.000000 volume_segmantics-0.3.1/setup.py
--rw-r--r--   0        0        0     9283 1970-01-01 00:00:00.000000 volume_segmantics-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 17:08:00.564532 volume_segmantics-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     8052 2023-04-19 17:08:00.564532 volume_segmantics-0.3.2/README.md
+-rw-r--r--   0        0        0     1623 2023-04-19 17:08:00.568532 volume_segmantics-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/augmentations.py
+-rw-r--r--   0        0        0     1611 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/base_data_manager.py
+-rw-r--r--   0        0        0     2564 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/dataloaders.py
+-rw-r--r--   0        0        0     5532 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/datasets.py
+-rw-r--r--   0        0        0    13578 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/pytorch3dunet_losses.py
+-rw-r--r--   0        0        0     5315 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/pytorch3dunet_metrics.py
+-rw-r--r--   0        0        0      882 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/settings_data.py
+-rw-r--r--   0        0        0     5947 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/data/slicers.py
+-rw-r--r--   0        0        0      251 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/model/__init__.py
+-rw-r--r--   0        0        0     2534 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/model/model_2d.py
+-rw-r--r--   0        0        0     6416 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_2d_predictor.py
+-rw-r--r--   0        0        0    22077 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_2d_trainer.py
+-rw-r--r--   0        0        0     4128 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_prediction_manager.py
+-rw-r--r--   0        0        0     1419 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/scripts/predict_2d_model.py
+-rw-r--r--   0        0        0     3107 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/scripts/train_2d_model.py
+-rw-r--r--   0        0        0      256 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/__init__.py
+-rw-r--r--   0        0        0     4339 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/arg_parsing.py
+-rw-r--r--   0        0        0    11231 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/base_data_utils.py
+-rw-r--r--   0        0        0     1821 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/config.py
+-rw-r--r--   0        0        0     2537 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/early_stopping.py
+-rw-r--r--   0        0        0     1903 2023-04-19 17:08:00.596532 volume_segmantics-0.3.2/volume_segmantics/utilities/pytorch3dunet_utils.py
+-rw-r--r--   0        0        0     9467 1970-01-01 00:00:00.000000 volume_segmantics-0.3.2/PKG-INFO
```

### Comparing `volume_segmantics-0.3.1/LICENSE.md` & `volume_segmantics-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/README.md` & `volume_segmantics-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## Development is moving
+
+Development of this package is moving to the Rosalind Franklin Institute. A fork is now available at https://github.com/rosalindfranklininstitute/volume-segmantics
+
 # Volume Segmantics
 
 A toolkit for semantic segmentation of volumetric data using PyTorch deep learning models.
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04691/status.svg)](https://doi.org/10.21105/joss.04691) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/tests.yml/badge.svg) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/release.yml/badge.svg)
 
 Volume Segmantics provides a simple command-line interface and API that allows researchers to quickly train a variety of 2D PyTorch segmentation models (e.g.  U-Net, U-Net++, FPN, DeepLabV3+) on their 3D datasets. These models use pre-trained encoders, enabling fast training on small datasets. Subsequently, the library enables using these trained models to segment larger 3D datasets, automatically merging predictions made in orthogonal planes and rotations to reduce artifacts that may result from predicting 3D segmentation using a 2D network.  
@@ -18,15 +22,15 @@
 
 The easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. 
 
 ## Configuration and command line use
 
 After installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.
 
-These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.1/volseg-settings.zip). 
+These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.2/volseg-settings.zip). 
 
 The file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. 
 
 ### For training a 2d model on a 3d image volume and corresponding labels
 Run the following command. Input files can be in HDF5 or multi-page TIFF format.
 
 ```shell
```

### Comparing `volume_segmantics-0.3.1/pyproject.toml` & `volume_segmantics-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volume-segmantics"
-version = "0.3.1"
+version = "0.3.2"
 description = "A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models"
 authors = ["Oliver King <olly.king@diamond.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DiamondLightSource/volume-segmantics"
 keywords = ["segmentation", "deep-learning", "volumetric", "3d"]
 classifiers = [
@@ -16,15 +16,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 albumentations = "^1.1.0"
 h5py = "^3.0.0"
 numpy = "^1.18.0"
 matplotlib = "^3.3.0"
-torch = "^1.7.1"
+torch = ">=1.7.1"
 segmentation-models-pytorch = "^0.2.1"
 termplotlib = "^0.3.6"
 imagecodecs = "*"
 
 [tool.poetry.dev-dependencies]
 black = ">=22.1.0"
 pdoc = ">=10"
```

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/augmentations.py` & `volume_segmantics-0.3.2/volume_segmantics/data/augmentations.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/base_data_manager.py` & `volume_segmantics-0.3.2/volume_segmantics/data/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/dataloaders.py` & `volume_segmantics-0.3.2/volume_segmantics/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/datasets.py` & `volume_segmantics-0.3.2/volume_segmantics/data/datasets.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/pytorch3dunet_losses.py` & `volume_segmantics-0.3.2/volume_segmantics/data/pytorch3dunet_losses.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/pytorch3dunet_metrics.py` & `volume_segmantics-0.3.2/volume_segmantics/data/pytorch3dunet_metrics.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/settings_data.py` & `volume_segmantics-0.3.2/volume_segmantics/data/settings_data.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/data/slicers.py` & `volume_segmantics-0.3.2/volume_segmantics/data/slicers.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/model/model_2d.py` & `volume_segmantics-0.3.2/volume_segmantics/model/model_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,18 @@
         model = smp.DeepLabV3Plus(**struct_dict_copy)
         logging.info(f"Sending the DeepLabV3+ model to device {device_num}")
     elif model_type == utils.ModelType.MA_NET:
         model = smp.MAnet(**struct_dict_copy)
         logging.info(f"Sending the MA-Net model to device {device_num}")
     elif model_type == utils.ModelType.LINKNET:
         model = smp.Linknet(**struct_dict_copy)
+        logging.info(f"Sending the Linknet model to device {device_num}")
     elif model_type == utils.ModelType.PAN:
         model = smp.PAN(**struct_dict_copy)
-        logging.info(f"Sending the Linknet model to device {device_num}")
+        logging.info(f"Sending the PAN model to device {device_num}")
     return model.to(device_num)
 
 
 def create_model_from_file(
     weights_fn: Path, gpu: bool = True, device_num: int = 0,
 ) -> Tuple[torch.nn.Module, int, dict]:
     """Creates and returns a model and the number of segmentation labels
```

### Comparing `volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_2d_predictor.py` & `volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_2d_predictor.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_2d_trainer.py` & `volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_2d_trainer.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/model/operations/vol_seg_prediction_manager.py` & `volume_segmantics-0.3.2/volume_segmantics/model/operations/vol_seg_prediction_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/scripts/predict_2d_model.py` & `volume_segmantics-0.3.2/volume_segmantics/scripts/predict_2d_model.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/scripts/train_2d_model.py` & `volume_segmantics-0.3.2/volume_segmantics/scripts/train_2d_model.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/utilities/arg_parsing.py` & `volume_segmantics-0.3.2/volume_segmantics/utilities/arg_parsing.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/utilities/base_data_utils.py` & `volume_segmantics-0.3.2/volume_segmantics/utilities/base_data_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/utilities/config.py` & `volume_segmantics-0.3.2/volume_segmantics/utilities/config.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/utilities/early_stopping.py` & `volume_segmantics-0.3.2/volume_segmantics/utilities/early_stopping.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/volume_segmantics/utilities/pytorch3dunet_utils.py` & `volume_segmantics-0.3.2/volume_segmantics/utilities/pytorch3dunet_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics-0.3.1/setup.py` & `volume_segmantics-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,151 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volume-segmantics
+Version: 0.3.2
+Summary: A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models
+Home-page: https://github.com/DiamondLightSource/volume-segmantics
+License: Apache-2.0
+Keywords: segmentation,deep-learning,volumetric,3d
+Author: Oliver King
+Author-email: olly.king@diamond.ac.uk
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Dist: albumentations (>=1.1.0,<2.0.0)
+Requires-Dist: h5py (>=3.0.0,<4.0.0)
+Requires-Dist: imagecodecs
+Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
+Requires-Dist: numpy (>=1.18.0,<2.0.0)
+Requires-Dist: segmentation-models-pytorch (>=0.2.1,<0.3.0)
+Requires-Dist: termplotlib (>=0.3.6,<0.4.0)
+Requires-Dist: torch (>=1.7.1)
+Project-URL: Repository, https://github.com/DiamondLightSource/volume-segmantics
+Description-Content-Type: text/markdown
 
-packages = \
-['volume_segmantics',
- 'volume_segmantics.data',
- 'volume_segmantics.model',
- 'volume_segmantics.model.operations',
- 'volume_segmantics.scripts',
- 'volume_segmantics.utilities']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['albumentations>=1.1.0,<2.0.0',
- 'h5py>=3.0.0,<4.0.0',
- 'imagecodecs',
- 'matplotlib>=3.3.0,<4.0.0',
- 'numpy>=1.18.0,<2.0.0',
- 'segmentation-models-pytorch>=0.2.1,<0.3.0',
- 'termplotlib>=0.3.6,<0.4.0',
- 'torch>=1.7.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['model-predict-2d = '
-                     'volume_segmantics.scripts.predict_2d_model:main',
-                     'model-train-2d = '
-                     'volume_segmantics.scripts.train_2d_model:main']}
-
-setup_kwargs = {
-    'name': 'volume-segmantics',
-    'version': '0.3.1',
-    'description': 'A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models',
-    'long_description': '# Volume Segmantics\n\nA toolkit for semantic segmentation of volumetric data using PyTorch deep learning models.\n\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04691/status.svg)](https://doi.org/10.21105/joss.04691) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/tests.yml/badge.svg) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/release.yml/badge.svg)\n\nVolume Segmantics provides a simple command-line interface and API that allows researchers to quickly train a variety of 2D PyTorch segmentation models (e.g.  U-Net, U-Net++, FPN, DeepLabV3+) on their 3D datasets. These models use pre-trained encoders, enabling fast training on small datasets. Subsequently, the library enables using these trained models to segment larger 3D datasets, automatically merging predictions made in orthogonal planes and rotations to reduce artifacts that may result from predicting 3D segmentation using a 2D network.  \n\nGiven a 3d image volume and corresponding dense labels (the segmentation), a 2d model is trained on image slices taken along the x, y, and z axes. The method is optimised for small training datasets, e.g a single dataset in between $128^3$ and $512^3$ pixels. To achieve this, all models use pre-trained encoders and image augmentations are used to expand the size of the training dataset.\n\nThis work utilises the abilities afforded by the excellent [segmentation-models-pytorch](https://github.com/qubvel/segmentation_models.pytorch) library in combination with augmentations made available via [Albumentations](https://albumentations.ai/). Also the metrics and loss functions used make use of the hard work done by Adrian Wolny in his [pytorch-3dunet](https://github.com/wolny/pytorch-3dunet) repository. \n\n## Requirements\n\nA machine capable of running CUDA enabled PyTorch version 1.7.1 or greater is required. This generally means a reasonably modern NVIDIA GPU. The exact requirements differ according to operating system. For example on Windows you will need Visual Studio Build Tools as well as CUDA Toolkit installed see [the CUDA docs](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) for more details. \n\n## Installation\n\nThe easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. \n\n## Configuration and command line use\n\nAfter installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.\n\nThese commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.1/volseg-settings.zip). \n\nThe file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. \n\n### For training a 2d model on a 3d image volume and corresponding labels\nRun the following command. Input files can be in HDF5 or multi-page TIFF format.\n\n```shell\nmodel-train-2d --data path/to/image/data.h5 --labels path/to/corresponding/segmentation/labels.h5\n```\n\nPaths to multiple data and label volumes can be added after the `--data` and `--labels` flags respectively. A model will be trained according to the settings defined in `/volseg-settings/2d_model_train_settings.yaml` and saved to your working directory. In addition, a figure showing "ground truth" segmentation vs model segmentation for some images in the validation set will be saved. \n\n### For 3d volume segmentation prediction using a 2d model\nRun the following command. Input image files can be in HDF5 or multi-page TIFF format.\n\n```shell\nmodel-predict-2d path/to/model_file.pytorch path/to/data_for_prediction.h5\n```\n\nThe input data will be segmented using the input model following the settings specified in `volseg-settings/2d_model_predict_settings.yaml`. An HDF5 file containing the segmented volume will be saved to your working directory.\n\n### Tutorial using example data\n\nA tutorial is available [here](training_data/README.md) that provides a walk-through of how to segment blood vessels from synchrotron X-ray micro-CT data collected on a sample of human placental tissue.\n\n## Currently supported model architectures and encoders\n\nThe model architectures which are currently available and tested are: \n- U-Net\n- U-Net++\n- FPN\n- DeepLabV3\n- DeepLabV3+\n- MA-Net\n- LinkNet\n- PAN\n\nThe pre-trained encoders that can be used with these architectures are: \n- ResNet-34\n- ResNet50\n- ResNeXt-50_32x4d\n- Efficientnet-b3\n- Efficientnet-b4\n- Resnest50d\\*\n- Resnest101e\\*\n\n\\* Encoders with asterisk not compatible with PAN.\n\n## Using the API\n\nYou can use the functionality of the package in your own program via the API, this is [documented here](https://diamondlightsource.github.io/volume-segmantics/). This interface is the one used by [SuRVoS2](https://github.com/DiamondLightSource/SuRVoS2), a client/server GUI application that allows fast annotation and segmentation of volumetric data. \n\n## Contributing\n\nWe welcome contributions from the community. Please take a look at out [contribution guidelines](https://github.com/DiamondLightSource/volume-segmantics/blob/main/CONTRIBUTING.md) for more information.\n\n## Citation\n\nIf you use this package for you research, please cite:\n\n[King O.N.F, Bellos, D. and Basham, M. (2022). Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models. Journal of Open Source Software, 7(78), 4691. doi: 10.21105/joss.04691](https://doi.org/10.21105/joss.04691)\n\n```bibtex\n@article{King2022,\n    doi = {10.21105/joss.04691},\n    url = {https://doi.org/10.21105/joss.04691},\n    year = {2022},\n    publisher = {The Open Journal},\n    volume = {7},\n    number = {78},\n    pages = {4691},\n    author = {Oliver N. F. King and Dimitrios Bellos and Mark Basham},\n    title = {Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models},\n    journal = {Journal of Open Source Software} }\n```\n\n## References\n\n**Albumentations**\n\nBuslaev, A., Iglovikov, V.I., Khvedchenya, E., Parinov, A., Druzhinin, M., and Kalinin, A.A. (2020). Albumentations: Fast and Flexible Image Augmentations. Information 11. [https://doi.org/10.3390/info11020125](https://doi.org/10.3390/info11020125)\n\n**Segmentation Models PyTorch**\n\nYakubovskiy, P. (2020). Segmentation Models Pytorch. [GitHub](https://github.com/qubvel/segmentation_models.pytorch)\n\n**PyTorch-3dUnet**\n\nWolny, A., Cerrone, L., Vijayan, A., Tofanelli, R., Barro, A.V., Louveaux, M., Wenzl, C., Strauss, S., Wilson-Sánchez, D., Lymbouridou, R., et al. (2020). Accurate and versatile 3D segmentation of plant tissues at cellular resolution. ELife 9, e57613. [https://doi.org/10.7554/eLife.57613](https://doi.org/10.7554/eLife.57613)\n',
-    'author': 'Oliver King',
-    'author_email': 'olly.king@diamond.ac.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DiamondLightSource/volume-segmantics',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Development is moving
 
+Development of this package is moving to the Rosalind Franklin Institute. A fork is now available at https://github.com/rosalindfranklininstitute/volume-segmantics
+
+# Volume Segmantics
+
+A toolkit for semantic segmentation of volumetric data using PyTorch deep learning models.
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04691/status.svg)](https://doi.org/10.21105/joss.04691) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/tests.yml/badge.svg) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/release.yml/badge.svg)
+
+Volume Segmantics provides a simple command-line interface and API that allows researchers to quickly train a variety of 2D PyTorch segmentation models (e.g.  U-Net, U-Net++, FPN, DeepLabV3+) on their 3D datasets. These models use pre-trained encoders, enabling fast training on small datasets. Subsequently, the library enables using these trained models to segment larger 3D datasets, automatically merging predictions made in orthogonal planes and rotations to reduce artifacts that may result from predicting 3D segmentation using a 2D network.  
+
+Given a 3d image volume and corresponding dense labels (the segmentation), a 2d model is trained on image slices taken along the x, y, and z axes. The method is optimised for small training datasets, e.g a single dataset in between $128^3$ and $512^3$ pixels. To achieve this, all models use pre-trained encoders and image augmentations are used to expand the size of the training dataset.
+
+This work utilises the abilities afforded by the excellent [segmentation-models-pytorch](https://github.com/qubvel/segmentation_models.pytorch) library in combination with augmentations made available via [Albumentations](https://albumentations.ai/). Also the metrics and loss functions used make use of the hard work done by Adrian Wolny in his [pytorch-3dunet](https://github.com/wolny/pytorch-3dunet) repository. 
+
+## Requirements
+
+A machine capable of running CUDA enabled PyTorch version 1.7.1 or greater is required. This generally means a reasonably modern NVIDIA GPU. The exact requirements differ according to operating system. For example on Windows you will need Visual Studio Build Tools as well as CUDA Toolkit installed see [the CUDA docs](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) for more details. 
+
+## Installation
+
+The easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. 
+
+## Configuration and command line use
+
+After installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.
+
+These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.2/volseg-settings.zip). 
+
+The file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. 
+
+### For training a 2d model on a 3d image volume and corresponding labels
+Run the following command. Input files can be in HDF5 or multi-page TIFF format.
+
+```shell
+model-train-2d --data path/to/image/data.h5 --labels path/to/corresponding/segmentation/labels.h5
+```
+
+Paths to multiple data and label volumes can be added after the `--data` and `--labels` flags respectively. A model will be trained according to the settings defined in `/volseg-settings/2d_model_train_settings.yaml` and saved to your working directory. In addition, a figure showing "ground truth" segmentation vs model segmentation for some images in the validation set will be saved. 
+
+### For 3d volume segmentation prediction using a 2d model
+Run the following command. Input image files can be in HDF5 or multi-page TIFF format.
+
+```shell
+model-predict-2d path/to/model_file.pytorch path/to/data_for_prediction.h5
+```
+
+The input data will be segmented using the input model following the settings specified in `volseg-settings/2d_model_predict_settings.yaml`. An HDF5 file containing the segmented volume will be saved to your working directory.
+
+### Tutorial using example data
+
+A tutorial is available [here](training_data/README.md) that provides a walk-through of how to segment blood vessels from synchrotron X-ray micro-CT data collected on a sample of human placental tissue.
+
+## Currently supported model architectures and encoders
+
+The model architectures which are currently available and tested are: 
+- U-Net
+- U-Net++
+- FPN
+- DeepLabV3
+- DeepLabV3+
+- MA-Net
+- LinkNet
+- PAN
+
+The pre-trained encoders that can be used with these architectures are: 
+- ResNet-34
+- ResNet50
+- ResNeXt-50_32x4d
+- Efficientnet-b3
+- Efficientnet-b4
+- Resnest50d\*
+- Resnest101e\*
+
+\* Encoders with asterisk not compatible with PAN.
+
+## Using the API
+
+You can use the functionality of the package in your own program via the API, this is [documented here](https://diamondlightsource.github.io/volume-segmantics/). This interface is the one used by [SuRVoS2](https://github.com/DiamondLightSource/SuRVoS2), a client/server GUI application that allows fast annotation and segmentation of volumetric data. 
+
+## Contributing
+
+We welcome contributions from the community. Please take a look at out [contribution guidelines](https://github.com/DiamondLightSource/volume-segmantics/blob/main/CONTRIBUTING.md) for more information.
+
+## Citation
+
+If you use this package for you research, please cite:
+
+[King O.N.F, Bellos, D. and Basham, M. (2022). Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models. Journal of Open Source Software, 7(78), 4691. doi: 10.21105/joss.04691](https://doi.org/10.21105/joss.04691)
+
+```bibtex
+@article{King2022,
+    doi = {10.21105/joss.04691},
+    url = {https://doi.org/10.21105/joss.04691},
+    year = {2022},
+    publisher = {The Open Journal},
+    volume = {7},
+    number = {78},
+    pages = {4691},
+    author = {Oliver N. F. King and Dimitrios Bellos and Mark Basham},
+    title = {Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models},
+    journal = {Journal of Open Source Software} }
+```
+
+## References
+
+**Albumentations**
+
+Buslaev, A., Iglovikov, V.I., Khvedchenya, E., Parinov, A., Druzhinin, M., and Kalinin, A.A. (2020). Albumentations: Fast and Flexible Image Augmentations. Information 11. [https://doi.org/10.3390/info11020125](https://doi.org/10.3390/info11020125)
+
+**Segmentation Models PyTorch**
+
+Yakubovskiy, P. (2020). Segmentation Models Pytorch. [GitHub](https://github.com/qubvel/segmentation_models.pytorch)
+
+**PyTorch-3dUnet**
+
+Wolny, A., Cerrone, L., Vijayan, A., Tofanelli, R., Barro, A.V., Louveaux, M., Wenzl, C., Strauss, S., Wilson-Sánchez, D., Lymbouridou, R., et al. (2020). Accurate and versatile 3D segmentation of plant tissues at cellular resolution. ELife 9, e57613. [https://doi.org/10.7554/eLife.57613](https://doi.org/10.7554/eLife.57613)
 
-setup(**setup_kwargs)
```

