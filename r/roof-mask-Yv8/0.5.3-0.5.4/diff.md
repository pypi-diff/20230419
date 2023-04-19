# Comparing `tmp/roof_mask_Yv8-0.5.3.tar.gz` & `tmp/roof_mask_Yv8-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask_Yv8-0.5.3.tar", last modified: Fri Apr  7 17:38:27 2023, max compression
+gzip compressed data, was "roof_mask_Yv8-0.5.4.tar", last modified: Wed Apr 19 20:20:20 2023, max compression
```

## Comparing `roof_mask_Yv8-0.5.3.tar` & `roof_mask_Yv8-0.5.4.tar`

### file list

```diff
@@ -1,182 +1,271 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.684330 roof_mask_Yv8-0.5.3/
--rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-07 17:38:26.946950 roof_mask_Yv8-0.5.3/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.728304 roof_mask_Yv8-0.5.3/detectron2/
--rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.786271 roof_mask_Yv8-0.5.3/detectron2/checkpoint/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/c2_model_loading.py
--rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.839241 roof_mask_Yv8-0.5.3/detectron2/config/
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/config.py
--rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/instantiate.py
--rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/lazy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.887214 roof_mask_Yv8-0.5.3/detectron2/data/
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/common.py
--rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.944181 roof_mask_Yv8-0.5.3/detectron2/data/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin.py
--rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin_meta.py
--rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco.py
--rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis.py
--rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v0_5_categories.py
--rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_categories.py
--rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_category_image_count.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/pascal_voc.py
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/register_coco.py
--rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/detection_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.999150 roof_mask_Yv8-0.5.3/detectron2/data/samplers/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/distributed_sampler.py
--rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.065112 roof_mask_Yv8-0.5.3/detectron2/data/transforms/
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation.py
--rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation_impl.py
--rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/transform.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.104090 roof_mask_Yv8-0.5.3/detectron2/engine/
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/launch.py
--rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/train_loop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.160057 roof_mask_Yv8-0.5.3/detectron2/evaluation/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/cityscapes_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/evaluator.py
--rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/fast_eval_api.py
--rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/lvis_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/panoptic_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/pascal_voc_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/rotated_coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/sem_seg_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/testing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.216026 roof_mask_Yv8-0.5.3/detectron2/export/
--rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/api.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/c10.py
--rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_export.py
--rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_inference.py
--rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_modeling.py
--rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_patch.py
--rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/flatten.py
--rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/shared.py
--rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/torchscript.py
--rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/torchscript_patch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.270995 roof_mask_Yv8-0.5.3/detectron2/layers/
--rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/aspp.py
--rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/batch_norm.py
--rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/blocks.py
--rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/deform_conv.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/losses.py
--rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/mask_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/nms.py
--rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/roi_align.py
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/roi_align_rotated.py
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/rotated_boxes.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/shape_spec.py
--rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.325963 roof_mask_Yv8-0.5.3/detectron2/modeling/
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.379932 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/backbone.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/build.py
--rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/regnet.py
--rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/resnet.py
--rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/box_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/matcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.429904 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/
--rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/build.py
--rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/dense_detector.py
--rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/fcos.py
--rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/panoptic_fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/retinanet.py
--rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/semantic_seg.py
--rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/mmdet_wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/poolers.py
--rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.489869 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/
--rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/proposal_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rpn.py
--rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.544838 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/box_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/cascade_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/keypoint_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/mask_head.py
--rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/roi_heads.py
--rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/sampling.py
--rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/test_time_augmentation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.588813 roof_mask_Yv8-0.5.3/detectron2/solver/
--rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/lr_scheduler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.642782 roof_mask_Yv8-0.5.3/detectron2/structures/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/structures/boxes.py
--rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/structures/image_list.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/instances.py
--rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/keypoints.py
--rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/masks.py
--rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/rotated_boxes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.694752 roof_mask_Yv8-0.5.3/detectron2/tracking/
--rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/base_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/hungarian_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.750720 roof_mask_Yv8-0.5.3/detectron2/utils/
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/collect_env.py
--rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/colormap.py
--rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/comm.py
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/develop.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/env.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/events.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/file_io.py
--rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/memory.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/registry.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/serialize.py
--rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/testing.py
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/video_visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/visualizer_new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.789698 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-07 17:38:04.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5655 2023-04-07 17:38:05.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-07 17:38:04.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-07 17:38:05.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-07 17:38:27.030951 roof_mask_Yv8-0.5.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      604 2023-04-07 17:37:51.000000 roof_mask_Yv8-0.5.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.841668 roof_mask_Yv8-0.5.3/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26220 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    45837 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.060782 roof_mask_Yv8-0.5.4/
+-rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-19 20:20:19.827347 roof_mask_Yv8-0.5.4/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.102758 roof_mask_Yv8-0.5.4/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.157726 roof_mask_Yv8-0.5.4/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.213694 roof_mask_Yv8-0.5.4/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.275659 roof_mask_Yv8-0.5.4/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.4/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.342620 roof_mask_Yv8-0.5.4/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.394591 roof_mask_Yv8-0.5.4/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.446561 roof_mask_Yv8-0.5.4/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.487537 roof_mask_Yv8-0.5.4/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.543506 roof_mask_Yv8-0.5.4/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.610467 roof_mask_Yv8-0.5.4/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.656441 roof_mask_Yv8-0.5.4/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.4/detectron2/layers/blocks.py
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.716407 roof_mask_Yv8-0.5.4/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.770375 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.815349 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.871317 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.928285 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:51.969261 roof_mask_Yv8-0.5.4/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.4/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.024230 roof_mask_Yv8-0.5.4/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.088193 roof_mask_Yv8-0.5.4/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.138165 roof_mask_Yv8-0.5.4/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.4/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.4/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.4/detectron2/utils/visualizer_new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.259095 roof_mask_Yv8-0.5.4/roof_mask_Yv8.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-19 20:19:49.000000 roof_mask_Yv8-0.5.4/roof_mask_Yv8.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     8222 2023-04-19 20:19:50.000000 roof_mask_Yv8-0.5.4/roof_mask_Yv8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-19 20:19:49.000000 roof_mask_Yv8-0.5.4/roof_mask_Yv8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-19 20:19:49.000000 roof_mask_Yv8-0.5.4/roof_mask_Yv8.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-19 20:20:19.923348 roof_mask_Yv8-0.5.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      601 2023-04-19 20:19:26.000000 roof_mask_Yv8-0.5.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.331054 roof_mask_Yv8-0.5.4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     3211 2023-04-19 15:22:00.000000 roof_mask_Yv8-0.5.4/tests/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.393019 roof_mask_Yv8-0.5.4/ultralytics/
+-rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.444989 roof_mask_Yv8-0.5.4/ultralytics/hub/
+-rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/hub/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/hub/auth.py
+-rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/hub/session.py
+-rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/hub/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.504954 roof_mask_Yv8-0.5.4/ultralytics/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/nn/autobackend.py
+-rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/nn/autoshape.py
+-rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/nn/modules.py
+-rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/nn/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.560922 roof_mask_Yv8-0.5.4/ultralytics/yolo/
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.617890 roof_mask_Yv8-0.5.4/ultralytics/yolo/cfg/
+-rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/cfg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.685851 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/augment.py
+-rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/build.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.743818 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataloaders/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataloaders/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataloaders/v5loader.py
+-rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/dataset_wrappers.py
+-rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.783794 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/exporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/predictor.py
+-rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/results.py
+-rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/trainer.py
+-rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.835765 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/
+-rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/autobatch.py
+-rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.895730 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/clearml.py
+-rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/comet.py
+-rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/hub.py
+-rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/mlflow.py
+-rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/raytune.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/callbacks/wb.py
+-rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/checks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/dist.py
+-rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/downloads.py
+-rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/tal.py
+-rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/torch_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/utils/tuner.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:52.941704 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:53.003668 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/classify/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/classify/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/classify/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/classify/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:53.060636 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/detect/
+-rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/detect/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/detect/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/detect/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:53.128597 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/pose/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/pose/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/pose/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/pose/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/pose/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:53.183566 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/segment/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/segment/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/segment/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/segment/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.4/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 20:19:53.229539 roof_mask_Yv8-0.5.4/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.4/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    33279 2023-04-19 14:59:59.000000 roof_mask_Yv8-0.5.4/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.4/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    41759 2023-04-18 18:11:13.000000 roof_mask_Yv8-0.5.4/yolo_roof/report_functions.py
```

### Comparing `roof_mask_Yv8-0.5.3/detectron2/checkpoint/c2_model_loading.py` & `roof_mask_Yv8-0.5.4/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/checkpoint/catalog.py` & `roof_mask_Yv8-0.5.4/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/checkpoint/detection_checkpoint.py` & `roof_mask_Yv8-0.5.4/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/compat.py` & `roof_mask_Yv8-0.5.4/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/config.py` & `roof_mask_Yv8-0.5.4/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/defaults.py` & `roof_mask_Yv8-0.5.4/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/instantiate.py` & `roof_mask_Yv8-0.5.4/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/config/lazy.py` & `roof_mask_Yv8-0.5.4/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/benchmark.py` & `roof_mask_Yv8-0.5.4/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/build.py` & `roof_mask_Yv8-0.5.4/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/catalog.py` & `roof_mask_Yv8-0.5.4/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/common.py` & `roof_mask_Yv8-0.5.4/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/dataset_mapper.py` & `roof_mask_Yv8-0.5.4/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin_meta.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes_panoptic.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco_panoptic.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v0_5_categories.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_categories.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_category_image_count.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/datasets/pascal_voc.py` & `roof_mask_Yv8-0.5.4/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/detection_utils.py` & `roof_mask_Yv8-0.5.4/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/samplers/distributed_sampler.py` & `roof_mask_Yv8-0.5.4/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/samplers/grouped_batch_sampler.py` & `roof_mask_Yv8-0.5.4/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation.py` & `roof_mask_Yv8-0.5.4/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation_impl.py` & `roof_mask_Yv8-0.5.4/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/data/transforms/transform.py` & `roof_mask_Yv8-0.5.4/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/engine/defaults.py` & `roof_mask_Yv8-0.5.4/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/engine/hooks.py` & `roof_mask_Yv8-0.5.4/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/engine/launch.py` & `roof_mask_Yv8-0.5.4/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/engine/train_loop.py` & `roof_mask_Yv8-0.5.4/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/cityscapes_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/coco_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/evaluator.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/fast_eval_api.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/lvis_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/panoptic_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/pascal_voc_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/rotated_coco_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/sem_seg_evaluation.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/evaluation/testing.py` & `roof_mask_Yv8-0.5.4/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/api.py` & `roof_mask_Yv8-0.5.4/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/c10.py` & `roof_mask_Yv8-0.5.4/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/caffe2_export.py` & `roof_mask_Yv8-0.5.4/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/caffe2_inference.py` & `roof_mask_Yv8-0.5.4/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/caffe2_modeling.py` & `roof_mask_Yv8-0.5.4/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/caffe2_patch.py` & `roof_mask_Yv8-0.5.4/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/flatten.py` & `roof_mask_Yv8-0.5.4/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/shared.py` & `roof_mask_Yv8-0.5.4/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/torchscript.py` & `roof_mask_Yv8-0.5.4/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/export/torchscript_patch.py` & `roof_mask_Yv8-0.5.4/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/aspp.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/batch_norm.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/blocks.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/deform_conv.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/losses.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/mask_ops.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/nms.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/roi_align.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/roi_align_rotated.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/rotated_boxes.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/shape_spec.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/layers/wrappers.py` & `roof_mask_Yv8-0.5.4/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/anchor_generator.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/backbone.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/build.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/fpn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/regnet.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/resnet.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/box_regression.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/matcher.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/build.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/dense_detector.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/fcos.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/panoptic_fpn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/rcnn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/retinanet.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/semantic_seg.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/mmdet_wrapper.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/poolers.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/postprocessing.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/build.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/proposal_utils.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rpn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rrpn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/box_head.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/cascade_rcnn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/fast_rcnn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/keypoint_head.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/mask_head.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/roi_heads.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/sampling.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/modeling/test_time_augmentation.py` & `roof_mask_Yv8-0.5.4/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/solver/build.py` & `roof_mask_Yv8-0.5.4/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/solver/lr_scheduler.py` & `roof_mask_Yv8-0.5.4/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/boxes.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/image_list.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/instances.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/keypoints.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/masks.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/structures/rotated_boxes.py` & `roof_mask_Yv8-0.5.4/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/__init__.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/base_tracker.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/hungarian_tracker.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/utils.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.4/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/analysis.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/collect_env.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/colormap.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/comm.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/develop.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/env.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/events.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/file_io.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/logger.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/memory.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/registry.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/serialize.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/testing.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/video_visualizer.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/visualizer.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/detectron2/utils/visualizer_new.py` & `roof_mask_Yv8-0.5.4/detectron2/utils/visualizer_new.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/setup.py` & `roof_mask_Yv8-0.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
     name = "roof_mask_Yv8",
-    version = "0.5.3",
+    version = "0.5.4",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
-    long_description = 'package supporting Yolo_v8 roof model deployment',
+    long_description = 'package supporing Yolo_v8 roof model backend.',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `roof_mask_Yv8-0.5.3/yolo_roof/detect_functions.py` & `roof_mask_Yv8-0.5.4/yolo_roof/detect_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import pandas as pd
 import math
 import cv2
 import platform
 import requests
 import logging
+from tqdm import tqdm
 
 import time
 import timeit
 from datetime import datetime
 
 # from pathlib import Path
 # plot
@@ -49,18 +50,35 @@
 from detectron2.data import detection_utils as utils
 from detectron2.utils.logger import setup_logger
 from detectron2.utils.visualizer_new import Visualizer
 from detectron2.utils.visualizer_new import ColorMode
 from detectron2.engine.defaults import DefaultPredictor
 from detectron2.data import MetadataCatalog
 
-# yolo v8
-from ultralytics import YOLO
+### yolo ###
+# from models.common import DetectMultiBackend
+# from utils.dataloaders import IMG_FORMATS, VID_FORMATS, LoadImages, LoadStreams
+# from utils.general import (LOGGER, Profile, check_file, check_img_size, check_imshow, check_requirements, colorstr, cv2,
+#                            increment_path, non_max_suppression, print_args, scale_coords, strip_optimizer, xyxy2xywh)
+# from utils.plots import Annotator, save_one_box
+# from utils.plots import colors as yolo_colors
+# from utils.segment.general import process_mask, scale_masks
+# from utils.segment.plots import plot_masks
+# from utils.torch_utils import select_device, smart_inference_mode
+# from utils.augmentations import letterbox
+
+# import yolo_roof.export
+
+# new yolo
+# from ultralytics import YOLO
+# from ultralytics.yolo.utils.ops import scale_image
+from ultralytics.yolo.engine.model import YOLO
 from ultralytics.yolo.utils.ops import scale_image
 
+
 ################################################### yolo model
 class Colors:
     # Ultralytics color palette https://ultralytics.com/
     def __init__(self):
         # hex = matplotlib.colors.TABLEAU_COLORS.values()
         hexs = ('FF3838', 'FF9D97', 'FF701F', 'FFB21D', 'CFD231', '48F90A', '92CC17', '3DDB86', '1A9334', '00D4BB',
                 '2C99A8', '00C2FF', '344593', '6473FF', '0018EC', '8438FF', '520085', 'CB38FF', 'FF95C8', 'FF37C7')
@@ -72,14 +90,26 @@
         return (c[2], c[1], c[0]) if bgr else c
 
     @staticmethod
     def hex2rgb(h):  # rgb order (PIL)
         return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
 
 def overlay(image, mask, color, alpha, resize=None):
+    """Combines image and its segmentation mask into a single image.
+    https://www.kaggle.com/code/purplejester/showing-samples-with-segmentation-mask-overlay
+    Params:
+        image: Training image. np.ndarray,
+        mask: Segmentation mask. np.ndarray,
+        color: Color for segmentation mask rendering.  tuple[int, int, int] = (255, 0, 0)
+        alpha: Segmentation mask's transparency. float = 0.5,
+        resize: If provided, both image and its mask are resized before blending them together.
+        tuple[int, int] = (1024, 1024))
+    Returns:
+        image_combined: The combined image. np.ndarray
+    """
     color = color[::-1]
     colored_mask = np.expand_dims(mask, 0).repeat(3, axis=0)
     colored_mask = np.moveaxis(colored_mask, 0, -1)
     masked = np.ma.MaskedArray(image, mask=colored_mask, fill_value=color)
     image_overlay = masked.filled()
 
     if resize is not None:
@@ -92,35 +122,41 @@
 
 def load_yolov8_model(weights='best.pt'):
     model = YOLO(weights)
     return model
 
 def yolo_predict(yolo_model,
                  im0,
-                 imgsz=640,
+                 imgsz=1536,
                  conf_thres=0.2,
                  iou_thres=0.6,
                  max_det=50,
                  verb=False,
                  ):
     im0 = np.ascontiguousarray(im0)
     results = yolo_model.predict(source=im0, imgsz=imgsz, conf=conf_thres, iou=iou_thres, max_det=max_det, retina_masks=True, verbose=verb)
 
     result = results[0].cpu().numpy()
     image_with_masks = np.copy(im0)
     if len(result):
         # all_class_probs = results[1].cpu().numpy()
-        masks = result.masks.masks
-        scores = result.boxes.conf  # confidence score, (N, 1)
+        # masks = result.masks.masks
+        masks = result.masks.data
+        #scores = result.boxes.conf  # confidence score, (N, 1)
+        scores = results[1].cpu().numpy()  # confidence score, (N, number of classes)
         classes = result.boxes.cls
 
         ### plot
         masks = np.moveaxis(masks, 0, -1) # masks, (H, W, N)
         # rescale masks to original image
-        masks = scale_image(masks.shape[:2], masks, result.masks.orig_shape)
+        # masks = scale_image(masks.shape[:2], masks, result.masks.orig_shape) before 8.0.65
+        masks = scale_image(
+            masks=masks, 
+            im0_shape=result.masks.orig_shape
+            )
 
         colors = Colors()
         mcolors = [colors(int(cls), True) for cls in classes]
         
         for idx in range(len(classes)):
             image_with_masks = overlay(image_with_masks, masks[:,:,idx], color=mcolors[idx], alpha=0.3)
     else:
@@ -249,40 +285,57 @@
                 for each_class_id in set(all_labels):
                     each_class_masks = [each_mask for each_mask, each_label in zip(all_masks, all_labels) if each_label == each_class_id and each_mask.is_valid]
                     union_masks = unary_union(each_class_masks)
                     label_names = metadata.get("thing_classes", None)
                     # print(union_masks.geom_type)
                     if union_masks.geom_type == 'MultiPolygon':
                         for current_mask in union_masks.geoms:
+                            shapely_bounding_box = current_mask.bounds
+                            coco_box_format = np.array(
+                                [int(shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[1]),
+                                 int(shapely_bounding_box[2]-shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[3]-shapely_bounding_box[1])]
+                            ).tolist()
                             current_polygon_list = current_mask.exterior.coords
                             current_polygon_list_xy = current_mask.exterior.coords.xy
 
                             coco_segmentation_format = np.array(current_mask.exterior.coords).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
                             # append annotation to coco jason file list
                             new_annotations.append({"id": ann_id,
                                                     "image_id": new_image_id,
                                                     "category_id": each_class_id,
                                                     "iscrowd": 0,
                                                     # "area": current_mask.area,
+                                                    "bbox": coco_box_format,
                                                     "segmentation": coco_segmentation_format
                                                     })
                             # get new annotation id
                             ann_id += 1
                             
                     elif union_masks.geom_type =='Polygon':
+                        shapely_bounding_box = union_masks.bounds
+                        coco_box_format = np.array(
+                            [int(shapely_bounding_box[0]),
+                             int(shapely_bounding_box[1]),
+                             int(shapely_bounding_box[2]-shapely_bounding_box[0]),
+                             int(shapely_bounding_box[3]-shapely_bounding_box[1])]
+                        ).tolist()
+                        
                         current_polygon_list = union_masks.exterior.coords
                         current_polygon_list_xy = union_masks.exterior.coords.xy
 
                         coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(union_masks.exterior.coords) * 2).tolist()
                         # append annotation to coco jason file list
                         new_annotations.append({"id": ann_id,
                                                 "image_id": new_image_id,
                                                 "category_id": each_class_id,
                                                 "iscrowd": 0,
                                                 # "area": union_masks.area,
+                                                "bbox": coco_box_format,
                                                 "segmentation": coco_segmentation_format
                                                 })
                         # get new annotation id
                         ann_id += 1
                     else:
                         # print(union_masks)
                         continue
@@ -329,41 +382,61 @@
                     union_masks = unary_union(each_class_masks)
                     label_names = metadata.get("thing_classes", None)
                     # print(type(union_masks))
                     if union_masks.geom_type == 'MultiPolygon':
                         for current_mask in union_masks.geoms:
                             if current_mask.area < 100:
                                 continue
+                            
+                            shapely_bounding_box = current_mask.bounds
+                            coco_box_format = np.array(
+                                [int(shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[1]),
+                                 int(shapely_bounding_box[2]-shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[3]-shapely_bounding_box[1])]
+                            ).tolist()
+                        
                             current_polygon_list = current_mask.exterior.coords
                             current_polygon_list_xy = current_mask.exterior.coords.xy
 
                             coco_segmentation_format = np.array(current_mask.exterior.coords).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
                             # append annotation to coco jason file list
                             new_annotations.append({"id": ann_id,
                                                     "image_id": new_image_id,
                                                     "category_id": each_class_id,
                                                     "iscrowd": 0,
                                                     # "area": current_mask.area,
+                                                    "bbox": coco_box_format,
                                                     "segmentation": coco_segmentation_format
                                                     })
                             # get new annotation id
                             ann_id += 1
                     elif union_masks.geom_type == 'Polygon':
                         if union_masks.area < 100:
                             continue
+                            
+                        shapely_bounding_box = union_masks.bounds
+                        coco_box_format = np.array(
+                            [int(shapely_bounding_box[0]),
+                             int(shapely_bounding_box[1]),
+                             int(shapely_bounding_box[2]-shapely_bounding_box[0]),
+                             int(shapely_bounding_box[3]-shapely_bounding_box[1])]
+                        ).tolist()
+                        
                         current_polygon_list = union_masks.exterior.coords
                         current_polygon_list_xy = union_masks.exterior.coords.xy
 
                         coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(union_masks.exterior.coords) * 2).tolist()
                         # append annotation to coco jason file list
                         new_annotations.append({"id": ann_id,
                                                 "image_id": new_image_id,
                                                 "category_id": each_class_id,
                                                 "iscrowd": 0,
                                                 # "area": union_masks.area,
+                                                "bbox": coco_box_format,
                                                 "segmentation": coco_segmentation_format
                                                 })
                         # get new annotation id
                         ann_id += 1
                     else:
                         continue
                         
@@ -477,15 +550,15 @@
 def inputimage_list(input_folder):
     files = os.listdir(input_folder)
     input_files = [os.path.join(input_folder, x) for x in files if os.path.splitext(x)[1] in ['.jpg','.png']]
     return input_files
 
 
 def roof_predict_5models(yolo_roof_model,yolo_roof_type_model, yolo_roof_material_model,
-                         yolo_data_all_model,yolo_phase3_model, file_root_path, #input_files,
+                         yolo_data_all_model,yolo_phase3_model, file_root_path, input_files,
                          demoFolder='roof_score_new_20230101'):
 
     ############################################ input Image
     input_files = inputimage_list(input_folder = demoFolder)
     # logging.info(input_files)
     ########################################## dataset config
     imgsetUrl =  os.path.join(file_root_path,'test_360.jpg')
@@ -519,10 +592,55 @@
         else: 
             logging.info('%s already registered!' % datasetName)
 
     ############################################# Models
     last_roof_boundary_result = mask_prediction(yolo_roof_model, input_files, trainingDataset='Roof_boundary', output_folder=demoFolder, thresh_hold=0.426, cut_image = False, tile_len = 960, tile_overlap = 200, save_image=True)
     # last_roof_type_result = mask_prediction(yolo_roof_type_model, input_files, trainingDataset='Roof_type', output_folder=demoFolder, thresh_hold=0.295, cut_image = False, tile_len = 1536, tile_overlap = 200, save_image=True)
     # last_roof_material_result = mask_prediction(yolo_roof_material_model, input_files, trainingDataset='Roof_material', output_folder=demoFolder, thresh_hold=0.253, cut_image = False, tile_len = 1536, tile_overlap = 200, save_image=True)
-    last_data_all_result = mask_prediction(yolo_data_all_model, input_files, trainingDataset='Data_all_equipment_damage', output_folder=demoFolder, thresh_hold=0.221, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=True)
+    last_data_all_result = mask_prediction(yolo_data_all_model, input_files, trainingDataset='Data_all_equipment_damage', output_folder=demoFolder, thresh_hold=0.22, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=True)
     last_phase3_result = mask_prediction(yolo_phase3_model, input_files, trainingDataset='Phase3_equipment_damage', output_folder=demoFolder, thresh_hold=0.203, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=True)
+    
+    
+    
+def roof_condition_predict(yolo_roof_condition_model, file_root_path,
+                           input_files, demoFolder='roof_score_new_20230101'):
 
+    ############################################ input Image
+    input_files = inputimage_list(input_folder = demoFolder)
+    # logging.info(input_files)
+    ########################################## dataset config
+    imgsetUrl =  os.path.join(file_root_path,'test_360.jpg')
+
+    cocoJsonPairs = {
+        'Roof_condition' :  os.path.join(file_root_path,'roof_condition.json'),
+        'Roof_condition_three_classes' :  os.path.join(file_root_path,'roof_condition_three_classes.json'),
+    }
+
+    for datasetName, jsonURL in cocoJsonPairs.items():     
+        if datasetName not in DatasetCatalog:
+            # there is a way to load the labels from the detectron2 datasets. should replace this piece.
+            with open(jsonURL) as f:
+                cocoFile = json.load(f)
+            catMap = {str(cat['id']): cat['name'] for cat in cocoFile['categories']}  # coco file category ID starts from 1
+            logging.info(catMap)
+            catIDs = [int(key) for key in catMap.keys()] # when detectron2 load a coco dataset, the categories are sorted by IDs, and mapped to [1, lengthOfCatetories] as a subset of [1,80).
+
+            # To make sure the labels are in the same order as the IDs when passed to register the dataset
+            catIDs.sort() 
+            labels = [catMap[str(catID)] for catID in catIDs]
+            allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8 
+            # 12 colors; repeat 8 times in case there are more labels than 12; need a better way to assign the colors
+            colors = allColors[:len(labels)]
+            logging.info('dataset: %s has %i labels and %i colors ' % (datasetName, len(labels), len(colors)))
+            register_coco_instances(datasetName, {'thing_classes':labels, 'thing_colors':colors}, jsonURL, imgsetUrl) 
+            # the 2nd parameter is metadata, in this case we pass over thing_classes for Visualizer to use    
+        else: 
+            logging.info('%s already registered!' % datasetName)
+
+    ############################################# Models
+    # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition', output_folder=demoFolder, thresh_hold=0.244, cut_image = False, tile_len = 960, tile_overlap = 200,save_image=False)
+    
+    # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.245, cut_image = False, tile_len = 960, tile_overlap = 200, save_image=False)
+    
+    last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.236, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
+
+
```

### Comparing `roof_mask_Yv8-0.5.3/yolo_roof/geo_functions.py` & `roof_mask_Yv8-0.5.4/yolo_roof/geo_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.3/yolo_roof/report_functions.py` & `roof_mask_Yv8-0.5.4/yolo_roof/report_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+import os
+import numpy as np
+from pycocotools.coco import COCO
+from tqdm import tqdm
+import json 
+import uuid
+import pandas as pd
+import math
+import cv2
+
 ### report ###
 import reportlab
 from reportlab.pdfgen import canvas
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
 from reportlab.lib import colors
 
-from yolo_roof.detect_functions import *
+### detectron2 ###
+from detectron2.data import DatasetCatalog
+from detectron2.data.datasets.coco import register_coco_instances 
+from detectron2.data.detection_utils import read_image
+from detectron2.data import detection_utils as utils
+from detectron2.utils.logger import setup_logger
+from detectron2.utils.visualizer_new import Visualizer
+from detectron2.utils.visualizer import Visualizer as Vis_box
+from detectron2.utils.visualizer_new import ColorMode
+from detectron2.engine.defaults import DefaultPredictor
+from detectron2.data import MetadataCatalog
+
 #### shapely ###
 import shapely
 import shapely.wkt
-from shapely.ops import unary_union
 from shapely.geometry import Polygon, MultiPoint
 from shapely.geometry import Polygon
 
 ## PDF
 import reportlab
 from reportlab.pdfgen import canvas
 from reportlab.pdfbase.ttfonts import TTFont
@@ -59,42 +79,22 @@
 
     n = 2.0 ** zoom
     lon_deg = xtile / n * 360.0 - 180.0
     lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * ytile / n)))
     lat_deg = math.degrees(lat_rad)
     return [lat_deg, lon_deg]
 
-def merge_polygones(image_folder,json_file,trainingDataset):
-    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
-    filename = str(uuid.uuid4())
-    register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
-    metadata = MetadataCatalog.get(filename)
-    dicts = DatasetCatalog.get(filename)
-    model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
-    print(f"Merging {trainingDataset} polygons")
-    for dic in dicts:
-        img = utils.read_image(dic["file_name"], "RGB")
-        visualizer = Visualizer(img, metadata=metadata, instance_mode=ColorMode.SEGMENTATION)
-        vis = visualizer.draw_dataset_dict(dic)
-        out_filename = os.path.join(os.path.splitext(os.path.basename(dic["file_name"]))[0],trainingDataset +'_merged.jpg')
-        
-        out_filename2_extention = os.path.splitext(os.path.basename(dic["file_name"]))[1]
-        out_filename2 = os.path.basename(dic["file_name"]).replace(out_filename2_extention,'_merged'+out_filename2_extention)
-        vis.save(os.path.join(image_folder,out_filename))
-        # vis.save(os.path.join(model_folder,out_filename2)) # model folder is not necessary
-    print("Merging Finished.")
-    return vis
 
 def generate_referral_json(demoFolder, coco_json, new_cat, new_json_file_name):
     catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
     # Obtain the category names
     categories = coco_json.loadCats(catIds)
     new_categories = [x['name'] for x in categories if x['name'] in new_cat]
     new_catIds = coco_json.getCatIds(catNms=new_categories, supNms=[], catIds=[])
-    print(new_catIds)
+    # print(new_catIds)
     imgIds = coco_json.getImgIds()
     
     new_json_file = os.path.join(demoFolder, new_json_file_name)
     
     new_images = []
     new_annotations = []
     ann_id = 1
@@ -116,15 +116,15 @@
                 
                 # append annotation to coco jason file list
                 new_annotations.append({"id": ann_id,
                                         "image_id": new_image_id,
                                         "category_id": ann['category_id'],
                                         "iscrowd": 0,
                                         # "area": ann['area'],
-                                        # "bbox": ann['bbox'],
+                                        "bbox": ann['bbox'],
                                         "segmentation": ann['segmentation']
                                         })
                 # get new annotation id
                 ann_id += 1
 
         # get new image id
         new_image_id += 1
@@ -143,22 +143,22 @@
                  "annotations": new_annotations
                  }
 
     with open(new_json_file, "w") as jsonfile:
         json.dump(json_data, jsonfile, sort_keys=True, indent=4)
 
 
-        
+
 def generate_referral_damage_json(demoFolder, coco_json, roof_boundary_json, new_cat, new_json_file_name):
     catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
     # Obtain the category names
     categories = coco_json.loadCats(catIds)
     new_categories = [x['name'] for x in categories if x['name'] in new_cat]
     new_catIds = coco_json.getCatIds(catNms=new_categories, supNms=[], catIds=[])
-    print(new_catIds)
+    # print(new_catIds)
     imgIds = coco_json.getImgIds()
     
     new_json_file = os.path.join(demoFolder, new_json_file_name)
     
     new_images = []
     new_annotations = []
     ann_id = 1
@@ -181,15 +181,15 @@
         roof_annotations = roof_boundary_json.loadAnns(annIds)
         for ann in roof_annotations:
             for seg in ann['segmentation']:
                 mask = np.array(seg).reshape(len(seg) // 2, 2)
                 poly = Polygon(mask)
                 roof_poly = roof_poly.union(poly)
         
-        # roof_poly = roof_poly.buffer(-5.0)
+        # roof_poly = roof_poly.buffer(5.0)
         
         ann_start = ann_id
         for ann in annotations:
             # print(ann)
             # class selection
             if ann['category_id'] in new_catIds:
                 current_poly = Polygon()
@@ -211,31 +211,31 @@
                         coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
                         # append annotation to coco jason file list
                         new_annotations.append({"id": ann_id,
                                                 "image_id": new_image_id,
                                                 "category_id": ann['category_id'],
                                                 "iscrowd": 0,
                                                 # "area": ann['area'],
-                                                # "bbox": ann['bbox'],
+                                                "bbox": ann['bbox'],
                                                 "segmentation": coco_segmentation_format
                                                 })
                         # get new annotation id
                         ann_id += 1
                 elif intersection_poly.geom_type == 'Polygon':
-                    if intersection_poly.area < 100:
+                    if intersection_poly.area < 25:
                         continue
                     current_polygon_list = intersection_poly.exterior.coords
                     coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(current_polygon_list) * 2).tolist()
                     # append annotation to coco jason file list
                     new_annotations.append({"id": ann_id,
                                             "image_id": new_image_id,
                                             "category_id": ann['category_id'],
                                             "iscrowd": 0,
                                             # "area": ann['area'],
-                                            # "bbox": ann['bbox'],
+                                            "bbox": ann['bbox'],
                                             "segmentation": coco_segmentation_format
                                             })
                     # get new annotation id
                     ann_id += 1             
 
         # get new image id
         new_image_id += 1
@@ -355,51 +355,157 @@
                         # update the value
                         if self.buffer[referral_cat][refferal_type]!=0:
                             if referral_value['min'] <= self.buffer[referral_cat][refferal_type] < referral_value['max']:
                                 if referral_value['point'] > self.score[referral_cat]:
                                     self.set_points(referral_cat, points=referral_value['point'])
                 # print(referral_cat)
                 # print(self.buffer[referral_cat])  
+
+                
+                
+def generate_displayed_polygones(image_folder,json_file,trainingDataset):
+    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
+    filename = str(uuid.uuid4())
+    register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
+    metadata = MetadataCatalog.get(filename)
+    dicts = DatasetCatalog.get(filename)
+    model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
+    print(f"Generating {trainingDataset} polygons")
+    for dic in dicts:
+        img = utils.read_image(dic["file_name"], "RGB")
+        visualizer = Visualizer(img, metadata=metadata, instance_mode=ColorMode.SEGMENTATION)
+        vis = visualizer.draw_dataset_dict(dic)
+        out_filename = os.path.join(os.path.splitext(os.path.basename(dic["file_name"]))[0],trainingDataset +'_merged.jpg')
         
-def generate_report_merged_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
+        out_filename2_extention = os.path.splitext(os.path.basename(dic["file_name"]))[1]
+        out_filename2 = os.path.basename(dic["file_name"]).replace(out_filename2_extention,'_merged'+out_filename2_extention)
+        vis.save(os.path.join(image_folder,out_filename))
+        # vis.save(os.path.join(model_folder,out_filename2)) # model folder is not necessary
+    print("Gereating Finished.")
+    return vis
+
+def generate_displayed_condition_polygones(image_folder,json_file,trainingDataset):
+    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
+    filename = str(uuid.uuid4())
+    register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
+    metadata = MetadataCatalog.get(filename)
+    dicts = DatasetCatalog.get(filename)
+    model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
+    print(f"Generating {trainingDataset} polygons")
+    for dic in dicts:
+        img = utils.read_image(dic["file_name"], "RGB")
+        visualizer = Vis_box(img, metadata=metadata, scale=0.3, instance_mode=ColorMode.SEGMENTATION)
+        vis = visualizer.draw_dataset_dict(dic)
+        out_filename = os.path.join(os.path.splitext(os.path.basename(dic["file_name"]))[0],trainingDataset +'_merged.jpg')
+        vis.save(os.path.join(image_folder,out_filename))
+
+    print("Gereating Finished.")
+    return vis
+
+def generate_referral_condition_json(demoFolder, coco_json, new_json_file_name):
+    catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
+    categories = coco_json.loadCats(catIds)    
+    imgIds = coco_json.getImgIds()
+    new_json_file = os.path.join(demoFolder, new_json_file_name)
+    new_images = []
+    new_annotations = []
+    ann_id = 1
+    new_image_id = 1
+
+    for img_id in range(len(imgIds)):
+        # get image information
+        coco_img_info = coco_json.loadImgs(imgIds[img_id])[0]
+        # get the raw image annotations Id
+        annIds = coco_json.getAnnIds(imgIds=coco_img_info['id'])
+        # get annotations from annotation Id
+        annotations = coco_json.loadAnns(annIds)
+
+        ann_start = ann_id
+        for ann in annotations:
+            # print(ann)
+            # # class selection
+            # if ann['category_id'] in new_catIds:
+                
+            # append annotation to coco jason file list
+            new_annotations.append({"id": ann_id,
+                                    "image_id": new_image_id,
+                                    "category_id": ann['category_id'],
+                                    "iscrowd": 0,
+                                    # "area": ann['area'],
+                                    "bbox": ann['bbox'],
+                                    # "segmentation": ann['segmentation']
+                                    })
+            # get new annotation id
+            ann_id += 1
+
+        # get new image id
+        new_image_id += 1
+        # append image information to coco jason file list
+        new_images.append(coco_img_info)
+
+    info = {"year": 2022,
+            "version": "1.0",
+            "description": "Phase 2 data and coco json file",
+            "contributor": "Ruixu Liu, Delin Shen, Aaron Lee and Qiang Wang",
+            }
+
+    json_data = {"info": info,
+                 "categories": categories,
+                 "images": new_images,
+                 "annotations": new_annotations
+                 }
+
+    with open(new_json_file, "w") as jsonfile:
+        json.dump(json_data, jsonfile, sort_keys=True, indent=4)
+
+    
+    
+def generate_condition_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
+    pred_condition_file = os.path.join(demoFolder,'prediction_Roof_condition_three_classes/Roof_condition_three_classes_all_in_one.json')
+    red_condition = COCO(pred_condition_file)
+    generate_referral_condition_json(demoFolder, red_condition,'Referral_condition.json')
+    vis_out = generate_displayed_condition_polygones(demoFolder,os.path.join(demoFolder, 'Referral_condition.json'),'Roof_condition_three_classes')
+    
+    referral_condition = COCO(os.path.join(demoFolder, 'Referral_condition.json'))
+    for referral_condition_id in referral_condition.getImgIds():
+        coco_img_info = referral_condition.loadImgs(referral_condition_id)[0]
+        address = os.path.splitext(coco_img_info['file_name'])[0]
+        print(address)
+
+def generate_condition_and_merged_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
     # pred_damage_file = os.path.join(demoFolder,'prediction_Roof_damage/Roof_damage_all_in_one.json')
     # pred_equip_file = os.path.join(demoFolder, 'prediction_Roof_equipment/Roof_equipment_all_in_one.json')
     pred_phase3_file = os.path.join(demoFolder,'prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json')
     pred_data_all_file = os.path.join(demoFolder, 'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json')
     pred_boundary_file =os.path.join(demoFolder, 'prediction_Roof_boundary/Roof_boundary_all_in_one.json')
 
     # read in referral rules and create corresponding functions
     referral_label_file = os.path.join(file_root_path,'referral_labels_20230315.json')
-    referral_damage_label_file = os.path.join(file_root_path,'referral_labels_20230315_for_merged_damage.json')
-    
-    # referral_label_file = os.path.join(file_root_path,'referral_labels_20221006.json')
-    # referral_damage_label_file = os.path.join(file_root_path,'referral_labels_20221006_for_merged_damage.json')
-    referral_equip_label_file = os.path.join(file_root_path,'referral_labels_20221006_for_merged_equip.json')
-    with open(referral_damage_label_file) as f1:
+
+    with open(referral_label_file) as f1:
         ref_json = json.load(f1)
     cat_damage = [x for x in ref_json]
-    # Load json file
-    # pred_damage = COCO(pred_damage_file)
-    # pred_equip = COCO(pred_equip_file)
+
     pred_phase3 = COCO(pred_phase3_file)
     pred_data_all = COCO(pred_data_all_file)
     pred_boundary = COCO(pred_boundary_file)
-    generate_referral_damage_json(demoFolder, pred_data_all,pred_boundary,cat_damage,'Referral_damage.json')
-    
-    with open(referral_equip_label_file) as f1:
+    generate_referral_damage_json(demoFolder, pred_data_all,pred_boundary,cat_damage,'Referral_data_all.json')
+    # generate_referral_json(demoFolder, pred_data_all,cat_damage,'Referral_data_all.json')
+    with open(referral_label_file) as f1:
         ref_json = json.load(f1)
     cat_equip = [x for x in ref_json]
 
-    generate_referral_json(demoFolder, pred_data_all, cat_equip,'Referral_equipment.json')
-    vis_out = merge_polygones(demoFolder,os.path.join(demoFolder, 'Referral_damage.json'),'Damage')
-    vis_out = merge_polygones(demoFolder,os.path.join(demoFolder, 'Referral_equipment.json'),'Equipment')
+    generate_referral_damage_json(demoFolder, pred_phase3, pred_boundary, cat_equip,'Referral_phase3.json')
+    # generate_referral_json(demoFolder, pred_phase3, cat_equip,'Referral_phase3.json')
+    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_data_all.json'),'Data_all_equipment_damage')
+    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_phase3.json'),'Phase3_equipment_damage')
 
     ################################### Referral
-    referral_damage = COCO(os.path.join(demoFolder, 'Referral_damage.json'))
-    referral_equip = COCO(os.path.join(demoFolder, 'Referral_equipment.json'))
+    referral_damage = COCO(os.path.join(demoFolder, 'Referral_data_all.json'))
+    referral_equip = COCO(os.path.join(demoFolder, 'Referral_phase3.json'))
     referral_output = []
     # Obtain the category ID numbers
     catIds = referral_damage.getCatIds()
     # Obtain the category names
     categories = referral_damage.loadCats(catIds)
     # Id2catname
     Damage_labels = [value['name'] for value in categories]
@@ -489,16 +595,18 @@
         url = f'https://apps.nearmap.com/maps/#/@{url_lat},{url_lon},{url_zoom_level}z,0d/V/{url_date}'
 
         fileName = os.path.join(demoFolder,address+'.pdf')
         documentTitle = f'Refferal'
         title = f'{insured_name[address_index]}'
         subTitle = address
 
-        Damage_image_name = os.path.join(demoFolder,address+'/Damage_merged.jpg')
-        Equipment_image_name = os.path.join(demoFolder,address+'/Equipment_merged.jpg')
+        Damage_image_name = os.path.join(demoFolder,address+'/Data_all_equipment_damage_merged.jpg')
+        Equipment_image_name = os.path.join(demoFolder,address+'/Phase3_equipment_damage_merged.jpg')
+        # Equipment_image_name = os.path.join(demoFolder,address+'/Roof_condition_three_classes_merged.jpg')
+        Roof_condition_image_name = os.path.join(demoFolder,address+'/Roof_condition_three_classes_merged.jpg')
 
         pdf = canvas.Canvas(fileName)
         pdf.setTitle(documentTitle)
         pdf.setFont("Times-Roman", 14)
         pdf.drawCentredString(300, 800, title)
 
         pdf.setFillColorRGB(0, 0, 0)
@@ -554,15 +662,15 @@
         for i in range(key_name_index+1, len(key_name)):
             if i == pixels_area_key:
                 gsd_area = row[gsd_key] * row[gsd_key] * row[pixels_area_key]
                 text.textLine(f'Roof area: {int(gsd_area)} m\u00b2')
                 continue
             if int(row[i]) == 0:
                 line = key_name[i] + ': ' + 'Not detected'
-                text.textLine(line)
+                # text.textLine(line)     # Hide no detected case
             elif int(row[i]) == 1:
                 if key_name[i] == 'Pipline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Minor'
                     text.textLine(line)
@@ -602,17 +710,21 @@
         #     if row[i]>0:
         #         line = key_name[i] + ': ' + str(int(row[i]))
         #         text.textLine(line)
         # pdf.drawText(text)
     ##########################################################
 
         # images
-        textLines = ['Image',
-                    'Damage',
-                    'Equipment'
+        # textLines = ['Image',
+        #             'Attributes',
+        #             'Condition'
+        # ]
+        textLines = ['Condition',
+                    'Attributes',
+                    'Rare damage'
         ]
         image_name = address + '.jpg'
         image_full_name = os.path.join(demoFolder,image_name)
 
         image = cv2.imread(image_full_name)
         height = image.shape[0]
         width = image.shape[1]
@@ -629,15 +741,16 @@
                 draw_width = new_width
                 draw_height = tmp_height
             text = pdf.beginText(100, 500)
             text.setFont("Courier", 12)
             text.setFillColor(colors.blue)
             text.textLine(textLines[-3])
             pdf.drawText(text)
-            pdf.drawInlineImage(image_full_name, 230, 440, width = draw_width, height = draw_height)
+            # pdf.drawInlineImage(image_full_name, 230, 440, width = draw_width, height = draw_height)
+            pdf.drawInlineImage(Roof_condition_image_name, 230, 440, width = draw_width, height = draw_height)
             pdf.linkURL(url, (200, 440, 230+draw_width, 440+draw_height), relative=1)
     # https://apps.nearmap.com/maps/#/@30.6622190,-88.1816001,20.00z,0d/V/20220110
 
             text = pdf.beginText(100, 300)
             text.setFont("Courier", 12)
             text.setFillColor(colors.blue)
             text.textLine(textLines[-2])
@@ -665,15 +778,16 @@
                 draw_width = new_width
                 draw_height = tmp_height
             text = pdf.beginText(310, 370)
             text.setFont("Courier", 12)
             text.setFillColor(colors.blue)
             text.textLine(textLines[-3])
             pdf.drawText(text)
-            pdf.drawInlineImage(image_full_name, 310, 380, width = draw_width, height = draw_height)
+            # pdf.drawInlineImage(image_full_name, 310, 380, width = draw_width, height = draw_height)
+            pdf.drawInlineImage(Roof_condition_image_name, 310, 380, width = draw_width, height = draw_height)
             pdf.linkURL(url, (310, 380, 310+draw_width, 380+draw_height), relative=1)
 
             text = pdf.beginText(40, 30)
             text.setFont("Courier", 12)
             text.setFillColor(colors.blue)
             text.textLine(textLines[-2])
             pdf.drawText(text)
@@ -689,311 +803,107 @@
             pdf.drawInlineImage(Equipment_image_name, 310, 40, width = draw_width, height = draw_height)
             pdf.linkURL(url, (310, 40, 310+draw_width, 40+draw_height), relative=1)
 
 
         # saving the pdf
         pdf.save()
 
-def generate_report_SB_referral_merged_mdoel(file_root_path,demoFolder= 'roof_score_new_20230101'):
-    # pred_damage_file = os.path.join(demoFolder,'prediction_Roof_damage/Roof_damage_all_in_one.json')
-    # pred_equip_file = os.path.join(demoFolder, 'prediction_Roof_equipment/Roof_equipment_all_in_one.json')
-    pred_phase3_file = os.path.join(demoFolder,'prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json')
-    pred_data_all_file = os.path.join(demoFolder, 'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json')
-    pred_boundary_file =os.path.join(demoFolder, 'prediction_Roof_boundary/Roof_boundary_all_in_one.json')
-
-    # read in referral rules and create corresponding functions
-    referral_label_file = os.path.join(file_root_path,'referral_labels_20221006.json')
-    damage_referral_label_file = os.path.join(file_root_path,'referral_labels_20221006_for_merged_damage.json')
-    with open(damage_referral_label_file) as f1:
-        ref_json = json.load(f1)
-    damage_cat = [x for x in ref_json]
-    # Load json file
-    # pred_damage = COCO(pred_damage_file)
-    # pred_equip = COCO(pred_equip_file)
-    pred_phase3 = COCO(pred_phase3_file)
-    pred_data_all = COCO(pred_data_all_file)
-    pred_boundary = COCO(pred_boundary_file)
-    generate_referral_damage_json(demoFolder, pred_data_all,pred_boundary,damage_cat,'Referral_damage.json')
-    
-    
-    equip_referral_label_file = os.path.join(file_root_path,'referral_labels_20221006_for_merged_equip.json')
-    with open(equip_referral_label_file) as f1:
-        ref_json = json.load(f1)
-    equip_cat = [x for x in ref_json]
-    generate_referral_damage_json(demoFolder, pred_data_all,pred_boundary,equip_cat,'Referral_equipment.json')
-    # generate_referral_json(demoFolder, pred_equip,cat,'Referral_equipment.json')
-    vis_out = merge_polygones(demoFolder,os.path.join(demoFolder, 'Referral_damage.json'),'Damage')
-    vis_out = merge_polygones(demoFolder,os.path.join(demoFolder, 'Referral_equipment.json'),'Equipment')
-    
-    # change back
-    referral_label_file = os.path.join(file_root_path,'referral_labels_20221006.json')
-
-    ################################### Referral
-    referral_damage = COCO(os.path.join(demoFolder, 'Referral_damage.json'))
-    referral_equip = COCO(os.path.join(demoFolder, 'Referral_equipment.json'))
-    referral_output = []
-    # Obtain the category ID numbers
-    catIds = referral_damage.getCatIds()
-    # Obtain the category names
-    categories = referral_damage.loadCats(catIds)
-    # Id2catname
-    Damage_labels = [value['name'] for value in categories]
-
-    # Obtain the category ID numbers
-    catIds = referral_equip.getCatIds()
-    # Obtain the category names
-    categories = referral_equip.loadCats(catIds)
-    # Id2catname
-    Equipment_labels = [value['name'] for value in categories]
-
-    for damage_img_id, equp_image_id in zip(referral_damage.getImgIds(), referral_equip.getImgIds()):
-        assert referral_damage.loadImgs(damage_img_id) == referral_equip.loadImgs(equp_image_id)
-        # get image information
-        coco_img_info = referral_damage.loadImgs(damage_img_id)[0]
-        address = os.path.splitext(coco_img_info['file_name'])[0]
-        print(address)
-        # zoom_level = int(address[-13:-11])
-
-        # using :-14 to only keep address no zoom level and date
-        # new_referral = ReferralPoints(referral_label_file, index=address[:-14])
-        new_referral = ReferralPoints(referral_label_file, index=address) 
-
-        # Roof Boundary
-        # new_referral.buffer['Roof boundary'] = np.sqrt(coco_img_info['height'] * coco_img_info['width'])
-        # new_referral.buffer['Roof_boundary'] = 0.5* coco_img_info['height'] * coco_img_info['width']
-        # print(coco_img_info['height'] * coco_img_info['width'])
-        new_referral.obtation_roof_boundary(pred_boundary, image_id = coco_img_info['id'])
-
-
-        # Damage
-        #################################################
-        new_referral.update_buffer_value(referral_damage, Damage_labels, image_id = coco_img_info['id'] )
-        # if zoom_level==22:
-        #     print(new_referral.buffer['Roof_boundary']*0.0002)
-        #     print(new_referral.buffer['Water pooling']['area_percentage']*new_referral.buffer['Roof_boundary']*0.0002)
-        # else:
-        #     print(new_referral.buffer['Roof_boundary']*0.00085)
-        #     print(new_referral.buffer['Water pooling']['area_percentage']*new_referral.buffer['Roof_boundary']*0.00085)
-
-        # Equipment
-        #################################################
-        new_referral.update_buffer_value(referral_equip, Equipment_labels, image_id = coco_img_info['id'])
-
-        new_referral.update_total_points()
-        referral_output.append(new_referral.score)
-        df = pd.DataFrame.from_dict([new_referral.score])
-        df.to_csv(os.path.join(demoFolder,address+'/referral.csv'), index=False, header=True)
-
-    df = pd.DataFrame.from_dict(referral_output)
-    df.to_csv(os.path.join(demoFolder,'all_referral.csv'), index=False, header=True)
-    image_csv = pd.read_csv(os.path.join(demoFolder,"image.csv"))
-    referral_csv = pd.read_csv(os.path.join(demoFolder,"all_referral.csv"))
-
-    image_csv.merge(referral_csv,how='outer',on='Address').to_csv(os.path.join(demoFolder, 'all_address.csv'), index=False, header=True)
-
-    ################################################################# PDF
-    image_csv = pd.read_csv(os.path.join(demoFolder,'image.csv'))
-    referral_csv = pd.read_csv(os.path.join(demoFolder,'all_referral.csv'))
-    all_address_csv = pd.read_csv(os.path.join(demoFolder, 'all_address.csv'))
-    # Today_date = datetime.today().strftime('%Y-%m-%d')
-    # # print(Today_date)
-    full_address = all_address_csv["Address"].tolist()
-    insured_name = all_address_csv["InsuredName"].tolist()
-    image_date = all_address_csv["Image date"].tolist()
-    image_info = all_address_csv["Image info"].tolist()
-    zoom_level = all_address_csv["Image level"].tolist()
-
-    key_name = all_address_csv.columns
-    key_name_index = all_address_csv.columns.get_loc('Total points')
-    gsd_key = all_address_csv.columns.get_loc('Image gsd (meters/pixels)')
-    pixels_area_key = all_address_csv.columns.get_loc('Roof area (pixels)')
-    # print(key_name[key_name_index])
-
-    for address_index in range(len(full_address)):
-        address = full_address[address_index]
-        row = all_address_csv.iloc[address_index]
-        print(f'index:{address_index}, address:{address}')
-        if np.isnan(row[key_name_index]):
-            continue
-        # initializing variables with values
-        url_zoom_level = zoom_level[address_index]
-        cat_lon_coord = image_info_to_center_lat_lon(image_info[address_index], url_zoom_level)
-        url_lat = cat_lon_coord[0]
-        url_lon = cat_lon_coord[1]
-        url_date = image_date[address_index].replace('-','')
-        url = f'https://apps.nearmap.com/maps/#/@{url_lat},{url_lon},{url_zoom_level}z,0d/V/{url_date}'
-
-        fileName = os.path.join(demoFolder,address+'.pdf')
-        documentTitle = f'Refferal'
-        title = f'{insured_name[address_index]}'
-        subTitle = address
-
-        Damage_image_name = os.path.join(demoFolder,address+'/Damage_merged.jpg')
-        Equipment_image_name = os.path.join(demoFolder,address+'/Equipment_merged.jpg')
-
-        pdf = canvas.Canvas(fileName)
-        pdf.setTitle(documentTitle)
-        pdf.setFont("Times-Roman", 14)
-        pdf.drawCentredString(300, 770, title)
-
-        pdf.setFillColorRGB(0, 0, 0)
-        pdf.setFont("Times-Roman", 12)
-        pdf.drawCentredString(290, 720, subTitle)
-
-        # drawing a line
-        pdf.line(30, 710, 550, 710)
-
-        # information
-        text = pdf.beginText(40, 670)
-        text.setFont("Courier", 12)
-        text.setFillColor(colors.blue)
-        text.textLine(f'Image date: {image_date[address_index]}')
-
-        if row[key_name_index]!=0:
-            line= f'Total points: {int(row[key_name_index])}'
-            text.textLine(line)
-        else:
-            line = 'Total points: 0'
-            text.textLine(line)
-        for i in range(key_name_index+1, len(key_name)):
-            if i == pixels_area_key:
-                gsd_area = row[gsd_key] * row[gsd_key] * row[pixels_area_key]
-                text.textLine(f'Roof area: {int(gsd_area)} m\u00b2')
-                continue
-            if row[i]>0:
-                line = key_name[i] + ': ' + str(int(row[i]))
-                text.textLine(line)
-        pdf.drawText(text)
-
-        # images
-        textLines = ['Image',
-                     'Damage',
-                     'Equipment'
-        ]
-        image_name = address + '.jpg'
-        image_full_name = os.path.join(demoFolder,image_name)
-
-        image = cv2.imread(image_full_name)
-        height = image.shape[0]
-        width = image.shape[1]
-        ratio = width/height
-
-        if height < width: # height < width horizontal
-            tmp_width = 350
-            tmp_height = 180
-            new_width = ratio * tmp_height
-            if new_width > tmp_width:
-                draw_width = tmp_width
-                draw_height = draw_width/ratio
-            else:
-                draw_width = new_width
-                draw_height = tmp_height
-            text = pdf.beginText(100, 500)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-3])
-            pdf.drawText(text)
-            pdf.drawInlineImage(image_full_name, 220, 440, width = draw_width, height = draw_height)
-
-
-            text = pdf.beginText(100, 300)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-2])
-            pdf.drawText(text)
-            pdf.drawInlineImage(Damage_image_name, 220, 240, width = draw_width, height = draw_height)
-
-
-            text = pdf.beginText(100, 100)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-1])
-            pdf.drawText(text)
-            pdf.drawInlineImage(Equipment_image_name, 220, 40, width = draw_width, height = draw_height)
-
-        else: # vertical
-            tmp_width = 250
-            tmp_height = 300
-            new_width = ratio * tmp_height
-            if new_width > tmp_width:
-                draw_width = tmp_width
-                draw_height = draw_width/ratio
-            else:
-                draw_width = new_width
-                draw_height = tmp_height
-            text = pdf.beginText(310, 370)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-3])
-            pdf.drawText(text)
-            pdf.drawInlineImage(image_full_name, 310, 380, width = draw_width, height = draw_height)
-
-
-            text = pdf.beginText(40, 30)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-2])
-            pdf.drawText(text)
-            pdf.drawInlineImage(Damage_image_name, 40, 40, width = draw_width, height = draw_height)
-
-
-            text = pdf.beginText(310, 30)
-            text.setFont("Courier", 12)
-            text.setFillColor(colors.blue)
-            text.textLine(textLines[-1])
-            pdf.drawText(text)
-            pdf.drawInlineImage(Equipment_image_name, 310, 40, width = draw_width, height = draw_height)
-
-        # saving the pdf
-        pdf.save()
-        
 def zipdir(folder, path, ziph):
     file_path = os.path.join(folder, path)
     # ziph is zipfile handle
     if not os.path.isdir(file_path):
         if path[-3:]=='jpg': # move the orignial image to image folder
             ziph.write(file_path,path.replace('.jpg','/Image.jpg'))
         else:
             ziph.write(file_path, path)
     else:
         for root, dirs, files in os.walk(file_path):           
             for file in files:
                 if file[0:4] != 'Roof': # don't include the roof boundary model
                     ziph.write(os.path.join(root, file), os.path.join(path, file))
-                    
-def zip_download_file(file_name):
+
+def zip_download_file(file_name, image_folder_name='roof_score_new_20230101'):
     ############################## ZIP
     # excel_file_path = "roof_score_new_20220803.csv"
     # excel_file_path = "roof_score_new_20220726.csv"
     # image_folder_name = os.path.splitext(os.path.basename(excel_file_path))[0]
 
     # import glob
     # jpgFilenamesList = glob.glob(image_folder_name + '/*.jpg')
     # pdfFilenamesList = glob.glob(image_folder_name + '/*.pdf')
         # for f in jpgFilenamesList:   
         #     myzip.write(f)
         # for f in pdfFilenamesList:   
         #     myzip.write(f)
-    image_folder_name = 'roof_score_new_20230101'
 
     file_list = [f for f in os.listdir(image_folder_name) if f[0].isnumeric()]
     print('Zipping')
     with zipfile.ZipFile(os.path.join(image_folder_name, file_name), 'w') as myzip:
         myzip.write(os.path.join(image_folder_name, 'all_address.csv'), 'all_address_' + image_folder_name[-8:] + '.csv')
         for f in file_list:    
             zipdir(image_folder_name, f, myzip)
     print('Zipping Done')
 
+def zip_download_file_csv(file_name, image_folder_name='roof_score_new_20230101'):
+    ############################## ZIP
+    # excel_file_path = "roof_score_new_20220803.csv"
+    # excel_file_path = "roof_score_new_20220726.csv"
+    # image_folder_name = os.path.splitext(os.path.basename(excel_file_path))[0]
+
+    # import glob
+    # jpgFilenamesList = glob.glob(image_folder_name + '/*.jpg')
+    # pdfFilenamesList = glob.glob(image_folder_name + '/*.pdf')
+        # for f in jpgFilenamesList:   
+        #     myzip.write(f)
+        # for f in pdfFilenamesList:   
+        #     myzip.write(f)
+
+    file_list = ['prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json',
+                 'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json',
+                 'prediction_Roof_boundary/Roof_boundary_all_in_one.json',
+                 # 'prediction_Roof_type/Roof_type_all_in_one.json',
+                 # 'prediction_Roof_material/Roof_material_all_in_one.json'
+                ]
+    print('Zipping')
+    with zipfile.ZipFile(os.path.join(image_folder_name, file_name), 'w') as myzip:
+        myzip.write(os.path.join(image_folder_name, 'all_referral.csv'), 'roof_condition_predicted.csv')
+        for f in file_list:    
+            zipdir(image_folder_name, f, myzip)
+    print('Zipping Done')
+
+def zip_download_condition_json(file_name, image_folder_name='roof_score_new_20230101'):
+    ############################## ZIP
+    # excel_file_path = "roof_score_new_20220803.csv"
+    # excel_file_path = "roof_score_new_20220726.csv"
+    # image_folder_name = os.path.splitext(os.path.basename(excel_file_path))[0]
+
+    # import glob
+    # jpgFilenamesList = glob.glob(image_folder_name + '/*.jpg')
+    # pdfFilenamesList = glob.glob(image_folder_name + '/*.pdf')
+        # for f in jpgFilenamesList:   
+        #     myzip.write(f)
+        # for f in pdfFilenamesList:   
+        #     myzip.write(f)
+
+    file_list = ['prediction_Roof_condition/Roof_condition_all_in_one.json']
+    print('Zipping')
+    with zipfile.ZipFile(os.path.join(image_folder_name, file_name), 'w') as myzip:
+        # myzip.write(os.path.join(image_folder_name, 'all_referral.csv'), 'roof_condition_predicted.csv')
+        for f in file_list:    
+            zipdir(image_folder_name, f, myzip)
+    print('Zipping Done')
+
 def send_email(receiver_email, address):
     host_server = 'smtp.qq.com'
     sender_qq = '1303242060'
     pwd = 'fhzevydopuvagfae'
     # pwd = input('Please input the password (not the login pwd)')
 
     sender_qq_mail = '1303242060@qq.com'
+    # receiver = 'ruixu_liu@cinfin.com'
 
     smtp = SMTP_SSL(host_server)
     smtp.set_debuglevel(0)   # 1 for debug
     smtp.ehlo(host_server)
     smtp.login(sender_qq, pwd)
```

