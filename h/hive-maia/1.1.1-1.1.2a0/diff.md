# Comparing `tmp/hive-maia-1.1.1.tar.gz` & `tmp/hive-maia-1.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-maia-1.1.1.tar", last modified: Wed Apr 19 13:57:16 2023, max compression
+gzip compressed data, was "hive-maia-1.1.2a0.tar", last modified: Wed Apr 19 14:41:10 2023, max compression
```

## Comparing `hive-maia-1.1.1.tar` & `hive-maia-1.1.2a0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.680844 hive-maia-1.1.1/Hive/
--rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/__init__.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/configs/
--rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/ATM_nnUNet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/configs/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/configs/nnDet_config_template.json
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/evaluation/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 12:06:26.000000 hive-maia-1.1.1/Hive/evaluation/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/abstract.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/evaluation/detection/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 12:49:04.000000 hive-maia-1.1.1/Hive/evaluation/detection/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/coco.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/froc.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/hist.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 12:57:19.000000 hive-maia-1.1.1/Hive/evaluation/detection/matching.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive/utils/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    23403 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/utils/file_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/log_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive/utils/seg_mask_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive/utils/volume_utils.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.684844 hive-maia-1.1.1/Hive_scripts/
--rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 13:12:18.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_create_subset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.1/Hive_scripts/Hive_extract_experiment_predictions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_order_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1413 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/Hive_run_pipeline_from_file.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 13:05:53.000000 hive-maia-1.1.1/Hive_scripts/nndet_compute_metric_results.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     5238 2023-04-19 13:52:16.000000 hive-maia-1.1.1/Hive_scripts/nndet_create_pipeline.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/nndet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_prediction.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/nnunet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.1/Hive_scripts/script_template.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 13:12:19.000000 hive-maia-1.1.1/Hive_scripts/upload_DICOM_to_Orthanc.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.1/LICENSE
--rw-rw-r--   0 simone    (1000) simone    (1000)     1647 2023-04-19 13:57:16.688844 hive-maia-1.1.1/PKG-INFO
--rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 13:38:38.000000 hive-maia-1.1.1/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)        5 2023-04-19 13:56:27.000000 hive-maia-1.1.1/VERSION
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/hive_maia.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1647 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-19 13:57:16.000000 hive-maia-1.1.1/hive_maia.egg-info/top_level.txt
--rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.1/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 13:12:49.000000 hive-maia-1.1.1/requirements.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-19 13:57:16.688844 hive-maia-1.1.1/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 13:53:59.000000 hive-maia-1.1.1/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 13:57:16.688844 hive-maia-1.1.1/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 13:12:19.000000 hive-maia-1.1.1/tests/test_file_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/__init__.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/configs/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/ATM_nnUNet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/configs/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/nnDet_config_template.json
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/evaluation/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/abstract.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/evaluation/detection/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/coco.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/froc.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/hist.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/matching.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/utils/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    23360 2023-04-19 14:39:29.000000 hive-maia-1.1.2a0/Hive/utils/file_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/log_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/seg_mask_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/utils/volume_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/Hive_scripts/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_create_subset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_extract_experiment_predictions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_order_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1413 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_run_pipeline_from_file.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_compute_metric_results.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     5238 2023-04-19 14:28:18.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_create_pipeline.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_prediction.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/script_template.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/upload_DICOM_to_Orthanc.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.2a0/LICENSE
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/PKG-INFO
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)        7 2023-04-19 14:40:19.000000 hive-maia-1.1.2a0/VERSION
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/hive_maia.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-19 14:41:09.000000 hive-maia-1.1.2a0/hive_maia.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:41:09.000000 hive-maia-1.1.2a0/hive_maia.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/top_level.txt
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.2a0/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 14:25:55.000000 hive-maia-1.1.2a0/requirements.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/tests/test_file_utils.py
```

### Comparing `hive-maia-1.1.1/Hive/__init__.py` & `hive-maia-1.1.2a0/Hive/__init__.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json` & `hive-maia-1.1.2a0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/configs/nnDet_config_template.json` & `hive-maia-1.1.2a0/Hive/configs/nnDet_config_template.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/evaluation/abstract.py` & `hive-maia-1.1.2a0/Hive/evaluation/abstract.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/evaluation/detection/coco.py` & `hive-maia-1.1.2a0/Hive/evaluation/detection/coco.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/evaluation/detection/froc.py` & `hive-maia-1.1.2a0/Hive/evaluation/detection/froc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/evaluation/detection/hist.py` & `hive-maia-1.1.2a0/Hive/evaluation/detection/hist.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/evaluation/detection/matching.py` & `hive-maia-1.1.2a0/Hive/evaluation/detection/matching.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/utils/file_utils.py` & `hive-maia-1.1.2a0/Hive/utils/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,34 +91,33 @@
     :param data_folder: folder path corresponding to the nnUNet_raw_data_base ENV variable
     :param task_id: string used as task_id when creating task folder
     :param task_name: string used as task_name when creating task folder
     :param subfolder: optional subfolder path for the data_folder tree
     """  # noqa E501
     logger.log(DEBUG, ' Creating Dataset tree at "{}"'.format(data_folder))
 
+    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "imagesTr", ).mkdir(
+        parents=True,
+        exist_ok=True,
+    )
 
-    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "imagesTr",).mkdir(
-            parents=True,
-            exist_ok=True,
-        )
-
-    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "labelsTr",).mkdir(
-            parents=True,
-            exist_ok=True,
-        )
+    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "labelsTr", ).mkdir(
+        parents=True,
+        exist_ok=True,
+    )
 
-    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "imagesTs",).mkdir(
-            parents=True,
-            exist_ok=True,
-        )
+    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "imagesTs", ).mkdir(
+        parents=True,
+        exist_ok=True,
+    )
 
-    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "labelsTs",).mkdir(
-            parents=True,
-            exist_ok=True,
-        )
+    Path(data_folder).joinpath("nnUNet_raw_data", "Task" + task_id + "_" + task_name, "labelsTs", ).mkdir(
+        parents=True,
+        exist_ok=True,
+    )
 
 
 def create_nndet_data_folder_tree(data_folder: Union[str, PathLike], task_name: str, task_id: str):
     """
     Create nnDetection folder tree, ready to be populated with the dataset.
 
     nnDetection folder tree:
@@ -452,15 +451,15 @@
     json_dict = {
         "name": dataset_name,
         "task": task_name,
         "dim": 3,
         "test_labels": True,
         "task_type": task_type,
         "tensorImageSize": "4D",
-        "modality": {str(i): modalities[i] for i in range(len(modalities))},
+        "modalities": {str(i): modalities[i] for i in range(len(modalities))},
         "labels": labels,  # {str(i): labels[i] for i in labels.keys()},
         "numTraining": len(train_subjects),
         "numTest": len(test_subjects),
         "n_tasks": n_tasks,
         "training": [{"image": "./imagesTr/%s.nii.gz" % i, "label": "./labelsTr/%s.nii.gz" % i} for i in
                      train_subjects],
         "test": ["./imagesTs/%s.nii.gz" % i for i in test_subjects],
```

### Comparing `hive-maia-1.1.1/Hive/utils/log_utils.py` & `hive-maia-1.1.2a0/Hive/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/utils/seg_mask_utils.py` & `hive-maia-1.1.2a0/Hive/utils/seg_mask_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive/utils/volume_utils.py` & `hive-maia-1.1.2a0/Hive/utils/volume_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_create_subset.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_create_subset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_extract_experiment_predictions.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_extract_experiment_predictions.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_order_data_folder.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_order_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/Hive_run_pipeline_from_file.py` & `hive-maia-1.1.2a0/Hive_scripts/Hive_run_pipeline_from_file.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nndet_compute_metric_results.py` & `hive-maia-1.1.2a0/Hive_scripts/nndet_compute_metric_results.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nndet_create_pipeline.py` & `hive-maia-1.1.2a0/Hive_scripts/nndet_create_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     pipeline_steps = []
 
     pipeline_steps.append(run_data_and_folder_preparation_step(arguments))
     pipeline_steps.append(run_preprocessing_step(output_json_config_file))
 
     [pipeline_steps.append(step) for step in run_training_step(output_json_config_file, range(config_dict["n_folds"]))]
 
-    pipeline_steps.append(run_training_step(output_json_config_file, "-1"))
+    pipeline_steps.append(run_training_step(output_json_config_file, [-1]))
 
     Path(os.environ["root_experiment_folder"]).joinpath(config_dict["Experiment Name"]).mkdir(exist_ok=True,
                                                                                               parents=True)
     pipeline_steps_summary = open(
         Path(os.environ["root_experiment_folder"]).joinpath(
             config_dict["Experiment Name"], "Task_" + arguments["task_ID"] + "_" + TIMESTAMP + ".txt"
         ),
```

### Comparing `hive-maia-1.1.1/Hive_scripts/nndet_prepare_data_folder.py` & `hive-maia-1.1.2a0/Hive_scripts/nndet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nndet_run_preprocessing.py` & `hive-maia-1.1.2a0/Hive_scripts/nndet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nndet_run_training.py` & `hive-maia-1.1.2a0/Hive_scripts/nndet_run_training.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nnunet_prepare_data_folder.py` & `hive-maia-1.1.2a0/Hive_scripts/nnunet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nnunet_run_prediction.py` & `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_prediction.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nnunet_run_preprocessing.py` & `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/nnunet_run_training.py` & `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_training.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/script_template.py` & `hive-maia-1.1.2a0/Hive_scripts/script_template.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/Hive_scripts/upload_DICOM_to_Orthanc.py` & `hive-maia-1.1.2a0/Hive_scripts/upload_DICOM_to_Orthanc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/LICENSE` & `hive-maia-1.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/PKG-INFO` & `hive-maia-1.1.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.1
+Version: 1.1.2a0
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.1/README.md` & `hive-maia-1.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/hive_maia.egg-info/PKG-INFO` & `hive-maia-1.1.2a0/hive_maia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.1
+Version: 1.1.2a0
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.1/hive_maia.egg-info/SOURCES.txt` & `hive-maia-1.1.2a0/hive_maia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/hive_maia.egg-info/entry_points.txt` & `hive-maia-1.1.2a0/hive_maia.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.1/setup.py` & `hive-maia-1.1.2a0/setup.py`

 * *Files identical despite different names*

