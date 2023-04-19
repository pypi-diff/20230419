# Comparing `tmp/Simba-UW-tf-dev-1.56.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.56.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.7.tar", last modified: Mon Apr 17 19:48:01 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.8.tar", last modified: Wed Apr 19 14:56:18 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.7.tar` & `Simba-UW-tf-dev-1.56.8.tar`

### file list

```diff
@@ -1,397 +1,391 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.7/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5554 2023-04-16 21:21:48.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     1727 2023-04-17 15:19:16.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-04-16 17:14:22.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    10405 2023-04-17 17:36:52.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/umap_embedder_2.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     7096 2023-04-17 19:46:42.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/grd_search_img_visualizer_2.py
--rw-r--r--   0 simon      (501) staff       (20)     6885 2023-04-16 21:07:58.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/dataset_creator_2.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)     8392 2023-04-17 17:37:22.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/hdbscan_clusterer_2.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6702 2023-04-17 16:45:09.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19468 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.7/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-17 14:05:31.000000 Simba-UW-tf-dev-1.56.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-17 19:14:16.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.7/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.7/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.7/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     4865 2023-04-17 19:13:41.000000 Simba-UW-tf-dev-1.56.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.7/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.7/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.7/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.7/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.7/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.7/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.7/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.7/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    46716 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.7/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.7/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.7/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.7/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.7/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.7/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.7/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.7/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.7/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.7/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.7/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.7/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56820 2023-04-15 18:59:15.000000 Simba-UW-tf-dev-1.56.7/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.7/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.7/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.7/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.7/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.7/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.7/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-17 19:14:16.000000 Simba-UW-tf-dev-1.56.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.7/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.7/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.7/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.7/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.7/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.7/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.7/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.7/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13557 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-17 19:48:00.000000 Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.7/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-17 19:47:59.000000 Simba-UW-tf-dev-1.56.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-17 19:48:01.000000 Simba-UW-tf-dev-1.56.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.8/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11585 2023-04-19 14:00:17.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     1759 2023-04-18 23:05:39.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     5384 2023-04-17 20:49:22.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/grd_search_cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-19 14:11:27.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7061 2023-04-18 19:40:55.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6681 2023-04-19 12:53:45.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    10557 2023-04-18 23:05:39.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    18462 2023-04-18 17:25:40.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8392 2023-04-17 17:37:22.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.56.8/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-19 14:11:32.000000 Simba-UW-tf-dev-1.56.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.8/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.8/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8217 2023-04-18 15:24:14.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     5584 2023-04-18 16:54:56.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.8/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.56.8/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.8/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.8/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.8/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    46900 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.8/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.8/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.8/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.8/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.8/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.8/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.8/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.8/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.8/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.8/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56935 2023-04-18 14:46:46.000000 Simba-UW-tf-dev-1.56.8/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.8/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.8/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.8/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.8/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.8/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.8/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.8/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.56.8/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.8/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13367 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.8/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-19 14:54:56.000000 Simba-UW-tf-dev-1.56.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.7/PKG-INFO` & `Simba-UW-tf-dev-1.56.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.7
+Version: 1.56.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/video_processing.py` & `Simba-UW-tf-dev-1.56.8/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     FEATURE_PATH = 'feature_path'
     BOUT_AGGREGATION_TYPE = 'bout_aggregation_type'
     MIN_BOUT_LENGTH = 'min_bout_length'
     N_NEIGHBORS = 'n_neighbors'
     HASHED_NAME = 'HASH'
     DATA = 'DATA'
     RAW = 'RAW'
+    SCALER_TYPE = 'SCALER_TYPE'
     CSV = 'CSV'
     FORMAT = 'format'
     SCALED_DATA = 'SCALED_DATA'
     PARAMETERS = 'PARAMETERS'
     METHODS = 'METHODS'
     DR_MODEL = 'DR_MODEL'
     MODEL = 'MODEL'
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
-00000050: 0000 0001 0000 1000 0061 006c 0069 007a  .........a.l.i.z
-00000060: 0061 0074 0000 0000 0000 0000 0000 0000  .a.t............
+00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
+00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,128 +250,128 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0004 0000 0013  ................
-00001010: 0076 0069 0073 0075 0061 006c 0069 007a  .v.i.s.u.a.l.i.z
-00001020: 0061 0074 0069 006f 006e 005f 0074 006f  .a.t.i.o.n._.t.o
-00001030: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
-00001040: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00001050: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00001060: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00001070: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00001080: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001090: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-000010a0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-000010b0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-000010c0: 5f10 197b 7b31 3132 302c 2034 3738 7d2c  _..{{1120, 478},
-000010d0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
-000010e0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-000010f0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00001100: 0000 0000 0000 0000 0000 009b 0000 0013  ................
-00001110: 0076 0069 0073 0075 0061 006c 0069 007a  .v.i.s.u.a.l.i.z
-00001120: 0061 0074 0069 006f 006e 005f 0074 006f  .a.t.i.o.n._.t.o
-00001130: 006f 006c 0073 6c73 7643 626c 6f62 0000  .o.l.slsvCblob..
-00001140: 02d4 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
-00001150: 0607 0809 0a0b 0c0d 1d4a 4b4c 4d0c 4f5f  .........JKLM.O_
-00001160: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00001170: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-00001180: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00001190: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-000011a0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-000011b0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-000011c0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-000011d0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000011e0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000011f0: 6f6e 5369 7a65 1001 09ab 0e17 1f24 282d  onSize.......$(-
-00001200: 3237 3c40 45d4 0f10 1112 130c 150c 5a69  27<@E.........Zi
-00001210: 6465 6e74 6966 6965 7259 6173 6365 6e64  dentifierYascend
-00001220: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00001230: 6554 6e61 6d65 0911 012c 09d4 0f18 191a  eTname...,......
-00001240: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00001250: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00001260: 7175 6974 7910 2308 08d4 0f10 1112 201d  quity.#....... .
-00001270: 220c 5c64 6174 654d 6f64 6966 6965 6408  ".\dateModified.
-00001280: 10b5 09d4 0f10 1112 251d 221d 5b64 6174  ........%.".[dat
-00001290: 6543 7265 6174 6564 0808 d40f 1011 1229  eCreated.......)
-000012a0: 1d2b 0c54 7369 7a65 0810 6109 d40f 1011  .+.Tsize..a.....
-000012b0: 122e 0c30 0c54 6b69 6e64 0910 7309 d40f  ...0.Tkind..s...
-000012c0: 1011 1233 0c35 1d55 6c61 6265 6c09 1064  ...3.5.Ulabel..d
-000012d0: 08d4 0f10 1112 380c 3a1d 5776 6572 7369  ......8.:.Wversi
-000012e0: 6f6e 0910 4b08 d40f 1011 123d 0c15 1d58  on..K......=...X
-000012f0: 636f 6d6d 656e 7473 0908 d40f 1011 1241  comments.......A
-00001300: 1d43 1d5e 6461 7465 4c61 7374 4f70 656e  .C.^dateLastOpen
-00001310: 6564 0810 c808 d40f 1819 1a46 221d 1d59  ed.........F"..Y
-00001320: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-00001330: 0000 0000 0023 4028 0000 0000 0000 2340  .....#@(......#@
-00001340: 1800 0000 0000 0054 6e61 6d65 0923 4030  .......Tname.#@0
-00001350: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
-00001360: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
-00001370: 00b7 00c3 00cc 00d7 00e1 00e7 00ef 00f4  ................
-00001380: 00f5 00f8 00f9 0102 0108 0112 011a 0123  ...............#
-00001390: 0125 0126 0127 0130 013d 013e 0140 0141  .%.&.'.0.=.>.@.A
-000013a0: 014a 0156 0157 0158 0161 0166 0167 0169  .J.V.W.X.a.f.g.i
-000013b0: 016a 0173 0178 0179 017b 017c 0185 018b  .j.s.x.y.{.|....
-000013c0: 018c 018e 018f 0198 01a0 01a1 01a3 01a4  ................
-000013d0: 01ad 01b6 01b7 01b8 01c1 01d0 01d1 01d3  ................
-000013e0: 01d4 01dd 01e7 01e8 01e9 01ea 01f3 01fc  ................
-000013f0: 0205 020a 020b 0000 0000 0000 0201 0000  ................
-00001400: 0000 0000 0050 0000 0000 0000 0000 0000  .....P..........
-00001410: 0000 0000 0214 0000 0013 0076 0069 0073  ...........v.i.s
-00001420: 0075 0061 006c 0069 007a 0061 0074 0069  .u.a.l.i.z.a.t.i
-00001430: 006f 006e 005f 0074 006f 006f 006c 0073  .o.n._.t.o.o.l.s
-00001440: 6c73 7670 626c 6f62 0000 029b 6270 6c69  lsvpblob....bpli
-00001450: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00001460: 0c0d 1c46 4748 490c 4b5f 1012 7669 6577  ...FGHI.K_..view
-00001470: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00001480: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001490: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000014a0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-000014b0: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-000014c0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-000014d0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-000014e0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000014f0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-00001500: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-00001510: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
-00001520: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
-00001530: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001540: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001550: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001560: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001570: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001580: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001590: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-000015a0: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-000015b0: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-000015c0: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-000015d0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-000015e0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-000015f0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-00001600: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-00001610: 2800 0000 0000 0023 4018 0000 0000 0000  (......#@.......
-00001620: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001630: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001640: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001650: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001660: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001670: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001680: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001690: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-000016a0: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-000016b0: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-000016c0: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-000016d0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-000016e0: 0000 0000 0001 e300 0000 1300 7600 6900  ............v.i.
-000016f0: 7300 7500 6100 6c00 6900 7a00 6100 7400  s.u.a.l.i.z.a.t.
-00001700: 6900 6f00 6e00 5f00 7400 6f00 6f00 6c00  i.o.n._.t.o.o.l.
-00001710: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
+00001000: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00001020: 0065 005f 005f 6277 7370 626c 6f62 0000  .e._._bwspblob..
+00001030: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00001040: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00001050: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00001060: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00001070: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001080: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001090: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000010a0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+000010b0: 5f10 197b 7b31 3036 322c 2033 3733 7d2c  _..{{1062, 373},
+000010c0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
+000010d0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+000010e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+000010f0: 0000 0000 0000 0000 0000 009b 0000 000b  ................
+00001100: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00001110: 0065 005f 005f 6c73 7643 626c 6f62 0000  .e._._lsvCblob..
+00001120: 02d4 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
+00001130: 0607 0809 0a0b 0c0d 1d4a 4b4c 4d0c 4f5f  .........JKLM.O_
+00001140: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00001150: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+00001160: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00001170: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00001180: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
+00001190: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
+000011a0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
+000011b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+000011c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
+000011d0: 6f6e 5369 7a65 1001 09ab 0e17 1f24 282d  onSize.......$(-
+000011e0: 3237 3c40 45d4 0f10 1112 130c 150c 5a69  27<@E.........Zi
+000011f0: 6465 6e74 6966 6965 7259 6173 6365 6e64  dentifierYascend
+00001200: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
+00001210: 6554 6e61 6d65 0911 012c 09d4 0f18 191a  eTname...,......
+00001220: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
+00001230: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
+00001240: 7175 6974 7910 2308 08d4 0f10 1112 201d  quity.#....... .
+00001250: 220c 5c64 6174 654d 6f64 6966 6965 6408  ".\dateModified.
+00001260: 10b5 09d4 0f10 1112 251d 221d 5b64 6174  ........%.".[dat
+00001270: 6543 7265 6174 6564 0808 d40f 1011 1229  eCreated.......)
+00001280: 1d2b 0c54 7369 7a65 0810 6109 d40f 1011  .+.Tsize..a.....
+00001290: 122e 0c30 0c54 6b69 6e64 0910 7309 d40f  ...0.Tkind..s...
+000012a0: 1011 1233 0c35 1d55 6c61 6265 6c09 1064  ...3.5.Ulabel..d
+000012b0: 08d4 0f10 1112 380c 3a1d 5776 6572 7369  ......8.:.Wversi
+000012c0: 6f6e 0910 4b08 d40f 1011 123d 0c15 1d58  on..K......=...X
+000012d0: 636f 6d6d 656e 7473 0908 d40f 1011 1241  comments.......A
+000012e0: 1d43 1d5e 6461 7465 4c61 7374 4f70 656e  .C.^dateLastOpen
+000012f0: 6564 0810 c808 d40f 1819 1a46 221d 1d59  ed.........F"..Y
+00001300: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
+00001310: 0000 0000 0023 4028 0000 0000 0000 2340  .....#@(......#@
+00001320: 1400 0000 0000 0054 6e61 6d65 0923 4030  .......Tname.#@0
+00001330: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
+00001340: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
+00001350: 00b7 00c3 00cc 00d7 00e1 00e7 00ef 00f4  ................
+00001360: 00f5 00f8 00f9 0102 0108 0112 011a 0123  ...............#
+00001370: 0125 0126 0127 0130 013d 013e 0140 0141  .%.&.'.0.=.>.@.A
+00001380: 014a 0156 0157 0158 0161 0166 0167 0169  .J.V.W.X.a.f.g.i
+00001390: 016a 0173 0178 0179 017b 017c 0185 018b  .j.s.x.y.{.|....
+000013a0: 018c 018e 018f 0198 01a0 01a1 01a3 01a4  ................
+000013b0: 01ad 01b6 01b7 01b8 01c1 01d0 01d1 01d3  ................
+000013c0: 01d4 01dd 01e7 01e8 01e9 01ea 01f3 01fc  ................
+000013d0: 0205 020a 020b 0000 0000 0000 0201 0000  ................
+000013e0: 0000 0000 0050 0000 0000 0000 0000 0000  .....P..........
+000013f0: 0000 0000 0214 0000 000b 005f 005f 0070  ..........._._.p
+00001400: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00001410: 6c73 7670 626c 6f62 0000 029b 6270 6c69  lsvpblob....bpli
+00001420: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001430: 0c0d 1c46 4748 490c 4b5f 1012 7669 6577  ...FGHI.K_..view
+00001440: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00001450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001470: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00001480: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00001490: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000014a0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000014b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000014c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000014d0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+000014e0: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
+000014f0: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
+00001500: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001510: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001520: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
+00001530: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
+00001540: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
+00001550: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
+00001560: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
+00001570: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
+00001580: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
+00001590: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
+000015a0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
+000015b0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
+000015c0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
+000015d0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
+000015e0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
+000015f0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
+00001600: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+00001610: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+00001620: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
+00001630: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
+00001640: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
+00001650: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
+00001660: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
+00001670: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
+00001680: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
+00001690: cb01 d401 d901 da00 0000 0000 0002 0100  ................
+000016a0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+000016b0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
+000016c0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+000016d0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
+000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,49 +457,49 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0069 7a65  .....@.......ize
-00001d00: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-00001d10: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
-00001d20: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
-00001d30: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001d40: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001d50: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001d60: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001d70: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001d80: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001d90: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-00001da0: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-00001db0: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-00001dc0: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-00001dd0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-00001de0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-00001df0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-00001e00: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-00001e10: 2800 0000 0000 0023 4018 0000 0000 0000  (......#@.......
-00001e20: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001e30: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001e40: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001e50: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001e60: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001e70: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001e80: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001e90: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-00001ea0: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-00001eb0: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-00001ec0: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-00001ed0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-00001ee0: 0000 0000 0001 e300 0000 1300 7600 6900  ............v.i.
-00001ef0: 7300 7500 6100 6c00 6900 7a00 6100 7400  s.u.a.l.i.z.a.t.
-00001f00: 6900 6f00 6e00 5f00 7400 6f00 6f00 6c00  i.o.n._.t.o.o.l.
-00001f10: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
+00001cf0: 0000 0000 0140 0000 0000 0000 0064 5b64  .....@.......d[d
+00001d00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001d10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001d20: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
+00001d30: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
+00001d40: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
+00001d50: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
+00001d60: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
+00001d70: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
+00001d80: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
+00001d90: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
+00001da0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
+00001db0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
+00001dc0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
+00001dd0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
+00001de0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
+00001df0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
+00001e00: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+00001e10: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+00001e20: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
+00001e30: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
+00001e40: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
+00001e50: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
+00001e60: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
+00001e70: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
+00001e80: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
+00001e90: cb01 d401 d901 da00 0000 0000 0002 0100  ................
+00001ea0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+00001eb0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
+00001ec0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+00001ed0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
+00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/movement_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-import os, glob
+__author__ = "Simon Nilsson"
+
 import pandas as pd
-from simba.read_config_unit_tests import (read_project_path_and_file_type,
-                                          read_config_file,
-                                          read_config_entry,
-                                          check_if_filepath_list_is_empty,
-                                          check_file_exist_and_readable)
-from simba.unsupervised.misc import bout_aggregator
-from simba.train_model_functions import get_all_clf_names
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer)
-from simba.feature_extractors.unit_tests import read_video_info, read_video_info_csv
-from simba.drop_bp_cords import getBpNames
+                              framewise_euclidean_distance,
+                              )
+from simba.utils.printing import stdout_success
+from simba.feature_extractors.unit_tests import read_video_info
+from simba.read_config_unit_tests import (read_config_entry,
+                                          check_if_filepath_list_is_empty)
+from simba.utils.errors import NoSpecifiedOutputError
+from simba.enums import ReadConfig
+import os
+from simba.mixins.config_reader import ConfigReader
+from collections import defaultdict
 from simba.rw_dfs import read_df
-from simba.enums import Paths, ReadConfig, Dtypes
-from datetime import datetime
-import pickle
+import numpy as np
+from statistics import mean
+
+class MovementProcessor(ConfigReader):
+    """
+    Class for computing aggregate movement statistics.
+
+    Parameters
+    ----------
+    config_path: str
+        path to SimBA project config file in Configparser format
+
+    Notes
+    ----------
+
+    Examples
+    ----------
+    >>> movement_processor = MovementProcessor(config_path='MyConfigPath')
+    >>> movement_processor.process_movement()
+    >>> movement_processor.save_results()
 
+    """
 
-class DatasetCreator(object):
     def __init__(self,
                  config_path: str,
-                 settings: dict):
+                 visualization: bool = False,
+                 files: list=None):
 
-        self.config, self.settings = read_config_file(ini_path=config_path), settings
-        self.config_path, self.clf_type = config_path, None
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.model_cnt = read_config_entry(self.config, ReadConfig.SML_SETTINGS.value, ReadConfig.TARGET_CNT.value, data_type=Dtypes.INT.value)
-        self.clf_names = get_all_clf_names(config=self.config, target_cnt=self.model_cnt)
-        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
-        self.logs_path = os.path.join(self.project_path, 'logs')
-        self.save_path = os.path.join(self.logs_path, 'unsupervised_data_{}.pickle'.format(self.datetime))
-        self.input_dir = os.path.join(self.project_path, Paths.MACHINE_RESULTS_DIR.value)
-        self.video_info_df = read_video_info_csv(os.path.join(self.project_path, Paths.VIDEO_INFO.value))
-        self.files_found = glob.glob(f'{self.input_dir}/*.{self.file_type}')
-        self.model_cnt = read_config_entry(self.config, ReadConfig.SML_SETTINGS.value, ReadConfig.TARGET_CNT.value, data_type=Dtypes.INT.value)
-        self.clf_names = get_all_clf_names(config=self.config, target_cnt=self.model_cnt)
-        self.clf_probability_cols = ['Probability_' + x for x in self.clf_names]
-
-        self.clf_cols = self.clf_names + self.clf_probability_cols
-        self.bp_names = list(getBpNames(inifile=self.config_path))
-        self.bp_names = [item for sublist in self.bp_names for item in sublist]
-        check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg='NO MACHINE LEARNING DATA FOUND')
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
-        print('Creating unsupervised learning dataset...')
-        if settings['data_slice'] == 'ALL FEATURES (EXCLUDING POSE)':
-            self.all_features_concatenator()
-        elif settings['data_slice'] == 'USER-DEFINED FEATURE SET':
-            self.user_defined_concatenator()
+        super().__init__(config_path=config_path)
+        self.save_path = os.path.join(self.logs_path, 'Movement_log_{}.csv'.format(self.datetime))
+        try:
+            self.animal_cnt = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'no_of_animals', 'int')
+            self.p_threshold = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'probability_threshold', 'float')
+        except:
+            raise NoSpecifiedOutputError(msg='Please analyze movements before visualizing data.')
+        self.bp_dict = defaultdict(list)
+        self.bp_columns = []
+        if not visualization:
+            for cnt, animal in enumerate(self.multi_animal_id_list):
+                bp_name = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt+1), 'str')
+                if bp_name == 'None':
+                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
+                for c in ['_x', '_y', '_p']:
+                    self.bp_dict[animal].append(bp_name + c)
+                    self.bp_columns.append(bp_name + c)
+            check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
+                                            error_msg=f'SIMBA ERROR: Cannot process movement. ZERO data files found in the {self.outlier_corrected_dir} directory.')
+            self.files_found = self.outlier_corrected_paths
         else:
-            self.all_data_concatenator()
-        self.get_feature_names()
-        self.clf_slicer()
-        self.save()
-
-    def all_data_concatenator(self):
-        self.df = []
-        for file_path in self.files_found:
-            _, video_name, _ = get_fn_ext(filepath=file_path)
-            df = read_df(file_path=file_path,file_type=self.file_type)
-            df.insert(0, 'FRAME', df.index)
-            df.insert(0, 'VIDEO', video_name)
-            self.df.append(df)
-        self.df = pd.concat(self.df, axis=0).reset_index(drop=True)
-        self.df_bp = self.df[self.bp_names + ['FRAME', 'VIDEO']]
-
-    def all_features_concatenator(self):
-        self.df = []
-        for file_path in self.files_found:
-            _, video_name, _ = get_fn_ext(filepath=file_path)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            df.insert(0, 'FRAME', df.index)
-            df.insert(0, 'VIDEO', video_name)
-            self.df.append(df)
-        self.df = pd.concat(self.df, axis=0).reset_index(drop=True)
-        self.df_bp = self.df[self.bp_names + ['FRAME', 'VIDEO']]
-        self.df = self.df.drop(self.bp_names, axis=1)
-
-    def user_defined_concatenator(self):
-        if not self.settings['feature_path']:
-            raise FileNotFoundError('Select a feature file path')
-        check_file_exist_and_readable(self.settings['feature_path'])
-        feature_lst = list(pd.read_csv(self.settings['feature_path'], header=None)[0])
-        self.df = []
-        for file_path in self.files_found:
-            _, video_name, _ = get_fn_ext(filepath=file_path)
-            df = read_df(file_path=file_path, file_type=self.file_type, usecols=feature_lst + self.clf_cols + self.bp_names)
-            df.insert(0, 'FRAME', df.index)
-            df.insert(0, 'VIDEO', video_name)
-            self.df.append(df)
-        self.df = pd.concat(self.df, axis=0).reset_index(drop=True)
-        self.df_bp = self.df[self.bp_names + ['FRAME', 'VIDEO']]
-        self.df = self.df.drop(self.bp_names, axis=1)
-
-
-    def clf_slicer(self):
-        self.df = bout_aggregator(data=self.df,
-                                  clfs=self.clf_names,
-                                  video_info=self.video_info_df,
-                                  feature_names=self.feature_names,
-                                  min_bout_length=int(self.settings['min_bout_length']),
-                                  aggregator=self.settings['bout_aggregation']).reset_index(drop=True)
-        if self.settings['clf_slice'] in self.clf_names:
-            self.df = self.df[self.df['CLASSIFIER'] == self.settings['clf_slice']].reset_index(drop=True)
-
-    def get_feature_names(self):
-        self.feature_names = [x for x in self.df.columns if x not in self.clf_cols]
-        self.feature_names = self.feature_names[2:]
-
-    def save(self):
-        if len(self.df) == 0:
-            print('SIMBA ERROR: The data contains zero frames after the chosen slice setting')
-            raise ValueError()
+            for cnt in range(self.animal_cnt):
+                bp_name = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt+1), 'str')
+                if bp_name == 'None':
+                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
+                for c in ['_x', '_y', '_p']:
+                    self.bp_dict[self.multi_animal_id_list[cnt]].append(bp_name + c)
+                    self.bp_columns.append(bp_name + c)
+            self.files_found = files
+        print(f'Processing {str(len(self.outlier_corrected_paths))} video(s)...')
+
+    def process_movement(self):
+        """
+        Method to run movement aggregation computations.
+
+        Returns
+        ----------
+        Attribute: dict
+            results
 
+        """
         self.results = {}
-        self.results['VIDEO_NAMES'] = self.df[['VIDEO']]
-        self.results['DATA'] = self.df[self.feature_names]
-        self.results['POSE'] = self.df_bp
-        self.results['START_FRAME'] = self.df[['START_FRAME']]
-        self.results['END_FRAME'] = self.df[['END_FRAME']]
-        self.results['CLF'] = pd.get_dummies(self.df[["CLASSIFIER"]], prefix='', prefix_sep='')
-        self.results['CLF_PROBABILITY'] = self.df[['PROBABILITY']]
-
-        with open(self.save_path, 'wb') as f:
-            pickle.dump(self.results, f, protocol=pickle.HIGHEST_PROTOCOL)
+        self.movement_dict = {}
+        for file_path in self.files_found:
+            _, video_name, _ = get_fn_ext(file_path)
+            print('Analysing {}...'.format(video_name))
+            self.data_df = read_df(file_path, self.file_type)[self.bp_columns]
+            self.video_info, self.px_per_mm, self.fps = read_video_info(vid_info_df=self.video_info_df, video_name=video_name)
+            self.results[video_name] = {}
+            self.movement_dict[video_name] = {}
+            for animal_name, animal_bps in self.bp_dict.items():
+                self.results[video_name][animal_name] = {}
+                animal_df = self.data_df[animal_bps]
+                if self.p_threshold > 0.00:
+                    animal_df = animal_df[animal_df[animal_bps[2]] >= self.p_threshold]
+                animal_df = animal_df.iloc[:, 0:2].reset_index(drop=True)
+                df_shifted = animal_df.shift(1)
+                df_shifted = df_shifted.combine_first(animal_df).add_suffix('_shifted')
+                animal_df = pd.concat([animal_df, df_shifted], axis=1)
+                bp_time_1 = animal_df[[animal_bps[0], animal_bps[1]]].values.astype(float)
+                bp_time_2 = animal_df[[animal_bps[0] + '_shifted', animal_bps[1] + '_shifted']].values.astype(float)
+                self.movement = pd.Series(framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=self.px_per_mm))
+                self.movement.loc[0] = 0
+                self.movement_dict[video_name][animal_name] = self.movement
+                self.results[video_name][animal_name]['Distance (cm)'] = round((self.movement.sum() / 10), 4)
+                velocity_lst = []
+                for df in np.array_split(self.movement, int(len(self.movement) / self.fps)):
+                    velocity_lst.append(df.sum())
+                self.results[video_name][animal_name]['Velocity (cm/s)'] = round((mean(velocity_lst) / 10), 4)
+
+    def save_results(self):
+        """
+        Method to save movement aggregation data into the `project_folder/logs` directory
+        of the SimBA project.
+
+        Returns
+        ----------
+        None
+
+        """
+
+        self.out_df = pd.DataFrame(columns=['Video', 'Animal', 'Measurement', 'Value'])
+        for video, video_data in self.results.items():
+            for animal, animal_data in video_data.items():
+                for measure, mesure_val in animal_data.items():
+                    self.out_df.loc[len(self.out_df)] = [video, animal, measure, mesure_val]
+        self.out_df.set_index('Video').to_csv(self.save_path)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Dataset for unsupervised learning saved at {self.save_path}. The dataset contains {str(len(self.results["DATA"]))} bouts (elapsed time {self.timer.elapsed_time_str}s)')
-
+        stdout_success(msg= f'Movement log saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-#
-# settings = {'data_slice': 'ALL FEATURES (EXCLUDING POSE)',
-#             'clf_slice': 'Attack',
-#             'bout_aggregation': 'MEDIAN',
-#             'min_bout_length': 66,
-#             'feature_path': '/Users/simon/Desktop/envs/simba_dev/simba/assets/unsupervised/features.csv'}
-# #
-# _ = DatasetCreator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
-#                    settings=settings)
-#
+#test = MovementProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
+# test.process_movement()
+# test.save_results()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/umap_embedder_2.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/umap_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import random
 from copy import deepcopy
 from simba.misc_tools import SimbaTimer
 from simba.read_config_unit_tests import check_file_exist_and_readable
-from simba.unsupervised.misc import (check_that_directory_is_empty,
-                                     check_directory_exists)
+from simba.unsupervised.misc import check_that_directory_is_empty
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.unsupervised.enums import Unsupervised
 from simba.utils.printing import stdout_success
-from simba.rw_dfs import save_df
 
 import itertools
 import pandas as pd
 
 
 try:
     from cuml import UMAP
@@ -32,15 +30,15 @@
 
         self.data_path = data_path
         check_file_exist_and_readable(file_path=self.data_path)
         self.data = self.read_pickle(data_path=data_path)
         self.umap_df = deepcopy(self.data[Unsupervised.BOUTS_FEATURES.value]).set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value])
         self.save_dir = save_dir
         check_that_directory_is_empty(directory=self.save_dir)
-        self.low_var_cols = None
+        self.low_var_cols, self.hyper_parameters = None, hyper_parameters
         self.check_umap_hyperparameters(hyper_parameters=hyper_parameters)
         self.search_space = list(itertools.product(*[hyper_parameters[Unsupervised.N_NEIGHBORS.value],
                                                      hyper_parameters[Unsupervised.MIN_DISTANCE.value],
                                                      hyper_parameters[Unsupervised.SPREAD.value]]))
         print(f'Building {len(self.search_space)} UMAP model(s)...')
         if hyper_parameters[Unsupervised.VARIANCE.value] > 0:
             self.low_var_cols = self.find_low_variance_fields(data=self.umap_df, variance=hyper_parameters[Unsupervised.VARIANCE.value])
@@ -52,15 +50,17 @@
         self.__fit_umaps()
         self.timer.stop_timer()
         stdout_success(msg=f'{len(self.search_space)} models saved in {self.save_dir} directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __create_methods_log(self):
         self.methods = {}
         self.methods[Unsupervised.SCALER.value] = self.scaler
+        self.methods[Unsupervised.SCALER_TYPE.value] = self.hyper_parameters[Unsupervised.SCALER.value]
         self.methods[Unsupervised.SCALED_DATA.value] = self.scaled_umap_data
+        self.methods[Unsupervised.VARIANCE.value] = self.hyper_parameters[Unsupervised.VARIANCE.value]
         self.methods[Unsupervised.LOW_VARIANCE_FIELDS.value] = self.low_var_cols
         self.methods[Unsupervised.FEATURE_NAMES.value] = self.scaled_umap_data.columns
 
     def __fit_umaps(self):
         for cnt, h in enumerate(self.search_space):
             self.model_count = cnt
             self.model = {}
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/dbcv_calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os.path
-
 import pandas as pd
-
-from simba.unsupervised.misc import (read_pickle,
-                                     find_embedding,
-                                     check_directory_exists)
-from simba.misc_tools import SimbaTimer
+from simba.unsupervised.misc import check_directory_exists
+from simba.misc_tools import SimbaTimer, check_file_exist_and_readable
 import numpy as np
 from numba import jit, prange
 from numba.typed import List
 from scipy.sparse.csgraph import minimum_spanning_tree
 from scipy.sparse import csgraph
-from datetime import datetime
-from simba.read_config_unit_tests import read_project_path_and_file_type, read_config_file
+from simba.unsupervised.enums import Unsupervised, Clustering
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
+from simba.mixins.config_reader import ConfigReader
+from simba.utils.printing import stdout_success
 
 
+CLUSTERER_NAME = 'CLUSTERER_NAME'
+CLUSTER_COUNT = 'CLUSTER_COUNT'
+EMBEDDER_NAME = 'EMBEDDER_NAME'
+DBCV = 'DBCV'
 
-class DBCVCalculator(object):
+
+class DBCVCalculator(UnsupervisedMixin, ConfigReader):
     """
     Density-based Cluster Validation (DBCV).
 
     Parameters
     ----------
     embedders_path: str
         Directory holding dimensionality reduction models in pickle format.
@@ -41,59 +44,55 @@
     Examples
     -----
     >>> dbcv_calculator = DBCVCalculator(clusterers_path='unsupervised/cluster_models', config_path='my_simba_config')
     >>> results = dbcv_calculator.run()
     """
 
     def __init__(self,
-                 clusterers_path: str,
-                 config_path: str):
-
-        check_directory_exists(clusterers_path)
-        print('Reading in data...')
-        self.config = read_config_file(ini_path=config_path)
-        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
-        self.clusterers = read_pickle(data_path=clusterers_path)
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.save_path = os.path.join(self.project_path, 'logs', f'DBCV_{self.datetime}.xlsx')
-        print(f'Analyzing DBCV for {len(self.clusterers.keys())} clusterers...')
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
+                 config_path: str,
+                 data_path: str):
 
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
+        if os.path.isdir(data_path):
+            check_directory_exists(data_path)
+            self.data = self.read_pickle(data_path=data_path)
+        else:
+            check_file_exist_and_readable(file_path=data_path)
+            self.data = {0: self.read_pickle(data_path=data_path)}
+        self.save_path = os.path.join(self.logs_path, f'DBCV_{self.datetime}.xlsx')
         with pd.ExcelWriter(self.save_path, mode='w') as writer:
             pd.DataFrame().to_excel(writer, sheet_name=' ', index=True)
 
     def run(self):
+        print(f'Analyzing DBCV for {len(self.data.keys())} clusterers...')
         self.results = {}
-        for k, v in self.clusterers.items():
-            self.results[k] = {}
-            print(f"Performing DBCV for model {v['NAME']}...")
-            model_timer = SimbaTimer()
-            model_timer.start_timer()
-            embedder = v['EMBEDDER']['MODEL']
-            labels = v['MODEL'].labels_.reshape(-1, 1).astype(np.int8)
-            unique_labels = np.unique(labels).shape[0]
-            X = embedder.embedding_
-            self.results[k]['clusterer_name'] = v['NAME']
-            self.results[k]['embedder_name'] = v['HASH']
-            self.results[k] = {**self.results[k], **v['PARAMETERS']}
-            dbcv = 'nan'
-            if unique_labels > 1:
-                dbcv = self.DBCV(X, labels)
-            self.results[k] = {**self.results[k], **{'dbcv': dbcv}}
-            self.results[k] = {**self.results[k], **{'cluster_cnt': unique_labels}}
+        for k, v in self.data.items():
+            model_timer = SimbaTimer(start=True)
+            self.results[k], dbcv_results = {}, 'nan'
+            self.results[k][CLUSTERER_NAME] = v[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value]
+            self.results[k][EMBEDDER_NAME] = v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]
+            print(f"Performing DBCV for cluster model {self.results[k][CLUSTERER_NAME]}...")
+            cluster_lbls = v[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
+            x = v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_
+            self.results[k] = {**self.results[k], **v[Clustering.CLUSTER_MODEL.value][Unsupervised.PARAMETERS.value], **v[Unsupervised.DR_MODEL.value][Unsupervised.PARAMETERS.value]}
+            cluster_cnt = self.get_cluster_cnt(data=cluster_lbls, clusterer_name=v[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value], minimum_clusters=1)
+
+            if cluster_cnt > 1:
+                dbcv_results = self.DBCV(x, cluster_lbls)
+            self.results[k] = {**self.results[k], **{DBCV: dbcv_results}, **{CLUSTER_COUNT: cluster_cnt}}
             model_timer.stop_timer()
-            print(f"DBCV complete for model {self.results[k]['clusterer_name']} (elapsed time {model_timer.elapsed_time_str}s)...")
+            stdout_success(msg=f"DBCV complete for model {self.results[k][CLUSTERER_NAME]}", elapsed_time=model_timer.elapsed_time_str)
         self.__save_results()
 
     def __save_results(self):
         for k, v in self.results.items():
-            df = pd.DataFrame.from_dict(v, orient='index')
+            df = pd.DataFrame.from_dict(v, orient='index', columns=['VALUE'])
             with pd.ExcelWriter(self.save_path, mode='a') as writer:
-                df.to_excel(writer, sheet_name=v['clusterer_name'], index=True)
+                df.to_excel(writer, sheet_name=v[CLUSTERER_NAME], index=True)
 
     def DBCV(self, X, labels):
         """
         Parameters
         ----------
         X : array with shape len(observations) x len(dimentionality reduced dimensions)
         labels : 1D array with cluster labels
@@ -272,11 +271,11 @@
     @jit(nopython=True)
     def _cluster_density_sparseness(MST, labels, cluster):
         indices = np.where(labels == cluster)[0]
         cluster_MST = MST[indices][:, indices]
         cluster_density_sparseness = np.max(cluster_MST)
         return cluster_density_sparseness
 
-# test = DBCVCalculator(clusterers_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/cluster_models_ex',
-#                       config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-# dbcv = test.run()
+test = DBCVCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
+                      config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,141 @@
-import os
-import random
-from simba.enums import Paths
-from simba.read_config_unit_tests import check_file_exist_and_readable
+from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
+                                          check_file_exist_and_readable)
 from simba.misc_tools import SimbaTimer
-
-from simba.unsupervised.misc import (check_that_directory_is_empty,
-                                     check_directory_exists,
-                                     read_pickle,
-                                     write_pickle,
-                                     define_scaler,
-                                     find_low_variance_fields,
-                                     drop_low_variance_fields,
-                                     scaler_transform,
-                                     check_expected_fields)
-
+from simba.unsupervised.misc import (check_directory_exists,
+                                     check_that_directory_is_empty)
+from simba.unsupervised.enums import Clustering, Unsupervised
 import itertools
+import os, glob
+import random
 import pandas as pd
-from datetime import datetime
-import simba
+from simba.utils.printing import stdout_success
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
+from simba.unsupervised.umap_embedder_2 import UmapEmbedder
 try:
-    from cuml import UMAP
+    from cuml.cluster.hdbscan import HDBSCAN
+    from cuml.cluster import hdbscan
     gpu_flag = True
 except ModuleNotFoundError:
-    from umap import UMAP
+    from hdbscan import HDBSCAN
+    import hdbscan
+
 
-class UMAPGridSearch(object):
+class HDBSCANClusterer(UnsupervisedMixin):
     def __init__(self,
                  data_path: str,
                  save_dir: str):
 
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.data_path = data_path
-        self.save_dir = save_dir
-        check_file_exist_and_readable(file_path=self.data_path)
-        check_directory_exists(directory=self.save_dir)
-        check_that_directory_is_empty(directory=self.save_dir)
-        model_names_dir = os.path.join(os.path.dirname(simba.__file__), Paths.UNSUPERVISED_MODEL_NAMES.value)
-        self.model_names = list(pd.read_parquet(model_names_dir)['NAMES'])
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
+        super().__init__()
+        self.save_dir, self.data_path = save_dir, data_path
+        check_directory_exists(directory=save_dir)
+        if os.path.isdir(data_path):
+            check_directory_exists(directory=data_path)
+            self.data_path = glob.glob(data_path + '/*.pickle')
+            check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
 
     def fit(self,
             hyper_parameters: dict):
-        self.hyp, self.low_var_cols = hyper_parameters, []
-        self.search_space = list(itertools.product(*[self.hyp['n_neighbors'],
-                                                     self.hyp['min_distance'],
-                                                     self.hyp['spread']]))
-        self.data = read_pickle(data_path=self.data_path)
-        self.original_feature_names = self.data['DATA'].columns
-        if self.hyp['variance']:
-            self.low_var_cols = find_low_variance_fields(data=self.data['DATA'], variance=self.hyp['variance'])
-            self.data['DATA'] = drop_low_variance_fields(data=self.data['DATA'], fields=self.low_var_cols)
-
-        self.out_feature_names = [x for x in self.original_feature_names if x not in self.low_var_cols]
-        self.scaler = define_scaler(scaler_name=self.hyp['scaler'])
-        self.scaler.fit(self.data['DATA'])
-        self.scaled_data = scaler_transform(data=self.data['DATA'],scaler=self.scaler)
-        self.__fit_umap()
-
-    def __fit_umap(self):
-        self.model_timer = SimbaTimer()
-        self.model_timer.start_timer()
-        self.results = {}
-        self.results['SCALER'] = self.scaler
-        self.results['LOW_VARIANCE_FIELDS'] = self.low_var_cols
-        self.results['ORIGINAL_FEATURE_NAMES'] = self.original_feature_names
-        self.results['OUT_FEATURE_NAMES'] = self.out_feature_names
-        self.results['VIDEO NAMES'] = self.data['VIDEO_NAMES']
-        self.results['START FRAME'] = self.data['START_FRAME']
-        self.results['END FRAME'] = self.data['END_FRAME']
-        self.results['POSE'] = self.data['POSE']
-        self.results['DATA'] = self.scaler
-        self.results['CLASSIFIER'] = self.data['CLF']
-        self.results['CLASSIFIER PROBABILITY'] = self.data['CLF_PROBABILITY']
-
-        for h_cnt, h in enumerate(self.search_space):
-            self.h_cnt = h_cnt
-            self.parameters = {'n_neighbors': h[0],
-                               'min_distance': h[1],
-                               'spread': h[2]}
-            embedder = UMAP(min_dist=self.parameters['min_distance'],
-                            n_neighbors=int(self.parameters['n_neighbors']),
-                            spread=self.parameters['spread'],
-                            metric='euclidean',
-                            verbose=2)
-            embedder.fit(self.scaled_data.values)
-            self.results['PARAMETERS'] = self.parameters
-            self.results['MODEL'] = embedder
-            self.results['TYPE'] = 'UMAP'
-            self.results['HASH'] = random.sample(self.model_names, 1)[0]
-            write_pickle(data=self.results, save_path=os.path.join(self.save_dir, '{}.pickle'.format(self.results['HASH'])))
+
+        check_that_directory_is_empty(directory=self.save_dir)
+        self.search_space = list(itertools.product(*[hyper_parameters[Clustering.ALPHA.value],
+                                                     hyper_parameters[Clustering.MIN_CLUSTER_SIZE.value],
+                                                     hyper_parameters[Clustering.MIN_SAMPLES.value],
+                                                     hyper_parameters[Clustering.EPSILON.value]]))
+        self.embeddings = self.read_pickle(data_path=self.data_path)
+        print(f'Fitting {str(len(self.search_space) * len(self.embeddings.keys()))} HDBSCAN model(s)...')
+        self.__fit_hdbscan()
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: {} umap models saved in {} (elapsed time: {}s)'.format(str(len(self.search_space)), self.save_dir, self.timer.elapsed_time_str))
+        stdout_success(msg=f'{str(len(self.search_space) * len(self.embeddings.keys()))} saved in {self.save_dir}', elapsed_time=self.timer.elapsed_time_str)
+
+    def __fit_hdbscan(self):
+        for k, v in self.embeddings.items():
+            fit_timer = SimbaTimer()
+            fit_timer.start_timer()
+            embedder = v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value]
+            for cnt, h in enumerate(self.search_space):
+                results, self.model, self.model_count = {}, {}, cnt
+                self.model_timer = SimbaTimer()
+                self.model_timer.start_timer()
+                self.model[Unsupervised.HASHED_NAME.value] = random.sample(self.model_names, 1)[0]
+                self.model[Unsupervised.PARAMETERS.value] = {Clustering.ALPHA.value: h[0],
+                                                             Clustering.MIN_CLUSTER_SIZE.value: h[1],
+                                                             Clustering.MIN_SAMPLES.value: h[2],
+                                                             Clustering.EPSILON.value: h[3]}
+                self.model[Unsupervised.MODEL.value] = HDBSCAN(algorithm="best",
+                                                          alpha=self.model[Unsupervised.PARAMETERS.value][Clustering.ALPHA.value],
+                                                          approx_min_span_tree=True,
+                                                          gen_min_span_tree=True,
+                                                          min_cluster_size=self.model[Unsupervised.PARAMETERS.value][Clustering.MIN_CLUSTER_SIZE.value],
+                                                          min_samples=self.model[Unsupervised.PARAMETERS.value][Clustering.MIN_SAMPLES.value],
+                                                          cluster_selection_epsilon=self.model[Unsupervised.PARAMETERS.value][Clustering.EPSILON.value],
+                                                          p=None,
+                                                          prediction_data=True)
+
+                self.model[Unsupervised.MODEL.value].fit(embedder.embedding_)
+                results[Unsupervised.DATA.value] = v[Unsupervised.DATA.value]
+                results[Unsupervised.METHODS.value] = v[Unsupervised.METHODS.value]
+                results[Unsupervised.DR_MODEL.value] = v[Unsupervised.DR_MODEL.value]
+                results[Clustering.CLUSTER_MODEL.value] = self.model
+                self.__save(data=results)
+
+    def __save(self, data: dict) -> None:
+        self.write_pickle(data=data, save_path=os.path.join(self.save_dir, f'{self.model[Unsupervised.HASHED_NAME.value]}.pickle'))
+        self.model_timer.stop_timer()
+        stdout_success(msg=f'Model {self.model_count + 1}/{len(self.search_space)} ({self.model[Unsupervised.HASHED_NAME.value]}) saved...', elapsed_time=self.model_timer.elapsed_time)
 
-def UMAPTransform(model: str or object,
+
+    def transform(self,
                   data_path: str,
-                  settings: dict or None=None,
-                  save_dir: str or None=None):
+                  model: str or dict,
+                  save_dir: str or None=None,
+                  settings: dict or None=None):
 
         timer = SimbaTimer()
         timer.start_timer()
-        if save_dir is not None:
-            check_directory_exists(directory=save_dir)
-        if type(model) == 'str':
+        if isinstance(model, str):
             check_file_exist_and_readable(file_path=model)
-            embedder = read_pickle(data_path=model)
-        else:
-            embedder = model
+            model = self.read_pickle(data_path=model)
+
         check_file_exist_and_readable(file_path=data_path)
-        data = read_pickle(data_path=data_path)
-        data_df = drop_low_variance_fields(data=data['DATA'], fields=embedder['LOW_VARIANCE_FIELDS'])
-        check_expected_fields(data_fields=data_df.columns, expected_fields=embedder['OUT_FEATURE_NAMES'])
-        scaled_data = scaler_transform(data=data_df, scaler=embedder['SCALER'])
-        transformed_data = pd.DataFrame(embedder['MODEL'].transform(scaled_data), columns=['X', 'Y'])
-
-        results = pd.concat([data['VIDEO_NAMES'],
-                             data['START_FRAME'],
-                             data['END_FRAME'],
-                             data['CLF'],
-                             data['CLF_PROBABILITY'],
-                             transformed_data], axis=1)
-        if settings:
-            if settings['features'] == 'INCLUDE: ORIGINAL':
-                results = pd.concat([results, data_df], axis=1)
-            if settings['features'] == 'INCLUDE: SCALED':
-                results = pd.concat([results, scaled_data], axis=1)
-            if settings['save_format'] is 'csv':
-                save_path = os.path.join(save_dir, f'transformed_{embedder["HASH"]}.csv')
-                results.to_csv(save_path, index=False)
-
-        else:
-            return transformed_data
-
-        timer.stop_timer()
-        print('Transformed data saved at {} (elapsed time: {}s)'.format(save_dir, timer.elapsed_time_str))
-
-
-# settings = {'features': 'INCLUDE: SCALED', 'save': 'csv}
-# model_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/funny_heisenberg.pickle'
-# data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230222150701.pickle'
-# save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/'
-# _ = UMAPTransform(model_path=model_path, data_path=data_path, save_dir=save_dir, settings=settings)
-
-#
-#
-#
-#
-#
-# hyper_parameters = {'n_neighbors': [10, 2], 'min_distance': [1.0], 'spread': [1.0], 'scaler': 'MIN-MAX', 'variance': 0.25}
-# data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230222134410.pickle'
-# save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+        umap_embedder = UmapEmbedder()
+        umap_embedder.transform(model=model, data_path=data_path, settings={'DATA': None, 'format': None})
+        self.label, self.strength = hdbscan.approximate_predict(model[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value], umap_embedder.results[['X', 'Y']].values)
+        self.results = pd.DataFrame({'HDBSCAN_LABEL': self.label, 'HDBSCAN_STRENGTH': self.strength}, columns=['HDBSCAN_LABEL', 'HDBSCAN_STRENGTH'], index=umap_embedder.umap_df.index)
+        self.results = pd.concat([umap_embedder.results[['X', 'Y']], self.results], axis=1)
+        if settings[Unsupervised.DATA.value] == Unsupervised.SCALED.value:
+            self.results = pd.concat([umap_embedder.scaled_umap_data, self.results], axis=1)
+        elif settings[Unsupervised.DATA.value] == Unsupervised.RAW.value:
+            self.results = pd.concat([umap_embedder.umap_df, self.results], axis=1)
+        if save_dir:
+            save_path = os.path.join(save_dir, f'Transformed_{model[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}.csv')
+            if settings[Unsupervised.FORMAT.value] is Unsupervised.CSV.value:
+                self.results.to_csv(save_path)
+            timer.stop_timer()
+            print(f'Transformed data saved at {save_dir} (elapsed time: {timer.elapsed_time_str}s)')
+
+# hyper_parameters = {'alpha': [1.0], 'min_cluster_size': [10], 'min_samples': [1], 'cluster_selection_epsilon': [20]}
+# embedding_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+# save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models'
 # config_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini'
-# embedder = UMAPEmbedder(data_path=data_path, save_dir=save_dir)
-# embedder.fit(hyper_parameters=hyper_parameters)
+# clusterer = HDBSCANClusterer(data_path=embedding_dir, save_dir=save_dir)
+# clusterer.fit(hyper_parameters=hyper_parameters)
+
+
+data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
+save_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+clusterer = HDBSCANClusterer(data_path=data_path, save_dir=save_path)
+clusterer.transform(model='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle', settings={'DATA': None}, data_path=data_path)
+
+#settings = {'feature_values': True, 'scaled_features': True, 'save_format': 'csv'}
+# clusterer_model_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/amazing_burnell.pickle'
+# data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230215093552.pickle'
+# save_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+
+# _ = HDBSCANTransform(clusterer_model_path=clusterer_model_path,
+#                      data_path=data_path,
+#                      save_dir=save_path,
+#                      settings=settings)
+
+
+
+
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/dataset_creator_2.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/dataset_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         stdout_success(msg=f'Log for unsupervised learning saved at {self.log_save_path}')
 
     def save(self):
         if len(self.bouts_x_df) == 0:
             raise NoDataError(msg='The data contains zero frames after the chosen slice setting')
         results = {}
         results['DATETIME'] = self.datetime
+        results['AGGREGATION_METHOD'] = self.settings[Unsupervised.BOUT_AGGREGATION_TYPE.value]
+        results['MIN_BOUT'] = self.settings[Unsupervised.MIN_BOUT_LENGTH.value]
         results['FEATURE_NAMES'] = self.feature_names
         results['FRAME_FEATURES'] = self.raw_x_df
         results['FRAME_POSE'] = self.raw_bp_df
         results['FRAME_TARGETS'] = self.raw_y_df
         results['BOUTS_FEATURES'] = self.bouts_x_df
         results['BOUTS_TARGETS'] = self.bouts_y_df
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_statistics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,265 +1,303 @@
-import pandas as pd
-from simba.read_config_unit_tests import (read_config_file,
-                                          read_project_path_and_file_type,
-                                          check_file_exist_and_readable)
-from simba.unsupervised.misc import (read_pickle,
-                                     get_cluster_cnt)
-from sklearn.inspection import permutation_importance
-from simba.misc_tools import SimbaTimer
-import seaborn as sns
-import matplotlib.pyplot as plt
+from simba.mixins.config_reader import ConfigReader
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 import os
-from datetime import datetime
-from scipy.stats import f_oneway
-from statsmodels.stats.multicomp import pairwise_tukeyhsd
 import numpy as np
+import pandas as pd
 from copy import deepcopy
+from simba.unsupervised.enums import Clustering, Unsupervised
+from simba.enums import Methods
+from simba.utils.printing import stdout_success
+from simba.misc_tools import (check_file_exist_and_readable,
+                              SimbaTimer)
+from scipy.stats import f_oneway
+import shap
+from statsmodels.stats.multicomp import pairwise_tukeyhsd
 from statsmodels.stats.libqsturng import psturng
 from sklearn.ensemble import RandomForestClassifier
+from sklearn.inspection import permutation_importance
+import seaborn as sns
+import matplotlib.pyplot as plt
 import itertools
-import warnings
-import shap
-warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
-class ClusterFrequentistCalculator(object):
+FEATURE_NAME = 'FEATURE NAME'
+FEATURE_IMPORTANCE = 'IMPORTANCE'
+F_STATISTIC = 'F-STATISTIC'
+MEASURE = 'MEASURE'
+P_VALUE = 'P-VALUE'
+CLUSTER = 'CLUSTER'
+PAIRED = 'cluster_paired'
+CORRELATION_METHODS = 'correlation_methods'
+GINI_IMPORTANCE = 'gini_importance'
+TUKEY = 'tukey_posthoc'
+METHOD = 'method'
+TARGET = 'TARGET'
+PEARSON = 'pearson'
+KENDALL = 'kendall'
+SHAP = 'shap'
+PLOTS = 'plots'
+CREATE = 'create'
+SPEARMAN = 'spearman'
+MEAN = 'MEAN'
+STDEV = 'STANDARD DEVIATION'
+PERMUTATION_IMPORTANCE = 'permutation_importance'
+DESCRIPTIVE_STATISTICS = 'descriptive_statistics'
+ANOVA_HEADERS = ['FEATURE NAME', 'F-STATISTIC', 'P-VALUE']
+
+
+class ClusterFrequentistCalculator(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  config_path: str,
                  data_path: str,
                  settings: dict):
 
-        self.config = read_config_file(ini_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
         self.settings = settings
-        self.project_path, _ = read_project_path_and_file_type(config=self.config)
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.save_path = os.path.join(self.project_path, 'logs', f'cluster_descriptive_statistics_{self.datetime}.xlsx')
         check_file_exist_and_readable(file_path=data_path)
-        self.data = read_pickle(data_path=data_path)
-        self.feature_data = self.data['EMBEDDER']['MODEL']._raw_data
-        if not settings['scaled']:
-            self.feature_data = self.data['EMBEDDER']['SCALER'].inverse_transform(self.feature_data)
-        self.feature_data = pd.DataFrame(data=self.feature_data, columns=self.data['EMBEDDER']['OUT_FEATURE_NAMES'])
-        self.cluster_data = self.data['MODEL'].labels_
-        _ = get_cluster_cnt(data=self.cluster_data, clusterer_name=self.data['NAME'], minimum_clusters=2)
-        self.feature_data['CLUSTER'] = self.cluster_data
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
+        self.data = self.read_pickle(data_path=data_path)
+        self.save_path = os.path.join(self.logs_path, f'cluster_descriptive_statistics_{self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.xlsx')
+        self.check_key_exist_in_object(object=self.data, key=Clustering.CLUSTER_MODEL.value)
+
 
+    def run(self):
+        self.x_data = self.data[Unsupervised.METHODS.value][Unsupervised.SCALED_DATA.value]
+        self.cluster_data = self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
+        if not settings[Unsupervised.SCALED.value]:
+            self.feature_data = self.scaler_inverse_transform(scaler=self.data[Unsupervised.METHODS.value][Unsupervised.SCALER.value], data=self.x_data)
+        self.x_y_df = pd.concat([self.x_data, pd.DataFrame(self.cluster_data, columns=[CLUSTER], index=self.x_data.index)], axis=1)
+        self.cluster_cnt = self.get_cluster_cnt(data=self.cluster_data, clusterer_name=self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value], minimum_clusters=2)
         with pd.ExcelWriter(self.save_path, mode='w') as writer:
             pd.DataFrame().to_excel(writer, sheet_name=' ', index=True)
+        if self.settings[Methods.ANOVA.value]:
+            self.__one_way_anovas()
+        if self.settings[DESCRIPTIVE_STATISTICS]:
+            self.__descriptive_stats()
+        if self.settings[TUKEY]:
+            self.__tukey_posthoc()
+        self.timer.stop_timer()
+        stdout_success(msg=f'Cluster statistics complete. Data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
+
+    def __save_results(self, df: pd.DataFrame, name: str):
+        with pd.ExcelWriter(self.save_path, mode='a') as writer:
+            df.to_excel(writer, sheet_name=name, index=True)
 
     def __one_way_anovas(self):
         print('Calculating ANOVAs...')
-        self.anova_results = pd.DataFrame(columns=['FEATURE NAME', 'F-STATISTIC', 'P-VALUE'])
-        for feature_name in self.data['EMBEDDER']['OUT_FEATURE_NAMES']:
-            stats_data = self.feature_data[[feature_name, 'CLUSTER']].sort_values(by=['CLUSTER']).values
+        timer = SimbaTimer(start=True)
+        self.anova_results = pd.DataFrame(columns=ANOVA_HEADERS)
+        for feature_name in self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value]:
+            stats_data = self.x_y_df[[feature_name, 'CLUSTER']].sort_values(by=['CLUSTER']).values
             stats_data = np.split(stats_data[:, 0], np.unique(stats_data[:, 1], return_index=True)[1][1:])
             f_val, p_val = f_oneway(*stats_data)
             self.anova_results.loc[len(self.anova_results)] = [feature_name, f_val, p_val]
-        self.anova_results = self.anova_results.sort_values(by=['P-VALUE']).set_index('FEATURE NAME')
-        self.anova_results['P-VALUE'] = self.anova_results['P-VALUE'].round(5)
-        self.__save_results(df=self.anova_results, name='ANOVA')
+        self.anova_results = self.anova_results.sort_values(by=[P_VALUE]).set_index(FEATURE_NAME)
+        self.anova_results[P_VALUE] = self.anova_results[P_VALUE].round(5)
+        self.__save_results(df=self.anova_results, name=Methods.ANOVA.value)
+        timer.stop_timer()
+        stdout_success(msg=f'ANOVAs saved in {self.save_path}', elapsed_time=timer.elapsed_time_str)
+
 
     def __descriptive_stats(self):
         print('Calculating descriptive statistics..')
+        timer = SimbaTimer(start=True)
         self.descriptive_results = []
-        for feature_name in self.data['EMBEDDER']['OUT_FEATURE_NAMES']:
-            agg = self.feature_data.groupby(['CLUSTER'])[feature_name].agg(['mean','std', 'sem']).T
-            agg['FEATURE_NAME'] = feature_name
-            agg = agg.reset_index(drop=False).set_index('FEATURE_NAME').rename(columns={'index': 'MEASSURE'})
+        for feature_name in self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value]:
+            agg = self.x_y_df.groupby([CLUSTER])[feature_name].agg(['mean','std', 'sem']).T
+            agg[FEATURE_NAME] = feature_name
+            agg = agg.reset_index(drop=False).set_index(FEATURE_NAME).rename(columns={'index': MEASURE})
             self.descriptive_results.append(pd.DataFrame(agg))
         self.descriptive_results = pd.concat(self.descriptive_results, axis=0)
-        self.__save_results(df=self.descriptive_results, name='DESCRIPTIVE STATISTICS')
+        self.__save_results(df=self.descriptive_results, name=DESCRIPTIVE_STATISTICS)
+        timer.stop_timer()
+        stdout_success(msg=f'Descriptive statistics saved in {self.save_path}', elapsed_time=timer.elapsed_time_str)
 
     def __tukey_posthoc(self):
         print('Calculating tukey posthocs...')
+        timer = SimbaTimer(start=True)
         self.post_hoc_results = []
-        for feature_name in self.data['EMBEDDER']['OUT_FEATURE_NAMES']:
-            data = pairwise_tukeyhsd(self.feature_data[feature_name], self.feature_data['CLUSTER'])
+        for feature_name in self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value]:
+            data = pairwise_tukeyhsd(self.x_y_df[feature_name], self.x_y_df[CLUSTER])
             df = pd.DataFrame(data=data._results_table.data[1:], columns=data._results_table.data[0])
-            df['P-VALUE'] = psturng(np.abs(data.meandiffs / data.std_pairs), len(data.groupsunique), data.df_total)
-            df['FEATURE_NAME'] = feature_name
-            df = df.reset_index(drop=True).set_index('FEATURE_NAME')
+            df[P_VALUE] = psturng(np.abs(data.meandiffs / data.std_pairs), len(data.groupsunique), data.df_total)
+            df[FEATURE_NAME] = feature_name
+            df = df.reset_index(drop=True).set_index(FEATURE_NAME)
             self.post_hoc_results.append(df)
         self.post_hoc_results = pd.concat(self.post_hoc_results, axis=0)
-        self.__save_results(df=self.post_hoc_results, name='TUKEY POST-HOC')
+        self.__save_results(df=self.post_hoc_results, name=TUKEY)
+        timer.stop_timer()
+        stdout_success(msg=f"Tukey post-hocs' statistics saved in {self.save_path}", elapsed_time=timer.elapsed_time_str)
 
-    def __save_results(self, df: pd.DataFrame, name: str):
-        with pd.ExcelWriter(self.save_path, mode='a') as writer:
-            df.to_excel(writer, sheet_name=name, index=True)
+class EmbeddingCorrelationCalculator(UnsupervisedMixin, ConfigReader):
+    def __init__(self,
+                 data_path: str,
+                 config_path: str,
+                 settings: dict):
+
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
+        check_file_exist_and_readable(file_path=data_path)
+        self.settings, self.data_path = settings, data_path
+        self.data = self.read_pickle(data_path=self.data_path)
+        self.save_path = os.path.join(self.logs_path, f'embedding_correlations_{self.data[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.csv')
 
     def run(self):
-        if self.settings['descriptive_statistics']:
-            self.__descriptive_stats()
-        if self.settings['anova']:
-            self.__one_way_anovas()
-        if self.settings['tukey_posthoc']:
-            self.__tukey_posthoc()
+        print('Calculating embedding correlations...')
+        self.x_df = self.data[Unsupervised.METHODS.value][Unsupervised.SCALED_DATA.value]
+        self.y_df = pd.DataFrame(self.data[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'], index=self.x_df.index)
+        results = pd.DataFrame()
+        for correlation_method in self.settings[CORRELATION_METHODS]:
+            results[f'{correlation_method}_Y'] = self.x_df.corrwith(self.y_df['Y'], method=correlation_method)
+            results[f'{correlation_method}_X'] = self.x_df.corrwith(self.y_df['X'], method=correlation_method)
+        results.to_csv(self.save_path)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Cluster statistics complete. Data saved at {self.save_path} (elapsed time: {self.timer.elapsed_time_str}s)')
+        stdout_success(msg=f'Embedding correlations saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-class ClusterXAICalculator(object):
+        if self.settings[PLOTS][CREATE]:
+            print('Creating embedding correlation plots...')
+            df = pd.concat([self.x_df, self.y_df], axis=1)
+            save_dir = os.path.join(self.logs_path, 'embedding_correlation_plots')
+            if not os.path.exists(save_dir): os.makedirs(save_dir)
+            for feature_cnt, feature_name in enumerate(self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value]):
+                color_bar = plt.cm.ScalarMappable(cmap=self.settings[PLOTS]['palette'])
+                color_bar.set_array([])
+                plot = sns.scatterplot(data=df, x="X", y="Y", hue=feature_name, cmap=self.settings[PLOTS]['palette'])
+                plot.get_legend().remove()
+                plot.figure.colorbar(color_bar, label=feature)
+                plt.suptitle(feature_name, x=0.5, y=0.92)
+                save_path = os.path.join(save_dir, f'{feature_name}.png')
+                plot.figure.savefig(save_path, bbox_inches="tight")
+                plot.clear()
+                plt.close()
+                print(f'Saving image {str(feature_cnt+1)}/{str(len(df.columns))} ({feature_name})')
+        stdout_success(msg=f'Embedding correlation calculations complete')
+
+
+
+class ClusterXAICalculator(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  data_path: str,
                  config_path: str,
                  settings: dict):
 
-        self.config = read_config_file(ini_path=config_path)
-        self.settings = settings
-        self.project_path, _ = read_project_path_and_file_type(config=self.config)
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.save_path = os.path.join(self.project_path, 'logs', f'cluster_xai_statistics_{self.datetime}.xlsx')
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
+        self.settings, self.data_path = settings, data_path
         check_file_exist_and_readable(file_path=data_path)
-        self.data = read_pickle(data_path=data_path)
-        self.feature_data = self.data['EMBEDDER']['MODEL']._raw_data
-        self.feature_data = pd.DataFrame(data=self.feature_data, columns=self.data['EMBEDDER']['OUT_FEATURE_NAMES'])
-        self.cluster_data = self.data['MODEL'].labels_
-        _ = get_cluster_cnt(data=self.cluster_data, clusterer_name=self.data['NAME'], minimum_clusters=2)
-        self.feature_data['CLUSTER'] = self.cluster_data
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
+        self.data = self.read_pickle(data_path=self.data_path)
+        self.save_path = os.path.join(self.logs_path, f'cluster_xai_statistics_{self.data[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.xlsx')
 
+    def run(self):
+        self.x_df = self.data[Unsupervised.METHODS.value][Unsupervised.SCALED_DATA.value]
+        self.cluster_data = self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
+        self.x_y_df = pd.concat([self.x_df, pd.DataFrame(self.cluster_data, columns=[CLUSTER], index=self.x_df.index)], axis=1)
+        self.cluster_cnt = self.get_cluster_cnt(data=self.cluster_data, clusterer_name=self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value], minimum_clusters=2)
         with pd.ExcelWriter(self.save_path, mode='w') as writer:
             pd.DataFrame().to_excel(writer, sheet_name=' ', index=True)
+        self.__train_rf_models()
+        print(self.settings[GINI_IMPORTANCE])
+        if self.settings[GINI_IMPORTANCE]:
+            self.__gini_importance()
+        if self.settings[PERMUTATION_IMPORTANCE]:
+            self.__permutation_importance()
+        if self.settings[SHAP][CREATE]:
+            self.__shap_values()
+        self.timer.stop_timer()
+        stdout_success(msg=f'Cluster XAI complete. Data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
+
+
+    def __save_results(self, df: pd.DataFrame, name: str):
+        with pd.ExcelWriter(self.save_path, mode='a') as writer:
+            df.to_excel(writer, sheet_name=name, index=True)
 
     def __train_rf_models(self):
         print('Training ML model...')
         rf_clf = RandomForestClassifier(n_estimators=100,
                                         max_features='sqrt',
                                         n_jobs=-1, criterion='gini',
                                         min_samples_leaf=1,
                                         bootstrap=True,
                                         verbose=1)
         self.rf_data = {}
-        for cluster_id in self.feature_data['CLUSTER'].unique():
+        for clf_cnt, cluster_id in enumerate(self.x_y_df[CLUSTER].unique()):
+            print(f'Training model {clf_cnt+1}/{self.cluster_cnt}')
             self.rf_data[cluster_id] = {}
-            target_df = self.feature_data[self.feature_data['CLUSTER'] == cluster_id].drop(['CLUSTER'], axis=1)
-            nontarget_df = self.feature_data[self.feature_data['CLUSTER'] != cluster_id].drop(['CLUSTER'], axis=1)
-            target_df['TARGET'] = 1
-            nontarget_df['TARGET'] = 0
-            self.rf_data[cluster_id]['X'] = pd.concat([target_df, nontarget_df], axis=0).reset_index(drop=True).sample(frac=1)
-            self.rf_data[cluster_id]['Y'] = self.rf_data[cluster_id]['X'].pop('TARGET')
+            target_df = self.x_y_df[self.x_y_df[CLUSTER] == cluster_id].drop([CLUSTER], axis=1)
+            non_target_df = self.x_y_df[self.x_y_df[CLUSTER] != cluster_id].drop([CLUSTER], axis=1)
+            target_df[TARGET] = 1
+            non_target_df[TARGET] = 0
+            self.rf_data[cluster_id]['X'] = pd.concat([target_df, non_target_df], axis=0).reset_index(drop=True).sample(frac=1)
+            self.rf_data[cluster_id]['Y'] = self.rf_data[cluster_id]['X'].pop(TARGET)
             rf_clf.fit(self.rf_data[cluster_id]['X'], self.rf_data[cluster_id]['Y'])
-            self.rf_data[cluster_id]['MODEL'] = deepcopy(rf_clf)
-
+            self.rf_data[cluster_id][Unsupervised.MODEL.value] = deepcopy(rf_clf)
 
     def __gini_importance(self):
-        print('Calculating cluster gini...')
+        print("Calculating cluster gini importances'...")
+        timer = SimbaTimer(start=True)
         for cluster_id, cluster_data in self.rf_data.items():
-            importances = list(cluster_data['MODEL'].feature_importances_)
-            gini_data = [(feature, round(importance, 6)) for feature, importance in zip(self.data['EMBEDDER']['OUT_FEATURE_NAMES'], importances)]
-            df = pd.DataFrame(gini_data, columns=['FEATURE', 'FEATURE_IMPORTANCE']).sort_values(by=['FEATURE_IMPORTANCE'], ascending=False).reset_index(drop=True)
+            importances = list(cluster_data[Unsupervised.MODEL.value].feature_importances_)
+            gini_data = [(feature, round(importance, 6)) for feature, importance in zip(self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value], importances)]
+            df = pd.DataFrame(gini_data, columns=[FEATURE_NAME, FEATURE_IMPORTANCE]).sort_values(by=[FEATURE_IMPORTANCE], ascending=False).reset_index(drop=True)
             self.__save_results(df=df, name=f'GINI CLUSTER {str(cluster_id)}')
+        timer.stop_timer()
+        stdout_success(msg=f"Cluster features gini importances' complete", elapsed_time=timer.elapsed_time_str)
 
     def __permutation_importance(self):
         print('Calculating permutation importance...')
+        timer = SimbaTimer(start=True)
         for cluster_id, cluster_data in self.rf_data.items():
-            p_importances = permutation_importance(cluster_data['MODEL'], cluster_data['X'], cluster_data['Y'], n_repeats=5, random_state=0)
-            df = pd.DataFrame(np.column_stack([self.data['EMBEDDER']['OUT_FEATURE_NAMES'], p_importances.importances_mean, p_importances.importances_std]), columns=['FEATURE_NAME', 'FEATURE_IMPORTANCE_MEAN', 'FEATURE_IMPORTANCE_STDEV'])
-            df = df.sort_values(by=['FEATURE_IMPORTANCE_MEAN'], ascending=False).reset_index(drop=True)
+            p_importances = permutation_importance(cluster_data[Unsupervised.MODEL.value], cluster_data['X'], cluster_data['Y'], n_repeats=5, random_state=0)
+            df = pd.DataFrame(np.column_stack([self.data[Unsupervised.METHODS.value][Unsupervised.FEATURE_NAMES.value], p_importances.importances_mean, p_importances.importances_std]), columns=[FEATURE_NAME, MEAN, STDEV])
+            df = df.sort_values(by=[MEAN], ascending=False).reset_index(drop=True)
             self.__save_results(df=df, name=f'PERMUTATION CLUSTER {str(cluster_id)}')
-
-    def __save_results(self, df: pd.DataFrame, name: str):
-        with pd.ExcelWriter(self.save_path, mode='a') as writer:
-            df.to_excel(writer, sheet_name=name, index=True)
+        timer.stop_timer()
+        stdout_success(msg=f"Cluster features permutation importances' complete", elapsed_time=timer.elapsed_time_str)
 
     def __shap_values(self):
-        if self.settings['shap']['run']:
-            if self.settings['shap']['method'] == 'Paired clusters':
-                cluster_combinations = list(itertools.combinations(list(self.rf_data.keys()), 2))
-                for (cluster_one_id, cluster_two_id) in cluster_combinations:
-                    explainer = shap.TreeExplainer(self.rf_data[cluster_one_id]['MODEL'], data=None, model_output='raw', feature_perturbation='tree_path_dependent')
-                    if self.settings['shap']['sample'] > (len(self.rf_data[cluster_one_id]['X']) or len(self.rf_data[cluster_two_id]['X'])):
-                        self.settings['shap']['sample'] = min(len(self.rf_data[cluster_one_id]['X']), len(self.rf_data[cluster_two_id]['X']))
-                    cluster_one_sample = self.rf_data[cluster_one_id]['X'].sample(self.settings['shap']['sample'], replace=False)
-                    cluster_two_sample = self.rf_data[cluster_two_id]['X'].sample(self.settings['shap']['sample'], replace=False)
-                    cluster_one_shap = pd.DataFrame(explainer.shap_values(cluster_one_sample, check_additivity=False)[1], columns=self.rf_data[cluster_one_id]['X'].columns)
-                    cluster_two_shap = pd.DataFrame(explainer.shap_values(cluster_two_sample, check_additivity=False)[1], columns=self.rf_data[cluster_two_id]['X'].columns)
-                    mean_df_cluster_one, stdev_df_cluster_one = pd.DataFrame(cluster_one_shap.mean(), columns=['MEAN']), pd.DataFrame(cluster_one_shap.std(), columns=['STDEV'])
-                    mean_df_cluster_two, stdev_df_cluster_two = pd.DataFrame(cluster_two_shap.mean(), columns=['MEAN']), pd.DataFrame(cluster_two_shap.std(), columns=['STDEV'])
-                    results_cluster_one = mean_df_cluster_one.join(stdev_df_cluster_one).sort_values(by='MEAN', ascending=False)
-                    results_cluster_two = mean_df_cluster_two.join(stdev_df_cluster_two).sort_values(by='MEAN', ascending=False)
-                    self.__save_results(df=results_cluster_one, name=f'SHAP CLUSTER {str(cluster_one_id)} vs. {str(cluster_two_id)}')
-                    self.__save_results(df=results_cluster_two, name=f'SHAP CLUSTER {str(cluster_two_id)} vs. {str(cluster_one_id)}')
+        if self.settings[SHAP][METHOD] == PAIRED:
+            print('Calculating paired-clusters shap values ...')
+            timer = SimbaTimer(start=True)
+            cluster_combinations = list(itertools.combinations(list(self.rf_data.keys()), 2))
+            for (cluster_one_id, cluster_two_id) in cluster_combinations:
+                explainer = shap.TreeExplainer(self.rf_data[cluster_one_id]['MODEL'], data=None, model_output='raw', feature_perturbation='tree_path_dependent')
+                if self.settings['shap']['sample'] > (len(self.rf_data[cluster_one_id]['X']) or len(self.rf_data[cluster_two_id]['X'])):
+                    self.settings['shap']['sample'] = min(len(self.rf_data[cluster_one_id]['X']), len(self.rf_data[cluster_two_id]['X']))
+                cluster_one_sample = self.rf_data[cluster_one_id]['X'].sample(self.settings['shap']['sample'], replace=False)
+                cluster_two_sample = self.rf_data[cluster_two_id]['X'].sample(self.settings['shap']['sample'], replace=False)
+                cluster_one_shap = pd.DataFrame(explainer.shap_values(cluster_one_sample, check_additivity=False)[1], columns=self.rf_data[cluster_one_id]['X'].columns)
+                cluster_two_shap = pd.DataFrame(explainer.shap_values(cluster_two_sample, check_additivity=False)[1], columns=self.rf_data[cluster_two_id]['X'].columns)
+                mean_df_cluster_one, stdev_df_cluster_one = pd.DataFrame(cluster_one_shap.mean(), columns=['MEAN']), pd.DataFrame(cluster_one_shap.std(), columns=['STDEV'])
+                mean_df_cluster_two, stdev_df_cluster_two = pd.DataFrame(cluster_two_shap.mean(), columns=['MEAN']), pd.DataFrame(cluster_two_shap.std(), columns=['STDEV'])
+                results_cluster_one = mean_df_cluster_one.join(stdev_df_cluster_one).sort_values(by='MEAN', ascending=False)
+                results_cluster_two = mean_df_cluster_two.join(stdev_df_cluster_two).sort_values(by='MEAN', ascending=False)
+                self.__save_results(df=results_cluster_one, name=f'SHAP CLUSTER {str(cluster_one_id)} vs. {str(cluster_two_id)}')
+                self.__save_results(df=results_cluster_two, name=f'SHAP CLUSTER {str(cluster_two_id)} vs. {str(cluster_one_id)}')
+            timer.stop_timer()
+            stdout_success(msg=f"Paired clusters SHAP values complete", elapsed_time=timer.elapsed_time_str)
+
+
+settings = {'gini_importance': True, 'permutation_importance': True, 'shap': {'method': 'cluster_paired', 'create': True, 'sample': 100}}
+test = ClusterXAICalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
+                            data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
+                            settings=settings)
+test.run()
 
-    def run(self):
-        self.__train_rf_models()
-        if self.settings['gini_importance']:
-            self.__gini_importance()
-        if self.settings['permutation_importance']:
-            self.__permutation_importance()
-        if self.settings['shap']:
-            self.__shap_values()
-        self.timer.stop_timer()
-        print(f'XAI statistics saved (elapsed time {self.timer.elapsed_time_str}s)')
 
-class EmbeddingCorrelationCalculator(object):
-    def __init__(self,
-                 data_path: str,
-                 config_path: str,
-                 settings: dict):
-
-        check_file_exist_and_readable(file_path=data_path)
-        config = read_config_file(ini_path=config_path)
-        self.project_path, _ = read_project_path_and_file_type(config=config)
-        self.logs_path = os.path.join(self.project_path, 'logs')
-        data = read_pickle(data_path=data_path)
-        results = pd.DataFrame()
-        if data['MODEL'].__class__.__name__ is 'UMAP':
-            df = pd.DataFrame(data['MODEL']._raw_data, columns=data['OUT_FEATURE_NAMES'])
-            embedder_name = data['HASH']
-            embedding = df.join(pd.DataFrame(data['MODEL'].embedding_, columns=['X', 'Y']))
-        elif data['MODEL'].__class__.__name__ is 'HDBSCAN':
-            df = pd.DataFrame(data['EMBEDDER']['MODEL']._raw_data, columns=data['OUT_FEATURE_NAMES'])
-            embedder_name = data['EMBEDDER']['HASH']
-            embedding = df.join(pd.DataFrame(data['EMBEDDER']['MODEL'].embedding_, columns=['X', 'Y']))
-        for method in settings['correlations']:
-            results[f'{method}_Y'] = df.corrwith(embedding['Y'], method=method)
-            results[f'{method}_X'] = df.corrwith(embedding['X'], method=method)
-        save_path = os.path.join(self.logs_path, embedder_name + '_embedding_stats.csv')
-        results.to_csv(save_path)
-
-        if settings['plots']['create']:
-            plots_dir = os.path.join(self.logs_path, 'embedding_correlations')
-            if not os.path.exists(plots_dir): os.makedirs(plots_dir)
-            for feature_cnt, feature in enumerate(df.columns):
-                color_bar = plt.cm.ScalarMappable(cmap=settings['plots']['palette'])
-                color_bar.set_array([])
-                plot = sns.scatterplot(data=embedding, x="X", y="Y", hue=feature, cmap=settings['plots']['palette'])
-                plot.get_legend().remove()
-                plot.figure.colorbar(color_bar, label=feature)
-                plt.suptitle(feature, x=0.5, y=0.92)
-                save_path = os.path.join(plots_dir, feature + '.png')
-                plot.figure.savefig(save_path, bbox_inches="tight")
-                plot.clear()
-                plt.close()
-                print(f'Saving image {str(feature_cnt+1)}/{str(len(df.columns))} ({feature})')
 
-        print(f'SIMBA COMPLETE: Data saved at {save_path}')
 
-# settings = {'correlations': ['pearson', 'kendall', 'spearman'], 'plots': {'create': True, 'correlations': 'pearson', 'palette': 'jet'}}
-# _ = EmbeddingCorrelationCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/funny_heisenberg.pickle',
+# settings = {'correlation_methods': ['pearson', 'kendall', 'spearman'], 'plots': {'create': True, 'correlations': 'pearson', 'palette': 'jet'}}
+# test = EmbeddingCorrelationCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
 #                                    config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
 #                                    settings=settings)
-
-
-
-
-# settings = {'gini_importance': False, 'permutation_importance': False, 'shap': {'method': 'cluster-wise', 'run': True, 'sample': 100}}
-# test = ClusterXAICalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
-#                             data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/amazing_burnell.pickle',
-#                             settings=settings)
 # test.run()
 
 
-
-
-# settings = {'scaled': True, 'anova': True, 'tukey_posthoc': True, 'descriptive_statistics': True}
+# settings = {'scaled': True, 'ANOVA': True, 'tukey_posthoc': True, 'descriptive_statistics': True}
 # test = ClusterFrequentistCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
-#                                    data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/nostalgic_albattani.pickle',
+#                                    data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
 #                                    settings=settings)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_visualizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,102 @@
-from simba.misc_tools import check_file_exist_and_readable, get_video_meta_data, find_all_videos_in_directory, check_multi_animal_status
-from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, createColorListofList
-from simba.unsupervised.misc import read_pickle
-from simba.read_config_unit_tests import read_config_file, read_config_entry, read_project_path_and_file_type
-from simba.enums import Paths, Formats, ReadConfig, Dtypes
+from simba.misc_tools import (check_file_exist_and_readable,
+                              find_all_videos_in_directory,
+                              get_video_meta_data)
+from simba.enums import Paths, Formats
+from simba.mixins.config_reader import ConfigReader
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
+from simba.unsupervised.enums import Clustering, Unsupervised
+from simba.utils.printing import stdout_success
+import pandas as pd
+import numpy as np
 import os
-import warnings
+from simba.utils.warnings import NoFileFoundWarning
 import cv2
 
-class ClusterVisualizer(object):
+CLUSTER = 'CLUSTER'
+FPS = 'fps'
+VIDEO_SPEED = 'video_speed'
+START_FRAME = 'START_FRAME'
+POSE = 'pose'
+CREATE = 'create'
+CIRCLE_SIZE = 'circle_size'
+
+
+class ClusterVisualizer(ConfigReader, UnsupervisedMixin):
     def __init__(self,
                  config_path: str,
                  video_dir: str,
                  data_path: str,
                  settings: dict):
 
-        self.config, self.settings = read_config_file(ini_path=config_path), settings
-        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
+        self.settings, self.video_dir, self.data_path = settings, video_dir, data_path
         self.save_parent_dir = os.path.join(self.project_path, Paths.CLUSTER_EXAMPLES.value)
         if not os.path.exists(self.save_parent_dir): os.makedirs(self.save_parent_dir)
         check_file_exist_and_readable(file_path=data_path)
-        self.x_cols, self.y_cols, self.pcols = getBpNames(config_path)
-        self.no_animals = read_config_entry(self.config, ReadConfig.GENERAL_SETTINGS.value, ReadConfig.ANIMAL_CNT.value, Dtypes.INT.value)
-        self.pose_colors = createColorListofList(self.no_animals, int(len(self.x_cols) + 1))
-        self.multi_animal_status, self.multi_animal_id_lst = check_multi_animal_status(self.config, self.no_animals)
-        self.animal_bp_dict = create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_lst, self.no_animals, self.x_cols, self.y_cols, [], self.pose_colors)
         self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
         self.video_files = find_all_videos_in_directory(directory=video_dir, as_dict=True)
-        self.data = read_pickle(data_path=data_path)
-        self.video_dir, self.pose_df = video_dir, None
-        self.cluster_ids = self.data['DATA']['CLUSTER'].unique()
 
-    def create(self):
-        for cluster_id in self.cluster_ids:
+    def run(self):
+        self.video_counter = 0
+        self.data = self.read_pickle(data_path=self.data_path)
+        self.cluster_data = self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
+        self.x_df = self.data[Unsupervised.METHODS.value][Unsupervised.SCALED_DATA.value].reset_index()
+        self.x_y_df = pd.concat([self.x_df, pd.DataFrame(self.cluster_data, columns=[CLUSTER])], axis=1)
+        self.bout_cnt = len(self.data[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value])
+        for cluster_id in np.unique(self.cluster_data):
             self.cluster_id = cluster_id
-            cluster_df = self.data['DATA'][self.data['DATA']['CLUSTER'] == cluster_id]
-            for video_name in cluster_df['VIDEO'].unique():
+            for video_name in self.data[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value][Unsupervised.VIDEO.value].unique():
                 self.video_name = video_name
                 if video_name not in self.video_files.keys():
-                    warnings.warn(f'SIMBA WARNING: Video {video_name} not found in video directory {self.video_dir}')
+                    NoFileFoundWarning(msg=f'Video {video_name} not found in video directory {self.video_dir}')
                     continue
                 else:
-                    self.cluster_video_df = cluster_df[cluster_df['VIDEO'] == video_name]
-                    self.__cluster_video_creator()
+                    self.cluster_video_df = self.x_y_df.loc[(self.x_y_df[Unsupervised.VIDEO.value] == video_name) & (self.x_y_df[CLUSTER] == cluster_id)]
+                    if len(self.cluster_video_df) > 0:
+                        self.__create_videos()
+        self.timer.stop_timer()
+        stdout_success(msg=f'Visualizations complete. Data saved at {self.save_parent_dir}', elapsed_time=self.timer.elapsed_time_str)
 
 
-    def __cluster_video_creator(self):
+    def __create_videos(self):
         self.save_directory = os.path.join(self.save_parent_dir, str(self.cluster_id), self.video_name)
-        if self.settings['pose']['include']:
-            self.pose_df = self.data['POSE'][self.data['POSE']['VIDEO'] == self.video_name].drop(['FRAME', 'VIDEO'], axis=1).reset_index(drop=True)
         if not os.path.exists(self.save_directory): os.makedirs(self.save_directory)
-        video_meta_data = get_video_meta_data(video_path=self.video_files[self.cluster_video_df['VIDEO'].values[0]])
-        output_fps = int(video_meta_data['fps'] * self.settings['video_speed'])
-        if output_fps < 1: output_fps = 1
-        cluster_frames = list(self.cluster_video_df.apply(lambda x: list(range(int(x['START_FRAME']), int(x['END_FRAME']) + 1)), 1))
+        video_meta_data = get_video_meta_data(video_path=self.video_files[self.cluster_video_df[Unsupervised.VIDEO.value].values[0]])
+        output_fps = max(1, int(video_meta_data[FPS] * self.settings[VIDEO_SPEED]))
         cap = cv2.VideoCapture(self.video_files[self.cluster_video_df['VIDEO'].values[0]])
+        cluster_frames = list(self.cluster_video_df.apply(lambda x: list(range(int(x[Unsupervised.START_FRAME.value]), int(x[Unsupervised.END_FRAME.value]) + 1)), 1))
         for cluster_event_cnt, cluster_event in enumerate(cluster_frames):
-            file_name = os.path.join(self.save_directory, f'Event_{str(cluster_event_cnt)}.mp4')
-            self.writer = cv2.VideoWriter(file_name, self.fourcc, output_fps, (video_meta_data['width'], video_meta_data['height']))
+            save_path = os.path.join(self.save_directory, f'Event_{str(cluster_event_cnt)}.mp4')
+            self.writer = cv2.VideoWriter(save_path, self.fourcc, output_fps, (video_meta_data['width'], video_meta_data['height']))
             start_frm, end_frm, current_frm = cluster_event[0], cluster_event[-1], cluster_event[0]
             cluster_event_frms = end_frm-start_frm
             cap.set(1, cluster_event[0])
             frame_cnt = 0
             while current_frm < end_frm:
                 _, img = cap.read()
-                if self.settings['pose']['include']:
-                    bp_data = self.pose_df.iloc[current_frm]
-                    for cnt, (animal_name, animal_bps) in enumerate(self.animal_bp_dict.items()):
-                        for bp in zip(animal_bps['X_bps'], animal_bps['Y_bps']):
+                if self.settings[POSE][CREATE]:
+                    bp_data = self.data[Unsupervised.DATA.value]['FRAME_POSE'].iloc[current_frm]
+                    for animal_cnt, (animal_name, animal_bps) in enumerate(self.animal_bp_dict.items()):
+                        for bp_cnt, bp in enumerate(zip(animal_bps['X_bps'], animal_bps['Y_bps'])):
                             x_bp, y_bp = bp_data[bp[0]], bp_data[bp[1]]
-                            cv2.circle(img, (int(x_bp), int(y_bp)), self.settings['pose']['circle_size'], self.animal_bp_dict[animal_name]['colors'][cnt], -1)
+                            cv2.circle(img, (int(x_bp), int(y_bp)), self.settings[POSE][CIRCLE_SIZE], self.clr_lst[animal_cnt][bp_cnt], -1)
                 self.writer.write(img)
-                print(f'Writing frame {str(frame_cnt)}/{str(cluster_event_frms)}, Bout {str(cluster_event_cnt+1)}/{len(cluster_frames)}, '
-                      f'Cluster: {self.cluster_id}, Video: {self.video_name}...')
+                print(f'Writing frame {str(frame_cnt)}/{str(cluster_event_frms)}, '
+                      f'Bout {str(cluster_event_cnt+1)}/{len(cluster_frames)}, '
+                      f''f'Cluster: {self.cluster_id}, '
+                      f'Video: {self.video_name}, '
+                      f'Total bout count: {self.video_counter}/{self.bout_cnt}...')
                 current_frm += 1
                 frame_cnt += 1
             cap.release()
             self.writer.release()
+            self.video_counter += 1
 
 
-
-
-# settings = {'video_speed': 0.01, 'pose': {'include': True, 'circle_size': 5}}
+# settings = {'video_speed': 0.5, 'pose': {'create': True, 'circle_size': 5}}
 # test = ClusterVisualizer(video_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/videos',
-#                          data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/dreamy_spence_awesome_elion.pickle',
+#                          data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
 #                          settings=settings,
 #                          config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
-# test.create()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/enums.py` & `Simba-UW-tf-dev-1.56.8/simba/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,16 +238,14 @@
     STR = 'str'
     INT = 'int'
     FLOAT = 'float'
     NONE = 'None'
     SQRT = 'sqrt'
     ENTROPY = 'entropy'
 
-
-
 class Methods(Enum):
     USER_DEFINED = 'user_defined'
     CLASSIC_TRACKING = 'Classic tracking'
     THREE_D_TRACKING = '3D tracking'
     MULTI_TRACKING = 'Multi tracking'
     CREATE_POSE_CONFIG = 'Create pose config...'
     RANDOM_UNDERSAMPLE = 'random undersample'
@@ -256,14 +254,15 @@
     GAUSSIAN = 'Gaussian'
     SAVITZKY_GOLAY = 'Savitzky Golay'
     SPLIT_TYPE_FRAMES = 'FRAMES'
     SPLIT_TYPE_BOUTS = 'BOUTS'
     BORIS = 'BORIS'
     WARNING = 'WARNING'
     ERROR = 'ERROR'
+    ANOVA = 'ANOVA'
     INVALID_THIRD_PARTY_APPENDER_FILE = 'INVALID annotations file data format'
     ADDITIONAL_THIRD_PARTY_CLFS = 'ADDITIONAL third-party behavior detected'
     ZERO_THIRD_PARTY_VIDEO_ANNOTATIONS = 'ZERO third-party video annotations found'
     THIRD_PARTY_FPS_CONFLICT = 'Annotations and pose FPS conflict'
     THIRD_PARTY_EVENT_COUNT_CONFLICT = 'Annotations EVENT COUNT conflict'
     THIRD_PARTY_EVENT_OVERLAP = 'Annotations OVERLAP inaccuracy'
     ZERO_THIRD_PARTY_VIDEO_BEHAVIOR_ANNOTATIONS = 'ZERO third-party video behavior annotations found'
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 0000 0001 4275 6431 0000 6800 0000 0800  ....Bud1..h.....
-00000010: 0000 6800 0000 100c 0000 700c 0000 200c  ..h.......p... .
+00000000: 0000 0001 4275 6431 0000 7800 0000 0800  ....Bud1..x.....
+00000010: 0000 7800 0000 100c 0000 700b 0000 200c  ..x.......p... .
 00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 0078  ...............x
+00000040: 0000 0000 0000 0003 0000 0001 0000 007a  ...............z
 00000050: 0000 0007 0000 1000 0074 0063 0068 005f  .........t.c.h._
 00000060: 0070 0072 0000 0000 0000 0000 0000 0000  .p.r............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,219 +250,219 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0014 0000 001b  ................
-00001010: 0074 0068 0069 0072 0064 005f 0070 0061  .t.h.i.r.d._.p.a
-00001020: 0072 0074 0079 005f 006c 0061 0062 0065  .r.t.y._.l.a.b.e
-00001030: 006c 005f 0061 0070 0070 0065 006e 0064  .l._.a.p.p.e.n.d
-00001040: 0065 0072 0073 6c73 7670 626c 6f62 0000  .e.r.slsvpblob..
-00001050: 025e 6270 6c69 7374 3030 d801 0203 0405  .^bplist00......
-00001060: 0607 0809 0a0b 1d45 4647 0a5f 1012 7669  .......EFG._..vi
-00001070: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00001080: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00001090: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-000010a0: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
-000010b0: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
-000010c0: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
-000010d0: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
-000010e0: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
-000010f0: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
-00001100: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
-00001110: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
-00001120: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
-00001130: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
-00001140: 6d65 d416 1718 191a 1b0a 1d55 696e 6465  me.........Uinde
-00001150: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
-00001160: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
-00001170: d416 1718 191f 201d 1d10 0810 c808 08d4  ...... .........
-00001180: 1617 1819 0924 1d0a 10b5 0809 d416 1718  .....$..........
-00001190: 1928 241d 1d10 0208 08d4 1617 1819 2c2d  .($...........,-
-000011a0: 1d0a 1003 1061 0809 d416 1718 1931 320a  .....a.......12.
-000011b0: 1d10 0510 6409 08d4 1617 1819 3637 0a0a  ....d.......67..
-000011c0: 1004 1073 0909 d416 1718 193b 3c0a 1d10  ...s.......;<...
-000011d0: 0610 4b09 08d4 1617 1819 4041 0a0a 1000  ..K.......@A....
-000011e0: 1101 a609 0908 2340 2800 0000 0000 0054  ......#@(......T
-000011f0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00001200: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-00001210: 008c 008e 008f 00a2 00ab 00ba 00c7 00d3  ................
-00001220: 00d8 00de 00e3 00eb 00f0 00f9 00ff 0105  ................
-00001230: 010f 0117 0119 011c 011d 011e 0127 0129  .............'.)
-00001240: 012b 012c 012d 0136 0138 0139 013a 0143  .+.,.-.6.8.9.:.C
-00001250: 0145 0146 0147 0150 0152 0154 0155 0156  .E.F.G.P.R.T.U.V
-00001260: 015f 0161 0163 0164 0165 016e 0170 0172  ._.a.c.d.e.n.p.r
-00001270: 0173 0174 017d 017f 0181 0182 0183 018c  .s.t.}..........
-00001280: 018e 0191 0192 0193 0194 019d 01a2 01ab  ................
-00001290: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
-000012a0: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
-000012b0: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
-000012c0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
-000012d0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-000012e0: 006e 0064 0065 0072 0073 6d6f 4444 626c  .n.d.e.r.smoDDbl
-000012f0: 6f62 0000 0008 6874 98e3 46f2 c441 0000  ob....ht..F..A..
-00001300: 001b 0074 0068 0069 0072 0064 005f 0070  ...t.h.i.r.d._.p
-00001310: 0061 0072 0074 0079 005f 006c 0061 0062  .a.r.t.y._.l.a.b
-00001320: 0065 006c 005f 0061 0070 0070 0065 006e  .e.l._.a.p.p.e.n
-00001330: 0064 0065 0072 0073 6d6f 6444 626c 6f62  .d.e.r.smodDblob
-00001340: 0000 0008 6874 98e3 46f2 c441 0000 001b  ....ht..F..A....
-00001350: 0074 0068 0069 0072 0064 005f 0070 0061  .t.h.i.r.d._.p.a
-00001360: 0072 0074 0079 005f 006c 0061 0062 0065  .r.t.y._.l.a.b.e
-00001370: 006c 005f 0061 0070 0070 0065 006e 0064  .l._.a.p.p.e.n.d
-00001380: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00001390: 0000 0002 c000 0000 001b 0074 0068 0069  ...........t.h.i
-000013a0: 0072 0064 005f 0070 0061 0072 0074 0079  .r.d._.p.a.r.t.y
-000013b0: 005f 006c 0061 0062 0065 006c 005f 0061  ._.l.a.b.e.l._.a
-000013c0: 0070 0070 0065 006e 0064 0065 0072 0073  .p.p.e.n.d.e.r.s
-000013d0: 7653 726e 6c6f 6e67 0000 0001 0000 000c  vSrnlong........
-000013e0: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-000013f0: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
-00001400: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00001410: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00001420: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00001430: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00001440: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00001450: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00001460: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00001470: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00001480: 0809 5f10 187b 7b33 3934 2c20 3138 317d  .._..{{394, 181}
-00001490: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-000014a0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-000014b0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000014c0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-000014d0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
-000014e0: 7600 6900 7300 6500 646c 6731 5363 6f6d  v.i.s.e.dlg1Scom
-000014f0: 7000 0000 0000 05bb b700 0000 0c00 7500  p.............u.
-00001500: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
-00001510: 7300 6500 646d 6f44 4462 6c6f 6200 0000  s.e.dmoDDblob...
-00001520: 08ff 2f6f 7569 f6c4 4100 0000 0c00 7500  ../oui..A.....u.
-00001530: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
-00001540: 7300 6500 646d 6f64 4462 6c6f 6200 0000  s.e.dmodDblob...
-00001550: 08ff 2f6f 7569 f6c4 4100 0000 0c00 7500  ../oui..A.....u.
-00001560: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
-00001570: 7300 6500 6470 6831 5363 6f6d 7000 0000  s.e.dph1Scomp...
-00001580: 0000 0700 0000 0000 0c00 7500 6e00 7300  ..........u.n.s.
-00001590: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-000015a0: 6476 5372 6e6c 6f6e 6700 0000 0100 0000  dvSrnlong.......
-000015b0: 0500 7500 7400 6900 6c00 7362 7773 7062  ..u.t.i.l.sbwspb
-000015c0: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
-000015d0: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-000015e0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-000015f0: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00001600: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00001610: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00001620: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00001630: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00001640: 0808 0908 095f 1018 7b7b 3734 362c 2033  ....._..{{746, 3
-00001650: 3230 7d2c 207b 3737 302c 2034 3336 7d7d  20}, {770, 436}}
-00001660: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
-00001670: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00001680: 0000 0000 0000 0000 0000 0000 0000 009a  ................
-00001690: 0000 0005 0075 0074 0069 006c 0073 6473  .....u.t.i.l.sds
-000016a0: 636c 626f 6f6c 0000 0000 0500 7500 7400  clbool......u.t.
-000016b0: 6900 6c00 736c 6731 5363 6f6d 7000 0000  i.l.slg1Scomp...
-000016c0: 0000 011c 5a00 0000 0500 7500 7400 6900  ....Z.....u.t.i.
-000016d0: 6c00 736c 7376 4362 6c6f 6200 0002 9762  l.slsvCblob....b
-000016e0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-000016f0: 090a 0b19 494a 0a4c 5f10 1276 6965 774f  ....IJ.L_..viewO
-00001700: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-00001710: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00001720: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00001730: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00001740: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
-00001750: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00001760: 6573 5869 636f 6e53 697a 6510 0109 ab0c  esXiconSize.....
-00001770: 151d 2226 2b30 353a 3f44 d40d 0e0f 100a  .."&+05:?D......
-00001780: 0a13 1457 7669 7369 626c 6559 6173 6365  ...WvisibleYasce
-00001790: 6e64 696e 6755 7769 6474 685a 6964 656e  ndingUwidthZiden
-000017a0: 7469 6669 6572 0909 1102 0454 6e61 6d65  tifier.....Tname
-000017b0: d416 1718 1019 1a19 1c57 7669 7369 626c  .........Wvisibl
-000017c0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-000017d0: 6708 1023 0858 7562 6971 7569 7479 d40d  g..#.Xubiquity..
-000017e0: 0e0f 100a 1920 2109 0810 b55c 6461 7465  ..... !....\date
-000017f0: 4d6f 6469 6669 6564 d40d 0e0f 1019 1920  Modified....... 
-00001800: 2508 085b 6461 7465 4372 6561 7465 64d4  %..[dateCreated.
-00001810: 0d0e 0f10 0a19 292a 0908 1061 5473 697a  ......)*...aTsiz
-00001820: 65d4 0d0e 0f10 0a0a 2e2f 0909 1073 546b  e......../...sTk
-00001830: 696e 64d4 0d0e 0f10 190a 3334 0809 1064  ind.......34...d
-00001840: 556c 6162 656c d40d 0e0f 1019 0a38 3908  Ulabel.......89.
-00001850: 0910 4b57 7665 7273 696f 6ed4 0d0e 0f10  ..KWversion.....
-00001860: 190a 3d3e 0809 1101 2c58 636f 6d6d 656e  ..=>....,Xcommen
-00001870: 7473 d40d 0e0f 1019 1942 4308 0810 c85e  ts.......BC....^
-00001880: 6461 7465 4c61 7374 4f70 656e 6564 d416  dateLastOpened..
-00001890: 1718 1019 2019 4708 0859 6461 7465 4164  .... .G..YdateAd
-000018a0: 6465 6408 2340 2800 0000 0000 0054 6e61  ded.#@(......Tna
-000018b0: 6d65 0923 4030 0000 0000 0000 0008 0019  me.#@0..........
-000018c0: 002e 0040 0048 005c 0065 0070 0083 008c  ...@.H.\.e.p....
-000018d0: 008e 008f 009b 00a4 00ac 00b6 00bc 00c7  ................
-000018e0: 00c8 00c9 00cc 00d1 00da 00e2 00e8 00f2  ................
-000018f0: 00f3 00f5 00f6 00ff 0108 0109 010a 010c  ................
-00001900: 0119 0122 0123 0124 0130 0139 013a 013b  ...".#.$.0.9.:.;
-00001910: 013d 0142 014b 014c 014d 014f 0154 015d  .=.B.K.L.M.O.T.]
-00001920: 015e 015f 0161 0167 0170 0171 0172 0174  .^._.a.g.p.q.r.t
-00001930: 017c 0185 0186 0187 018a 0193 019c 019d  .|..............
-00001940: 019e 01a0 01af 01b8 01b9 01ba 01c4 01c5  ................
-00001950: 01ce 01d3 01d4 0000 0000 0000 0201 0000  ................
-00001960: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-00001970: 0000 0000 01dd 0000 0005 0075 0074 0069  ...........u.t.i
-00001980: 006c 0073 6c73 7670 626c 6f62 0000 025e  .l.slsvpblob...^
-00001990: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-000019a0: 0809 0a0b 1d45 460a 485f 1012 7669 6577  .....EF.H_..view
-000019b0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-000019c0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-000019d0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000019e0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-000019f0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001a00: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00001a10: 7465 7358 6963 6f6e 5369 7a65 1001 09d9  tesXiconSize....
-00001a20: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00001a30: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00001a40: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00001a50: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00001a60: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00001a70: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-00001a80: d416 1718 191a 0a1c 1d55 696e 6465 7859  .........UindexY
-00001a90: 6173 6365 6e64 696e 6755 7769 6474 6857  ascendingUwidthW
-00001aa0: 7669 7369 626c 6510 0709 1101 2c08 d416  visible.....,...
-00001ab0: 1718 191f 1d21 1d10 0808 10c8 08d4 1617  .....!..........
-00001ac0: 1819 241d 261d 1002 0810 b508 d416 1718  ..$.&...........
-00001ad0: 1929 1d2b 0a10 0308 1061 09d4 1617 1819  .).+.....a......
-00001ae0: 2e0a 301d 1005 0910 6408 d416 1718 1933  ..0.....d......3
-00001af0: 0a35 0a10 0409 1073 09d4 1617 1819 380a  .5.....s......8.
-00001b00: 3a1d 1006 0910 4b08 d416 1718 193d 0a3f  :.....K......=.?
-00001b10: 0a10 0009 1102 0409 d416 1718 1909 1d26  ...............&
-00001b20: 0a08 0908 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00001b30: 6d65 0923 4030 0000 0000 0000 0008 0019  me.#@0..........
-00001b40: 002e 0040 0048 005c 0065 0070 0083 008c  ...@.H.\.e.p....
-00001b50: 008e 008f 00a2 00ab 00ba 00c6 00cb 00d1  ................
-00001b60: 00d6 00de 00e3 00f0 00f9 00ff 0109 010f  ................
-00001b70: 0117 0119 011a 011d 011e 0127 0129 012a  ...........'.).*
-00001b80: 012c 012d 0136 0138 0139 013b 013c 0145  .,.-.6.8.9.;.<.E
-00001b90: 0147 0148 014a 014b 0154 0156 0157 0159  .G.H.J.K.T.V.W.Y
-00001ba0: 015a 0163 0165 0166 0168 0169 0172 0174  .Z.c.e.f.h.i.r.t
-00001bb0: 0175 0177 0178 0181 0183 0184 0187 0188  .u.w.x..........
-00001bc0: 0191 0192 0193 0194 019d 01a2 01a3 0000  ................
-00001bd0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-00001be0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-00001bf0: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001c00: 626c 6f62 0000 0008 8551 cb34 d5f4 c441  blob.....Q.4...A
-00001c10: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
-00001c20: 6444 626c 6f62 0000 0008 b191 97e3 46f2  dDblob........F.
-00001c30: c441 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
-00001c40: 7068 3153 636f 6d70 0000 0000 0001 6000  ph1Scomp......`.
-00001c50: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
-00001c60: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
-00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001000: 0000 0000 0000 0000 0000 000f 0000 000c  ................
+00001010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+00001020: 0069 0073 0065 0064 6c73 7643 626c 6f62  .i.s.e.dlsvCblob
+00001030: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
+00001040: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
+00001050: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001060: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001070: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001080: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001090: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000010a0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000010b0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000010c0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
+000010d0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
+000010e0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
+000010f0: 5a69 6465 6e74 6966 6965 7209 0911 018f  Zidentifier.....
+00001100: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
+00001110: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00001120: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
+00001130: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
+00001140: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
+00001150: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
+00001160: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
+00001170: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
+00001180: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
+00001190: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
+000011a0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
+000011b0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
+000011c0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
+000011d0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+000011e0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
+000011f0: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
+00001200: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
+00001210: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+00001220: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
+00001230: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
+00001240: e200 e800 f200 f300 f500 f600 ff01 0801  ................
+00001250: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
+00001260: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
+00001270: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
+00001280: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
+00001290: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
+000012a0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
+000012b0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000012c0: 0000 0000 0000 0000 0001 dd00 0000 0c00  ................
+000012d0: 7500 6e00 7300 7500 7000 6500 7200 7600  u.n.s.u.p.e.r.v.
+000012e0: 6900 7300 6500 646c 7376 7062 6c6f 6200  i.s.e.dlsvpblob.
+000012f0: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
+00001300: 0506 0708 090a 0b1d 4546 0a48 5f10 1276  ........EF.H_..v
+00001310: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00001320: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00001330: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00001340: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00001350: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00001360: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+00001370: 6544 6174 6573 5869 636f 6e53 697a 6510  eDatesXiconSize.
+00001380: 0109 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
+00001390: 2d32 373c 4158 636f 6d6d 656e 7473 5e64  -27<AXcomments^d
+000013a0: 6174 654c 6173 744f 7065 6e65 645b 6461  ateLastOpened[da
+000013b0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+000013c0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+000013d0: 6e54 6e61 6d65 5c64 6174 654d 6f64 6966  nTname\dateModif
+000013e0: 6965 64d4 1617 1819 1a0a 1c1d 5569 6e64  ied.........Uind
+000013f0: 6578 5961 7363 656e 6469 6e67 5577 6964  exYascendingUwid
+00001400: 7468 5776 6973 6962 6c65 1007 0911 012c  thWvisible.....,
+00001410: 08d4 1617 1819 1f1d 211d 1008 0810 c808  ........!.......
+00001420: d416 1718 1924 1d26 1d10 0208 10b5 08d4  .....$.&........
+00001430: 1617 1819 291d 2b0a 1003 0810 6109 d416  ....).+.....a...
+00001440: 1718 192e 0a30 1d10 0509 1064 08d4 1617  .....0.....d....
+00001450: 1819 330a 350a 1004 0910 7309 d416 1718  ..3.5.....s.....
+00001460: 1938 0a3a 1d10 0609 104b 08d4 1617 1819  .8.:.....K......
+00001470: 3d0a 3f0a 1000 0911 018f 09d4 1617 1819  =.?.............
+00001480: 091d 260a 0809 0823 4028 0000 0000 0000  ..&....#@(......
+00001490: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
+000014a0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+000014b0: 8300 8c00 8e00 8f00 a200 ab00 ba00 c600  ................
+000014c0: cb00 d100 d600 de00 e300 f000 f900 ff01  ................
+000014d0: 0901 0f01 1701 1901 1a01 1d01 1e01 2701  ..............'.
+000014e0: 2901 2a01 2c01 2d01 3601 3801 3901 3b01  ).*.,.-.6.8.9.;.
+000014f0: 3c01 4501 4701 4801 4a01 4b01 5401 5601  <.E.G.H.J.K.T.V.
+00001500: 5701 5901 5a01 6301 6501 6601 6801 6901  W.Y.Z.c.e.f.h.i.
+00001510: 7201 7401 7501 7701 7801 8101 8301 8401  r.t.u.w.x.......
+00001520: 8701 8801 9101 9201 9301 9401 9d01 a201  ................
+00001530: a300 0000 0000 0002 0100 0000 0000 0000  ................
+00001540: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
+00001550: ac00 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
+00001560: 6500 7200 7600 6900 7300 6500 646d 6f44  e.r.v.i.s.e.dmoD
+00001570: 4462 6c6f 6200 0000 08f2 efa7 b815 f8c4  Dblob...........
+00001580: 4100 0000 0c00 7500 6e00 7300 7500 7000  A.....u.n.s.u.p.
+00001590: 6500 7200 7600 6900 7300 6500 646d 6f64  e.r.v.i.s.e.dmod
+000015a0: 4462 6c6f 6200 0000 08f2 efa7 b815 f8c4  Dblob...........
+000015b0: 4100 0000 0c00 7500 6e00 7300 7500 7000  A.....u.n.s.u.p.
+000015c0: 6500 7200 7600 6900 7300 6500 6470 6831  e.r.v.i.s.e.dph1
+000015d0: 5363 6f6d 7000 0000 0000 0840 0000 0000  Scomp......@....
+000015e0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
+000015f0: 7600 6900 7300 6500 6476 5372 6e6c 6f6e  v.i.s.e.dvSrnlon
+00001600: 6700 0000 0100 0000 0500 7500 7400 6900  g.........u.t.i.
+00001610: 6c00 7362 7773 7062 6c6f 6200 0000 c962  l.sbwspblob....b
+00001620: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00001630: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00001640: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00001650: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00001660: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00001670: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00001680: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00001690: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
+000016a0: 7b7b 3734 362c 2033 3230 7d2c 207b 3737  {{746, 320}, {77
+000016b0: 302c 2034 3336 7d7d 0908 1725 313d 4960  0, 436}}...%1=I`
+000016c0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
+000016d0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+000016e0: 0000 0000 0000 009a 0000 0005 0075 0074  .............u.t
+000016f0: 0069 006c 0073 6473 636c 626f 6f6c 0000  .i.l.sdsclbool..
+00001700: 0000 0500 7500 7400 6900 6c00 736c 6731  ....u.t.i.l.slg1
+00001710: 5363 6f6d 7000 0000 0000 011e f300 0000  Scomp...........
+00001720: 0500 7500 7400 6900 6c00 736c 7376 4362  ..u.t.i.l.slsvCb
+00001730: 6c6f 6200 0002 9762 706c 6973 7430 30d8  lob....bplist00.
+00001740: 0102 0304 0506 0708 090a 0b19 494a 0a4c  ............IJ.L
+00001750: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001760: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00001770: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001780: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001790: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+000017a0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+000017b0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
+000017c0: 697a 6510 0109 ab0c 151d 2226 2b30 353a  ize......."&+05:
+000017d0: 3f44 d40d 0e0f 100a 0a13 1457 7669 7369  ?D.........Wvisi
+000017e0: 626c 6559 6173 6365 6e64 696e 6755 7769  bleYascendingUwi
+000017f0: 6474 685a 6964 656e 7469 6669 6572 0909  dthZidentifier..
+00001800: 1102 0454 6e61 6d65 d416 1718 1019 1a19  ...Tname........
+00001810: 1c57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00001820: 6173 6365 6e64 696e 6708 1023 0858 7562  ascending..#.Xub
+00001830: 6971 7569 7479 d40d 0e0f 100a 1920 2109  iquity....... !.
+00001840: 0810 b55c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00001850: d40d 0e0f 1019 1920 2508 085b 6461 7465  ....... %..[date
+00001860: 4372 6561 7465 64d4 0d0e 0f10 0a19 292a  Created.......)*
+00001870: 0908 1061 5473 697a 65d4 0d0e 0f10 0a0a  ...aTsize.......
+00001880: 2e2f 0909 1073 546b 696e 64d4 0d0e 0f10  ./...sTkind.....
+00001890: 190a 3334 0809 1064 556c 6162 656c d40d  ..34...dUlabel..
+000018a0: 0e0f 1019 0a38 3908 0910 4b57 7665 7273  .....89...KWvers
+000018b0: 696f 6ed4 0d0e 0f10 190a 3d3e 0809 1101  ion.......=>....
+000018c0: 2c58 636f 6d6d 656e 7473 d40d 0e0f 1019  ,Xcomments......
+000018d0: 1942 4308 0810 c85e 6461 7465 4c61 7374  .BC....^dateLast
+000018e0: 4f70 656e 6564 d416 1718 1019 2019 4708  Opened...... .G.
+000018f0: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
+00001900: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
+00001910: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
+00001920: 0065 0070 0083 008c 008e 008f 009b 00a4  .e.p............
+00001930: 00ac 00b6 00bc 00c7 00c8 00c9 00cc 00d1  ................
+00001940: 00da 00e2 00e8 00f2 00f3 00f5 00f6 00ff  ................
+00001950: 0108 0109 010a 010c 0119 0122 0123 0124  ...........".#.$
+00001960: 0130 0139 013a 013b 013d 0142 014b 014c  .0.9.:.;.=.B.K.L
+00001970: 014d 014f 0154 015d 015e 015f 0161 0167  .M.O.T.].^._.a.g
+00001980: 0170 0171 0172 0174 017c 0185 0186 0187  .p.q.r.t.|......
+00001990: 018a 0193 019c 019d 019e 01a0 01af 01b8  ................
+000019a0: 01b9 01ba 01c4 01c5 01ce 01d3 01d4 0000  ................
+000019b0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+000019c0: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
+000019d0: 0005 0075 0074 0069 006c 0073 6c73 7670  ...u.t.i.l.slsvp
+000019e0: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+000019f0: d801 0203 0405 0607 0809 0a0b 1d45 460a  .............EF.
+00001a00: 485f 1012 7669 6577 4f70 7469 6f6e 7356  H_..viewOptionsV
+00001a10: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+00001a20: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00001a30: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00001a40: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00001a50: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00001a60: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
+00001a70: 5369 7a65 1001 09d9 0c0d 0e0f 1011 1213  Size............
+00001a80: 1415 1e23 282d 3237 3c41 5863 6f6d 6d65  ...#(-27<AXcomme
+00001a90: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+00001aa0: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00001ab0: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00001ac0: 6572 7369 6f6e 546e 616d 655c 6461 7465  ersionTname\date
+00001ad0: 4d6f 6469 6669 6564 d416 1718 191a 0a1c  Modified........
+00001ae0: 1d55 696e 6465 7859 6173 6365 6e64 696e  .UindexYascendin
+00001af0: 6755 7769 6474 6857 7669 7369 626c 6510  gUwidthWvisible.
+00001b00: 0709 1101 2c08 d416 1718 191f 1d21 1d10  ....,........!..
+00001b10: 0808 10c8 08d4 1617 1819 241d 261d 1002  ..........$.&...
+00001b20: 0810 b508 d416 1718 1929 1d2b 0a10 0308  .........).+....
+00001b30: 1061 09d4 1617 1819 2e0a 301d 1005 0910  .a........0.....
+00001b40: 6408 d416 1718 1933 0a35 0a10 0409 1073  d......3.5.....s
+00001b50: 09d4 1617 1819 380a 3a1d 1006 0910 4b08  ......8.:.....K.
+00001b60: d416 1718 193d 0a3f 0a10 0009 1102 0409  .....=.?........
+00001b70: d416 1718 1909 1d26 0a08 0908 2340 2800  .......&....#@(.
+00001b80: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
+00001b90: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
+00001ba0: 0065 0070 0083 008c 008e 008f 00a2 00ab  .e.p............
+00001bb0: 00ba 00c6 00cb 00d1 00d6 00de 00e3 00f0  ................
+00001bc0: 00f9 00ff 0109 010f 0117 0119 011a 011d  ................
+00001bd0: 011e 0127 0129 012a 012c 012d 0136 0138  ...'.).*.,.-.6.8
+00001be0: 0139 013b 013c 0145 0147 0148 014a 014b  .9.;.<.E.G.H.J.K
+00001bf0: 0154 0156 0157 0159 015a 0163 0165 0166  .T.V.W.Y.Z.c.e.f
+00001c00: 0168 0169 0172 0174 0175 0177 0178 0181  .h.i.r.t.u.w.x..
+00001c10: 0183 0184 0187 0188 0191 0192 0193 0194  ................
+00001c20: 019d 01a2 01a3 0000 0000 0000 0201 0000  ................
+00001c30: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+00001c40: 0000 0000 01ac 0000 0005 0075 0074 0069  ...........u.t.i
+00001c50: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
+00001c60: 54f1 87c2 44f6 c441 0000 0005 0075 0074  T...D..A.....u.t
+00001c70: 0069 006c 0073 6d6f 6444 626c 6f62 0000  .i.l.smodDblob..
+00001c80: 0008 b191 97e3 46f2 c441 0000 0005 0075  ......F..A.....u
+00001c90: 0074 0069 006c 0073 7068 3153 636f 6d70  .t.i.l.sph1Scomp
+00001ca0: 0000 0000 0001 6000 0000 0005 0075 0074  ......`......u.t
+00001cb0: 0069 006c 0073 7653 726e 6c6f 6e67 0000  .i.l.svSrnlong..
+00001cc0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -509,23 +509,23 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 095a 0000 000b 005f 005f 0070  ...B.Z....._._.p
+00002030: 0000 0042 0ef0 0000 000b 005f 005f 0070  ...B......._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 08d6 dc03  moDDblob........
-00002060: dff4 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 8577 e207  moDDblob.....w..
+00002060: 73f7 c441 0000 000b 005f 005f 0070 0079  s..A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00002080: 6444 626c 6f62 0000 0008 08d6 dc03 dff4  dDblob..........
+00002080: 6444 626c 6f62 0000 0008 6a13 8953 eaf6  dDblob....j..S..
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000020b0: 636f 6d70 0000 0000 004f f000 0000 0006  comp.....O......
+000020b0: 636f 6d70 0000 0000 0050 0000 0000 0006  comp.....P......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
 000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
@@ -649,15 +649,15 @@
 00002880: 2c20 3337 337d 2c20 7b37 3730 2c20 3433  , 373}, {770, 43
 00002890: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
 000028a0: 7d7e 9a00 0000 0000 0001 0100 0000 0000  }~..............
 000028b0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 000028c0: 0000 9b00 0000 1400 6200 6100 7400 6300  ........b.a.t.c.
 000028d0: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
 000028e0: 7300 5f00 7600 6900 6400 6500 6f00 736c  s._.v.i.d.e.o.sl
-000028f0: 6731 5363 6f6d 7000 0000 0000 017d e700  g1Scomp......}..
+000028f0: 6731 5363 6f6d 7000 0000 0000 017e 5700  g1Scomp......~W.
 00002900: 0000 1400 6200 6100 7400 6300 6800 5f00  ....b.a.t.c.h._.
 00002910: 7000 7200 6f00 6300 6500 7300 7300 5f00  p.r.o.c.e.s.s._.
 00002920: 7600 6900 6400 6500 6f00 736c 7376 4362  v.i.d.e.o.slsvCb
 00002930: 6c6f 6200 0003 0762 706c 6973 7430 30d8  lob....bplist00.
 00002940: 0102 0304 0506 0708 090a 0b19 5657 0a59  ............VW.Y
 00002950: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
 00002960: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
@@ -746,16 +746,16 @@
 00002e90: 0177 0178 017a 017b 017d 0186 0187 018a  .w.x.z.{.}......
 00002ea0: 018b 018d 0196 0197 0199 019a 019c 019d  ................
 00002eb0: 01a6 01ab 0000 0000 0000 0201 0000 0000  ................
 00002ec0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
 00002ed0: 0000 01ac 0000 0014 0062 0061 0074 0063  .........b.a.t.c
 00002ee0: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
 00002ef0: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
-00002f00: 6d6f 4444 626c 6f62 0000 0008 4b60 d4fa  moDDblob....K`..
-00002f10: 99f1 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
+00002f00: 6d6f 4444 626c 6f62 0000 0008 f203 dcf3  moDDblob........
+00002f10: ebf6 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
 00002f20: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
 00002f30: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
 00002f40: 6d6f 6444 626c 6f62 0000 0008 4b60 d4fa  modDblob....K`..
 00002f50: 99f1 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
 00002f60: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
 00002f70: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
 00002f80: 7068 3153 636f 6d70 0000 0000 0001 f000  ph1Scomp........
@@ -965,15 +965,15 @@
 00003c40: 0000 0000 0000 0000 0000 0000 0000 9900  ................
 00003c50: 0000 1200 6600 6500 6100 7400 7500 7200  ....f.e.a.t.u.r.
 00003c60: 6500 5f00 6500 7800 7400 7200 6100 6300  e._.e.x.t.r.a.c.
 00003c70: 7400 6f00 7200 7364 7363 6c62 6f6f 6c00  t.o.r.sdsclbool.
 00003c80: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
 00003c90: 0065 005f 0065 0078 0074 0072 0061 0063  .e._.e.x.t.r.a.c
 00003ca0: 0074 006f 0072 0073 6c67 3153 636f 6d70  .t.o.r.slg1Scomp
-00003cb0: 0000 0000 0012 686f 0000 0012 0066 0065  ......ho.....f.e
+00003cb0: 0000 0000 0012 6893 0000 0012 0066 0065  ......h......f.e
 00003cc0: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00003cd0: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
 00003ce0: 6c73 7643 626c 6f62 0000 02b8 6270 6c69  lsvCblob....bpli
 00003cf0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 00003d00: 0c0d 1a48 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
 00003d10: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 00003d20: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
@@ -1022,15 +1022,15 @@
 00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004000: 0000 0000 0000 0000 0000 0015 0000 0012  ................
 00004010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00004020: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 00004030: 0072 0073 6d6f 4444 626c 6f62 0000 0008  .r.smoDDblob....
-00004040: ae8b 457c 94f5 c441 0000 0012 0066 0065  ..E|...A.....f.e
+00004040: e84a b14c eaf6 c441 0000 0012 0066 0065  .J.L...A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
 00004070: 6d6f 6444 626c 6f62 0000 0008 ae8b 457c  modDblob......E|
 00004080: 94f5 c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
 000040b0: 636f 6d70 0000 0000 0014 d000 0000 0012  comp............
@@ -1049,17 +1049,17 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 01a4 2400 0000 0600 6d00 6900 7800  ....$.....m.i.x.
+000041f0: 0000 01ad c200 0000 0600 6d00 6900 7800  ..........m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 08ef 201d a05b f6c4 4100 0000 0600 6d00  .. ..[..A.....m.
+00004210: 08e3 5739 7081 f7c4 4100 0000 0600 6d00  ..W9p...A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
 00004230: 6200 0000 08ef 201d a05b f6c4 4100 0000  b..... ..[..A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
 00004250: 5363 6f6d 7000 0000 0000 0200 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
@@ -1274,15 +1274,15 @@
 00004f90: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
 00004fa0: 0000 01fe 0000 0000 0000 0000 0000 0000  ................
 00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
+00005000: 0000 0000 0000 0000 0000 0014 0000 0008  ................
 00005010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00005020: 6d6f 4444 626c 6f62 0000 0008 e63c 5181  moDDblob.....<Q.
 00005030: 52f2 c441 0000 0008 0070 006c 006f 0074  R..A.....p.l.o.t
 00005040: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
 00005050: 0000 0008 65be f96a 3ef2 c441 0000 0008  ....e..j>..A....
 00005060: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00005070: 7068 3153 636f 6d70 0000 0000 000c 4000  ph1Scomp......@.
@@ -1523,278 +1523,278 @@
 00005f20: 4444 626c 6f62 0000 0008 0b30 86dc dcf4  DDblob.....0....
 00005f30: c441 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 00005f40: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 00005f50: 0073 6d6f 6444 626c 6f62 0000 0008 be76  .smodDblob.....v
 00005f60: 2985 44f2 c441 0000 000e 0070 006f 0073  ).D..A.....p.o.s
 00005f70: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00005f80: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00005f90: 0000 0004 4000 0000 000e 0070 006f 0073  ....@......p.o.s
-00005fa0: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
-00005fb0: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
-00005fc0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00005f90: 0000 0004 4000 0000 0000 0000 0000 0000  ....@...........
+00005fa0: 0000 01fe 0000 0000 0000 0000 0000 0000  ................
+00005fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006000: 0000 0000 0000 0000 0000 0009 0000 0009  ................
+00006000: 0000 0000 0000 0000 0000 0011 0000 0009  ................
 00006010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
-00006020: 0073 6c67 3153 636f 6d70 0000 0000 0004  .slg1Scomp......
-00006030: 4973 0000 0009 0072 006f 0069 005f 0074  Is.....r.o.i._.t
-00006040: 006f 006f 006c 0073 6c73 7643 626c 6f62  .o.o.l.slsvCblob
-00006050: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
-00006060: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
-00006070: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00006080: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00006090: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-000060a0: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-000060b0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-000060c0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-000060d0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000060e0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
-000060f0: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
-00006100: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00006110: 5a69 6465 6e74 6966 6965 7209 1102 d009  Zidentifier.....
-00006120: 546e 616d 65d4 0d0e 0f10 1617 1619 0810  Tname...........
-00006130: 2308 5875 6269 7175 6974 79d4 0d0e 0f10  #.Xubiquity.....
-00006140: 0a1c 161e 0910 b508 5c64 6174 654d 6f64  ........\dateMod
-00006150: 6966 6965 64d4 0d0e 0f10 161c 1622 0808  ified........"..
-00006160: 5b64 6174 6543 7265 6174 6564 d40d 0e0f  [dateCreated....
-00006170: 100a 2516 2709 1061 0854 7369 7a65 d40d  ..%.'..a.Tsize..
-00006180: 0e0f 100a 2a0a 2c09 1073 0954 6b69 6e64  ....*.,..s.Tkind
-00006190: d40d 0e0f 1016 2f0a 3108 1064 0955 6c61  ....../.1..d.Ula
-000061a0: 6265 6cd4 0d0e 0f10 1634 0a36 0810 4b09  bel......4.6..K.
-000061b0: 5776 6572 7369 6f6e d40d 0e0f 1016 390a  Wversion......9.
-000061c0: 3b08 1101 2c09 5863 6f6d 6d65 6e74 73d4  ;...,.Xcomments.
-000061d0: 0d0e 0f10 163e 1640 0810 c808 5e64 6174  .....>.@....^dat
-000061e0: 654c 6173 744f 7065 6e65 64d4 0d0e 0f10  eLastOpened.....
-000061f0: 161c 1644 0808 5964 6174 6541 6464 6564  ...D..YdateAdded
-00006200: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
-00006210: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
-00006220: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
-00006230: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
-00006240: cb00 cc00 d100 da00 db00 dd00 de00 e700  ................
-00006250: f000 f100 f300 f401 0101 0a01 0b01 0c01  ................
-00006260: 1801 2101 2201 2401 2501 2a01 3301 3401  ..!.".$.%.*.3.4.
-00006270: 3601 3701 3c01 4501 4601 4801 4901 4f01  6.7.<.E.F.H.I.O.
-00006280: 5801 5901 5b01 5c01 6401 6d01 6e01 7101  X.Y.[.\.d.m.n.q.
-00006290: 7201 7b01 8401 8501 8701 8801 9701 a001  r.{.............
-000062a0: a101 a201 ac01 ad01 b601 bb01 c400 0000  ................
-000062b0: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
-000062c0: 0000 0000 0000 0000 0000 0001 c500 0000  ................
-000062d0: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
-000062e0: 6c00 736c 7376 7062 6c6f 6200 0002 5e62  l.slsvpblob...^b
-000062f0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-00006300: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
-00006310: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-00006320: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00006330: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00006340: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00006350: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-00006360: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-00006370: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
-00006380: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
-00006390: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
-000063a0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-000063b0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-000063c0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-000063d0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-000063e0: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
-000063f0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-00006400: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
-00006410: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
-00006420: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
-00006430: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
-00006440: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
-00006450: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
-00006460: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
-00006470: 0908 d416 1718 1940 410a 0a10 0011 02d0  .......@A.......
-00006480: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00006490: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
-000064a0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
-000064b0: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
-000064c0: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
-000064d0: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
-000064e0: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
-000064f0: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
-00006500: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
-00006510: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
-00006520: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
-00006530: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
-00006540: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
-00006550: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
-00006560: 6c00 736d 6f44 4462 6c6f 6200 0000 0860  l.smoDDblob....`
-00006570: 3099 e346 f2c4 4100 0000 0900 7200 6f00  0..F..A.....r.o.
-00006580: 6900 5f00 7400 6f00 6f00 6c00 736d 6f64  i._.t.o.o.l.smod
-00006590: 4462 6c6f 6200 0000 0860 3099 e346 f2c4  Dblob....`0..F..
-000065a0: 4100 0000 0900 7200 6f00 6900 5f00 7400  A.....r.o.i._.t.
-000065b0: 6f00 6f00 6c00 7370 6831 5363 6f6d 7000  o.o.l.sph1Scomp.
-000065c0: 0000 0000 0520 0000 0000 0900 7200 6f00  ..... ......r.o.
-000065d0: 6900 5f00 7400 6f00 6f00 6c00 7376 5372  i._.t.o.o.l.svSr
-000065e0: 6e6c 6f6e 6700 0000 0100 0000 1b00 7400  nlong.........t.
-000065f0: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
-00006600: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
-00006610: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
-00006620: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
-00006630: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00006640: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00006650: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00006660: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00006670: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00006680: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00006690: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000066a0: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-000066b0: 7b7b 3332 2c20 3132 337d 2c20 7b31 3230  {{32, 123}, {120
-000066c0: 332c 2037 3534 7d7d 0908 1725 313d 4960  3, 754}}...%1=I`
-000066d0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-000066e0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000066f0: 0000 0000 0000 009a 0000 001b 0074 0068  .............t.h
-00006700: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
-00006710: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
-00006720: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-00006730: 0073 6c67 3153 636f 6d70 0000 0000 0002  .slg1Scomp......
-00006740: 211f 0142 0143 0145 014e 014f 0151 0152  !..B.C.E.N.O.Q.R
-00006750: 0154 015d 015e 0160 0161 0163 016c 016d  .T.].^.`.a.c.l.m
-00006760: 016e 0170 0179 017a 017c 017d 017f 0188  .n.p.y.z.|.}....
-00006770: 0189 018b 018c 018e 0197 0198 019a 019b  ................
-00006780: 019d 01a6 01a7 01a9 01aa 01ac 01b5 01b6  ................
-00006790: 01b9 01ba 01bc 01bd 01c6 01cf 01d4 0000  ................
-000067a0: 0000 0000 0201 0000 0000 0000 004c 0000  .............L..
-000067b0: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
-000067c0: 0013 0070 006f 0073 0065 005f 0063 006f  ...p.o.s.e._.c.o
-000067d0: 006e 0066 0069 0067 0075 0072 0061 0074  .n.f.i.g.u.r.a.t
-000067e0: 0069 006f 006e 0073 6d6f 4444 626c 6f62  .i.o.n.smoDDblob
-000067f0: 0000 0008 d97e 4b74 e2dd c441 0000 0013  .....~Kt...A....
-00006800: 0070 006f 0000 0009 0000 0000 0000 680b  .p.o..........h.
-00006810: 0000 0045 0000 100c 0000 700c 0000 200c  ...E......p... .
-00006820: 0000 300c 0000 400c 0000 500c 0000 600b  ..0...@...P...`.
-00006830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000068f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000069f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00006c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
-00006c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00006c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00006c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00006c60: 0100 0008 0000 0000 0000 0000 0000 0000  ................
-00006c70: 0000 0000 0100 0080 0000 0000 0100 0100  ................
-00006c80: 0000 0000 0100 0200 0000 0000 0100 0400  ................
-00006c90: 0000 0000 0100 0800 0000 0000 0100 1000  ................
-00006ca0: 0000 0000 0100 2000 0000 0000 0100 4000  ...... .......@.
-00006cb0: 0000 0000 0100 8000 0000 0000 0101 0000  ................
-00006cc0: 0000 0000 0102 0000 0000 0000 0104 0000  ................
-00006cd0: 0000 0000 0108 0000 0000 0000 0110 0000  ................
-00006ce0: 0000 0000 0120 0000 0000 0000 0140 0000  ..... .......@..
-00006cf0: 0000 0000 0009 1101 2709 1000 0823 4048  ........'....#@H
-00006d00: 0000 0000 0000 2340 2800 0000 0000 0023  ......#@(......#
-00006d10: 0000 0000 0000 0000 546e 616d 6523 4030  ........Tname#@0
-00006d20: 0000 0000 0000 0900 0800 1d00 3200 4400  ............2.D.
-00006d30: 4c00 6000 7200 7b00 8d00 9800 a100 b400  L.`.r.{.........
-00006d40: b600 b700 ca00 d300 e200 ef00 fb01 0001  ................
-00006d50: 0601 0b01 1301 1801 2101 2901 2f01 3901  ........!.)./.9.
-00006d60: 3f01 4001 4301 4401 4601 4f01 5001 5201  ?.@.C.D.F.O.P.R.
-00006d70: 5301 5501 5e01 5f01 6101 6201 6b01 6c01  S.U.^._.a.b.k.l.
-00006d80: 6d01 6f01 7801 7901 7b01 7c01 7e01 8701  m.o.x.y.{.|.~...
-00006d90: 8801 8a01 8b01 8d01 9601 9701 9901 9a01  ................
-00006da0: 9c01 a501 a601 a801 a901 ab01 b401 b501  ................
-00006db0: b801 b901 bb01 bc01 c501 ce01 d701 dc01  ................
-00006dc0: e500 0000 0000 0002 0100 0000 0000 0000  ................
-00006dd0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
-00006de0: e600 0000 0700 0000 0900 7200 6f00 6900  ..........r.o.i.
-00006df0: 5f00 7400 6f00 6f00 6c00 7362 7773 7062  _.t.o.o.l.sbwspb
-00006e00: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
-00006e10: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00006e20: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00006e30: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00006e40: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00006e50: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00006e60: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00006e70: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00006e80: 0808 0908 095f 1018 7b7b 3332 342c 2033  ....._..{{324, 3
-00006e90: 327d 2c20 7b31 3235 302c 2037 3631 7d7d  2}, {1250, 761}}
-00006ea0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
-00006eb0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00006ec0: 0000 0000 0000 0000 0000 0000 0000 009a  ................
-00006ed0: 0000 0008 0000 001b 0074 0068 0069 0072  .........t.h.i.r
-00006ee0: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
-00006ef0: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
-00006f00: 0070 0065 006e 0064 0065 0072 0073 6c73  .p.e.n.d.e.r.sls
-00006f10: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-00006f20: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00006f30: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00006f40: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00006f50: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00006f60: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00006f70: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00006f80: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00006f90: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00006fa0: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-00006fb0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-00006fc0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00006fd0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-00006fe0: 7209 1101 a609 546e 616d 65d4 0d0e 0f10  r.....Tname.....
-00006ff0: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00007000: 79d4 0d0e 0000 0002 0000 0005 0000 0004  y...............
+00006020: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+00006030: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00006040: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00006050: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00006060: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00006070: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00006080: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00006090: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+000060a0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+000060b0: 7b33 3234 2c20 3332 7d2c 207b 3132 3530  {324, 32}, {1250
+000060c0: 2c20 3736 317d 7d09 0817 2531 3d49 606d  , 761}}...%1=I`m
+000060d0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+000060e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+000060f0: 0000 0000 0000 9a00 0000 0900 7200 6f00  ............r.o.
+00006100: 6900 5f00 7400 6f00 6f00 6c00 736c 6731  i._.t.o.o.l.slg1
+00006110: 5363 6f6d 7000 0000 0000 0449 7300 0000  Scomp......Is...
+00006120: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
+00006130: 6c00 736c 7376 4362 6c6f 6200 0002 7962  l.slsvCblob...yb
+00006140: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+00006150: 090a 0b16 4647 480a 5f10 1276 6965 774f  ....FGH._..viewO
+00006160: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+00006170: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00006180: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00006190: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+000061a0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
+000061b0: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
+000061c0: 6c61 7469 7665 4461 7465 7310 0109 ab0c  lativeDates.....
+000061d0: 151a 1f23 282d 3237 3c41 d40d 0e0f 100a  ...#(-27<A......
+000061e0: 120a 1457 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
+000061f0: 6859 6173 6365 6e64 696e 675a 6964 656e  hYascendingZiden
+00006200: 7469 6669 6572 0911 02d0 0954 6e61 6d65  tifier.....Tname
+00006210: d40d 0e0f 1016 1716 1908 1023 0858 7562  ...........#.Xub
+00006220: 6971 7569 7479 d40d 0e0f 100a 1c16 1e09  iquity..........
+00006230: 10b5 085c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00006240: d40d 0e0f 1016 1c16 2208 085b 6461 7465  ........"..[date
+00006250: 4372 6561 7465 64d4 0d0e 0f10 0a25 1627  Created......%.'
+00006260: 0910 6108 5473 697a 65d4 0d0e 0f10 0a2a  ..a.Tsize......*
+00006270: 0a2c 0910 7309 546b 696e 64d4 0d0e 0f10  .,..s.Tkind.....
+00006280: 162f 0a31 0810 6409 556c 6162 656c d40d  ./.1..d.Ulabel..
+00006290: 0e0f 1016 340a 3608 104b 0957 7665 7273  ....4.6..K.Wvers
+000062a0: 696f 6ed4 0d0e 0f10 1639 0a3b 0811 012c  ion......9.;...,
+000062b0: 0958 636f 6d6d 656e 7473 d40d 0e0f 1016  .Xcomments......
+000062c0: 3e16 4008 10c8 085e 6461 7465 4c61 7374  >.@....^dateLast
+000062d0: 4f70 656e 6564 d40d 0e0f 1016 1c16 4408  Opened........D.
+000062e0: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
+000062f0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+00006300: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+00006310: 0065 0070 0079 008c 008e 008f 009b 00a4  .e.p.y..........
+00006320: 00ac 00b2 00bc 00c7 00c8 00cb 00cc 00d1  ................
+00006330: 00da 00db 00dd 00de 00e7 00f0 00f1 00f3  ................
+00006340: 00f4 0101 010a 010b 010c 0118 0121 0122  .............!."
+00006350: 0124 0125 012a 0133 0134 0136 0137 013c  .$.%.*.3.4.6.7.<
+00006360: 0145 0146 0148 0149 014f 0158 0159 015b  .E.F.H.I.O.X.Y.[
+00006370: 015c 0164 016d 016e 0171 0172 017b 0184  .\.d.m.n.q.r.{..
+00006380: 0185 0187 0188 0197 01a0 01a1 01a2 01ac  ................
+00006390: 01ad 01b6 01bb 01c4 0000 0000 0000 0201  ................
+000063a0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+000063b0: 0000 0000 0000 01c5 0000 0009 0072 006f  .............r.o
+000063c0: 0069 005f 0074 006f 006f 006c 0073 6c73  .i._.t.o.o.l.sls
+000063d0: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
+000063e0: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
+000063f0: 4647 0a5f 1012 7669 6577 4f70 7469 6f6e  FG._..viewOption
+00006400: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00006410: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00006420: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00006430: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00006440: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
+00006450: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
+00006460: 6544 6174 6573 1001 09d9 0c0d 0e0f 1011  eDates..........
+00006470: 1213 1415 1e23 272b 3035 3a3f 5863 6f6d  .....#'+05:?Xcom
+00006480: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
+00006490: 656e 6564 5c64 6174 654d 6f64 6966 6965  ened\dateModifie
+000064a0: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
+000064b0: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
+000064c0: 7273 696f 6e54 6e61 6d65 d416 1718 191a  rsionTname......
+000064d0: 1b0a 1d55 696e 6465 7855 7769 6474 6859  ...UindexUwidthY
+000064e0: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+000064f0: 6510 0711 012c 0908 d416 1718 191f 201d  e....,........ .
+00006500: 1d10 0810 c808 08d4 1617 1819 0924 1d0a  .............$..
+00006510: 10b5 0809 d416 1718 1928 241d 1d10 0208  .........($.....
+00006520: 08d4 1617 1819 2c2d 1d0a 1003 1061 0809  ......,-.....a..
+00006530: d416 1718 1931 320a 1d10 0510 6409 08d4  .....12.....d...
+00006540: 1617 1819 3637 0a0a 1004 1073 0909 d416  ....67.....s....
+00006550: 1718 193b 3c0a 1d10 0610 4b09 08d4 1617  ...;<.....K.....
+00006560: 1819 4041 0a0a 1000 1102 d009 0908 2340  ..@A..........#@
+00006570: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
+00006580: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00006590: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
+000065a0: 00ab 00ba 00c7 00d3 00d8 00de 00e3 00eb  ................
+000065b0: 00f0 00f9 00ff 0105 010f 0117 0119 011c  ................
+000065c0: 011d 011e 0127 0129 012b 012c 012d 0136  .....'.).+.,.-.6
+000065d0: 0138 0139 013a 0143 0145 0146 0147 0150  .8.9.:.C.E.F.G.P
+000065e0: 0152 0154 0155 0156 015f 0161 0163 0164  .R.T.U.V._.a.c.d
+000065f0: 0165 016e 0170 0172 0173 0174 017d 017f  .e.n.p.r.s.t.}..
+00006600: 0181 0182 0183 018c 018e 0191 0192 0193  ................
+00006610: 0194 019d 01a2 01ab 0000 0000 0000 0201  ................
+00006620: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00006630: 0000 0000 0000 01ac 0000 0009 0072 006f  .............r.o
+00006640: 0069 005f 0074 006f 006f 006c 0073 6d6f  .i._.t.o.o.l.smo
+00006650: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
+00006660: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
+00006670: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
+00006680: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
+00006690: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
+000066a0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
+000066b0: 2000 0000 0009 0072 006f 0069 005f 0074   ......r.o.i._.t
+000066c0: 006f 006f 006c 0073 7653 726e 6c6f 6e67  .o.o.l.svSrnlong
+000066d0: 0000 0001 0000 001b 0074 0068 0069 0072  .........t.h.i.r
+000066e0: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
+000066f0: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
+00006700: 0070 0065 006e 0064 0065 0072 0073 6277  .p.e.n.d.e.r.sbw
+00006710: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
+00006720: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00006730: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00006740: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00006750: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00006760: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00006770: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00006780: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00006790: 6261 7208 0809 0809 5f10 187b 7b33 322c  bar....._..{{32,
+000067a0: 2031 3233 7d2c 207b 3132 3033 2c20 3735   123}, {1203, 75
+000067b0: 347d 7d09 0817 2531 3d49 606d 797a 7b7c  4}}...%1=I`myz{|
+000067c0: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+000067d0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+000067e0: 0000 9a00 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+000067f0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+00006800: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
+00006810: 7000 6500 6e00 6400 6500 7200 736c 6731  p.e.n.d.e.r.slg1
+00006820: 5363 6f6d 7000 0000 0000 0221 1f00 0000  Scomp......!....
+00006830: 1b00 7400 6800 6900 7200 6400 5f00 7000  ..t.h.i.r.d._.p.
+00006840: 6100 7200 7400 7900 5f00 6c00 6100 6200  a.r.t.y._.l.a.b.
+00006850: 6500 6c00 5f00 6100 7000 7000 6500 6e00  e.l._.a.p.p.e.n.
+00006860: 6400 6500 7200 736c 7376 4362 6c6f 6200  d.e.r.slsvCblob.
+00006870: 0002 7962 706c 6973 7430 30d8 0102 0304  ..ybplist00.....
+00006880: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
+00006890: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+000068a0: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+000068b0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+000068c0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+000068d0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+000068e0: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+000068f0: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+00006900: 0109 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
+00006910: 0e0f 100a 120a 1457 7669 7369 626c 6555  .......WvisibleU
+00006920: 7769 6474 6859 6173 6365 6e64 696e 675a  widthYascendingZ
+00006930: 6964 656e 7469 6669 6572 0911 01a6 0954  identifier.....T
+00006940: 6e61 6d65 d40d 0e0f 1016 1716 1908 1023  name...........#
+00006950: 0858 7562 6971 7569 7479 d40d 0e0f 100a  .Xubiquity......
+00006960: 1c16 1e09 10b5 085c 6461 7465 4d6f 6469  .......\dateModi
+00006970: 6669 6564 d40d 0e0f 1016 1c16 2208 085b  fied........"..[
+00006980: 6461 7465 4372 6561 7465 64d4 0d0e 0f10  dateCreated.....
+00006990: 0a25 1627 0910 6108 5473 697a 65d4 0d0e  .%.'..a.Tsize...
+000069a0: 0f10 0a2a 0a2c 0910 7309 546b 696e 64d4  ...*.,..s.Tkind.
+000069b0: 0d0e 0f10 162f 0a31 0810 6409 556c 6162  ...../.1..d.Ulab
+000069c0: 656c d40d 0e0f 1016 340a 3608 104b 0957  el......4.6..K.W
+000069d0: 7665 7273 696f 6ed4 0d0e 0f10 1639 0a3b  version......9.;
+000069e0: 0811 012c 0958 636f 6d6d 656e 7473 d40d  ...,.Xcomments..
+000069f0: 0e0f 1016 3e16 4008 10c8 085e 6461 7465  ....>.@....^date
+00006a00: 4c61 7374 4f70 656e 6564 d40d 0e0f 1016  LastOpened......
+00006a10: 1c16 4408 0859 6461 7465 4164 6465 6408  ..D..YdateAdded.
+00006a20: 2340 2800 0000 0000 0054 6e61 6d65 2340  #@(......Tname#@
+00006a30: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
+00006a40: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
+00006a50: 009b 00a4 00ac 00b2 00bc 00c7 00c8 00cb  ................
+00006a60: 00cc 00d1 00da 00db 00dd 00de 00e7 00f0  ................
+00006a70: 00f1 00f3 00f4 0101 010a 010b 010c 0118  ................
+00006a80: 0121 0122 0124 0125 012a 0133 0134 0136  .!.".$.%.*.3.4.6
+00006a90: 0137 013c 0145 0146 0148 0149 014f 0158  .7.<.E.F.H.I.O.X
+00006aa0: 0159 015b 015c 0164 016d 016e 0171 0172  .Y.[.\.d.m.n.q.r
+00006ab0: 017b 0184 0185 0187 0188 0197 01a0 01a1  .{..............
+00006ac0: 01a2 01ac 01ad 01b6 01bb 01c4 0000 0000  ................
+00006ad0: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+00006ae0: 0000 0000 0000 0000 0000 01c5 0000 001b  ................
+00006af0: 0074 0068 0069 0072 0064 005f 0070 0061  .t.h.i.r.d._.p.a
+00006b00: 0072 0074 0079 005f 006c 0061 0062 0065  .r.t.y._.l.a.b.e
+00006b10: 006c 005f 0061 0070 0070 0065 006e 0064  .l._.a.p.p.e.n.d
+00006b20: 0065 0072 0073 6c73 7670 626c 6f62 0000  .e.r.slsvpblob..
+00006b30: 025e 6270 6c69 7374 3030 d801 0203 0405  .^bplist00......
+00006b40: 0607 0809 0a0b 1d45 4647 0a5f 1012 7669  .......EFG._..vi
+00006b50: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00006b60: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00006b70: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00006b80: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00006b90: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00006ba0: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+00006bb0: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+00006bc0: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
+00006bd0: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
+00006be0: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00006bf0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00006c00: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00006c10: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00006c20: 6d65 d416 1718 191a 1b0a 1d55 696e 6465  me.........Uinde
+00006c30: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+00006c40: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+00006c50: d416 1718 191f 201d 1d10 0810 c808 08d4  ...... .........
+00006c60: 1617 1819 0924 1d0a 10b5 0809 d416 1718  .....$..........
+00006c70: 1928 241d 1d10 0208 08d4 1617 1819 2c2d  .($...........,-
+00006c80: 1d0a 1003 1061 0809 d416 1718 1931 320a  .....a.......12.
+00006c90: 1d10 0510 6409 08d4 1617 1819 3637 0a0a  ....d.......67..
+00006ca0: 1004 1073 0909 d416 1718 193b 3c0a 1d10  ...s.......;<...
+00006cb0: 0610 4b09 08d4 1617 1819 4041 0a0a 1000  ..K.......@A....
+00006cc0: 1101 a609 0908 2340 2800 0000 0000 0054  ......#@(......T
+00006cd0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00006ce0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
+00006cf0: 008c 008e 008f 00a2 00ab 00ba 00c7 00d3  ................
+00006d00: 00d8 00de 00e3 00eb 00f0 00f9 00ff 0105  ................
+00006d10: 010f 0117 0119 011c 011d 011e 0127 0129  .............'.)
+00006d20: 012b 012c 012d 0136 0138 0139 013a 0143  .+.,.-.6.8.9.:.C
+00006d30: 0145 0146 0147 0150 0152 0154 0155 0156  .E.F.G.P.R.T.U.V
+00006d40: 015f 0161 0163 0164 0165 016e 0170 0172  ._.a.c.d.e.n.p.r
+00006d50: 0173 0174 017d 017f 0181 0182 0183 018c  .s.t.}..........
+00006d60: 018e 0191 0192 0193 0194 019d 01a2 01ab  ................
+00006d70: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
+00006d80: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
+00006d90: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+00006da0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+00006db0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+00006dc0: 006e 0064 0065 0072 0073 6d6f 4444 626c  .n.d.e.r.smoDDbl
+00006dd0: 6f62 0000 0008 6874 98e3 46f2 c441 0000  ob....ht..F..A..
+00006de0: 001b 0074 0068 0069 0072 0064 005f 0070  ...t.h.i.r.d._.p
+00006df0: 0061 0072 0074 0079 005f 006c 0061 0062  .a.r.t.y._.l.a.b
+00006e00: 0065 006c 005f 0061 0070 0070 0065 006e  .e.l._.a.p.p.e.n
+00006e10: 0064 0065 0072 0073 6d6f 6444 626c 6f62  .d.e.r.smodDblob
+00006e20: 0000 0008 6874 98e3 46f2 c441 0000 001b  ....ht..F..A....
+00006e30: 0074 0068 0069 0072 0064 005f 0070 0061  .t.h.i.r.d._.p.a
+00006e40: 0072 0074 0079 005f 006c 0061 0062 0065  .r.t.y._.l.a.b.e
+00006e50: 006c 005f 0061 0070 0070 0065 006e 0064  .l._.a.p.p.e.n.d
+00006e60: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
+00006e70: 0000 0002 c000 0000 001b 0074 0068 0069  ...........t.h.i
+00006e80: 0072 0064 005f 0070 0061 0072 0074 0079  .r.d._.p.a.r.t.y
+00006e90: 005f 006c 0061 0062 0065 006c 005f 0061  ._.l.a.b.e.l._.a
+00006ea0: 0070 0070 0065 006e 0064 0065 0072 0073  .p.p.e.n.d.e.r.s
+00006eb0: 7653 726e 6c6f 6e67 0000 0001 0000 000c  vSrnlong........
+00006ec0: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+00006ed0: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
+00006ee0: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00006ef0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00006f00: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00006f10: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00006f20: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00006f30: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00006f40: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00006f50: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00006f60: 0809 5f10 197b 7b32 3630 2c20 3136 327d  .._..{{260, 162}
+00006f70: 2c20 7b31 3138 302c 2035 3538 7d7d 0908  , {1180, 558}}..
+00006f80: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+00006f90: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00006fa0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007000: 0000 0000 0000 0002 0000 0005 0000 0004  ................
 00007010: 0000 0014 0062 0061 0074 0063 0068 005f  .....b.a.t.c.h._
 00007020: 0070 0072 006f 0063 0065 0073 0073 005f  .p.r.o.c.e.s.s._
 00007030: 0076 0069 0064 0065 006f 0073 7653 726e  .v.i.d.e.o.svSrn
 00007040: 6c6f 6e67 0000 0001 0000 0005 0000 0012  long............
 00007050: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00007060: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 00007070: 0072 0073 6c73 7670 626c 6f62 0000 029d  .r.slsvpblob....
@@ -1880,170 +1880,170 @@
 00007570: 5301 5501 5e01 5f01 6101 6201 6b01 6c01  S.U.^._.a.b.k.l.
 00007580: 6d01 6f01 7801 7901 7b01 7c01 7e01 8701  m.o.x.y.{.|.~...
 00007590: 8801 8a01 8b01 8d01 9601 9701 9901 9a01  ................
 000075a0: 9c01 a501 a601 a801 a901 ab01 b401 b501  ................
 000075b0: b801 b901 bb01 bc01 c501 ce01 d701 dc01  ................
 000075c0: e500 0000 0000 0002 0100 0000 0000 0000  ................
 000075d0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
-000075e0: e600 0000 0700 0000 0900 7200 6f00 6900  ..........r.o.i.
-000075f0: 5f00 7400 6f00 6f00 6c00 7362 7773 7062  _.t.o.o.l.sbwspb
-00007600: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
-00007610: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00007620: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00007630: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00007640: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00007650: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00007660: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00007670: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00007680: 0808 0908 095f 1018 7b7b 3332 342c 2033  ....._..{{324, 3
-00007690: 327d 2c20 7b31 3235 302c 2037 3631 7d7d  2}, {1250, 761}}
-000076a0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
-000076b0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000076c0: 0000 0000 0000 0000 0000 0000 0000 009a  ................
-000076d0: 0000 0008 0000 001b 0074 0068 0069 0072  .........t.h.i.r
+000075e0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
+000075f0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
+00007600: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
+00007610: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
+00007620: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+00007630: 646c 6731 5363 6f6d 7000 0000 0000 06c2  dlg1Scomp.......
+00007640: 5369 005f 0074 006f 006f 006c 0073 6d6f  Si._.t.o.o.l.smo
+00007650: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
+00007660: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
+00007670: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
+00007680: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
+00007690: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
+000076a0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
+000076b0: 2000 0000 0009 0072 006f 0069 005f 0074   ......r.o.i._.t
+000076c0: 006f 006f 006c 0073 7653 726e 6c6f 6e67  .o.o.l.svSrnlong
+000076d0: 0000 0001 0000 001b 0074 0068 0069 0072  .........t.h.i.r
 000076e0: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
 000076f0: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
-00007700: 0070 0065 006e 0064 0065 0072 0073 6c73  .p.e.n.d.e.r.sls
-00007710: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-00007720: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00007730: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00007740: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00007750: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00007760: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00007770: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00007780: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00007790: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-000077a0: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-000077b0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-000077c0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-000077d0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-000077e0: 7209 1101 a609 546e 616d 65d4 0d0e 0f10  r.....Tname.....
-000077f0: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00007800: 79d4 0d0e 0f10 0a1c 161e 0910 b508 5c64  y.............\d
-00007810: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
-00007820: 161c 1622 0808 5b64 6174 6543 7265 6174  ..."..[dateCreat
-00007830: 6564 d40d 0e0f 100a 2516 2709 1061 0854  ed......%.'..a.T
-00007840: 7369 7a65 d40d 0e0f 100a 2a0a 2c09 1073  size......*.,..s
-00007850: 0954 6b69 6e64 d40d 0e0f 1016 2f0a 3108  .Tkind....../.1.
-00007860: 1064 0955 6c61 6265 6cd4 0d0e 0f10 1634  .d.Ulabel......4
-00007870: 0a36 0810 4b09 5776 6572 7369 6f6e d40d  .6..K.Wversion..
-00007880: 0e0f 1016 390a 3b08 1101 2c09 5863 6f6d  ....9.;...,.Xcom
-00007890: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
-000078a0: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-000078b0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
-000078c0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-000078d0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-000078e0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-000078f0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-00007900: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
-00007910: dd00 de00 e700 f000 f100 f300 f401 0101  ................
-00007920: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
-00007930: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
-00007940: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00007950: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00007960: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00007970: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00007980: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00007990: 0001 c500 0000 0000 0000 0000 0000 9a00  ................
-000079a0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
-000079b0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
-000079c0: 6731 5363 6f6d 7000 0000 0000 03b9 6300  g1Scomp.......c.
-000079d0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
-000079e0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
-000079f0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
-00007a00: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
-00007a10: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
-00007a20: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00007a30: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00007a40: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00007a50: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
-00007a60: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00007a70: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
-00007a80: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
-00007a90: 09ab 0c15 1a1f 2328 2d32 373c 41d4 0d0e  ......#(-27<A...
-00007aa0: 0f10 1112 0a0a 5a69 6465 6e74 6966 6965  ......Zidentifie
-00007ab0: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
-00007ac0: 6757 7669 7369 626c 6554 6e61 6d65 1102  gWvisibleTname..
-00007ad0: d009 09d4 0d0e 0f10 1617 1818 5875 6269  ............Xubi
-00007ae0: 7175 6974 7910 2308 08d4 0d0e 0f10 1b1c  quity.#.........
-00007af0: 180a 5c64 6174 654d 6f64 6966 6965 6410  ..\dateModified.
-00007b00: b508 09d4 0d0e 0f10 201c 1818 5b64 6174  ........ ...[dat
-00007b10: 6543 7265 6174 6564 0808 d40d 0e0f 1024  eCreated.......$
-00007b20: 2518 0a54 7369 7a65 1061 0809 d40d 0e0f  %..Tsize.a......
-00007b30: 1029 2a0a 0a54 6b69 6e64 1073 0909 d40d  .)*..Tkind.s....
-00007b40: 0e0f 102e 2f0a 1855 6c61 6265 6c10 6409  ..../..Ulabel.d.
-00007b50: 08d4 0d0e 0f10 3334 0a18 5776 6572 7369  ......34..Wversi
-00007b60: 6f6e 104b 0908 d40d 0e0f 1038 390a 1858  on.K.......89..X
-00007b70: 636f 6d6d 656e 7473 1101 2c09 08d4 0d0e  comments..,.....
-00007b80: 0f10 3d3e 1818 5e64 6174 654c 6173 744f  ..=>..^dateLastO
-00007b90: 7065 6e65 6410 c808 08d4 0d0e 0f10 421c  pened.........B.
-00007ba0: 1818 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
-00007bb0: 4028 0000 0000 0000 546e 616d 6509 1001  @(......Tname...
-00007bc0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00007bd0: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
-00007be0: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
-00007bf0: 00ec 00ed 00ee 00f7 0104 0106 0107 0108  ................
-00007c00: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
-00007c10: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
-00007c20: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
-00007c30: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
-00007c40: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
-00007c50: 01c2 01c3 0000 0000 0000 0201 0000 0000  ................
-00007c60: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00007c70: 0000 01c5 0000 000e 0070 006f 0073 0065  .........p.o.s.e
-00007c80: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
-00007c90: 0072 0073 6c73 7670 626c 6f62 0000 025e  .r.slsvpblob...^
-00007ca0: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-00007cb0: 0809 0a0b 1a46 470a 2758 6963 6f6e 5369  .....FG.'XiconSi
-00007cc0: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
-00007cd0: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00007ce0: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00007cf0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00007d00: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-00007d10: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-00007d20: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-00007d30: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
-00007d40: 151e 2328 2c31 363b 4058 636f 6d6d 656e  ..#(,16;@Xcommen
-00007d50: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-00007d60: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-00007d70: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00007d80: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00007d90: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
-00007da0: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00007db0: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-00007dc0: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-00007dd0: c808 1008 d416 1718 190a 251a 2709 10b5  ..........%.'...
-00007de0: 0810 01d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
-00007df0: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
-00007e00: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
-00007e10: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
-00007e20: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
-00007e30: 190a 420a 4409 1102 d009 1000 0823 4028  ..B.D........#@(
-00007e40: 0000 0000 0000 546e 616d 6509 0008 0019  ......Tname.....
-00007e50: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00007e60: 0095 0096 00a9 00b2 00c1 00ce 00da 00df  ................
-00007e70: 00e5 00ea 00f2 00f7 0100 0108 010e 0118  ................
-00007e80: 011e 011f 0122 0123 0125 012e 012f 0131  .....".#.%.../.1
-00007e90: 0132 0134 013d 013e 0140 0141 0143 014c  .2.4.=.>.@.A.C.L
-00007ea0: 014d 014e 0150 0159 015a 015c 015d 015f  .M.N.P.Y.Z.\.]._
-00007eb0: 0168 0169 016b 016c 016e 0177 0178 017a  .h.i.k.l.n.w.x.z
-00007ec0: 017b 017d 0186 0187 0189 018a 018c 0195  .{.}............
-00007ed0: 0196 0199 019a 019c 019d 01a6 01ab 0000  ................
-00007ee0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-00007ef0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-00007f00: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
-00007f10: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-00007f20: 4444 626c 6f62 0000 0008 0b30 86dc dcf4  DDblob.....0....
-00007f30: c441 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
-00007f40: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
-00007f50: 0073 6d6f 6444 626c 6f62 0000 0008 be76  .smodDblob.....v
-00007f60: 2985 44f2 c441 0000 000e 0070 006f 0073  ).D..A.....p.o.s
-00007f70: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
-00007f80: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00007f90: 0000 0004 4000 0000 000e 0070 006f 0073  ....@......p.o.s
-00007fa0: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
-00007fb0: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
-00007fc0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008000: 0000 0000                                ....
+00007700: 0070 0065 006e 0064 0065 0072 0073 6277  .p.e.n.d.e.r.sbw
+00007710: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
+00007720: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00007730: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00007740: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00007750: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00007760: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00007770: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00007780: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00007790: 6261 7208 0809 0809 5f10 187b 7b33 322c  bar....._..{{32,
+000077a0: 2031 3233 7d2c 207b 3132 3033 2c20 3735   123}, {1203, 75
+000077b0: 347d 7d09 0817 2531 3d49 606d 797a 7b7c  4}}...%1=I`myz{|
+000077c0: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+000077d0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+000077e0: 0000 9a00 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+000077f0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+00007800: 6c00 6100 0000 0009 0000 0000 0000 780b  l.a...........x.
+00007810: 0000 0045 0000 100c 0000 700b 0000 200c  ...E......p... .
+00007820: 0000 300c 0000 400c 0000 500c 0000 600c  ..0...@...P...`.
+00007830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000078f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000079f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00007c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00007c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00007c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00007c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
+00007c60: 0100 0008 0000 0000 0000 0000 0000 0000  ................
+00007c70: 0000 0000 0100 0080 0000 0000 0100 0100  ................
+00007c80: 0000 0000 0100 0200 0000 0000 0100 0400  ................
+00007c90: 0000 0000 0100 0800 0000 0000 0100 1000  ................
+00007ca0: 0000 0000 0100 2000 0000 0000 0100 4000  ...... .......@.
+00007cb0: 0000 0000 0100 8000 0000 0000 0101 0000  ................
+00007cc0: 0000 0000 0102 0000 0000 0000 0104 0000  ................
+00007cd0: 0000 0000 0108 0000 0000 0000 0110 0000  ................
+00007ce0: 0000 0000 0120 0000 0000 0000 0140 0000  ..... .......@..
+00007cf0: 0000 0000 0009 1101 2709 1000 0823 4048  ........'....#@H
+00007d00: 0000 0000 0000 2340 2800 0000 0000 0023  ......#@(......#
+00007d10: 0000 0000 0000 0000 546e 616d 6523 4030  ........Tname#@0
+00007d20: 0000 0000 0000 0900 0800 1d00 3200 4400  ............2.D.
+00007d30: 4c00 6000 7200 7b00 8d00 9800 a100 b400  L.`.r.{.........
+00007d40: b600 b700 ca00 d300 e200 ef00 fb01 0001  ................
+00007d50: 0601 0b01 1301 1801 2101 2901 2f01 3901  ........!.)./.9.
+00007d60: 3f01 4001 4301 4401 4601 4f01 5001 5201  ?.@.C.D.F.O.P.R.
+00007d70: 5301 5501 5e01 5f01 6101 6201 6b01 6c01  S.U.^._.a.b.k.l.
+00007d80: 6d01 6f01 7801 7901 7b01 7c01 7e01 8701  m.o.x.y.{.|.~...
+00007d90: 8801 8a01 8b01 8d01 9601 9701 9901 9a01  ................
+00007da0: 9c01 a501 a601 a801 a901 ab01 b401 b501  ................
+00007db0: b801 b901 bb01 bc01 c501 ce01 d701 dc01  ................
+00007dc0: e500 0000 0000 0002 0100 0000 0000 0000  ................
+00007dd0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
+00007de0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
+00007df0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
+00007e00: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
+00007e10: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
+00007e20: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+00007e30: 646c 6731 5363 6f6d 7000 0000 0000 06c2  dlg1Scomp.......
+00007e40: 5369 005f 0074 006f 006f 006c 0073 6d6f  Si._.t.o.o.l.smo
+00007e50: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
+00007e60: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
+00007e70: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
+00007e80: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
+00007e90: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
+00007ea0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
+00007eb0: 2000 0000 0009 0072 006f 0069 005f 0074   ......r.o.i._.t
+00007ec0: 006f 006f 006c 0073 7653 726e 6c6f 6e67  .o.o.l.svSrnlong
+00007ed0: 0000 0001 0000 001b 0074 0068 0069 0072  .........t.h.i.r
+00007ee0: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
+00007ef0: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
+00007f00: 0070 0065 006e 0064 0065 0072 0073 6277  .p.e.n.d.e.r.sbw
+00007f10: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
+00007f20: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00007f30: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00007f40: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00007f50: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00007f60: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00007f70: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00007f80: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00007f90: 6261 7208 0809 0809 5f10 187b 7b33 322c  bar....._..{{32,
+00007fa0: 2031 3233 7d2c 207b 3132 3033 2c20 3735   123}, {1203, 75
+00007fb0: 347d 7d09 0817 2531 3d49 606d 797a 7b7c  4}}...%1=I`myz{|
+00007fc0: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+00007fd0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+00007fe0: 0000 9a00 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+00007ff0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+00008000: 6c00 6100                                l.a.
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -276,18 +276,18 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 000b e20e 0000 000b 005f 005f 0070  ..........._._.p
+000011a0: 0000 000b e224 0000 000b 005f 005f 0070  .....$....._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 4cb8 15d8  moDDblob....L...
-000011d0: dcf4 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 00ee c752  moDDblob.......R
+000011d0: eaf6 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 000011f0: 6444 626c 6f62 0000 0008 0a8c 6973 23f2  dDblob......is#.
 00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 000c 9000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
@@ -302,15 +302,15 @@
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
 000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
 00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
 00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
 00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
-00001340: 3153 636f 6d70 0000 0000 0002 7de8 0000  1Scomp......}...
+00001340: 3153 636f 6d70 0000 0000 0002 7de9 0000  1Scomp......}...
 00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
 00001360: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
 00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
 00001380: 4a4b 0c5f 1012 7669 6577 4f70 7469 6f6e  JK._..viewOption
 00001390: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 000013a0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 000013b0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -391,15 +391,15 @@
 00001860: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
 00001870: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
 00001880: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
 00001890: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
 000018a0: d301 dc00 0000 0000 0002 0100 0000 0000  ................
 000018b0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 000018c0: 0001 dd00 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
-000018d0: 6f44 4462 6c6f 6200 0000 081a 1af6 afc4  oDDblob.........
+000018d0: 6f44 4462 6c6f 6200 0000 08d6 e178 04e6  oDDblob......x..
 000018e0: f6c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
 000018f0: 6f64 4462 6c6f 6200 0000 081a 1af6 afc4  odDblob.........
 00001900: f6c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
 00001910: 6831 5363 6f6d 7000 0000 0000 0360 0000  h1Scomp......`..
 00001920: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
 00001930: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.56.8/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.56.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/severity_processor.py` & `Simba-UW-tf-dev-1.56.8/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.56.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.56.8/simba/mixins/config_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from datetime import datetime
 
 class ConfigReader(object):
     def __init__(self,
                  config_path: str,
                  read_video_info: bool=True):
 
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
+        self.timer = SimbaTimer(start=True)
         self.config = read_config_file(ini_path=config_path)
         self.config_path = config_path
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.input_csv_dir = os.path.join(self.project_path, Paths.INPUT_CSV.value)
         self.features_dir = os.path.join(self.project_path, Paths.FEATURES_EXTRACTED_DIR.value)
         self.targets_folder = os.path.join(self.project_path, Paths.TARGETS_INSERTED_DIR.value)
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.56.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.56.8/simba/mixins/unsupervised_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from simba.read_config_unit_tests import check_float
 import simba
 from simba.enums import Paths
 from sklearn.feature_selection import VarianceThreshold
 from simba.unsupervised.enums import Unsupervised
 import pandas as pd
 from datetime import datetime
+import numpy as np
 from sklearn.preprocessing import (MinMaxScaler,
                                    StandardScaler,
                                    QuantileTransformer)
 from simba.utils.errors import (InvalidInputError,
                                 NoDataError,
                                 NoFilesFoundError,
                                 InvalidFileTypeError,
-                                MissingColumnsError)
+                                MissingColumnsError,
+                                IntegerError)
 
 
 class UnsupervisedMixin(object):
     def __init__(self):
 
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.timer = SimbaTimer()
@@ -84,15 +86,27 @@
             return StandardScaler()
         elif scaler_name == Unsupervised.QUANTILE.value:
             return QuantileTransformer()
 
     def scaler_transform(self, data: pd.DataFrame, scaler: MinMaxScaler or StandardScaler or QuantileTransformer):
         return pd.DataFrame(scaler.transform(data), columns=data.columns).set_index(data.index)
 
+    def scaler_inverse_transform(self, data: pd.DataFrame, scaler=MinMaxScaler or StandardScaler or QuantileTransformer):
+        return pd.DataFrame(scaler.inverse_transform(data), columns=data.columns).set_index(data.index)
+
     def check_expected_fields(self, data_fields: list, expected_fields: list):
         remaining_fields = [x for x in data_fields if x not in expected_fields]
         if len(remaining_fields) > 0:
             raise MissingColumnsError(f'The data contains {str(len(remaining_fields))} unexpected field(s): {str(remaining_fields)}')
 
     def check_key_exist_in_object(self, object: dict, key: str):
         if key not in object.keys():
-            raise InvalidInputError(msg=f'{key} does not exist in object')
+            raise InvalidInputError(msg=f'{key} does not exist in object')
+
+    def get_cluster_cnt(self,
+                        data: np.array,
+                        clusterer_name: str,
+                        minimum_clusters: int = 1) -> int:
+        cnt = np.unique(data).shape[0]
+        if cnt < minimum_clusters:
+            raise IntegerError(msg=f'Clustrer {clusterer_name} has {str(cnt)} clusters, but {str(minimum_clusters)} clusters is required for the operation.')
+        return cnt
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.56.8/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.56.8/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.56.8/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.56.8/simba/FSTTC_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             data_df = self.out_df[self.out_df['Value'] != 'No events'].reset_index(drop=True)
             data_df['Value'] = pd.to_numeric(data_df['Value'], errors='coerce')
             figure_FSCTT = sns.violinplot(x="FSTTC", y="Value", data=data_df, cut=0)
             figure_FSCTT.set_xticklabels(figure_FSCTT.get_xticklabels(), rotation=45, size=7)
             figure_FSCTT.figure.set_size_inches(13.7, 8.27)
             save_plot_path = os.path.join(self.logs_path, 'FSTTC_{}.png'.format(str(self.datetime)))
             figure_FSCTT.figure.savefig(save_plot_path, bbox_inches="tight")
-            stdout_success(msg='FSTTC figure saved at {save_plot_path}')
+            stdout_success(msg=f'FSTTC figure saved at {save_plot_path}')
 
 
 # test = FSTTCPerformer(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini',
 #                      time_window=2,
 #                      behavior_lst=['Attack', 'Sniffing'],
 #                     create_graphs=True)
 # test.find_sequences()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.56.8/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/video_info_table.py` & `Simba-UW-tf-dev-1.56.8/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.56.8/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.56.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.56.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.56.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.56.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.56.8/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.56.8/simba/train_model_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                                 CorruptedFileError,
                                 FeatureNumberMismatchError,
                                 ClassifierInferenceError,
                                 CountError)
 from simba.utils.warnings import (NotEnoughDataWarning,
                                   NoModuleWarning,
                                   MissingUserInputWarning)
+from simba.utils.printing import stdout_success
 from simba.utils.lookups import get_meta_data_file_headers
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
@@ -660,16 +661,15 @@
 
     Returns
     -------
 
     """
 
     print('Calculating SHAP values...')
-    timer = SimbaTimer()
-    timer.start_timer()
+    shap_timer = SimbaTimer(start=True)
     data_df = pd.concat([x_df, y_df], axis=1)
     if save_file_no == None:
         out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
         out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
     else:
         out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
         out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
@@ -688,32 +688,35 @@
     explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
     expected_value = explainer.expected_value[1]
     out_df_raw = pd.DataFrame(columns=x_names)
     shap_headers = list(x_names)
     shap_headers.extend(('Expected_value', 'Sum', 'Prediction_probability', clf_name))
     out_df_shap = pd.DataFrame(columns=shap_headers)
     for cnt, frame in enumerate(range(len(shap_df))):
+        shap_frm_timer = SimbaTimer(start=True)
         frame_data = shap_df.iloc[[frame]]
         frame_shap = explainer.shap_values(frame_data, check_additivity=False)[1][0].tolist()
         frame_shap.extend((expected_value, sum(frame_shap), rf_clf.predict_proba(frame_data)[0][1], y_df[cnt]))
         out_df_raw.loc[len(out_df_raw)] = list(shap_df.iloc[frame])
         out_df_shap.loc[len(out_df_shap)] = frame_shap
-        if (cnt % save_it == 0) or (cnt == len(shap_df)-1):
+        if (cnt % save_it == 0) or (cnt == len(shap_df)-1) and (cnt != 0):
             print(f'Saving SHAP data after {cnt} iterations...')
             out_df_shap.to_csv(out_df_shap_path)
             out_df_raw.to_csv(out_df_raw_path)
-        print('SHAP frame: {} / {}'.format(str(cnt + 1), str(len(shap_df))))
+        shap_frm_timer.stop_timer()
+        print(f'SHAP frame: {cnt+1} / {len(shap_df)}, elapsed time: {shap_frm_timer.elapsed_time_str}...')
 
+    shap_timer.stop_timer()
+    stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
     _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                           classifier_name=clf_name,
                                           shap_df=out_df_shap,
-                                          shap_baseline_value=expected_value*100,
+                                          shap_baseline_value=int(expected_value * 100),
                                           save_path=save_path)
-    timer.stop_timer()
-    print('SHAP calculations complete (elapsed time: {}s) ...'.format(timer.elapsed_time_str))
+
 
 
 def print_machine_model_information(model_dict: dict):
     """
     Helper to print model information in tabular form.
 
     Parameters
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.56.8/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.56.8/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/movement_processor.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,119 @@
-__author__ = "Simon Nilsson"
-
+from datetime import datetime
+from simba.read_config_unit_tests import (read_config_entry,
+                                          read_config_file,
+                                          read_project_path_and_file_type)
+from simba.feature_extractors.unit_tests import (read_video_info_csv,
+                                               read_video_info)
+import os
 import pandas as pd
+from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.misc_tools import (get_fn_ext,
-                              framewise_euclidean_distance,
+                              SimbaTimer,
                               )
 from simba.utils.printing import stdout_success
-from simba.feature_extractors.unit_tests import read_video_info
-from simba.read_config_unit_tests import (read_config_entry,
-                                          check_if_filepath_list_is_empty)
-from simba.utils.errors import NoSpecifiedOutputError
-from simba.enums import ReadConfig
-import os
-from simba.mixins.config_reader import ConfigReader
-from collections import defaultdict
+from simba.enums import ReadConfig, Paths, DirNames, Dtypes
 from simba.rw_dfs import read_df
-import numpy as np
-from statistics import mean
+import itertools
 
-class MovementProcessor(ConfigReader):
+class ROITimebinCalculator(object):
     """
-    Class for computing aggregate movement statistics.
+    Class for calulating how much time and how many entries animals are making into user-defined ROIs
+    in user-defined time bins. Results are stored in the `project_folder/logs` directory of the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
+    bin_length: int
+        length of time bins in seconds.
 
     Notes
     ----------
 
     Examples
     ----------
-    >>> movement_processor = MovementProcessor(config_path='MyConfigPath')
-    >>> movement_processor.process_movement()
-    >>> movement_processor.save_results()
-
+    >>> roi_time_bin_calculator = ROITimebinCalculator(config_path='MySimBaConfigPath', bin_length=15)
+    >>> roi_time_bin_calculator.analyze_time_bins()
+    >>> roi_time_bin_calculator.save_results()
     """
 
     def __init__(self,
                  config_path: str,
-                 visualization: bool = False,
-                 files: list=None):
+                 bin_length: int):
 
-        super().__init__(config_path=config_path)
-        self.save_path = os.path.join(self.logs_path, 'Movement_log_{}.csv'.format(self.datetime))
-        try:
-            self.animal_cnt = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'no_of_animals', 'int')
-            self.p_threshold = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'probability_threshold', 'float')
-        except:
-            raise NoSpecifiedOutputError(msg='Please analyze movements before visualizing data.')
-        self.bp_dict = defaultdict(list)
-        self.bp_columns = []
-        if not visualization:
-            for cnt, animal in enumerate(self.multi_animal_id_list):
-                bp_name = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt+1), 'str')
-                if bp_name == 'None':
-                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
-                for c in ['_x', '_y', '_p']:
-                    self.bp_dict[animal].append(bp_name + c)
-                    self.bp_columns.append(bp_name + c)
-            check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
-                                            error_msg=f'SIMBA ERROR: Cannot process movement. ZERO data files found in the {self.outlier_corrected_dir} directory.')
-            self.files_found = self.outlier_corrected_paths
-        else:
-            for cnt in range(self.animal_cnt):
-                bp_name = read_config_entry(self.config, ReadConfig.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt+1), 'str')
-                if bp_name == 'None':
-                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
-                for c in ['_x', '_y', '_p']:
-                    self.bp_dict[self.multi_animal_id_list[cnt]].append(bp_name + c)
-                    self.bp_columns.append(bp_name + c)
-            self.files_found = files
-        print(f'Processing {str(len(self.outlier_corrected_paths))} video(s)...')
-
-    def process_movement(self):
-        """
-        Method to run movement aggregation computations.
-
-        Returns
-        ----------
-        Attribute: dict
-            results
-
-        """
-        self.results = {}
-        self.movement_dict = {}
-        for file_path in self.files_found:
-            _, video_name, _ = get_fn_ext(file_path)
-            print('Analysing {}...'.format(video_name))
-            self.data_df = read_df(file_path, self.file_type)[self.bp_columns]
-            self.video_info, self.px_per_mm, self.fps = read_video_info(vid_info_df=self.video_info_df, video_name=video_name)
-            self.results[video_name] = {}
-            self.movement_dict[video_name] = {}
-            for animal_name, animal_bps in self.bp_dict.items():
-                self.results[video_name][animal_name] = {}
-                animal_df = self.data_df[animal_bps]
-                if self.p_threshold > 0.00:
-                    animal_df = animal_df[animal_df[animal_bps[2]] >= self.p_threshold]
-                animal_df = animal_df.iloc[:, 0:2].reset_index(drop=True)
-                df_shifted = animal_df.shift(1)
-                df_shifted = df_shifted.combine_first(animal_df).add_suffix('_shifted')
-                animal_df = pd.concat([animal_df, df_shifted], axis=1)
-                bp_time_1 = animal_df[[animal_bps[0], animal_bps[1]]].values.astype(float)
-                bp_time_2 = animal_df[[animal_bps[0] + '_shifted', animal_bps[1] + '_shifted']].values.astype(float)
-                self.movement = pd.Series(framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=self.px_per_mm))
-                self.movement.loc[0] = 0
-                self.movement_dict[video_name][animal_name] = self.movement
-                self.results[video_name][animal_name]['Distance (cm)'] = round((self.movement.sum() / 10), 4)
-                velocity_lst = []
-                for df in np.array_split(self.movement, int(len(self.movement) / self.fps)):
-                    velocity_lst.append(df.sum())
-                self.results[video_name][animal_name]['Velocity (cm/s)'] = round((mean(velocity_lst) / 10), 4)
+        self.config_path, self.bin_length = config_path, bin_length
+        self.date_time = datetime.now().strftime('%Y%m%d%H%M%S')
+        self.config = read_config_file(config_path)
+        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
+        self.roi_animal_cnt = read_config_entry(config=self.config, section=ReadConfig.ROI_SETTINGS.value, option=ReadConfig.ROI_ANIMAL_CNT.value, data_type=Dtypes.INT.value)
+        self.probability_threshold = read_config_entry(config=self.config, section=ReadConfig.ROI_SETTINGS.value, option=ReadConfig.PROBABILITY_THRESHOLD.value, data_type=Dtypes.FLOAT.value,default_value=0.00)
+        self.logs_path = os.path.join(self.project_path, 'logs')
+        self.save_path_time = os.path.join(self.logs_path, 'ROI_time_bins_{}s_time_data_{}.csv'.format(str(bin_length), self.date_time))
+        self.save_path_entries = os.path.join(self.logs_path, 'ROI_time_bins_{}s_entry_data_{}.csv'.format(str(bin_length), self.date_time))
+        self.video_info_df = read_video_info_csv(file_path=os.path.join(self.project_path, Paths.VIDEO_INFO.value))
+        self.roi_analyzer = ROIAnalyzer(ini_path=self.config_path, data_path=DirNames.OUTLIER_MOVEMENT_LOCATION.value, calculate_distances=False)
+        self.roi_analyzer.read_roi_dfs()
+        self.roi_analyzer.analyze_ROIs()
+        self.shape_names = self.roi_analyzer.shape_names
+        self.animal_names = list(self.roi_analyzer.bp_dict.keys())
+        self.entries_exits_df = self.roi_analyzer.detailed_df
+        self.timer = SimbaTimer()
+        self.timer.start_timer()
+
+    def analyze_time_bins(self):
+        self.files_found = self.roi_analyzer.files_found
+        self.out_dict_time, self.out_dict_entries = {}, {}
+        print('Analyzing time-bin data for {} videos...'.format(str(len(self.files_found))))
+        for file_cnt, file_path in enumerate(self.files_found):
+            _, self.video_name, _ = get_fn_ext(filepath=file_path)
+            self.out_dict_time[self.video_name], self.out_dict_entries[self.video_name] = {}, {}
+            _, _, fps = read_video_info(vid_info_df=self.video_info_df, video_name=self.video_name)
+            frames_per_bin = int(fps * self.bin_length)
+            video_frms = list(range(0, len(read_df(file_path=file_path, file_type=self.file_type))))
+            frame_bins = [video_frms[i * frames_per_bin:(i + 1) * frames_per_bin] for i in range((len(video_frms) + frames_per_bin - 1) // frames_per_bin )]
+            self.video_data = self.entries_exits_df[self.entries_exits_df['VIDEO'] == self.video_name]
+            for animal_name, shape_name in list(itertools.product(self.animal_names, self.shape_names)):
+                self.results_time, self.results_entries = {}, {}
+                self.results_time[shape_name], self.results_entries[shape_name] = {}, {}
+                self.results_time[shape_name][animal_name], self.results_entries[shape_name][animal_name] = {}, {}
+                data_df = self.video_data.loc[(self.video_data['SHAPE'] == shape_name) & (self.video_data['ANIMAL'] == animal_name)]
+                entry_frms = list(data_df['ENTRY FRAMES'])
+                inside_shape_frms = [list(range(x, y)) for x, y in zip(list(data_df['ENTRY FRAMES'].astype(int)), list(data_df['EXIT FRAMES'].astype(int) + 1))]
+                inside_shape_frms = [i for s in inside_shape_frms for i in s]
+                for bin_cnt, bin_frms in enumerate(frame_bins):
+                    frms_inside_roi_in_timebin = [x for x in inside_shape_frms if x in bin_frms]
+                    entry_roi_in_timebin = [x for x in entry_frms if x in bin_frms]
+                    self.results_time[shape_name][animal_name][bin_cnt] = len(frms_inside_roi_in_timebin) / fps
+                    self.results_entries[shape_name][animal_name][bin_cnt] = len(entry_roi_in_timebin)
+                self.out_dict_time[self.video_name].update(self.results_time)
+                self.out_dict_entries[self.video_name].update(self.results_entries)
 
     def save_results(self):
-        """
-        Method to save movement aggregation data into the `project_folder/logs` directory
-        of the SimBA project.
-
-        Returns
-        ----------
-        None
-
-        """
-
-        self.out_df = pd.DataFrame(columns=['Video', 'Animal', 'Measurement', 'Value'])
-        for video, video_data in self.results.items():
-            for animal, animal_data in video_data.items():
-                for measure, mesure_val in animal_data.items():
-                    self.out_df.loc[len(self.out_df)] = [video, animal, measure, mesure_val]
-        self.out_df.set_index('Video').to_csv(self.save_path)
+        results_time_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'TIME INSIDE SHAPE (S)'])
+        results_entries_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'ENTRY COUNT'])
+        for video_name, video_data in self.out_dict_time.items():
+            for shape_name, shape_data in video_data.items():
+                for animal_name, animal_data in shape_data.items():
+                    for bin_name, bin_data in animal_data.items():
+                        results_time_df.loc[len(results_time_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
+        results_time_df['TIME INSIDE SHAPE (S)'] = results_time_df['TIME INSIDE SHAPE (S)'].round(6)
+        results_time_df.to_csv(self.save_path_time)
+        stdout_success(msg=f'ROI time bin time data saved at {self.save_path_time}')
+        for video_name, video_data in self.out_dict_entries.items():
+            for shape_name, shape_data in video_data.items():
+                for animal_name, animal_data in shape_data.items():
+                    for bin_name, bin_data in animal_data.items():
+                        results_entries_df.loc[len(results_entries_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
+        results_entries_df.to_csv(self.save_path_entries)
         self.timer.stop_timer()
-        stdout_success(msg= f'Movement log saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'ROI time bin entry data saved at {self.save_path_entries}', elapsed_time=self.timer.elapsed_time_str)
+
 
-#test = MovementProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
-# test.process_movement()
+# test = ROITimebinCalculator(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',bin_length=5)
+# test.analyze_time_bins()
 # test.save_results()
+
+
+# test = ROITimebinCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",bin_length=5)
+# test.analyze_time_bins()
+# test.save_results()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pybursts.py` & `Simba-UW-tf-dev-1.56.8/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.56.8/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.56.8/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.56.8/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.56.8/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/setting_menu.py` & `Simba-UW-tf-dev-1.56.8/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.56.8/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/run_inference.py` & `Simba-UW-tf-dev-1.56.8/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,25 @@
     Notes
     ----------
     `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/SHAP.md#step-3-interpreting-the-shap-value-ouput-generated-by-simba>`__.
     `Example output <https://github.com/sgoldenlab/simba/blob/master/images/example_shap_graph.png>`__.
 
     Example
     ----------
-    >>> _ = ShapAggregateStatisticsVisualizer(config_path='SimBAConfigFilePath', classifier_name='Attack', shap_df='ShapValueDataframe', shap_baseline_value=4, save_path='SaveDirectory')
+    >>> _ = ShapAggregateStatisticsVisualizer(config_path='SimBAConfigFilePath', classifier_name='Attack', shap_df='tests/test_data/test_shap/data/test_shap.csv', shap_baseline_value=4, save_path='SaveDirectory')
     """
 
     def __init__(self,
                 config_path: str,
                 classifier_name: str,
                 shap_df: pd.DataFrame,
-                shap_baseline_value: float,
+                shap_baseline_value: int,
                 save_path: str):
 
-        self.agg_stats_timer = SimbaTimer()
-        self.agg_stats_timer.start_timer()
+        self.agg_stats_timer = SimbaTimer(start=True)
         self.config = read_config_file(ini_path=config_path)
         bp_setting = read_config_entry(config=self.config, section=ReadConfig.CREATE_ENSEMBLE_SETTINGS.value, option=ReadConfig.POSE_SETTING.value, data_type=Dtypes.STR.value)
         if (bp_setting != '14') and (bp_setting != '16'):
             ShapWarning('SHAP visualizations/aggregate stats skipped (only viable for projects with two animals and default 7 or 8 body-parts per animal) ...')
         else:
             self.date_time, self.save_path = datetime.now().strftime('%Y%m%d%H%M%S'), save_path
             self.classifier_name, self.shap_df, self.shap_baseline_value = classifier_name, shap_df, shap_baseline_value
@@ -130,15 +129,15 @@
         baseline_scale_bottom_right = (self.baseline_scale_top_left[0] + self.baseline_scale_img.shape[0],
                                        self.baseline_scale_top_left[1] + self.baseline_scale_img.shape[1])
         baseline_scale_middle = ((int(700 + self.baseline_scale_img.shape[1] / 2)), 85)
         self.img[self.baseline_scale_top_left[0]:baseline_scale_bottom_right[0], self.baseline_scale_top_left[1]:baseline_scale_bottom_right[1]] = self.baseline_scale_img
         cv2.putText(self.img, 'BASELINE SHAP', baseline_scale_middle, cv2.FONT_HERSHEY_COMPLEX, 1, (0, 0, 0), 2)
 
         self.small_arrow_img = cv2.imread(self.scale_img_dict['small_arrow'])
-        small_arrow_top_left = (baseline_scale_bottom_right[0], int(self.baseline_scale_top_left[1] + (self.baseline_scale_img.shape[1] / 100) * (self.shap_baseline_value*100)))
+        small_arrow_top_left = (baseline_scale_bottom_right[0], int(self.baseline_scale_top_left[1] + (self.baseline_scale_img.shape[1] / 100) * (self.shap_baseline_value)))
         small_arrow_bottom_right = (small_arrow_top_left[0] + self.small_arrow_img.shape[0], small_arrow_top_left[1] + self.small_arrow_img.shape[1])
         self.img[small_arrow_top_left[0]:small_arrow_bottom_right[0], small_arrow_top_left[1]:small_arrow_bottom_right[1]] = self.small_arrow_img
 
         self.color_bar_img = cv2.imread(self.scale_img_dict['color_bar'])
 
         side_scale_img = cv2.imread(self.scale_img_dict['side_scale'])
         side_scale_top_left = (small_arrow_bottom_right[0] + 50, self.baseline_scale_top_left[1] - 50)
@@ -188,16 +187,23 @@
             if row_cnt != (len(list(self.category_img_dict.keys())) - 1):
                 self.arrow_start = (arrow_end[0], self.side_scale_y_tick_cords[row_cnt + 1][0])
 
         small_arrow_top_left = (int(arrow_end[1]) + 20, int(arrow_end[0] - self.small_arrow_img.shape[1] / 2))
         small_arrow_bottom_right = (small_arrow_top_left[0] + self.small_arrow_img.shape[0], small_arrow_top_left[1] + self.small_arrow_img.shape[1])
         self.img[small_arrow_top_left[0]:small_arrow_bottom_right[0], small_arrow_top_left[1]:small_arrow_bottom_right[1]] = self.small_arrow_img
         color_bar_top_left = (arrow_end[1] + self.small_arrow_img.shape[0] + 25, self.baseline_scale_top_left[1])
-        color_bar_bottom_right = (
-        color_bar_top_left[0] + self.color_bar_img.shape[0], color_bar_top_left[1] + self.color_bar_img.shape[1])
+        color_bar_bottom_right = (color_bar_top_left[0] + self.color_bar_img.shape[0], color_bar_top_left[1] + self.color_bar_img.shape[1])
         self.img[color_bar_top_left[0]:color_bar_bottom_right[0],color_bar_top_left[1]:color_bar_bottom_right[1]] = self.color_bar_img
 
         color_bar_middle = ((int(580 + self.baseline_scale_img.shape[1] / 2)), color_bar_bottom_right[0] + 50)
         cv2.putText(self.img, 'CLASSIFICATION PROBABILITY', color_bar_middle, cv2.FONT_HERSHEY_COMPLEX, 1, (0, 0, 0), 2)
         cv2.imwrite(self.img_save_path, self.img)
         self.visualization_timer.stop_timer()
-        stdout_success(msg=f'SHAP summary graph saved at {self.img_save_path}', elapsed_time=self.visualization_timer.elapsed_time_str)
+        stdout_success(msg=f'SHAP summary graph saved at {self.img_save_path}', elapsed_time=self.visualization_timer.elapsed_time_str)
+
+
+# shap_df = pd.read_csv('/Users/simon/Desktop/envs/simba_dev/tests/test_data/test_shap/data/test_shap.csv', index_col=0)
+# test = ShapAggregateStatisticsVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                          classifier_name='Attack',
+#                                          shap_df=shap_df,
+#                                          shap_baseline_value=40,
+#                                          save_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/logs/shap')
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.56.8/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.56.8/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/dash_app.py` & `Simba-UW-tf-dev-1.56.8/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.56.8/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.56.8/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.56.8/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/misc_tools.py` & `Simba-UW-tf-dev-1.56.8/simba/misc_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1147,14 +1147,19 @@
             'springgreen',
             'firebrick',
             'indigo'
             'white']
 
 
 class SimbaTimer(object):
+    def __init__(self,
+                 start: bool=False):
+        if start:
+            self.start_timer()
+
     def start_timer(self):
         self.timer = time.time()
 
     def stop_timer(self):
         if not hasattr(self, 'timer'):
             self.elapsed_time = -1
             self.elapsed_time_str = '-1'
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.8/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.56.8/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.56.8/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.56.8/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/pose_reset.py` & `Simba-UW-tf-dev-1.56.8/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.56.8/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.56.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.56.8/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.56.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.56.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.56.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.56.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.56.8/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.56.8/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.56.8/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.56.8/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/train_single_model.py` & `Simba-UW-tf-dev-1.56.8/simba/train_single_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         Returns
         ----------
         None
         """
 
         self.timer.stop_timer()
         save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out)
-        stdout_success(msg='Classifier {} saved in models/generated_models directory', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'Classifier {self.clf_name} saved in models/generated_models directory', elapsed_time=self.timer.elapsed_time_str)
         stdout_success(msg=f'Evaluation files are in models/generated_models/model_evaluations folders')
 
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
 # test.perform_sampling()
 # test.train_model()
 # test.save_model()
```

### Comparing `Simba-UW-tf-dev-1.56.7/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.56.8/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.56.8/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.56.8/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.56.8/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.7
+Version: 1.56.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -327,29 +327,24 @@
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
 simba/unsupervised/.DS_Store
 simba/unsupervised/cluster_statistics.py
 simba/unsupervised/cluster_visualizer.py
-simba/unsupervised/data_extractors.py
+simba/unsupervised/data_extractor.py
+simba/unsupervised/data_map.yaml
 simba/unsupervised/dataset_creator.py
-simba/unsupervised/dataset_creator_2.py
-simba/unsupervised/dbcv.py
+simba/unsupervised/dbcv_calculator.py
 simba/unsupervised/enums.py
-simba/unsupervised/grd_search_img_visualizer_2.py
+simba/unsupervised/grd_search_cluster_visualizer.py
 simba/unsupervised/hdbscan_clusterer.py
-simba/unsupervised/hdbscan_clusterer_2.py
-simba/unsupervised/misc.py
 simba/unsupervised/pop_up_classes.py
 simba/unsupervised/tsne.py
-simba/unsupervised/ui_tools.py
 simba/unsupervised/umap_embedder.py
-simba/unsupervised/umap_embedder_2.py
 simba/unsupervised/unsupervised_ui.py
 simba/unsupervised/visualizers.py
-simba/unsupervised/visualization_tools/vtk_embeddings.py
 simba/utils/.DS_Store
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
 simba/utils/warnings.py
```

### Comparing `Simba-UW-tf-dev-1.56.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/LICENSE.md` & `Simba-UW-tf-dev-1.56.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/README.md` & `Simba-UW-tf-dev-1.56.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.7/setup.py` & `Simba-UW-tf-dev-1.56.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.7",
+    version="1.56.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

