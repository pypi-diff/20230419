# Comparing `tmp/nerfstudio-0.2.0.tar.gz` & `tmp/nerfstudio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-0.2.0.tar", last modified: Mon Apr 17 16:19:31 2023, max compression
+gzip compressed data, was "nerfstudio-0.2.1.tar", last modified: Wed Apr 19 00:30:37 2023, max compression
```

## Comparing `nerfstudio-0.2.0.tar` & `nerfstudio-0.2.1.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.444048 nerfstudio-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-17 16:19:24.000000 nerfstudio-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/base_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/depth_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/sdf_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/semantic_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/dycheck_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/minimal_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfosr_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nuscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/phototourism_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/scannet_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/depth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/sdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20570 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/colmap_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/nerfstudio_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/exporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/marching_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/texture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/tsdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/base_field_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/field_components/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/cuda/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/spatial_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/temporal_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/temporal_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/instant_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/sdf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/generative/stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/scene_colliders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/base_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/depth_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfplayer_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfplayer_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/neus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/neus_facto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/dynamic_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/process_data/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/equirect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/hloc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/metashape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/polycam_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/process_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/realitycapture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/record3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/public/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio/viewer/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/leva_theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/server/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/nerfstudio/viewer/viser/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/message_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/blender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/blender/nerfstudio_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/datasets/process_nuscenes_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/add_nb_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/downloads/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/generative/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/generative/trace_stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/github/run_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35406 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/run_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/sync_viser_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:19:31.444048 nerfstudio-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-19 00:30:31.000000 nerfstudio-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.879915 nerfstudio-0.2.1/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.887915 nerfstudio-0.2.1/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/depth_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/sdf_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/semantic_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.891915 nerfstudio-0.2.1/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.891915 nerfstudio-0.2.1/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20570 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/nerfstudio_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.899915 nerfstudio-0.2.1/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/base_field_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.899915 nerfstudio-0.2.1/nerfstudio/field_components/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/cuda/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/temporal_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/temporal_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.903915 nerfstudio-0.2.1/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/instant_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.903915 nerfstudio-0.2.1/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/generative/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.907915 nerfstudio-0.2.1/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfplayer_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfplayer_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.915915 nerfstudio-0.2.1/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.919915 nerfstudio-0.2.1/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.919915 nerfstudio-0.2.1/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.875915 nerfstudio-0.2.1/nerfstudio/viewer/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/server/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/nerfstudio/viewer/viser/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.879915 nerfstudio-0.2.1/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/datasets/process_nuscenes_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/generative/trace_stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35406 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/sync_viser_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/tests/test_train.py
```

### Comparing `nerfstudio-0.2.0/LICENSE` & `nerfstudio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/PKG-INFO` & `nerfstudio-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.2.0
+Version: 0.2.1
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.0 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.1 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
 Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
```

### Comparing `nerfstudio-0.2.0/README.md` & `nerfstudio-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/__init__.py` & `nerfstudio-0.2.1/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/__init__.py` & `nerfstudio-0.2.1/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-0.2.1/nerfstudio/cameras/camera_optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/camera_paths.py` & `nerfstudio-0.2.1/nerfstudio/cameras/camera_paths.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/camera_utils.py` & `nerfstudio-0.2.1/nerfstudio/cameras/camera_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/cameras.py` & `nerfstudio-0.2.1/nerfstudio/cameras/cameras.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/lie_groups.py` & `nerfstudio-0.2.1/nerfstudio/cameras/lie_groups.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/cameras/rays.py` & `nerfstudio-0.2.1/nerfstudio/cameras/rays.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/configs/__init__.py` & `nerfstudio-0.2.1/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/configs/base_config.py` & `nerfstudio-0.2.1/nerfstudio/configs/base_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,17 +115,19 @@
     steps_per_log: int = 10
     """number of steps between logging stats"""
     max_buffer_size: int = 20
     """maximum history size to keep for computing running averages of stats.
      e.g. if 20, averages will be computed over past 20 occurrences."""
     local_writer: LocalWriterConfig = LocalWriterConfig(enable=True)
     """if provided, will print stats locally. if None, will disable printing"""
-    enable_profiler: bool = True
-    """whether to enable profiling code; prints speed of functions at the end of a program.
-    profiler logs run times of functions and prints at end of training"""
+    profiler: Literal["none", "basic", "pytorch"] = "basic"
+    """how to profile the code;
+        "basic" - prints speed of all decorated functions at the end of a program.
+        "pytorch" - same as basic, but it also traces few training steps.
+    """
 
 
 # Viewer related configs
 @dataclass
 class ViewerConfig(PrintableConfig):
     """Configuration for viewer instantiation"""
```

### Comparing `nerfstudio-0.2.0/nerfstudio/configs/config_utils.py` & `nerfstudio-0.2.1/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/configs/experiment_config.py` & `nerfstudio-0.2.1/nerfstudio/configs/experiment_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/configs/method_configs.py` & `nerfstudio-0.2.1/nerfstudio/configs/method_configs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/__init__.py` & `nerfstudio-0.2.1/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-0.2.1/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-0.2.1/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,24 +175,26 @@
 
 
     Attributes:
         train_count (int): the step number of our train iteration, needs to be incremented manually
         eval_count (int): the step number of our eval iteration, needs to be incremented manually
         train_dataset (Dataset): the dataset for the train dataset
         eval_dataset (Dataset): the dataset for the eval dataset
+        includes_time (bool): whether the dataset includes time information
 
         Additional attributes specific to each subclass are defined in the setup_train and setup_eval
         functions.
 
     """
 
     train_dataset: Optional[Dataset] = None
     eval_dataset: Optional[Dataset] = None
     train_sampler: Optional[DistributedSampler] = None
     eval_sampler: Optional[DistributedSampler] = None
+    includes_time: bool = False
 
     def __init__(self):
         """Constructor for the DataManager class.
 
         Subclassed DataManagers will likely need to override this constructor.
 
         If you aren't manually calling the setup_train and setup_eval functions from an overriden
@@ -403,14 +405,15 @@
         self.test_split = "test" if test_mode in ["test", "inference"] else "val"
         self.dataparser_config = self.config.dataparser
         if self.config.data is not None:
             self.config.dataparser.data = Path(self.config.data)
         else:
             self.config.data = self.config.dataparser.data
         self.dataparser = self.dataparser_config.setup()
+        self.includes_time = self.dataparser.includes_time
         self.train_dataparser_outputs = self.dataparser.get_dataparser_outputs(split="train")
 
         self.train_dataset = self.create_train_dataset()
         self.eval_dataset = self.create_eval_dataset()
 
         if self.train_dataparser_outputs is not None:
             cameras = self.train_dataparser_outputs.cameras
```

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datamanagers/depth_datamanager.py` & `nerfstudio-0.2.1/nerfstudio/data/datamanagers/depth_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datamanagers/sdf_datamanager.py` & `nerfstudio-0.2.1/nerfstudio/data/datamanagers/sdf_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datamanagers/semantic_datamanager.py` & `nerfstudio-0.2.1/nerfstudio/data/datamanagers/semantic_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/arkitscenes_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/base_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/base_dataparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,22 @@
 
 @dataclass
 class DataParser:
     """A dataset.
 
     Args:
         config: datasetparser config containing all information needed to instantiate dataset
+
+    Attributes:
+        config: datasetparser config containing all information needed to instantiate dataset
+        includes_time: Does the dataset include time information in the camera poses.
     """
 
     config: DataParserConfig
+    includes_time: bool = False
 
     def __init__(self, config: DataParserConfig):
         super().__init__()
         self.config = config
 
     @abstractmethod
     def _generate_dataparser_outputs(self, split: str = "train") -> DataparserOutputs:
```

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/blender_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/dnerf_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 
 @dataclass
 class DNeRF(DataParser):
     """DNeRF Dataset"""
 
     config: DNeRFDataParserConfig
+    includes_time: bool = True
 
     def __init__(self, config: DNeRFDataParserConfig):
         super().__init__(config=config)
         self.data: Path = config.data
         self.scale_factor: float = config.scale_factor
         self.alpha_color = config.alpha_color
```

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/dycheck_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/dycheck_dataparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 
 
 @dataclass
 class Dycheck(DataParser):
     """Dycheck (https://arxiv.org/abs/2210.13445) Dataset `iphone` subset"""
 
     config: DycheckDataParserConfig
+    includes_time: bool = True
 
     def __init__(self, config: DycheckDataParserConfig):
         super().__init__(config=config)
         self.data: Path = config.data
         self.scale_factor: float = config.scale_factor
         self.alpha_color = config.alpha_color
         # load extra info from "extra.json"
```

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/minimal_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/minimal_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfosr_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/nuscenes_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/phototourism_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/scannet_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/sdfstudio_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py` & `nerfstudio-0.2.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datasets/__init__.py` & `nerfstudio-0.2.1/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-0.2.1/nerfstudio/data/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datasets/depth_dataset.py` & `nerfstudio-0.2.1/nerfstudio/data/datasets/depth_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datasets/sdf_dataset.py` & `nerfstudio-0.2.1/nerfstudio/data/datasets/sdf_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-0.2.1/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/pixel_samplers.py` & `nerfstudio-0.2.1/nerfstudio/data/pixel_samplers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/scene_box.py` & `nerfstudio-0.2.1/nerfstudio/data/scene_box.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/utils/__init__.py` & `nerfstudio-0.2.1/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/utils/colmap_parsing_utils.py` & `nerfstudio-0.2.1/nerfstudio/data/utils/colmap_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/utils/data_utils.py` & `nerfstudio-0.2.1/nerfstudio/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-0.2.1/nerfstudio/data/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/data/utils/nerfstudio_collate.py` & `nerfstudio-0.2.1/nerfstudio/data/utils/nerfstudio_collate.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/engine/__init__.py` & `nerfstudio-0.2.1/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/engine/callbacks.py` & `nerfstudio-0.2.1/nerfstudio/engine/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/engine/optimizers.py` & `nerfstudio-0.2.1/nerfstudio/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/engine/schedulers.py` & `nerfstudio-0.2.1/nerfstudio/engine/schedulers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/engine/trainer.py` & `nerfstudio-0.2.1/nerfstudio/engine/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,29 +100,29 @@
         config: The configuration object.
         local_rank: Local rank of the process.
         world_size: World size of the process.
         device: The device to run the training on.
         pipeline: The pipeline object.
         optimizers: The optimizers object.
         callbacks: The callbacks object.
-        is_training: Whether the model is training.
+        training_state: Current model training state.
     """
 
     pipeline: VanillaPipeline
     optimizers: Optimizers
     callbacks: List[TrainingCallback]
 
     def __init__(self, config: TrainerConfig, local_rank: int = 0, world_size: int = 1) -> None:
         self.train_lock = Lock()
         self.config = config
         self.local_rank = local_rank
         self.world_size = world_size
         self.device: TORCH_DEVICE = "cpu" if world_size == 0 else f"cuda:{local_rank}"
         self.mixed_precision: bool = self.config.mixed_precision
-        self.is_training: bool = True
+        self.training_state: Literal["training", "paused", "completed"] = "training"
         if self.device == "cpu":
             self.mixed_precision = False
             CONSOLE.print("Mixed precision is disabled for CPU training.")
         self._start_step: int = 0
         # optimizers
         self.grad_scaler = GradScaler(enabled=self.mixed_precision)
 
@@ -180,15 +180,15 @@
         writer.setup_event_writer(
             self.config.is_wandb_enabled(), self.config.is_tensorboard_enabled(), log_dir=writer_log_path
         )
         writer.setup_local_writer(
             self.config.logging, max_iter=self.config.max_num_iterations, banner_messages=banner_messages
         )
         writer.put_config(name="config", config_dict=dataclasses.asdict(self.config), step=0)
-        profiler.setup_profiler(self.config.logging)
+        profiler.setup_profiler(self.config.logging, writer_log_path)
 
     def setup_optimizers(self) -> Optimizers:
         """Helper to set up the optimizers
 
         Returns:
             The optimizers object given the trainer config.
         """
@@ -212,15 +212,15 @@
         )
 
         self._init_viewer_state()
         with TimeWriter(writer, EventName.TOTAL_TRAIN_TIME):
             num_iterations = self.config.max_num_iterations
             step = 0
             for step in range(self._start_step, self._start_step + num_iterations):
-                while not self.is_training:
+                while self.training_state == "paused":
                     time.sleep(0.01)
                 with self.train_lock:
                     with TimeWriter(writer, EventName.ITER_TRAIN_TIME, step=step) as train_t:
                         self.pipeline.train()
 
                         # training callbacks before the training iteration
                         for callback in self.callbacks:
@@ -276,14 +276,16 @@
 
         # write out any remaining events (e.g., total train time)
         writer.write_out_storage()
 
         CONSOLE.rule()
         CONSOLE.print("[bold green]:tada: :tada: :tada: Training Finished :tada: :tada: :tada:", justify="center")
         if not self.config.viewer.quit_on_train_completion:
+            self.training_state = "completed"
+            self._train_complete_viewer()
             CONSOLE.print("Use ctrl+c to quit", justify="center")
             while True:
                 time.sleep(0.01)
 
     @check_main_thread
     def _check_viewer_warnings(self) -> None:
         """Helper to print out any warnings regarding the way the viewer/loggers are enabled"""
@@ -300,15 +302,15 @@
 
     @check_viewer_enabled
     def _init_viewer_state(self) -> None:
         """Initializes viewer scene with given train dataset"""
         assert self.viewer_state and self.pipeline.datamanager.train_dataset
         self.viewer_state.init_scene(
             dataset=self.pipeline.datamanager.train_dataset,
-            start_train=True,
+            train_state="training",
         )
 
     @check_viewer_enabled
     def _update_viewer_state(self, step: int) -> None:
         """Updates the viewer state by rendering out scene with current pipeline
         Returns the time taken to render scene.
 
@@ -320,14 +322,24 @@
         try:
             self.viewer_state.update_scene(step, num_rays_per_batch)
         except RuntimeError:
             time.sleep(0.03)  # sleep to allow buffer to reset
             CONSOLE.log("Viewer failed. Continuing training.")
 
     @check_viewer_enabled
+    def _train_complete_viewer(self) -> None:
+        """Let the viewer know that the training is complete"""
+        assert self.viewer_state is not None
+        try:
+            self.viewer_state.training_complete()
+        except RuntimeError:
+            time.sleep(0.03)  # sleep to allow buffer to reset
+            CONSOLE.log("Viewer failed. Continuing training.")
+
+    @check_viewer_enabled
     def _update_viewer_rays_per_sec(self, train_t: TimeWriter, vis_t: TimeWriter, step: int) -> None:
         """Performs update on rays/sec calculation for training
 
         Args:
             train_t: timer object carrying time to execute total training iteration
             vis_t: timer object carrying time to execute visualization step
             step: current step
```

### Comparing `nerfstudio-0.2.0/nerfstudio/exporter/__init__.py` & `nerfstudio-0.2.1/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/exporter/exporter_utils.py` & `nerfstudio-0.2.1/nerfstudio/exporter/exporter_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/exporter/marching_cubes.py` & `nerfstudio-0.2.1/nerfstudio/exporter/marching_cubes.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/exporter/texture_utils.py` & `nerfstudio-0.2.1/nerfstudio/exporter/texture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/exporter/tsdf_utils.py` & `nerfstudio-0.2.1/nerfstudio/exporter/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/__init__.py` & `nerfstudio-0.2.1/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/activations.py` & `nerfstudio-0.2.1/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/base_field_component.py` & `nerfstudio-0.2.1/nerfstudio/field_components/base_field_component.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/cuda/__init__.py` & `nerfstudio-0.2.1/nerfstudio/field_components/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/cuda/_backend.py` & `nerfstudio-0.2.1/nerfstudio/field_components/cuda/_backend.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/embedding.py` & `nerfstudio-0.2.1/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/encodings.py` & `nerfstudio-0.2.1/nerfstudio/field_components/encodings.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,17 +137,17 @@
 
         Args:
             in_tensor: For best performance, the input tensor should be between 0 and 1.
             covs: Covariances of input points.
         Returns:
             Output values will be between -1 and 1
         """
-        in_tensor = 2 * torch.pi * in_tensor  # scale to [0, 2pi]
+        scaled_in_tensor = 2 * torch.pi * in_tensor  # scale to [0, 2pi]
         freqs = 2 ** torch.linspace(self.min_freq, self.max_freq, self.num_frequencies).to(in_tensor.device)
-        scaled_inputs = in_tensor[..., None] * freqs  # [..., "input_dim", "num_scales"]
+        scaled_inputs = scaled_in_tensor[..., None] * freqs  # [..., "input_dim", "num_scales"]
         scaled_inputs = scaled_inputs.view(*scaled_inputs.shape[:-2], -1)  # [..., "input_dim" * "num_scales"]
 
         if covs is None:
             encoded_inputs = torch.sin(torch.cat([scaled_inputs, scaled_inputs + torch.pi / 2.0], dim=-1))
         else:
             input_var = torch.diagonal(covs, dim1=-2, dim2=-1)[..., :, None] * freqs[None, :] ** 2
             input_var = input_var.reshape((*input_var.shape[:-2], -1))
@@ -197,16 +197,16 @@
         Args:
             in_tensor: For best performance, the input tensor should be between 0 and 1.
             covs: Covariances of input points.
 
         Returns:
             Output values will be between -1 and 1
         """
-        in_tensor = 2 * torch.pi * in_tensor  # scale to [0, 2pi]
-        scaled_inputs = in_tensor @ self.b_matrix  # [..., "num_frequencies"]
+        scaled_in_tensor = 2 * torch.pi * in_tensor  # scale to [0, 2pi]
+        scaled_inputs = scaled_in_tensor @ self.b_matrix  # [..., "num_frequencies"]
 
         if covs is None:
             encoded_inputs = torch.sin(torch.cat([scaled_inputs, scaled_inputs + torch.pi / 2.0], dim=-1))
         else:
             input_var = torch.sum((covs @ self.b_matrix) * self.b_matrix, -2)
             encoded_inputs = expected_sin(
                 torch.cat([scaled_inputs, scaled_inputs + torch.pi / 2.0], dim=-1), torch.cat(2 * [input_var], dim=-1)
```

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/field_heads.py` & `nerfstudio-0.2.1/nerfstudio/field_components/field_heads.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/mlp.py` & `nerfstudio-0.2.1/nerfstudio/field_components/mlp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-0.2.1/nerfstudio/field_components/spatial_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/temporal_distortions.py` & `nerfstudio-0.2.1/nerfstudio/field_components/temporal_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/field_components/temporal_grid.py` & `nerfstudio-0.2.1/nerfstudio/field_components/temporal_grid.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/__init__.py` & `nerfstudio-0.2.1/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/base_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/density_fields.py` & `nerfstudio-0.2.1/nerfstudio/fields/density_fields.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/instant_ngp_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/instant_ngp_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/nerfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_nerfacto_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_nerfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_ngp_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_ngp_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/nerfw_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/nerfw_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/sdf_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/sdf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/semantic_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/tensorf_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/tensorf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-0.2.1/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/generative/__init__.py` & `nerfstudio-0.2.1/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/generative/stable_diffusion.py` & `nerfstudio-0.2.1/nerfstudio/generative/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/__init__.py` & `nerfstudio-0.2.1/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/losses.py` & `nerfstudio-0.2.1/nerfstudio/model_components/losses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/ray_generators.py` & `nerfstudio-0.2.1/nerfstudio/model_components/ray_generators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-0.2.1/nerfstudio/model_components/ray_samplers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/renderers.py` & `nerfstudio-0.2.1/nerfstudio/model_components/renderers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/scene_colliders.py` & `nerfstudio-0.2.1/nerfstudio/model_components/scene_colliders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/model_components/shaders.py` & `nerfstudio-0.2.1/nerfstudio/model_components/shaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/__init__.py` & `nerfstudio-0.2.1/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/base_model.py` & `nerfstudio-0.2.1/nerfstudio/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,20 +173,20 @@
         outputs_lists = defaultdict(list)
         for i in range(0, num_rays, num_rays_per_chunk):
             start_idx = i
             end_idx = i + num_rays_per_chunk
             ray_bundle = camera_ray_bundle.get_row_major_sliced_ray_bundle(start_idx, end_idx)
             outputs = self.forward(ray_bundle=ray_bundle)
             for output_name, output in outputs.items():  # type: ignore
+                if not torch.is_tensor(output):
+                    # TODO: handle lists of tensors as well
+                    continue
                 outputs_lists[output_name].append(output)
         outputs = {}
         for output_name, outputs_list in outputs_lists.items():
-            if not torch.is_tensor(outputs_list[0]):
-                # TODO: handle lists of tensors as well
-                continue
             outputs[output_name] = torch.cat(outputs_list).view(image_height, image_width, -1)  # type: ignore
         return outputs
 
     @abstractmethod
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
```

### Comparing `nerfstudio-0.2.0/nerfstudio/models/base_surface_model.py` & `nerfstudio-0.2.1/nerfstudio/models/base_surface_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/depth_nerfacto.py` & `nerfstudio-0.2.1/nerfstudio/models/depth_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/instant_ngp.py` & `nerfstudio-0.2.1/nerfstudio/models/instant_ngp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/mipnerf.py` & `nerfstudio-0.2.1/nerfstudio/models/mipnerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/nerfacto.py` & `nerfstudio-0.2.1/nerfstudio/models/nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/nerfplayer_nerfacto.py` & `nerfstudio-0.2.1/nerfstudio/models/nerfplayer_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/nerfplayer_ngp.py` & `nerfstudio-0.2.1/nerfstudio/models/nerfplayer_ngp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/neus.py` & `nerfstudio-0.2.1/nerfstudio/models/neus.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/neus_facto.py` & `nerfstudio-0.2.1/nerfstudio/models/neus_facto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-0.2.1/nerfstudio/models/semantic_nerfw.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/tensorf.py` & `nerfstudio-0.2.1/nerfstudio/models/tensorf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-0.2.1/nerfstudio/models/vanilla_nerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/pipelines/__init__.py` & `nerfstudio-0.2.1/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-0.2.1/nerfstudio/pipelines/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-0.2.1/nerfstudio/pipelines/dynamic_batch.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/plugins/__init__.py` & `nerfstudio-0.2.1/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/plugins/registry.py` & `nerfstudio-0.2.1/nerfstudio/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/plugins/types.py` & `nerfstudio-0.2.1/nerfstudio/plugins/types.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/__init__.py` & `nerfstudio-0.2.1/nerfstudio/process_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/colmap_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/colmap_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/equirect_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/equirect_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/hloc_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/hloc_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/metashape_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/metashape_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/polycam_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/polycam_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/process_data_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/process_data_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/realitycapture_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/realitycapture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/process_data/record3d_utils.py` & `nerfstudio-0.2.1/nerfstudio/process_data/record3d_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/__init__.py` & `nerfstudio-0.2.1/nerfstudio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/colormaps.py` & `nerfstudio-0.2.1/nerfstudio/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/colors.py` & `nerfstudio-0.2.1/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/comms.py` & `nerfstudio-0.2.1/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/decorators.py` & `nerfstudio-0.2.1/nerfstudio/utils/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 def check_profiler_enabled(func: Callable) -> Callable:
     """Decorator: check if profiler is enabled"""
 
     def wrapper(self, *args, **kwargs):
         ret = None
-        if self.config.enable_profiler:
+        if self.config.profiler != "none":
             ret = func(self, *args, **kwargs)
         return ret
 
     return wrapper
 
 
 def check_viewer_enabled(func: Callable) -> Callable:
```

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/eval_utils.py` & `nerfstudio-0.2.1/nerfstudio/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/install_checks.py` & `nerfstudio-0.2.1/nerfstudio/utils/install_checks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/io.py` & `nerfstudio-0.2.1/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/math.py` & `nerfstudio-0.2.1/nerfstudio/utils/math.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/misc.py` & `nerfstudio-0.2.1/nerfstudio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/plotly_utils.py` & `nerfstudio-0.2.1/nerfstudio/utils/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/poses.py` & `nerfstudio-0.2.1/nerfstudio/utils/poses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/printing.py` & `nerfstudio-0.2.1/nerfstudio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/rich_utils.py` & `nerfstudio-0.2.1/nerfstudio/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/scripts.py` & `nerfstudio-0.2.1/nerfstudio/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-0.2.1/nerfstudio/utils/tensor_dataclass.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/utils/writer.py` & `nerfstudio-0.2.1/nerfstudio/utils/writer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/__init__.py` & `nerfstudio-0.2.1/nerfstudio/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/app/package.json` & `nerfstudio-0.2.1/nerfstudio/viewer/app/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'23-04-18-0'"}*

```diff
@@ -81,9 +81,9 @@
         "eject": "react-scripts eject",
         "electron": "electron .",
         "lint": "eslint --ext .js,.jsx .",
         "lint:fix": "eslint --fix --ext .js,.jsx .",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "23-04-10-0"
+    "version": "23-04-18-0"
 }
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/app/run_deploy.py` & `nerfstudio-0.2.1/nerfstudio/viewer/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/leva_theme.json` & `nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/leva_theme.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/__init__.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/control_panel.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/control_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,22 @@
 from nerfstudio.viewer.viser import ViserServer
 
 
 class ControlPanel:
     """
     Initializes the control panel with all the elements
     Args:
+        time_enabled: whether or not the time slider should be enabled
         rerender_cb: a callback that will be called when the user changes a parameter that requires a rerender
             (eg train speed, max res, etc)
         crop_update_cb: a callback that will be called when the user changes the crop parameters
+        update_output_cb: a callback that will be called when the user changes the output render
     """
 
-    def __init__(self, rerender_cb: Callable, crop_update_cb: Callable, update_output_cb: Callable):
+    def __init__(self, time_enabled: bool, rerender_cb: Callable, crop_update_cb: Callable, update_output_cb: Callable):
         # elements holds a mapping from tag: [elements]
         self._elements_by_tag: DefaultDict[str, List[ViewerElement]] = defaultdict(lambda: [])
 
         self._train_speed = ViewerDropdown(
             "Train Speed", "Balanced", ["Fast", "Balanced", "Slow"], cb_hook=lambda han: self._train_speed_cb()
         )
         self._output_render = ViewerDropdown(
@@ -64,14 +66,16 @@
             "Crop Viewport",
             False,
             cb_hook=lambda han: [self.update_control_panel(), rerender_cb(han), crop_update_cb(han)],
         )
         self._background_color = ViewerRGB("| Background color", (38, 42, 55), cb_hook=crop_update_cb)
         self._crop_min = ViewerVec3("| Crop Min", (-1, -1, -1), 0.05, cb_hook=crop_update_cb)
         self._crop_max = ViewerVec3("| Crop Max", (1, 1, 1), 0.05, cb_hook=crop_update_cb)
+        self._time = ViewerSlider("Time", 0.0, 0.0, 1.0, 0.01, cb_hook=rerender_cb)
+        self._time_enabled = time_enabled
 
         self.add_element(self._train_speed)
         self.add_element(self._output_render)
         self.add_element(self._colormap)
         # colormap options
         self.add_element(self._invert, additional_tags=("colormap",))
         self.add_element(self._normalize, additional_tags=("colormap",))
@@ -82,14 +86,16 @@
         self.add_element(self._max_res)
         self.add_element(self._crop_viewport)
         # Crop options
         self.add_element(self._background_color, additional_tags=("crop",))
         self.add_element(self._crop_min, additional_tags=("crop",))
         self.add_element(self._crop_max, additional_tags=("crop",))
 
+        self.add_element(self._time, additional_tags=("time",))
+
     def _train_speed_cb(self) -> None:
         """Callback for when the train speed is changed"""
         if self.train_speed == "Fast":
             self._train_util.value = 0.95
             self._max_res.value = 256
         elif self.train_speed == "Balanced":
             self._train_util.value = 0.85
@@ -131,14 +137,15 @@
         Sets elements to be hidden or not based on the current state of the control panel
         """
         self._colormap.set_disabled(self.output_render == "rgb")
         for e in self._elements_by_tag["colormap"]:
             e.set_hidden(self.output_render == "rgb")
         for e in self._elements_by_tag["crop"]:
             e.set_hidden(not self.crop_viewport)
+        self._time.set_hidden(not self._time_enabled)
 
     def update_colormap_options(self, dimensions: int, dtype: type) -> None:
         """update the colormap options based on the current render
 
         Args:
             dimensions: the number of dimensions of the render
             dtype: the data type of the render
@@ -231,7 +238,17 @@
         """Returns the current background color"""
         return self._background_color.value
 
     @background_color.setter
     def background_color(self, value: Tuple[int, int, int]):
         """Sets the background color"""
         self._background_color.value = value
+
+    @property
+    def time(self) -> float:
+        """Returns the current background color"""
+        return self._time.value
+
+    @time.setter
+    def time(self, value: float):
+        """Sets the background color"""
+        self._time.value = value
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/gui_utils.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/gui_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/path.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/path.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/render_state_machine.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/render_state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         camera = Cameras(
             fx=intrinsics_matrix[0, 0],
             fy=intrinsics_matrix[1, 1],
             cx=intrinsics_matrix[0, 2],
             cy=intrinsics_matrix[1, 2],
             camera_type=camera_type,
             camera_to_worlds=camera_to_world[None, ...],
-            times=torch.tensor([0.0]),
+            times=torch.tensor([self.viewer.control_panel.time], dtype=torch.float32),
         )
         camera = camera.to(self.viewer.get_model().device)
 
         with (self.viewer.train_lock if self.viewer.train_lock is not None else contextlib.nullcontext()):
             camera_ray_bundle = camera.generate_rays(camera_indices=0, aabb_box=self.viewer.get_model().render_aabb)
 
             with TimeWriter(None, None, write=False) as vis_t:
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/state/node.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/state/state_node.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/utils.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_elements.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_state.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import numpy as np
 import torch
 from rich import box, style
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
+from typing_extensions import Literal
 
 from nerfstudio.configs import base_config as cfg
 from nerfstudio.data.datasets.base_dataset import InputDataset
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.models.base_model import Model
 from nerfstudio.pipelines.base_pipeline import Pipeline
 from nerfstudio.utils.decorators import check_main_thread, decorate_all
@@ -44,17 +45,18 @@
 from nerfstudio.viewer.server.viewer_elements import ViewerElement
 from nerfstudio.viewer.viser import ViserServer
 from nerfstudio.viewer.viser.messages import (
     CameraMessage,
     CameraPathOptionsRequest,
     CameraPathPayloadMessage,
     CropParamsMessage,
-    IsTrainingMessage,
     NerfstudioMessage,
     SaveCheckpointMessage,
+    TimeConditionMessage,
+    TrainingStateMessage,
 )
 
 if TYPE_CHECKING:
     from nerfstudio.engine.trainer import Trainer
 
 CONSOLE = Console(width=120)
 
@@ -106,36 +108,39 @@
             box=box.MINIMAL,
             title_style=style.Style(bold=True),
         )
         table.add_row("HTTP", f"[link={self.viewer_url}][blue]{self.viewer_url}[/link]")
 
         CONSOLE.print(Panel(table, title="[bold][yellow]Viewer[/bold]", expand=False))
 
+        self.include_time = self.pipeline.datamanager.includes_time
+
         # viewer specific variables
-        self.prev_moving = False
         self.output_type_changed = True
-        self.check_done_render = True
         self.step = 0
-        self.camera_moving = False
-        self.prev_camera_timestamp = 0
-        self.static_fps = 1.0
-        self.train_btn_state = True
+        self.train_btn_state: Literal["training", "paused", "completed"] = "training"
+        self._prev_train_state: Literal["training", "paused", "completed"] = "training"
 
         self.camera_message = None
 
-        self.viser_server = ViserServer(host="localhost", port=websocket_port)
+        self.viser_server = ViserServer(host="127.0.0.1", port=websocket_port)
 
-        self.viser_server.register_handler(IsTrainingMessage, self._handle_is_training)
+        self.viser_server.register_handler(TrainingStateMessage, self._handle_training_state_message)
         self.viser_server.register_handler(SaveCheckpointMessage, self._handle_save_checkpoint)
         self.viser_server.register_handler(CameraMessage, self._handle_camera_update)
         self.viser_server.register_handler(CameraPathOptionsRequest, self._handle_camera_path_option_request)
         self.viser_server.register_handler(CameraPathPayloadMessage, self._handle_camera_path_payload)
         self.viser_server.register_handler(CropParamsMessage, self._handle_crop_params_message)
+        if self.include_time:
+            self.viser_server.use_time_conditioning()
+            self.viser_server.register_handler(TimeConditionMessage, self._handle_time_condition_message)
 
-        self.control_panel = ControlPanel(self._interrupt_render, self._crop_params_update, self._output_type_change)
+        self.control_panel = ControlPanel(
+            self.include_time, self._interrupt_render, self._crop_params_update, self._output_type_change
+        )
         self.control_panel.install(self.viser_server)
 
         def nested_folder_install(folder_labels: List[str], element: ViewerElement):
             if len(folder_labels) == 0:
                 element.install(self.viser_server)
                 # also rewire the hook to rerender
                 prev_cb = element.cb_hook
@@ -172,38 +177,38 @@
         self.viser_server.send_crop_params(
             crop_enabled=self.control_panel.crop_viewport,
             crop_bg_color=self.control_panel.background_color,
             crop_scale=tuple(crop_scale.tolist()),
             crop_center=tuple(crop_center.tolist()),
         )
 
-    def _handle_is_training(self, message: NerfstudioMessage) -> None:
-        """Handle is_training message from viewer."""
-        assert isinstance(message, IsTrainingMessage)
-        self.is_training = message.is_training
-        self.train_btn_state = message.is_training
-        self.viser_server.set_is_training(message.is_training)
+    def _handle_training_state_message(self, message: NerfstudioMessage) -> None:
+        """Handle training state message from viewer."""
+        assert isinstance(message, TrainingStateMessage)
+        self.train_btn_state = message.training_state
+        self.training_state = message.training_state
+        self.viser_server.set_training_state(message.training_state)
 
     def _handle_save_checkpoint(self, message: NerfstudioMessage) -> None:
-        """Handle is_training message from viewer."""
+        """Handle save checkpoint message from viewer."""
         assert isinstance(message, SaveCheckpointMessage)
         if self.trainer is not None:
             self.trainer.save_checkpoint(self.step)
 
     def _handle_camera_update(self, message: NerfstudioMessage) -> None:
         """Handle camera update message from viewer."""
         assert isinstance(message, CameraMessage)
         self.camera_message = message
-        self.camera_moving = message.is_moving
         if message.is_moving:
             self.render_statemachine.action(RenderAction("move", self.camera_message))
-            self.is_training = False
+            if self.training_state == "training":
+                self.training_state = "paused"
         else:
             self.render_statemachine.action(RenderAction("static", self.camera_message))
-            self.is_training = self.train_btn_state
+            self.training_state = self.train_btn_state
 
     def _handle_camera_path_option_request(self, message: NerfstudioMessage) -> None:
         """Handle camera path option request message from viewer."""
         assert isinstance(message, CameraPathOptionsRequest)
         camera_path_dir = self.datapath / "camera_paths"
         if camera_path_dir.exists():
             all_path_dict = {}
@@ -229,26 +234,31 @@
         center = np.array(message.crop_center)
         scale = np.array(message.crop_scale)
         crop_min = center - scale / 2.0
         crop_max = center + scale / 2.0
         self.control_panel.crop_min = tuple(crop_min.tolist())
         self.control_panel.crop_max = tuple(crop_max.tolist())
 
+    def _handle_time_condition_message(self, message: NerfstudioMessage) -> None:
+        """Handle time conditioning message from viewer."""
+        assert isinstance(message, TimeConditionMessage)
+        self.control_panel.time = message.time
+
     @property
-    def is_training(self) -> bool:
-        """Get is_training flag from viewer."""
+    def training_state(self) -> Literal["training", "paused", "completed"]:
+        """Get training state flag."""
         if self.trainer is not None:
-            return self.trainer.is_training
-        return False
+            return self.trainer.training_state
+        return self.train_btn_state
 
-    @is_training.setter
-    def is_training(self, is_training: bool) -> None:
-        """Set is_training flag in viewer."""
+    @training_state.setter
+    def training_state(self, training_state: Literal["training", "paused", "completed"]) -> None:
+        """Set training state flag."""
         if self.trainer is not None:
-            self.trainer.is_training = is_training
+            self.trainer.training_state = training_state
 
     def _pick_drawn_image_idxs(self, total_num: int) -> list[int]:
         """Determine indicies of images to display in viewer.
 
         Args:
             total_num: total number of training images.
 
@@ -258,21 +268,20 @@
         if self.config.max_num_display_images < 0:
             num_display_images = total_num
         else:
             num_display_images = min(self.config.max_num_display_images, total_num)
         # draw indices, roughly evenly spaced
         return np.linspace(0, total_num - 1, num_display_images, dtype=np.int32).tolist()
 
-    def init_scene(self, dataset: InputDataset, start_train=True) -> None:
+    def init_scene(self, dataset: InputDataset, train_state=Literal["training", "paused", "completed"]) -> None:
         """Draw some images and the scene aabb in the viewer.
 
         Args:
             dataset: dataset to render in the scene
-            start_train: whether to start train when viewer init;
-                if False, only displays dataset until resume train is toggled
+            train_state: Current status of training
         """
         self.viser_server.send_file_path_info(
             config_base_dir=self.log_filename.parents[0],
             data_base_dir=self.datapath,
             export_path_name=self.log_filename.parent.stem,
         )
 
@@ -284,30 +293,34 @@
             camera_json = dataset.cameras.to_json(camera_idx=idx, image=bgr, max_size=100)
             self.viser_server.add_dataset_image(idx=f"{idx:06d}", json=camera_json)
 
         # draw the scene box (i.e., the bounding box)
         self.viser_server.update_scene_box(dataset.scene_box)
 
         # set the initial state whether to train or not
-        self.train_btn_state = start_train
-        self.viser_server.set_is_training(start_train)
+        self.train_btn_state = train_state
+        self.viser_server.set_training_state(train_state)
 
     def update_scene(self, step: int, num_rays_per_batch: Optional[int] = None) -> None:
         """updates the scene based on the graph weights
 
         Args:
             step: iteration step of training
             num_rays_per_batch: number of rays per batch, used during training
         """
         self.step = step
 
         if self.camera_message is None:
             return
 
-        if self.trainer is not None and self.trainer.is_training:
+        if (
+            self.trainer is not None
+            and self.trainer.training_state == "training"
+            and self.control_panel.train_util != 1
+        ):
             if (
                 EventName.TRAIN_RAYS_PER_SEC.value in GLOBAL_BUFFER["events"]
                 and EventName.VIS_RAYS_PER_SEC.value in GLOBAL_BUFFER["events"]
             ):
                 train_s = GLOBAL_BUFFER["events"][EventName.TRAIN_RAYS_PER_SEC.value]["avg"]
                 vis_s = GLOBAL_BUFFER["events"][EventName.VIS_RAYS_PER_SEC.value]["avg"]
                 train_util = self.control_panel.train_util
@@ -333,7 +346,12 @@
         if self.output_type_changed:
             self.control_panel.update_colormap_options(dimensions, dtype)
             self.output_type_changed = False
 
     def get_model(self) -> Model:
         """Returns the model."""
         return self.pipeline.model
+
+    def training_complete(self) -> None:
+        """Called when training is complete."""
+        self.training_state = "completed"
+        self.viser_server.set_training_state("completed")
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_utils.py` & `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/viser/__init__.py` & `nerfstudio-0.2.1/nerfstudio/viewer/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/viser/gui.py` & `nerfstudio-0.2.1/nerfstudio/viewer/viser/gui.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/viser/message_api.py` & `nerfstudio-0.2.1/nerfstudio/viewer/viser/message_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -435,21 +435,21 @@
 
         Args:
             idx: The index of the image.
             json: The json dict from the camera frustum and image.
         """
         self._queue(messages.DatasetImageMessage(idx=idx, json=json))
 
-    def set_is_training(self, is_training: bool) -> None:
+    def set_training_state(self, training_state: Literal["training", "paused", "completed"]) -> None:
         """Set the training mode.
 
         Args:
-            is_training: The training mode.
+            training_state: The training mode.
         """
-        self._queue(messages.IsTrainingMessage(is_training=is_training))
+        self._queue(messages.TrainingStateMessage(training_state=training_state))
 
     def send_camera_paths(self, camera_paths: Dict[str, Any]) -> None:
         """Send camera paths to the scene.
 
         Args:
             camera_paths: A dictionary of camera paths.
         """
@@ -528,14 +528,18 @@
                 name=name,
                 folder_labels=tuple(self._gui_folder_labels),
                 leva_conf=leva_conf,
             )
         )
         return GuiHandle(handle_state)
 
+    def use_time_conditioning(self) -> None:
+        """Use time conditioning."""
+        self._queue(messages.UseTimeConditioningMessage())
+
     def _handle_gui_updates(
         self: MessageApi,
         client_id: ClientId,
         message: messages.GuiUpdateMessage,
     ) -> None:
         handle_state = self._handle_state_from_gui_name.get(message.name, None)
         if handle_state is None:
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/viser/messages.py` & `nerfstudio-0.2.1/nerfstudio/viewer/viser/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,18 +167,18 @@
 
     @override
     def redundancy_key(self) -> str:
         return f"{type(self).__name__}_{self.idx}"
 
 
 @dataclasses.dataclass
-class IsTrainingMessage(NerfstudioMessage):
+class TrainingStateMessage(NerfstudioMessage):
     """Wheather the scene is in training mode or not."""
 
-    is_training: bool
+    training_state: Literal["training", "paused", "completed"]
     """True if the model is currently trianing, False otherwise"""
 
 
 @dataclasses.dataclass
 class CameraPathPayloadMessage(NerfstudioMessage):
     """Camera path"""
 
@@ -224,7 +224,20 @@
     step: int
     """ Current step """
 
 
 @dataclasses.dataclass
 class SaveCheckpointMessage(NerfstudioMessage):
     """Save checkpoint message."""
+
+
+@dataclasses.dataclass
+class UseTimeConditioningMessage(NerfstudioMessage):
+    """Use time conditioning message."""
+
+
+@dataclasses.dataclass
+class TimeConditionMessage(NerfstudioMessage):
+    """Time conditioning message."""
+
+    time: float
+    """ Time conditioning value """
```

### Comparing `nerfstudio-0.2.0/nerfstudio/viewer/viser/server.py` & `nerfstudio-0.2.1/nerfstudio/viewer/viser/server.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-0.2.1/nerfstudio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.2.0
+Version: 0.2.1
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.0 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.1 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
 Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
```

### Comparing `nerfstudio-0.2.0/nerfstudio.egg-info/SOURCES.txt` & `nerfstudio-0.2.1/nerfstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio.egg-info/entry_points.txt` & `nerfstudio-0.2.1/nerfstudio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/nerfstudio.egg-info/requires.txt` & `nerfstudio-0.2.1/nerfstudio.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 rich>=12.5.1
 scikit-image>=0.19.3
 tensorboard==2.9.0
 torch<2.0.0,>=1.12.1
 torchmetrics[image]>=0.9.3
 torchtyping>=0.1.4
 torchvision>=0.13.0
+typing_extensions>=4.4.0
 viser>=0.0.5
 nuscenes-devkit>=1.1.1
 wandb>=0.13.3
 xatlas
 trimesh>=3.20.2
 
 [:python_version < "3.10"]
```

### Comparing `nerfstudio-0.2.0/pyproject.toml` & `nerfstudio-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "0.2.0"
+version = "0.2.1"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.7.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
@@ -47,14 +47,15 @@
     "rich>=12.5.1",
     "scikit-image>=0.19.3",
     "tensorboard==2.9.0",
     "torch>=1.12.1,<2.0.0",
     "torchmetrics[image]>=0.9.3",
     "torchtyping>=0.1.4",
     "torchvision>=0.13.0",
+    "typing_extensions>=4.4.0",
     "viser>=0.0.5",
     "nuscenes-devkit>=1.1.1",
     "wandb>=0.13.3",
     "xatlas",
     "trimesh>=3.20.2"
 ]
 
@@ -139,14 +140,15 @@
   "duplicate-code",
   "fixme",
   "logging-fstring-interpolation",
   "too-many-arguments",
   "too-many-branches",
   "too-many-instance-attributes",
   "too-many-locals",
+  "too-many-statements",
   "unnecessary-ellipsis",
 ]
 
 #pytest
 [tool.pytest.ini_options]
 addopts = "-n=4 --typeguard-packages=nerfstudio --torchtyping-patch-typeguard --disable-warnings"
 testpaths = [
```

### Comparing `nerfstudio-0.2.0/scripts/blender/nerfstudio_blender.py` & `nerfstudio-0.2.1/scripts/blender/nerfstudio_blender.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/completions/install.py` & `nerfstudio-0.2.1/scripts/completions/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ShellType = Literal["zsh", "bash"]
 
 CONSOLE = Console(width=120)
 HEADER_LINE = "# Source nerfstudio autocompletions."
 
 
 def _get_all_entry_points() -> List[str]:
+    # TODO: we should filter out entrypoints that are not tyro CLIs.
     entry_points = importlib_metadata.distribution("nerfstudio").entry_points
     return [x.name for x in entry_points]
 
 
 def _check_tyro_cli(script_path: pathlib.Path) -> bool:
     """Check if a path points to a script containing a tyro.cli() call. Also checks
     for any permissions/shebang issues.
```

### Comparing `nerfstudio-0.2.0/scripts/completions/setup.zsh` & `nerfstudio-0.2.1/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/datasets/process_nuscenes_masks.py` & `nerfstudio-0.2.1/scripts/datasets/process_nuscenes_masks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/docs/add_nb_tags.py` & `nerfstudio-0.2.1/scripts/docs/add_nb_tags.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/docs/build_docs.py` & `nerfstudio-0.2.1/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/downloads/download_data.py` & `nerfstudio-0.2.1/scripts/downloads/download_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/eval.py` & `nerfstudio-0.2.1/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/exporter.py` & `nerfstudio-0.2.1/scripts/exporter.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/generative/trace_stable_diffusion.py` & `nerfstudio-0.2.1/scripts/generative/trace_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/github/run_actions.py` & `nerfstudio-0.2.1/scripts/github/run_actions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/process_data.py` & `nerfstudio-0.2.1/scripts/process_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/render.py` & `nerfstudio-0.2.1/scripts/render.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/texture.py` & `nerfstudio-0.2.1/scripts/texture.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/train.py` & `nerfstudio-0.2.1/scripts/train.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.0/scripts/viewer/run_viewer.py` & `nerfstudio-0.2.1/scripts/viewer/run_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     # We don't need logging, but writer.GLOBAL_BUFFER needs to be populated
     config.logging.local_writer.enable = False
     writer.setup_local_writer(config.logging, max_iter=config.max_num_iterations, banner_messages=banner_messages)
 
     assert viewer_state and pipeline.datamanager.train_dataset
     viewer_state.init_scene(
         dataset=pipeline.datamanager.train_dataset,
-        start_train=False,
+        train_state="completed",
     )
-    viewer_state.viser_server.set_is_training(False)
+    viewer_state.viser_server.set_training_state("completed")
     viewer_state.update_scene(step=step)
     while True:
         time.sleep(0.01)
 
 
 def entrypoint():
     """Entrypoint for use with pyproject scripts."""
```

### Comparing `nerfstudio-0.2.0/tests/test_train.py` & `nerfstudio-0.2.1/tests/test_train.py`

 * *Files identical despite different names*

