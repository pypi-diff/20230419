# Comparing `tmp/hive-maia-1.0.tar.gz` & `tmp/hive-maia-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-maia-1.0.tar", last modified: Wed Nov  2 19:18:24 2022, max compression
+gzip compressed data, was "hive-maia-1.1.1.tar", last modified: Wed Apr 19 13:57:16 2023, max compression
```

## Comparing `hive-maia-1.0.tar` & `hive-maia-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.614680 hive-maia-1.0/
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.503561 hive-maia-1.0/Hive/
--rw-rw-rw-   0        0        0      554 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.514771 hive-maia-1.0/Hive/configs/
--rw-rw-rw-   0        0        0      272 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
--rw-rw-rw-   0        0        0      272 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
--rw-rw-rw-   0        0        0        0 2022-11-02 18:37:39.000000 hive-maia-1.0/Hive/configs/__init__.py
--rw-rw-rw-   0        0        0     1043 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/configs/nnDet_config_template.json
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.533123 hive-maia-1.0/Hive/utils/
--rw-rw-rw-   0        0        0        0 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/utils/__init__.py
--rw-rw-rw-   0        0        0    15320 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/utils/file_utils.py
--rw-rw-rw-   0        0        0     1978 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/utils/log_utils.py
--rw-rw-rw-   0        0        0     1514 2022-11-02 18:37:39.000000 hive-maia-1.0/Hive/utils/seg_mask_utils.py
--rw-rw-rw-   0        0        0     8908 2022-11-01 19:38:11.000000 hive-maia-1.0/Hive/utils/volume_utils.py
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.556431 hive-maia-1.0/Hive_MAIA.egg-info/
--rw-rw-rw-   0        0        0     1648 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1366 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      162 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-02 19:18:24.000000 hive-maia-1.0/Hive_MAIA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2022-11-01 19:38:11.000000 hive-maia-1.0/LICENSE
--rw-rw-rw-   0        0        0     1648 2022-11-02 19:18:24.612682 hive-maia-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      914 2022-11-01 19:38:11.000000 hive-maia-1.0/README.md
--rw-rw-rw-   0        0        0      330 2022-11-01 19:38:20.000000 hive-maia-1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-11-02 19:18:24.608618 hive-maia-1.0/scripts/
--rw-rw-rw-   0        0        0     2911 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
--rw-rw-rw-   0        0        0     2962 2022-11-02 18:37:39.000000 hive-maia-1.0/scripts/Hive_convert_semantic_to_instance_segmentation.py
--rw-rw-rw-   0        0        0     3052 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/Hive_create_subset.py
--rw-rw-rw-   0        0        0     1413 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/Hive_run_pipeline_from_file.py
--rw-rw-rw-   0        0        0        0 2022-11-02 18:37:39.000000 hive-maia-1.0/scripts/__init__.py
--rw-rw-rw-   0        0        0     5011 2022-11-02 18:37:39.000000 hive-maia-1.0/scripts/nndet_create_pipeline.py
--rw-rw-rw-   0        0        0     8268 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/nndet_prepare_data_folder.py
--rw-rw-rw-   0        0        0     2744 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/nndet_run_preprocessing.py
--rw-rw-rw-   0        0        0     2932 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/nndet_run_training.py
--rw-rw-rw-   0        0        0     3870 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/nnunet_run_prediction.py
--rw-rw-rw-   0        0        0     1139 2022-11-01 19:38:11.000000 hive-maia-1.0/scripts/script_template.py
--rw-rw-rw-   0        0        0       42 2022-11-02 19:18:24.614680 hive-maia-1.0/setup.cfg
--rw-rw-rw-   0        0        0     2435 2022-11-02 19:18:10.000000 hive-maia-1.0/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.680844 hive-maia-1.1.1/Hive/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/__init__.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/configs/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/ATM_nnUNet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/configs/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/nnDet_config_template.json
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/evaluation/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 12:06:26.000000 hive-maia-1.1.1/Hive/evaluation/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/abstract.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/evaluation/detection/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 12:49:04.000000 hive-maia-1.1.1/Hive/evaluation/detection/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/coco.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/froc.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/hist.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/matching.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/utils/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    23403 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/utils/file_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/log_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/seg_mask_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/utils/volume_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive_scripts/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_create_subset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.1/Hive_scripts/Hive_extract_experiment_predictions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_order_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1413 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_run_pipeline_from_file.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 13:05:53.000000 hive-maia-1.1.1/Hive_scripts/nndet_compute_metric_results.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     5238 2023-04-19 13:52:16.000000 hive-maia-1.1.1/Hive_scripts/nndet_create_pipeline.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_prediction.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/script_template.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/upload_DICOM_to_Orthanc.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.1/LICENSE
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1647 2023-04-19 13:57:16.688844 hive-maia-1.1.1/PKG-INFO
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 13:38:38.000000 hive-maia-1.1.1/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)        5 2023-04-19 13:56:27.000000 hive-maia-1.1.1/VERSION
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/hive_maia.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1647 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/top_level.txt
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.1/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 13:12:49.000000 hive-maia-1.1.1/requirements.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-19 13:57:16.688844 hive-maia-1.1.1/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 13:53:59.000000 hive-maia-1.1.1/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 13:12:19.000000 hive-maia-1.1.1/tests/test_file_utils.py
```

### Comparing `hive-maia-1.0/Hive/__init__.py` & `hive-maia-1.1.1/Hive/__init__.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/Hive/configs/nnDet_config_template.json` & `hive-maia-1.1.1/Hive/configs/nnDet_config_template.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/Hive/utils/log_utils.py` & `hive-maia-1.1.1/Hive/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/Hive/utils/seg_mask_utils.py` & `hive-maia-1.1.1/Hive/utils/seg_mask_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 import nibabel as nib
 from scipy.ndimage import label
 
 
 def semantic_segmentation_to_instance(mask_filename: str, output_path: str) -> int:
     """
-    Given a semantic segmentation mask convert to instance segmentation and save in the given output path.
-    Return the number of labels in instance segmentation mask.
+        Given a semantic segmentation mask convert to instance segmentation and save in the given output path.
+        Return the number of labels in instance segmentation mask.
 
-    Parameters
-    ----------
-    mask_filename: str
-        File path of semantic segmentation mask.
-    output_path: str
-        Output path including new instance segmentation mask file name.
-
-    Returns
-    -------
-    int:
-        Number of labels in converted instance segmentation mask.
-    """
+        Parameters
+        ----------
+        mask_filename:
+            File path of semantic segmentation mask.
+        output_path:
+            Output path including new instance segmentation mask file name.
+
+        Returns
+        -------
+            Number of labels in converted instance segmentation mask.
+        """
 
     # load segmentation mask and properties
     mask = nib.load(mask_filename)
     affine = mask.affine
     np_mask = mask.get_fdata()
 
     # label connected regions in segmentation mask
     labeled_array, num_features = label(np_mask)
 
     thresh = 10
     # voxel count in each region from https://neurostars.org/t/roi-voxel-count-using-python/6451
     # ignore regions below threshold = 10
-
-    for i in range(1, labeled_array.max()+1):
-        # in case of healthy patient skip
-        if num_features == 0:
-            continue
+    for i in range(1, num_features + 1):
         vox_count = (labeled_array == i).sum()
         if vox_count < thresh:
             labeled_array[labeled_array == i] = 0
-        # print('{} for region {}'.format(vox_count, i))
+
+    labeled_array[labeled_array>0] = 1
+    labeled_array, num_features = label(labeled_array)
 
     # convert labeled array into Nifti file
     labeled_mask = nib.Nifti1Image(labeled_array, affine=affine)
     nib.save(labeled_mask, output_path)
     return num_features
```

### Comparing `hive-maia-1.0/Hive/utils/volume_utils.py` & `hive-maia-1.1.1/Hive/utils/volume_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import math
 import shutil
 import tempfile
 import time
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
+import re
 import SimpleITK as sitk
 import dicom2nifti
+import math
+import nilearn.image
 import nibabel as nib
 import numpy as np
 import pydicom
 from pydicom import dcmread
 
 from Hive.utils.file_utils import subfolders
 from Hive.utils.log_utils import get_logger
@@ -21,38 +23,60 @@
 
 def dcm2nii_CT(CT_dcm_path: Union[str, PathLike], nii_out_path: Union[str, PathLike]):
     """
     Conversion of CT DICOM to nifti and save in nii_out_path.
 
     Parameters
     ----------
-    CT_dcm_path : Union[str, PathLike]
+    CT_dcm_path :
         CT DICOM folder path.
-    nii_out_path : Union[str, PathLike]
+    nii_out_path :
         Output NIFTI file path.
     """
 
+    #with tempfile.TemporaryDirectory() as tmp:
+    #    tmp = Path(str(tmp))
+    #    dicom2nifti.convert_directory(CT_dcm_path, str(tmp), compression=True, reorient=True)
+    #    nii = next(tmp.glob("*nii.gz"))
+    #    shutil.copy(nii, nii_out_path)
+    reader = sitk.ImageSeriesReader()
+
+    dicom_names = reader.GetGDCMSeriesFileNames(CT_dcm_path)
+    reader.SetFileNames(dicom_names)
+
+    image = reader.Execute()
+    sitk.WriteImage(image,nii_out_path)
+
+def dcm2nii_CT_from_server(orthanc, nii_out_path: Union[str, PathLike]):
+    """
+    Conversion of CT DICOM to nifti and save in nii_out_path.
+
+    Parameters
+    ----------
+    nii_out_path :
+        Output NIFTI file path.
+    """
     with tempfile.TemporaryDirectory() as tmp:
         tmp = Path(str(tmp))
-        dicom2nifti.convert_directory(CT_dcm_path, str(tmp), compression=True, reorient=True)
-        nii = next(tmp.glob("*nii.gz"))
-        shutil.copy(nii, nii_out_path)
+        print(tmp)
+        orthanc.download(tmp)
+        dcm2nii_CT(tmp, nii_out_path)
 
 
 def dcm2nii_mask(mask_dcm_path: Union[str, PathLike], nii_out_path: Union[str, PathLike], ref_nii_path: Union[str, PathLike]):
     """
     Converts a SEG DICOM volume into NIFTI format. Requires an existing NIFTI file to derive the corresponding affine transform.
 
     Parameters
     ----------
-    mask_dcm_path : Union[str, PathLike]
+    mask_dcm_path :
         SEG DICOM folder.
-    nii_out_path : Union[str, PathLike]
+    nii_out_path :
         NIFTI file saved as output.
-    ref_nii_path : Union[str, PathLike]
+    ref_nii_path :
         Reference NIFTI used to correctly saved the segmentation volume.
     """
     mask_dcm = list(mask_dcm_path.glob("*.dcm"))[0]
     mask = pydicom.read_file(str(mask_dcm))
     mask_array = mask.pixel_array
 
     mask_array = np.transpose(mask_array, (2, 1, 0))
@@ -64,106 +88,155 @@
     pet = nib.load(ref_nii_path)
     pet_affine = pet.affine
 
     # return mask as nifti object
     mask_out = nib.Nifti1Image(mask_array, pet_affine)
     nib.save(mask_out, nii_out_path)
 
+def convert_DICOM_server_folder_to_NIFTI_image(patient: str, patient_nifti_folder: Union[str, PathLike], orthanc):
+    orthanc.reset()
+    orthanc.select(PatientName=patient)
+
+    studies = orthanc.StudyDescription
+
+    for study_id, study in enumerate(studies):
+        Path(str(patient_nifti_folder) + "_{}".format(study_id)).mkdir(parents=True, exist_ok=True)
+        orthanc.reset()
+        orthanc.select(PatientName=patient,StudyDescription=study)
+        series = orthanc.SeriesDescription
+        for serie in series:
+            orthanc.reset()
+            orthanc.select(PatientName=patient, StudyDescription=study, SeriesDescription=serie)
+
+            if orthanc.Modality[0] == "CT":
+
+                ct_filename = str(
+                        Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_CT.nii.gz".format(patient, study_id)
+                        )
+                    )
+
+
+                dcm2nii_CT_from_server(orthanc, ct_filename)
+            elif orthanc.Modality[0] == "PT":
+
+                pet_filename = str(
+                        Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_PET.nii.gz".format(patient, study_id)
+                        )
+                    )
+
+                #normalize_PET_to_SUV_BW(str(Path(patient_dicom_folder).joinpath(study, serie)), pet_filename)
+
 
 def convert_DICOM_folder_to_NIFTI_image(patient_dicom_folder: Union[str, PathLike], patient_nifti_folder: Union[str, PathLike]):
     """
     Converts a given Patient DICOM folder into NIFTI format, saving the DICOM Studies in different folders.
 
     Parameters
     ----------
-    patient_dicom_folder : Union[str, PathLike]
+    patient_dicom_folder :
         DICOM folder containing a single patient Studies.
-    patient_nifti_folder : str
+    patient_nifti_folder :
         Output NIFTI folder used as stem to save the DICOM Studies. The Study index is appended to this path to create
         the corresponding NIFTI study folder path.
     """
     studies = subfolders(patient_dicom_folder, join=False)
-    single_study = False
-    if len(studies) == 1:
-        single_study = True
 
+    patient_study_map = {Path(patient_dicom_folder).name: {}}
     for study_id, study in enumerate(studies):
 
-        if not single_study:
-            Path(str(patient_nifti_folder) + "_{}".format(study_id)).mkdir(parents=True, exist_ok=True)
-        else:
-            Path(str(patient_nifti_folder)).mkdir(parents=True, exist_ok=True)
         series = subfolders(Path(patient_dicom_folder).joinpath(study), join=False)
         for serie in series:
             first_file = next(Path(patient_dicom_folder).joinpath(study, serie).glob("*.dcm"))
             ds = pydicom.dcmread(str(first_file))
 
+            patient_study_map[Path(patient_dicom_folder).name][study_id] = str(ds['StudyInstanceUID'].value)
+
+            Path(str(patient_nifti_folder)).joinpath(str(ds['PatientID'].value) + "_{}".format(study_id)).mkdir(parents=True, exist_ok=True)
+
             if ds.Modality == "CT":
-                if not single_study:
-                    ct_filename = str(
-                        Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
-                            "{}_{}_CT.nii.gz".format(Path(patient_dicom_folder).name, study_id)
+
+                ct_filename = str(
+                        Path(str(patient_nifti_folder)).joinpath( str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_CT.nii.gz".format(str(ds['PatientID'].value), study_id)
                         )
                     )
-                else:
-                    ct_filename = str(
-                        Path(str(patient_nifti_folder)).joinpath("{}_CT.nii.gz".format(Path(patient_dicom_folder).name))
-                    )
+
 
                 dcm2nii_CT(str(Path(patient_dicom_folder).joinpath(study, serie)), ct_filename)
             elif ds.Modality == "PT":
-                if not single_study:
-                    pet_filename = str(
-                        Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
-                            "{}_{}_PET.nii.gz".format(Path(patient_dicom_folder).name, study_id)
+
+                pet_filename = str(
+                        Path(str(patient_nifti_folder)).joinpath(str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_PET.nii.gz".format(str(ds['PatientID'].value), study_id)
                         )
                     )
-                else:
-                    pet_filename = str(
-                        Path(str(patient_nifti_folder)).joinpath("{}_PET.nii.gz".format(Path(patient_dicom_folder).name))
-                    )
-                normalize_PET_to_SUV_BW(str(Path(patient_dicom_folder).joinpath(study, serie)), pet_filename)
 
-        for study_id, study in enumerate(studies):
-            series = subfolders(Path(patient_dicom_folder).joinpath(study), join=False)
-            for serie in series:
-                first_file = next(Path(patient_dicom_folder).joinpath(study, serie).glob("*.dcm"))
-                ds = pydicom.dcmread(str(first_file))
-
-                if ds.Modality == "SEG":
-                    if not single_study:
-                        seg_filename = str(
-                            Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
-                                "{}_{}_SEG.nii.gz".format(Path(patient_dicom_folder).name, study_id)
-                            )
-                        )
-                        ref_filename = str(
-                            Path(str(patient_nifti_folder) + "_{}".format(study_id)).joinpath(
-                                "{}_{}_PET.nii.gz".format(Path(patient_dicom_folder).name, study_id)
-                            )
-                        )
-                    else:
-                        seg_filename = str(
-                            Path(str(patient_nifti_folder)).joinpath("{}_SEG.nii.gz".format(Path(patient_dicom_folder).name))
+                normalize_PET_to_SUV_BW(str(Path(patient_dicom_folder).joinpath(study, serie)), pet_filename)
+            elif ds.Modality == "MR":
+                groups =re.findall(r'.+dyn ([0-9]).{2} pass.+', serie)
+                if len(groups) > 0:
+                    mr_filename = str(
+                        Path(str(patient_nifti_folder)).joinpath( str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_{}.nii.gz".format(str(ds['PatientID'].value), study_id,groups[0])
+                        )
+                    )
+                    #if not Path(mr_filename).is_file():
+                    dcm2nii_CT(str(Path(patient_dicom_folder).joinpath(study, serie)), mr_filename)
+                groups =re.findall(r'.+Ph([0-9])ax 3d dyn.+', serie)
+                if len(groups) > 0:
+                    mr_filename = str(
+                        Path(str(patient_nifti_folder)).joinpath( str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_{}.nii.gz".format(str(ds['PatientID'].value), study_id,groups[0])
                         )
-                        ref_filename = str(
-                            Path(str(patient_nifti_folder)).joinpath("{}_PET.nii.gz".format(Path(patient_dicom_folder).name))
+                    )
+                    #if not Path(mr_filename).is_file():
+                    dcm2nii_CT(str(Path(patient_dicom_folder).joinpath(study, serie)), mr_filename)
+                groups = re.findall(r'.+Ph([0-9])ax dyn.+', serie)
+                if len(groups) > 0:
+                    mr_filename = str(
+                        Path(str(patient_nifti_folder)).joinpath(
+                            str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+                            "{}_{}_{}.nii.gz".format(str(ds['PatientID'].value), study_id, groups[0])
                         )
-                    dcm2nii_mask(Path(patient_dicom_folder).joinpath(study, serie), seg_filename, ref_filename)
+                    )
+                    #if not Path(mr_filename).is_file():
+                    dcm2nii_CT(str(Path(patient_dicom_folder).joinpath(study, serie)), mr_filename)
+    for study_id, study in enumerate(studies):
+        series = subfolders(Path(patient_dicom_folder).joinpath(study), join=False)
+        for serie in series:
+            first_file = next(Path(patient_dicom_folder).joinpath(study, serie).glob("*.dcm"))
+            ds = pydicom.dcmread(str(first_file))
+
+            #if ds.Modality == "SEG":
 
+            #    seg_filename = str(
+            #                Path(str(patient_nifti_folder)).joinpath(str(ds['PatientID'].value) + "_{}".format(study_id)).joinpath(
+            #                    "{}_{}_SEG.nii.gz".format(str(ds['PatientID'].value), study_id)
+            #                )
+            #            )
+            #    ref_filename = str(
+            #                Path(str(patient_nifti_folder)).joinpath(str(ds['PatientID'].value)+ "_{}".format(study_id)).joinpath(
+            #                    "{}_{}_PET.nii.gz".format(str(ds['PatientID'].value), study_id)
+            #                )
+            #            )
+
+            #    dcm2nii_mask(Path(patient_dicom_folder).joinpath(study, serie), seg_filename, ref_filename)
+    return patient_study_map
 
 def normalize_PET_to_SUV_BW(dicom_pet_series_folder: Union[str, PathLike], suv_pet_filename: Union[str, PathLike]):
     """
     SUV BW Normalization of DICOM PET volume. The resulting normalized PET volume is saved at **suv_pet_filename**.
 
     Parameters
     ----------
-    dicom_pet_series_folder : Union[str, PathLike]
+    dicom_pet_series_folder :
         DICOM PET Folder to be normalized.
-    suv_pet_filename: Union[str, PathLike]
+    suv_pet_filename:
         Normalized SUV PET file location.
     """
     reader = sitk.ImageSeriesReader()
     dicom_names = reader.GetGDCMSeriesFileNames(dicom_pet_series_folder)
 
     ds = dcmread(dicom_names[0])
 
@@ -219,7 +292,15 @@
     image_array *= total_factor
 
     itk_image = sitk.GetImageFromArray(image_array)
 
     itk_image.CopyInformation(image)
 
     sitk.WriteImage(itk_image, suv_pet_filename)
+
+
+def resample_image(nii_input_path, nii_ref_path, nii_out_path):
+    # resample CT to PET and mask resolution
+    input_image   = nib.load(nii_input_path)
+    reference_image  = nib.load(nii_ref_path)
+    resampled_image = nilearn.image.resample_to_img(input_image, reference_image, fill_value=-1024)
+    nib.save(resampled_image, nii_out_path)
```

### Comparing `hive-maia-1.0/Hive_MAIA.egg-info/PKG-INFO` & `hive-maia-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1
-Name: hive-maia
-Version: 1.0
-Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
-Home-page: https://github.com/MAIA-KTH/Hive.git
-Author: Simone Bendazzoli
-Author-email: simben@kth.se
-License: GPLv3
-Project-URL: Documentation, https://hive-maia.readthedocs.io
-Project-URL: Source, https://github.com/MAIA-KTH/Hive/issues
-Project-URL: Tracker, https://github.com/MAIA-KTH/Hive/issues
-Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hive
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/SimoneBendazzoli93/Hive/main/images/MAI_A_logo.png" width="50%" alt='Hive'>
-</p>
-
-[![Documentation Status](https://readthedocs.org/projects/hive-maia/badge/?version=latest)](https://hive-maia.readthedocs.io/en/latest/?badge=latest)
-![Version](https://img.shields.io/badge/Hive-v1.0-blue)
-[![License](https://img.shields.io/badge/license-GPL%203.0-green.svg)](https://opensource.org/licenses/GPL-3.0)
-![Python](https://img.shields.io/badge/python-3.8+-orange)
-![CUDA](https://img.shields.io/badge/CUDA-10.1%2F10.2%2F11.0-green)
-
-## What is Hive?
-
-Hive is a Python package to support Deep Learning data preparation, pre-processing. training, result visualization and
-model deployment across different frameworks ([nnUNet](https://github.com/MIC-DKFZ/nnUNet)
-, [nnDetection](https://github.com/MIC-DKFZ/nnDetection), [MONAI](https://monai.io/) ).
+Metadata-Version: 2.1
+Name: hive-maia
+Version: 1.1.1
+Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
+Home-page: https://github.com/MAIA-KTH/Hive.git
+Author: Simone Bendazzoli
+Author-email: simben@kth.se
+License: GPLv3
+Project-URL: Documentation, https://hive-maia.readthedocs.io
+Project-URL: Source, https://github.com/MAIA-KTH/Hive
+Project-URL: Tracker, https://github.com/MAIA-KTH/Hive/issues
+Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation,object detection
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hive
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/SimoneBendazzoli93/Hive/main/images/MAI_A_logo.png" width="50%" alt='Hive'>
+</p>
+
+[![Documentation Status](https://readthedocs.org/projects/hive-maia/badge/?version=latest)](https://hive-maia.readthedocs.io/en/latest/?badge=latest)
+![Version](https://img.shields.io/badge/Hive-v1.1-blue)
+[![License](https://img.shields.io/badge/license-GPL%203.0-green.svg)](https://opensource.org/licenses/GPL-3.0)
+![Python](https://img.shields.io/badge/python-3.8+-orange)
+![CUDA](https://img.shields.io/badge/CUDA-10.1%2F10.2%2F11.0-green)
+
+## What is Hive?
+
+Hive is a Python package to support Deep Learning data preparation, pre-processing. training, result visualization and
+model deployment across different frameworks ([nnUNet](https://github.com/MIC-DKFZ/nnUNet)
+, [nnDetection](https://github.com/MIC-DKFZ/nnDetection), [MONAI](https://monai.io/) ).
+
```

### Comparing `hive-maia-1.0/Hive_MAIA.egg-info/SOURCES.txt` & `hive-maia-1.1.1/hive_maia.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 LICENSE
 README.md
+VERSION
 pyproject.toml
+requirements.txt
 setup.py
 Hive/__init__.py
+Hive/configs/ATM_nnUNet_3D_fullres_config.json
+Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
+Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
 Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
 Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
 Hive/configs/__init__.py
 Hive/configs/nnDet_config_template.json
+Hive/evaluation/__init__.py
+Hive/evaluation/abstract.py
+Hive/evaluation/detection/__init__.py
+Hive/evaluation/detection/coco.py
+Hive/evaluation/detection/froc.py
+Hive/evaluation/detection/hist.py
+Hive/evaluation/detection/matching.py
 Hive/utils/__init__.py
 Hive/utils/file_utils.py
 Hive/utils/log_utils.py
 Hive/utils/seg_mask_utils.py
 Hive/utils/volume_utils.py
-Hive_MAIA.egg-info/PKG-INFO
-Hive_MAIA.egg-info/SOURCES.txt
-Hive_MAIA.egg-info/dependency_links.txt
-Hive_MAIA.egg-info/entry_points.txt
-Hive_MAIA.egg-info/requires.txt
-Hive_MAIA.egg-info/top_level.txt
-Hive_maia.egg-info/PKG-INFO
-Hive_maia.egg-info/SOURCES.txt
-Hive_maia.egg-info/dependency_links.txt
-Hive_maia.egg-info/entry_points.txt
-Hive_maia.egg-info/requires.txt
-Hive_maia.egg-info/top_level.txt
+Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
+Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
+Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
+Hive_scripts/Hive_create_subset.py
+Hive_scripts/Hive_extract_experiment_predictions.py
+Hive_scripts/Hive_order_data_folder.py
+Hive_scripts/Hive_run_pipeline_from_file.py
+Hive_scripts/__init__.py
+Hive_scripts/nndet_compute_metric_results.py
+Hive_scripts/nndet_create_pipeline.py
+Hive_scripts/nndet_prepare_data_folder.py
+Hive_scripts/nndet_run_preprocessing.py
+Hive_scripts/nndet_run_training.py
+Hive_scripts/nnunet_prepare_data_folder.py
+Hive_scripts/nnunet_run_prediction.py
+Hive_scripts/nnunet_run_preprocessing.py
+Hive_scripts/nnunet_run_training.py
+Hive_scripts/script_template.py
+Hive_scripts/upload_DICOM_to_Orthanc.py
 hive_maia.egg-info/PKG-INFO
 hive_maia.egg-info/SOURCES.txt
 hive_maia.egg-info/dependency_links.txt
 hive_maia.egg-info/entry_points.txt
 hive_maia.egg-info/requires.txt
 hive_maia.egg-info/top_level.txt
-scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
-scripts/Hive_convert_semantic_to_instance_segmentation.py
-scripts/Hive_create_subset.py
-scripts/Hive_run_pipeline_from_file.py
-scripts/__init__.py
-scripts/nndet_create_pipeline.py
-scripts/nndet_prepare_data_folder.py
-scripts/nndet_run_preprocessing.py
-scripts/nndet_run_training.py
-scripts/nnunet_run_prediction.py
-scripts/script_template.py
+tests/test_file_utils.py
```

### Comparing `hive-maia-1.0/LICENSE` & `hive-maia-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/PKG-INFO` & `hive-maia-1.1.1/hive_maia.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1
-Name: hive-maia
-Version: 1.0
-Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
-Home-page: https://github.com/MAIA-KTH/Hive.git
-Author: Simone Bendazzoli
-Author-email: simben@kth.se
-License: GPLv3
-Project-URL: Documentation, https://hive-maia.readthedocs.io
-Project-URL: Source, https://github.com/MAIA-KTH/Hive/issues
-Project-URL: Tracker, https://github.com/MAIA-KTH/Hive/issues
-Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hive
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/SimoneBendazzoli93/Hive/main/images/MAI_A_logo.png" width="50%" alt='Hive'>
-</p>
-
-[![Documentation Status](https://readthedocs.org/projects/hive-maia/badge/?version=latest)](https://hive-maia.readthedocs.io/en/latest/?badge=latest)
-![Version](https://img.shields.io/badge/Hive-v1.0-blue)
-[![License](https://img.shields.io/badge/license-GPL%203.0-green.svg)](https://opensource.org/licenses/GPL-3.0)
-![Python](https://img.shields.io/badge/python-3.8+-orange)
-![CUDA](https://img.shields.io/badge/CUDA-10.1%2F10.2%2F11.0-green)
-
-## What is Hive?
-
-Hive is a Python package to support Deep Learning data preparation, pre-processing. training, result visualization and
-model deployment across different frameworks ([nnUNet](https://github.com/MIC-DKFZ/nnUNet)
-, [nnDetection](https://github.com/MIC-DKFZ/nnDetection), [MONAI](https://monai.io/) ).
+Metadata-Version: 2.1
+Name: hive-maia
+Version: 1.1.1
+Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
+Home-page: https://github.com/MAIA-KTH/Hive.git
+Author: Simone Bendazzoli
+Author-email: simben@kth.se
+License: GPLv3
+Project-URL: Documentation, https://hive-maia.readthedocs.io
+Project-URL: Source, https://github.com/MAIA-KTH/Hive
+Project-URL: Tracker, https://github.com/MAIA-KTH/Hive/issues
+Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation,object detection
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hive
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/SimoneBendazzoli93/Hive/main/images/MAI_A_logo.png" width="50%" alt='Hive'>
+</p>
+
+[![Documentation Status](https://readthedocs.org/projects/hive-maia/badge/?version=latest)](https://hive-maia.readthedocs.io/en/latest/?badge=latest)
+![Version](https://img.shields.io/badge/Hive-v1.1-blue)
+[![License](https://img.shields.io/badge/license-GPL%203.0-green.svg)](https://opensource.org/licenses/GPL-3.0)
+![Python](https://img.shields.io/badge/python-3.8+-orange)
+![CUDA](https://img.shields.io/badge/CUDA-10.1%2F10.2%2F11.0-green)
+
+## What is Hive?
+
+Hive is a Python package to support Deep Learning data preparation, pre-processing. training, result visualization and
+model deployment across different frameworks ([nnUNet](https://github.com/MIC-DKFZ/nnUNet)
+, [nnDetection](https://github.com/MIC-DKFZ/nnDetection), [MONAI](https://monai.io/) ).
+
```

### Comparing `hive-maia-1.0/README.md` & `hive-maia-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Hive
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/SimoneBendazzoli93/Hive/main/images/MAI_A_logo.png" width="50%" alt='Hive'>
 </p>
 
 [![Documentation Status](https://readthedocs.org/projects/hive-maia/badge/?version=latest)](https://hive-maia.readthedocs.io/en/latest/?badge=latest)
-![Version](https://img.shields.io/badge/Hive-v1.0-blue)
+![Version](https://img.shields.io/badge/Hive-v1.1-blue)
 [![License](https://img.shields.io/badge/license-GPL%203.0-green.svg)](https://opensource.org/licenses/GPL-3.0)
 ![Python](https://img.shields.io/badge/python-3.8+-orange)
 ![CUDA](https://img.shields.io/badge/CUDA-10.1%2F10.2%2F11.0-green)
 
 ## What is Hive?
 
 Hive is a Python package to support Deep Learning data preparation, pre-processing. training, result visualization and
```

### Comparing `hive-maia-1.0/scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py` & `hive-maia-1.1.1/Hive_scripts/nndet_run_preprocessing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 #!/usr/bin/env python
 
-import datetime
+import json
 import os
 from argparse import ArgumentParser, RawTextHelpFormatter
-from multiprocessing import Pool
 from pathlib import Path
 from textwrap import dedent
 
-from tqdm import tqdm
-
-from Hive.utils.file_utils import subfolders
-from Hive.utils.log_utils import add_verbosity_options_to_argparser, get_logger, log_lvl_from_verbosity_args
-from Hive.utils.volume_utils import convert_DICOM_folder_to_NIFTI_image
-
-TIMESTAMP = "{:%Y-%m-%d_%H-%M-%S}".format(datetime.datetime.now())
+from Hive.utils.log_utils import (
+    get_logger,
+    add_verbosity_options_to_argparser,
+    log_lvl_from_verbosity_args,
+)
 
 DESC = dedent(
     """
-    Script to convert a ``DICOM`` dataset (structured as Patient-Study-Series) into a NIFTI format (with the `Patient ID` as the folder name).
-    When multiple studies for the same patient are found, different **DICOM studies** are saved in different folders, appending the study index to the patient name.
-    *DICOM series* for the same study are saved in the same patient folder.
+    Run nnDetection pre-processing, data analysis, and image data unpacking.
+    The CL scripts called are  ``nndet_prep`` and ``nndet_unpack``, with the arguments extracted from the given configuration file.
     """  # noqa: E501
 )
 EPILOG = dedent(
     """
     Example call:
     ::
-        {filename}  --data-folder /PATH/TO/DICOM_DATA --output-folder /PATH/TO/NIFTI_DATASET
+        {filename} --config-file /PATH/TO/CONFIG_FILE.json
     """.format(  # noqa: E501
         filename=Path(__file__).stem
     )
 )
 
-if "N_THREADS" not in os.environ:
-    os.environ["N_THREADS"] = "1"
-
 
 def get_arg_parser():
     pars = ArgumentParser(description=DESC, epilog=EPILOG, formatter_class=RawTextHelpFormatter)
 
     pars.add_argument(
-        "--data-folder",
+        "--config-file",
         type=str,
         required=True,
-        help="DICOM Dataset folder.",
-    )
-
-    pars.add_argument(
-        "--output-folder",
-        type=str,
-        required=True,
-        help="Output folder where to save the converted NIFTI dataset.",
+        help="File path for the configuration dictionary, used to retrieve experiment variables (**Task_ID**, **results_folder**, ...) ",
+        # noqa: E501
     )
 
     pars.add_argument(
         "--n-workers",
-        type=int,
-        required=False,
-        default=os.environ["N_THREADS"],
-        help="Number of worker threads to use. (Default: {})".format(os.environ["N_THREADS"]),
+        type=str,
+        default=None,
+        help="Number of parallel processes used when pre-processing and unpacking the image data (Default: ``N_THREADS``)",
     )
 
     add_verbosity_options_to_argparser(pars)
 
     return pars
 
 
 def main():
     parser = get_arg_parser()
-    arguments = vars(parser.parse_args())
+    arguments, unknown_arguments = parser.parse_known_args()
+    args = vars(arguments)
 
     logger = get_logger(  # NOQA: F841
         name=Path(__file__).name,
-        level=log_lvl_from_verbosity_args(arguments),
+        level=log_lvl_from_verbosity_args(args),
     )
-    subjects = subfolders(arguments["data_folder"], join=False)
+    config_file = args["config_file"]
 
-    pool = Pool(int(arguments["n_workers"]))
-    Path(arguments["output_folder"]).mkdir(parents=True, exist_ok=True)
-    DICOM_to_NIFTI_conversions = []
-    for subject in subjects:
-        subject_dicom_folder = str(Path(arguments["data_folder"]).joinpath(subject))
-        subject_nifti_filename = str(Path(arguments["output_folder"]).joinpath(subject))
-        DICOM_to_NIFTI_conversions.append(
-            pool.starmap_async(
-                convert_DICOM_folder_to_NIFTI_image,
-                ((subject_dicom_folder, subject_nifti_filename),),
+    n_workers = "1"
+    if args["n_workers"] is None:
+        if "N_THREADS" in os.environ is not None:
+            n_workers = str(os.environ["N_THREADS"])
+    else:
+        n_workers = str(args["n_workers"])
+
+    with open(config_file) as json_file:
+        data = json.load(json_file)
+
+        arguments = [data["Task_ID"], "-np", n_workers, "-npp", n_workers]
+
+        os.environ["det_data"] = data["base_folder"]
+        os.environ["OMP_NUM_THREADS"] = "1"
+
+        os.environ["nnUNet_def_n_proc"] = n_workers
+        os.environ["det_models"] = data["results_folder"]
+        arguments.extend(unknown_arguments)
+        os.system("nndet_prep " + " ".join(arguments))
+        os.system(
+            "nndet_unpack {} {}".format(
+                str(
+                    Path(os.environ["det_data"]).joinpath(
+                        "Task{}_{}".format(data["Task_ID"], data["Task_Name"]), "preprocessed", "D3V001_3d", "imagesTr"
+                    )
+                ),
+                n_workers,
             )
         )
 
-    _ = [i.get() for i in tqdm(DICOM_to_NIFTI_conversions)]
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.0/scripts/Hive_convert_semantic_to_instance_segmentation.py` & `hive-maia-1.1.1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 
 import datetime
-import os
 import json
+import os
 from argparse import ArgumentParser, RawTextHelpFormatter
 from pathlib import Path
 from textwrap import dedent
 
-from Hive.utils.log_utils import add_verbosity_options_to_argparser
 from Hive.utils.file_utils import subfolders
+from Hive.utils.log_utils import add_verbosity_options_to_argparser
 from Hive.utils.seg_mask_utils import semantic_segmentation_to_instance
 
 TIMESTAMP = "{:%Y-%m-%d_%H-%M-%S}".format(datetime.datetime.now())
 
 DESC = dedent(
     """
     Script to convert a semantic segmentation dataset (with the `Patient ID` as the folder name) into an instance segmentation dataset.
@@ -21,15 +21,15 @@
     separate json file ('inst_seg_labels.json') alongside its 'Patient ID'. 
     """  # noqa: E501
 )
 EPILOG = dedent(
     """
     Example call:
     ::
-        {filename}  --data-folder /PATH/TO/SEMANTIC_SEG_DATA
+        {filename}  --data-folder /PATH/TO/SEMANTIC_SEG_DATA --sem-seg-suffix _SEG.nii.gz --inst-seg-suffix _INST_SEG.nii.gz --output-json-path /PATH/TO/JSON/inst_seg_labels.json
     """.format(  # noqa: E501
         filename=Path(__file__).stem
     )
 )
 
 
 def get_arg_parser():
```

### Comparing `hive-maia-1.0/scripts/Hive_create_subset.py` & `hive-maia-1.1.1/Hive_scripts/Hive_create_subset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/scripts/Hive_run_pipeline_from_file.py` & `hive-maia-1.1.1/Hive_scripts/Hive_run_pipeline_from_file.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/scripts/nndet_create_pipeline.py` & `hive-maia-1.1.1/Hive_scripts/nndet_create_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
         arguments["input_data_folder"],
         "--task-ID",
         arguments["task_ID"],
         "--task-name",
         config_dict["DatasetName"] + "_" + config_dict["Experiment Name"],
         "--config-file",
         arguments["config_file"],
+        "--test-split",
+        arguments["test_split"]
     ]
 
     return args
 
 
 def run_preprocessing_step(config_file):
     args = [
@@ -158,15 +160,18 @@
     pipeline_steps = []
 
     pipeline_steps.append(run_data_and_folder_preparation_step(arguments))
     pipeline_steps.append(run_preprocessing_step(output_json_config_file))
 
     [pipeline_steps.append(step) for step in run_training_step(output_json_config_file, range(config_dict["n_folds"]))]
 
-    Path(os.environ["root_experiment_folder"]).joinpath(config_dict["Experiment Name"]).mkdir(exist_ok=True, parents=True)
+    pipeline_steps.append(run_training_step(output_json_config_file, "-1"))
+
+    Path(os.environ["root_experiment_folder"]).joinpath(config_dict["Experiment Name"]).mkdir(exist_ok=True,
+                                                                                              parents=True)
     pipeline_steps_summary = open(
         Path(os.environ["root_experiment_folder"]).joinpath(
             config_dict["Experiment Name"], "Task_" + arguments["task_ID"] + "_" + TIMESTAMP + ".txt"
         ),
         "w",
     )
     for step in pipeline_steps:
```

### Comparing `hive-maia-1.0/scripts/nndet_prepare_data_folder.py` & `hive-maia-1.1.1/Hive_scripts/nndet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/scripts/nndet_run_preprocessing.py` & `hive-maia-1.1.1/Hive_scripts/nnunet_run_preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,45 +10,38 @@
     get_logger,
     add_verbosity_options_to_argparser,
     log_lvl_from_verbosity_args,
 )
 
 DESC = dedent(
     """
-    Run nnDetection pre-processing, data analysis, and image data unpacking.
-    The CL scripts called are  ``nndet_prep`` and ``nndet_unpack``, with the arguments extracted from the given configuration file.
+    Run nnUNet command to create experiment plan, preprocessing and ( optionally ) verify the dataset integrity.
+
     """  # noqa: E501
 )
 EPILOG = dedent(
     """
     Example call:
     ::
-        {filename} --config-file /PATH/TO/CONFIG_FILE.json
+        {filename} --config-file ../LungLobeSeg_3d_fullres_100_LungLobeSeg_3D_Single_Modality.json
+        {filename} --config-file ../LungLobeSeg_3d_fullres_100_LungLobeSeg_3D_Single_Modality.json --verify_dataset_integrity
     """.format(  # noqa: E501
-        filename=Path(__file__).stem
+        filename=Path(__file__).name
     )
 )
 
 
 def get_arg_parser():
     pars = ArgumentParser(description=DESC, epilog=EPILOG, formatter_class=RawTextHelpFormatter)
 
     pars.add_argument(
         "--config-file",
         type=str,
         required=True,
-        help="File path for the configuration dictionary, used to retrieve experiment variables (**Task_ID**, **results_folder**, ...) ",
-        # noqa: E501
-    )
-
-    pars.add_argument(
-        "--n-workers",
-        type=str,
-        default=None,
-        help="Number of parallel processes used when pre-processing and unpacking the image data (Default: ``N_THREADS``)",
+        help="File path for the configuration dictionary, used to retrieve experiments variables (Task_ID) ",
     )
 
     add_verbosity_options_to_argparser(pars)
 
     return pars
 
 
@@ -59,40 +52,25 @@
 
     logger = get_logger(  # NOQA: F841
         name=Path(__file__).name,
         level=log_lvl_from_verbosity_args(args),
     )
     config_file = args["config_file"]
 
-    n_workers = "1"
-    if args["n_workers"] is None:
-        if "N_THREADS" in os.environ is not None:
-            n_workers = str(os.environ["N_THREADS"])
-    else:
-        n_workers = str(args["n_workers"])
-
     with open(config_file) as json_file:
         data = json.load(json_file)
 
-        arguments = [data["Task_ID"], "-np", n_workers, "-npp", n_workers]
-
-        os.environ["det_data"] = data["base_folder"]
-        os.environ["OMP_NUM_THREADS"] = "1"
-
-        os.environ["nnUNet_def_n_proc"] = n_workers
-        os.environ["det_models"] = data["results_folder"]
+        arguments = [
+            "-t",
+            data["Task_ID"],
+        ]
+
+        os.environ["nnUNet_raw_data_base"] = data["base_folder"]
+        os.environ["nnUNet_preprocessed"] = data["preprocessing_folder"]
+        os.environ["nnUNet_def_n_proc"] = os.environ["N_THREADS"]
+        os.environ["RESULTS_FOLDER"] = data["results_folder"]
         arguments.extend(unknown_arguments)
-        os.system("nndet_prep " + " ".join(arguments))
-        os.system(
-            "nndet_unpack {} {}".format(
-                str(
-                    Path(os.environ["det_data"]).joinpath(
-                        "Task{}_{}".format(data["Task_ID"], data["Task_Name"]), "preprocessed", "D3V001_3d", "imagesTr"
-                    )
-                ),
-                n_workers,
-            )
-        )
+        os.system("nnUNet_plan_and_preprocess " + " ".join(arguments))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.0/scripts/nndet_run_training.py` & `hive-maia-1.1.1/Hive_scripts/nndet_run_training.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,24 @@
         os.environ["det_num_threads"] = os.environ["N_THREADS"]
         os.environ["nnUNet_def_n_proc"] = os.environ["N_THREADS"]
         os.environ["det_models"] = data["results_folder"]
 
         if "receiver_email" in data:
             os.environ["receiver_email"] = data["receiver_email"]
 
-        subprocess.run(arguments)
-        # subprocess.run(["nndet_sweep", data["Task_ID"], "RetinaUNetV001_D3V001_3d", str(args['run_fold'])])
-        # subprocess.run(["nndet_eval", data["Task_ID"], "RetinaUNetV001_D3V001_3d", str(args['run_fold']),"--boxes","--seg","--instances","--analyze_boxes"])
-        # subprocess.run(["nndet_consolidate", data["Task_ID"], "RetinaUNetV001_D3V001_3d","--sweep_boxes"])
+        if int(args["run_fold"]) >= 0:
+            subprocess.run(arguments)
+            subprocess.run(["nndet_sweep", data["Task_ID"], "RetinaUNetV001_D3V001_3d", str(args["run_fold"])])
+
+        # subprocess.run(
+        #    ["nndet_eval", data["Task_ID"], "RetinaUNetV001_D3V001_3d", str(args['run_fold']), "--boxes", "--seg",
+        #     "--analyze_boxes"])
+        else:
+            subprocess.run(["nndet_consolidate", data["Task_ID"], "RetinaUNetV001_D3V001_3d", "--sweep_boxes"])
+            subprocess.run(
+                ["nndet_seg2nii", data["Task_ID"], "RetinaUNetV001_D3V001_3d", "--fold", str(args["run_fold"])])
+            subprocess.run(
+                ["nndet_boxes2nii", data["Task_ID"], "RetinaUNetV001_D3V001_3d", "--fold", str(args["run_fold"])])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.0/scripts/nnunet_run_prediction.py` & `hive-maia-1.1.1/Hive_scripts/nnunet_run_prediction.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,14 @@
     pars.add_argument(
         "--config-file",
         type=str,
         required=True,
         help="File path for the configuration dictionary, used to retrieve experiments variables (Task_ID)",
     )
 
-    pars.add_argument(
-        "--sub-step",
-        type=str,
-        required=False,
-        default=None,
-        help="Optional selected sub-step, to run the script in multi-step contexts(Cascade/2.5D).",
-    )
-
     add_verbosity_options_to_argparser(pars)
 
     return pars
 
 
 def main():
     parser = get_arg_parser()
@@ -78,45 +70,47 @@
     )
 
     config_file = args["config_file"]
 
     with open(config_file) as json_file:
         data = json.load(json_file)
 
+
+
         os.environ["nnUNet_raw_data_base"] = data["base_folder"]
         if data["base_folder"][0] != "/":
             os.environ["nnUNet_raw_data_base"] = str(Path(data["root_results_folder"]).joinpath(data["base_folder"]))
         os.environ["nnUNet_preprocessed"] = data["preprocessing_folder"]
         if data["preprocessing_folder"][0] != "/":
             os.environ["nnUNet_preprocessed"] = str(Path(data["root_results_folder"]).joinpath(data["preprocessing_folder"]))
         os.environ["RESULTS_FOLDER"] = data["results_folder"]
         if data["results_folder"][0] != "/":
             os.environ["RESULTS_FOLDER"] = str(
                 Path(data["root_results_folder"]).joinpath(data["results_folder"]))
+        if data["predictions_path"][0] != "/":
+            data["predictions_path"] = str(
+                Path(data["root_results_folder"]).joinpath(data["predictions_path"]))
         os.environ["nnUNet_def_n_proc"] = os.environ["N_THREADS"]
         os.environ["MKL_THREADING_LAYER"] = "GNU"
         os.environ["nnunet_use_progress_bar"] = "1"
         Path(args["output_folder"]).mkdir(parents=True, exist_ok=True)
         arguments_list = [
             "-i",
             args["input_folder"],
             "-o",
             args["output_folder"],
-            #"--model_folder",
-            #data["predictions_path"],
+            "--model_folder",
+            data["predictions_path"],
             "-t",
             "Task" + data["Task_ID"] + "_" + data["Task_Name"],
             "-tr",
             data["TRAINER_CLASS_NAME"],
         ]
-        if args["sub_step"] is not None:
-            arguments_list.extend(["-m", args["sub_step"]])
-            arguments_list.extend(["--sub-step", args["sub_step"]])
-        else:
-            arguments_list.extend(["-m", data["TRAINING_CONFIGURATION"]])
+
+        arguments_list.extend(["-m", data["TRAINING_CONFIGURATION"]])
 
         arguments_list.extend(unknown_arguments)
         os.system("nnUNet_predict " + " ".join(arguments_list))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.0/scripts/script_template.py` & `hive-maia-1.1.1/Hive_scripts/script_template.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.0/setup.py` & `hive-maia-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
+with open(os.path.join('VERSION')) as version_file:
+    version = version_file.read().strip()
+
 
 def resolve_requirements(file):
     requirements = []
     with open(file) as f:
         req = f.read().splitlines()
         for r in req:
             if r.startswith("-r"):
@@ -20,42 +23,47 @@
     with open(file) as f:
         content = f.read()
     return content
 
 
 setup(
     name="hive-maia",
-    version="1.0",
+    version=version,
     url="https://github.com/MAIA-KTH/Hive.git",
     license="GPLv3",
     project_urls={
-        'Documentation': 'https://hive-maia.readthedocs.io',
-        'Source': 'https://github.com/MAIA-KTH/Hive/issues',
-        'Tracker': 'https://github.com/MAIA-KTH/Hive/issues',
+        "Documentation": "https://hive-maia.readthedocs.io",
+        "Source": "https://github.com/MAIA-KTH/Hive",
+        "Tracker": "https://github.com/MAIA-KTH/Hive/issues",
     },
     author="Simone Bendazzoli",
     author_email="simben@kth.se",
     description="Python Package to support Deep Learning data preparation, pre-processing. training, result visualization"
                 " and model deployment across different frameworks (nnUNet, nnDetection, MONAI).",
     long_description=read_file(os.path.join(os.path.dirname(__file__), "README.md")),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={
         "": ["configs/*.yml", "configs/*.json"],
     },
+    data_files=[('', ['VERSION', "requirements.txt"]), ],
     # package_dir={"": "src"},
     install_requires=resolve_requirements(os.path.join(os.path.dirname(__file__), "requirements.txt")),
     entry_points={
         "console_scripts": [
-            "Hive_convert_DICOM_dataset_to_NIFTI_dataset = scripts.Hive_convert_DICOM_dataset_to_NIFTI_dataset:main",
-            "Hive_run_pipeline_from_file = scripts.Hive_run_pipeline_from_file:main",
-            "Hive_create_subset = scripts.Hive_create_subset:main",
-            "nndet_create_pipeline = scripts.nndet_create_pipeline:main",
-            "nndet_prepare_data_folder = scripts.nndet_prepare_data_folder:main",
-            "nndet_run_preprocessing = scripts.nndet_run_preprocessing:main",
-            "nndet_run_training = scripts.nndet_run_training:main",
-            "Hive_convert_semantic_to_instance_segmentation = scripts.Hive_convert_semantic_to_instance_segmentation:main",
+            "Hive_convert_DICOM_dataset_to_NIFTI_dataset = Hive_scripts.Hive_convert_DICOM_dataset_to_NIFTI_dataset:main",
+            "Hive_run_pipeline_from_file = Hive_scripts.Hive_run_pipeline_from_file:main",
+            "Hive_create_subset = Hive_scripts.Hive_create_subset:main",
+            "nndet_create_pipeline = Hive_scripts.nndet_create_pipeline:main",
+            "nndet_prepare_data_folder = Hive_scripts.nndet_prepare_data_folder:main",
+            "nndet_run_preprocessing = Hive_scripts.nndet_run_preprocessing:main",
+            "nndet_run_training = Hive_scripts.nndet_run_training:main",
+            "Hive_convert_semantic_to_instance_segmentation = Hive_scripts.Hive_convert_semantic_to_instance_segmentation:main",
+            "Hive_extract_experiment_predictions = Hive_scripts.Hive_extract_experiment_predictions:main",
+            "nndet_compute_metric_results = Hive_scripts.nndet_compute_metric_results:main",
+            "Hive_order_data_folder = Hive_scripts.Hive_order_data_folder:main",
         ],
     },
-    keywords=["deep learning", "image segmentation", "medical image analysis", "medical image segmentation"],
+    keywords=["deep learning", "image segmentation", "medical image analysis", "medical image segmentation",
+              "object detection"],
     # scripts=glob.glob("scripts/*"),
 )
```

