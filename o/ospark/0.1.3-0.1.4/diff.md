# Comparing `tmp/ospark-0.1.3.tar.gz` & `tmp/ospark-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospark-0.1.3.tar", max compression
+gzip compressed data, was "ospark-0.1.4.tar", max compression
```

## Comparing `ospark-0.1.3.tar` & `ospark-0.1.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0        0 2021-08-18 09:31:59.073140 ospark-0.1.3/LICENSE.rst
--rw-r--r--   0        0        0      409 2023-01-18 15:54:14.574296 ospark-0.1.3/ospark/__init__.py
--rw-r--r--   0        0        0       71 2022-08-11 11:17:58.069070 ospark-0.1.3/ospark/backbone/__init__.py
--rw-r--r--   0        0        0      940 2022-08-11 11:17:58.069190 ospark-0.1.3/ospark/backbone/auto_encoder.py
--rw-r--r--   0        0        0      934 2022-08-11 11:17:58.069315 ospark-0.1.3/ospark/backbone/backbone.py
--rw-r--r--   0        0        0     4258 2022-08-11 11:17:58.069451 ospark-0.1.3/ospark/backbone/builder.py
--rw-r--r--   0        0        0     1701 2022-08-11 11:17:58.069573 ospark-0.1.3/ospark/backbone/resnet.py
--rw-r--r--   0        0        0     2776 2022-08-11 11:17:58.069695 ospark-0.1.3/ospark/backbone/u_net.py
--rw-r--r--   0        0        0     6204 2023-01-18 15:54:14.596263 ospark-0.1.3/ospark/backbone/vision_transformer.py
--rw-r--r--   0        0        0        0 2022-08-11 11:17:58.069805 ospark-0.1.3/ospark/data/__init__.py
--rw-r--r--   0        0        0      713 2022-08-13 11:56:06.890961 ospark-0.1.3/ospark/data/data_operator.py
--rw-r--r--   0        0        0      792 2022-08-11 11:17:58.069971 ospark-0.1.3/ospark/data/encoder.py
--rw-r--r--   0        0        0     2069 2022-08-11 11:17:58.070085 ospark-0.1.3/ospark/data/folder.py
--rw-r--r--   0        0        0     2315 2022-08-11 11:17:58.070276 ospark-0.1.3/ospark/data/generator/__init__.py
--rw-r--r--   0        0        0    12747 2022-08-11 11:17:58.070482 ospark-0.1.3/ospark/data/generator/fots_data_generator.py
--rw-r--r--   0        0        0    10035 2022-08-11 11:17:58.070619 ospark-0.1.3/ospark/data/generator/translate_data_generator.py
--rw-r--r--   0        0        0     1136 2022-08-11 11:17:58.070741 ospark-0.1.3/ospark/data/path.py
--rw-r--r--   0        0        0      182 2022-08-13 11:56:06.891445 ospark-0.1.3/ospark/data/save_delege.py
--rw-r--r--   0        0        0      384 2022-08-11 11:17:58.070907 ospark-0.1.3/ospark/models/__init__.py
--rw-r--r--   0        0        0    11330 2022-08-11 11:17:58.071097 ospark-0.1.3/ospark/models/builder.py
--rw-r--r--   0        0        0     9334 2023-01-18 15:54:14.615217 ospark-0.1.3/ospark/models/coca.py
--rw-r--r--   0        0        0     4056 2022-08-11 11:17:58.071233 ospark-0.1.3/ospark/models/exdeep_transformer.py
--rw-r--r--   0        0        0     7862 2022-08-13 11:56:06.892115 ospark-0.1.3/ospark/models/former.py
--rw-r--r--   0        0        0     2542 2022-08-11 11:17:58.071464 ospark-0.1.3/ospark/models/informer.py
--rw-r--r--   0        0        0     2206 2022-08-11 11:17:58.071579 ospark-0.1.3/ospark/models/pixel_wise.py
--rw-r--r--   0        0        0     3776 2022-08-11 11:17:58.071709 ospark-0.1.3/ospark/models/text_recognition.py
--rw-r--r--   0        0        0     3514 2022-08-11 11:17:58.071839 ospark-0.1.3/ospark/models/transformer.py
--rw-r--r--   0        0        0        0 2021-08-18 09:35:24.525543 ospark-0.1.3/ospark/nn/__init__.py
--rw-r--r--   0        0        0     1683 2023-01-18 15:54:14.616748 ospark-0.1.3/ospark/nn/block/__init__.py
--rw-r--r--   0        0        0     1927 2022-08-11 11:17:58.072413 ospark-0.1.3/ospark/nn/block/connection_block.py
--rw-r--r--   0        0        0     5661 2022-08-11 11:17:58.072569 ospark-0.1.3/ospark/nn/block/deep_transformer_block.py
--rw-r--r--   0        0        0     8158 2023-01-18 15:54:14.617191 ospark-0.1.3/ospark/nn/block/informer_block.py
--rw-r--r--   0        0        0     8202 2022-08-13 11:56:06.892746 ospark-0.1.3/ospark/nn/block/resnet_block.py
--rw-r--r--   0        0        0    12410 2022-08-11 11:17:58.073144 ospark-0.1.3/ospark/nn/block/transformer_block.py
--rw-r--r--   0        0        0     4756 2023-01-18 15:54:14.617572 ospark-0.1.3/ospark/nn/block/vgg_block.py
--rw-r--r--   0        0        0     1068 2023-01-18 15:54:14.617934 ospark-0.1.3/ospark/nn/cell/__init__.py
--rw-r--r--   0        0        0     4220 2023-01-18 15:54:14.618320 ospark-0.1.3/ospark/nn/cell/resnet_cell.py
--rw-r--r--   0        0        0        0 2021-08-18 09:35:24.526424 ospark-0.1.3/ospark/nn/component/__init__.py
--rw-r--r--   0        0        0     4473 2023-01-18 15:54:14.619680 ospark-0.1.3/ospark/nn/component/basic_module.py
--rw-r--r--   0        0        0      977 2022-08-11 11:17:58.074157 ospark-0.1.3/ospark/nn/component/name_space.py
--rw-r--r--   0        0        0     5126 2023-01-18 15:54:14.620073 ospark-0.1.3/ospark/nn/component/weight.py
--rw-r--r--   0        0        0      513 2023-01-18 15:54:14.620446 ospark-0.1.3/ospark/nn/layers/__init__.py
--rw-r--r--   0        0        0     2153 2023-01-18 15:54:14.620698 ospark-0.1.3/ospark/nn/layers/activation.py
--rw-r--r--   0        0        0     2738 2023-01-18 15:54:14.621025 ospark-0.1.3/ospark/nn/layers/connection_layer.py
--rw-r--r--   0        0        0     4651 2023-01-18 15:54:14.621347 ospark-0.1.3/ospark/nn/layers/convolution_layer.py
--rw-r--r--   0        0        0     3466 2023-01-18 15:54:14.621670 ospark-0.1.3/ospark/nn/layers/deep_attention.py
--rw-r--r--   0        0        0     1819 2023-01-18 15:54:14.622010 ospark-0.1.3/ospark/nn/layers/deep_feed_forward.py
--rw-r--r--   0        0        0     2855 2023-01-18 15:54:14.622361 ospark-0.1.3/ospark/nn/layers/dense_layer.py
--rw-r--r--   0        0        0     3189 2023-01-18 15:54:14.622745 ospark-0.1.3/ospark/nn/layers/distilling_layer.py
--rw-r--r--   0        0        0     1752 2022-08-13 11:56:06.894793 ospark-0.1.3/ospark/nn/layers/embedding_layer.py
--rw-r--r--   0        0        0     3422 2023-01-18 15:54:14.623088 ospark-0.1.3/ospark/nn/layers/feed_forward.py
--rw-r--r--   0        0        0     2200 2023-01-18 15:54:14.623378 ospark-0.1.3/ospark/nn/layers/gated_linear_units.py
--rw-r--r--   0        0        0     8201 2023-01-18 15:54:14.623839 ospark-0.1.3/ospark/nn/layers/normalization.py
--rw-r--r--   0        0        0     2396 2022-08-11 11:17:58.075862 ospark-0.1.3/ospark/nn/layers/pooling_layer.py
--rw-r--r--   0        0        0     4516 2023-01-18 15:54:14.624256 ospark-0.1.3/ospark/nn/layers/prob_sparse.py
--rw-r--r--   0        0        0    20043 2023-01-18 15:54:14.624844 ospark-0.1.3/ospark/nn/layers/self_attention.py
--rw-r--r--   0        0        0       40 2023-01-18 15:54:14.625987 ospark-0.1.3/ospark/nn/loss_function/__init__.py
--rw-r--r--   0        0        0     1037 2023-01-18 15:54:14.626476 ospark-0.1.3/ospark/nn/loss_function/balanced_loss.py
--rw-r--r--   0        0        0      827 2023-01-18 15:54:14.626937 ospark-0.1.3/ospark/nn/loss_function/contrastive_loss.py
--rw-r--r--   0        0        0     1211 2023-01-18 15:54:14.627579 ospark-0.1.3/ospark/nn/loss_function/cross_entropy.py
--rw-r--r--   0        0        0      955 2023-01-18 15:54:14.627970 ospark-0.1.3/ospark/nn/loss_function/degree_loss.py
--rw-r--r--   0        0        0      438 2023-01-18 15:54:14.628293 ospark-0.1.3/ospark/nn/loss_function/dice_loss.py
--rw-r--r--   0        0        0      758 2023-01-18 15:54:14.628684 ospark-0.1.3/ospark/nn/loss_function/focal_loss.py
--rw-r--r--   0        0        0     2250 2023-01-18 15:54:14.629089 ospark-0.1.3/ospark/nn/loss_function/iou_loss.py
--rw-r--r--   0        0        0      468 2023-01-18 15:54:14.629495 ospark-0.1.3/ospark/nn/loss_function/loss_function.py
--rw-r--r--   0        0        0      714 2023-01-18 15:54:14.629944 ospark-0.1.3/ospark/nn/loss_function/sparse_categorical_cross_entropy.py
--rw-r--r--   0        0        0      257 2022-08-11 11:17:58.076614 ospark-0.1.3/ospark/nn/metrics/__init__.py
--rw-r--r--   0        0        0     1489 2022-08-11 11:17:58.076858 ospark-0.1.3/ospark/nn/metrics/confusion_matrix.py
--rw-r--r--   0        0        0     1422 2023-01-18 15:54:14.630353 ospark-0.1.3/ospark/nn/model.py
--rw-r--r--   0        0        0        0 2021-08-18 09:35:24.528499 ospark-0.1.3/ospark/nn/optimizer/__init__.py
--rw-r--r--   0        0        0      721 2022-08-11 11:17:58.077229 ospark-0.1.3/ospark/nn/optimizer/learning_rate_schedule.py
--rw-r--r--   0        0        0        0 2022-08-11 11:17:58.077348 ospark-0.1.3/ospark/ocr/__init__.py
--rw-r--r--   0        0        0    15922 2023-01-18 15:54:14.630923 ospark-0.1.3/ospark/ocr/fots.py
--rw-r--r--   0        0        0      500 2022-08-11 11:17:58.077693 ospark-0.1.3/ospark/predictor/__init__.py
--rw-r--r--   0        0        0     5089 2022-08-11 11:17:58.077839 ospark-0.1.3/ospark/predictor/fots_predictor.py
--rw-r--r--   0        0        0     2564 2022-08-11 11:17:58.077957 ospark-0.1.3/ospark/predictor/translator.py
--rw-r--r--   0        0        0        0 2023-01-18 15:54:14.631020 ospark-0.1.3/ospark/samples/__init__.py
--rw-r--r--   0        0        0     8408 2023-01-18 15:54:14.631453 ospark-0.1.3/ospark/samples/exdeep_transformer_sample.py
--rw-r--r--   0        0        0     2907 2022-08-11 11:17:58.078311 ospark-0.1.3/ospark/samples/fots_sample.py
--rw-r--r--   0        0        0     4571 2022-08-11 11:17:58.078462 ospark-0.1.3/ospark/samples/translator_sample.py
--rw-r--r--   0        0        0     6190 2023-01-18 15:54:14.631940 ospark-0.1.3/ospark/trainer/__init__.py
--rw-r--r--   0        0        0     1029 2023-01-18 15:54:14.632302 ospark-0.1.3/ospark/trainer/coca_trainer.py
--rw-r--r--   0        0        0     5812 2023-01-18 15:54:14.632775 ospark-0.1.3/ospark/trainer/exdeep_transformer.py
--rw-r--r--   0        0        0     5234 2023-01-18 15:54:14.633313 ospark-0.1.3/ospark/trainer/transformer_trainer.py
--rw-r--r--   0        0        0        0 2022-08-11 11:17:58.079060 ospark-0.1.3/ospark/utility/__init__.py
--rw-r--r--   0        0        0     1841 2022-08-11 11:17:58.079216 ospark-0.1.3/ospark/utility/non_max_suppression.py
--rw-r--r--   0        0        0     3271 2022-08-11 11:17:58.079344 ospark-0.1.3/ospark/utility/padding_method.py
--rw-r--r--   0        0        0    11438 2022-08-11 11:17:58.079621 ospark-0.1.3/ospark/utility/roi_rotate.py
--rw-r--r--   0        0        0     2010 2022-08-13 11:56:06.896196 ospark-0.1.3/ospark/utility/weight_initializer.py
--rw-r--r--   0        0        0        0 2023-01-18 15:54:14.633604 ospark-0.1.3/ospark/validator/__init__.py
--rw-r--r--   0        0        0      964 2023-01-18 16:37:43.103165 ospark-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1021 2023-01-18 16:38:34.951616 ospark-0.1.3/setup.py
--rw-r--r--   0        0        0      845 2023-01-18 16:38:34.951888 ospark-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-08-18 09:31:59.073140 ospark-0.1.4/LICENSE.rst
+-rw-r--r--   0        0        0      409 2023-04-19 13:43:02.887648 ospark-0.1.4/ospark/__init__.py
+-rw-r--r--   0        0        0       71 2022-08-11 11:17:58.069070 ospark-0.1.4/ospark/backbone/__init__.py
+-rw-r--r--   0        0        0      940 2022-08-11 11:17:58.069190 ospark-0.1.4/ospark/backbone/auto_encoder.py
+-rw-r--r--   0        0        0      934 2022-08-11 11:17:58.069315 ospark-0.1.4/ospark/backbone/backbone.py
+-rw-r--r--   0        0        0     4258 2022-08-11 11:17:58.069451 ospark-0.1.4/ospark/backbone/builder.py
+-rw-r--r--   0        0        0     1701 2022-08-11 11:17:58.069573 ospark-0.1.4/ospark/backbone/resnet.py
+-rw-r--r--   0        0        0     2776 2022-08-11 11:17:58.069695 ospark-0.1.4/ospark/backbone/u_net.py
+-rw-r--r--   0        0        0     6204 2023-01-18 15:54:14.596263 ospark-0.1.4/ospark/backbone/vision_transformer.py
+-rw-r--r--   0        0        0        0 2022-08-11 11:17:58.069805 ospark-0.1.4/ospark/data/__init__.py
+-rw-r--r--   0        0        0      713 2022-08-13 11:56:06.890961 ospark-0.1.4/ospark/data/data_operator.py
+-rw-r--r--   0        0        0      792 2022-08-11 11:17:58.069971 ospark-0.1.4/ospark/data/encoder.py
+-rw-r--r--   0        0        0     2069 2022-08-11 11:17:58.070085 ospark-0.1.4/ospark/data/folder.py
+-rw-r--r--   0        0        0     2315 2022-08-11 11:17:58.070276 ospark-0.1.4/ospark/data/generator/__init__.py
+-rw-r--r--   0        0        0    12747 2022-08-11 11:17:58.070482 ospark-0.1.4/ospark/data/generator/fots_data_generator.py
+-rw-r--r--   0        0        0    10035 2023-01-30 10:42:23.961309 ospark-0.1.4/ospark/data/generator/translate_data_generator.py
+-rw-r--r--   0        0        0     1136 2022-08-11 11:17:58.070741 ospark-0.1.4/ospark/data/path.py
+-rw-r--r--   0        0        0      182 2022-08-13 11:56:06.891445 ospark-0.1.4/ospark/data/save_delege.py
+-rw-r--r--   0        0        0      384 2022-08-11 11:17:58.070907 ospark-0.1.4/ospark/models/__init__.py
+-rw-r--r--   0        0        0    11330 2022-08-11 11:17:58.071097 ospark-0.1.4/ospark/models/builder.py
+-rw-r--r--   0        0        0     9334 2023-01-18 15:54:14.615217 ospark-0.1.4/ospark/models/coca.py
+-rw-r--r--   0        0        0     4056 2022-08-11 11:17:58.071233 ospark-0.1.4/ospark/models/exdeep_transformer.py
+-rw-r--r--   0        0        0     7862 2022-08-13 11:56:06.892115 ospark-0.1.4/ospark/models/former.py
+-rw-r--r--   0        0        0     2542 2022-08-11 11:17:58.071464 ospark-0.1.4/ospark/models/informer.py
+-rw-r--r--   0        0        0     2206 2022-08-11 11:17:58.071579 ospark-0.1.4/ospark/models/pixel_wise.py
+-rw-r--r--   0        0        0     3776 2022-08-11 11:17:58.071709 ospark-0.1.4/ospark/models/text_recognition.py
+-rw-r--r--   0        0        0     3514 2022-08-11 11:17:58.071839 ospark-0.1.4/ospark/models/transformer.py
+-rw-r--r--   0        0        0        0 2021-08-18 09:35:24.525543 ospark-0.1.4/ospark/nn/__init__.py
+-rw-r--r--   0        0        0     1683 2023-01-18 15:54:14.616748 ospark-0.1.4/ospark/nn/block/__init__.py
+-rw-r--r--   0        0        0     1927 2022-08-11 11:17:58.072413 ospark-0.1.4/ospark/nn/block/connection_block.py
+-rw-r--r--   0        0        0     5661 2022-08-11 11:17:58.072569 ospark-0.1.4/ospark/nn/block/deep_transformer_block.py
+-rw-r--r--   0        0        0     8158 2023-01-18 15:54:14.617191 ospark-0.1.4/ospark/nn/block/informer_block.py
+-rw-r--r--   0        0        0     8202 2022-08-13 11:56:06.892746 ospark-0.1.4/ospark/nn/block/resnet_block.py
+-rw-r--r--   0        0        0    12410 2022-08-11 11:17:58.073144 ospark-0.1.4/ospark/nn/block/transformer_block.py
+-rw-r--r--   0        0        0     4756 2023-01-18 15:54:14.617572 ospark-0.1.4/ospark/nn/block/vgg_block.py
+-rw-r--r--   0        0        0     1068 2023-01-18 15:54:14.617934 ospark-0.1.4/ospark/nn/cell/__init__.py
+-rw-r--r--   0        0        0     4220 2023-01-18 15:54:14.618320 ospark-0.1.4/ospark/nn/cell/resnet_cell.py
+-rw-r--r--   0        0        0        0 2021-08-18 09:35:24.526424 ospark-0.1.4/ospark/nn/component/__init__.py
+-rw-r--r--   0        0        0     4473 2023-01-18 15:54:14.619680 ospark-0.1.4/ospark/nn/component/basic_module.py
+-rw-r--r--   0        0        0      977 2022-08-11 11:17:58.074157 ospark-0.1.4/ospark/nn/component/name_space.py
+-rw-r--r--   0        0        0     5126 2023-01-18 15:54:14.620073 ospark-0.1.4/ospark/nn/component/weight.py
+-rw-r--r--   0        0        0      513 2023-01-18 15:54:14.620446 ospark-0.1.4/ospark/nn/layers/__init__.py
+-rw-r--r--   0        0        0     2153 2023-01-18 15:54:14.620698 ospark-0.1.4/ospark/nn/layers/activation.py
+-rw-r--r--   0        0        0     2738 2023-01-18 15:54:14.621025 ospark-0.1.4/ospark/nn/layers/connection_layer.py
+-rw-r--r--   0        0        0     4651 2023-01-18 15:54:14.621347 ospark-0.1.4/ospark/nn/layers/convolution_layer.py
+-rw-r--r--   0        0        0     3466 2023-01-18 15:54:14.621670 ospark-0.1.4/ospark/nn/layers/deep_attention.py
+-rw-r--r--   0        0        0     1819 2023-01-18 15:54:14.622010 ospark-0.1.4/ospark/nn/layers/deep_feed_forward.py
+-rw-r--r--   0        0        0     2855 2023-01-18 15:54:14.622361 ospark-0.1.4/ospark/nn/layers/dense_layer.py
+-rw-r--r--   0        0        0     3189 2023-01-18 15:54:14.622745 ospark-0.1.4/ospark/nn/layers/distilling_layer.py
+-rw-r--r--   0        0        0     1752 2022-08-13 11:56:06.894793 ospark-0.1.4/ospark/nn/layers/embedding_layer.py
+-rw-r--r--   0        0        0     3422 2023-01-18 15:54:14.623088 ospark-0.1.4/ospark/nn/layers/feed_forward.py
+-rw-r--r--   0        0        0     2200 2023-01-18 15:54:14.623378 ospark-0.1.4/ospark/nn/layers/gated_linear_units.py
+-rw-r--r--   0        0        0     8201 2023-01-18 15:54:14.623839 ospark-0.1.4/ospark/nn/layers/normalization.py
+-rw-r--r--   0        0        0     2396 2022-08-11 11:17:58.075862 ospark-0.1.4/ospark/nn/layers/pooling_layer.py
+-rw-r--r--   0        0        0     4516 2023-01-18 15:54:14.624256 ospark-0.1.4/ospark/nn/layers/prob_sparse.py
+-rw-r--r--   0        0        0    20043 2023-01-18 15:54:14.624844 ospark-0.1.4/ospark/nn/layers/self_attention.py
+-rw-r--r--   0        0        0       40 2023-01-18 15:54:14.625987 ospark-0.1.4/ospark/nn/loss_function/__init__.py
+-rw-r--r--   0        0        0     1037 2023-01-18 15:54:14.626476 ospark-0.1.4/ospark/nn/loss_function/balanced_loss.py
+-rw-r--r--   0        0        0      827 2023-01-18 15:54:14.626937 ospark-0.1.4/ospark/nn/loss_function/contrastive_loss.py
+-rw-r--r--   0        0        0     1211 2023-01-18 15:54:14.627579 ospark-0.1.4/ospark/nn/loss_function/cross_entropy.py
+-rw-r--r--   0        0        0      955 2023-01-18 15:54:14.627970 ospark-0.1.4/ospark/nn/loss_function/degree_loss.py
+-rw-r--r--   0        0        0      438 2023-01-18 15:54:14.628293 ospark-0.1.4/ospark/nn/loss_function/dice_loss.py
+-rw-r--r--   0        0        0      758 2023-01-18 15:54:14.628684 ospark-0.1.4/ospark/nn/loss_function/focal_loss.py
+-rw-r--r--   0        0        0     2250 2023-01-18 15:54:14.629089 ospark-0.1.4/ospark/nn/loss_function/iou_loss.py
+-rw-r--r--   0        0        0      468 2023-01-18 15:54:14.629495 ospark-0.1.4/ospark/nn/loss_function/loss_function.py
+-rw-r--r--   0        0        0      714 2023-01-18 15:54:14.629944 ospark-0.1.4/ospark/nn/loss_function/sparse_categorical_cross_entropy.py
+-rw-r--r--   0        0        0      257 2022-08-11 11:17:58.076614 ospark-0.1.4/ospark/nn/metrics/__init__.py
+-rw-r--r--   0        0        0     1489 2022-08-11 11:17:58.076858 ospark-0.1.4/ospark/nn/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     1422 2023-01-18 15:54:14.630353 ospark-0.1.4/ospark/nn/model.py
+-rw-r--r--   0        0        0        0 2021-08-18 09:35:24.528499 ospark-0.1.4/ospark/nn/optimizer/__init__.py
+-rw-r--r--   0        0        0      721 2022-08-11 11:17:58.077229 ospark-0.1.4/ospark/nn/optimizer/learning_rate_schedule.py
+-rw-r--r--   0        0        0        0 2022-08-11 11:17:58.077348 ospark-0.1.4/ospark/ocr/__init__.py
+-rw-r--r--   0        0        0    15922 2023-01-18 15:54:14.630923 ospark-0.1.4/ospark/ocr/fots.py
+-rw-r--r--   0        0        0      500 2022-08-11 11:17:58.077693 ospark-0.1.4/ospark/predictor/__init__.py
+-rw-r--r--   0        0        0     5089 2022-08-11 11:17:58.077839 ospark-0.1.4/ospark/predictor/fots_predictor.py
+-rw-r--r--   0        0        0     2564 2022-08-11 11:17:58.077957 ospark-0.1.4/ospark/predictor/translator.py
+-rw-r--r--   0        0        0        0 2023-01-18 15:54:14.631020 ospark-0.1.4/ospark/samples/__init__.py
+-rw-r--r--   0        0        0     8408 2023-01-18 15:54:14.631453 ospark-0.1.4/ospark/samples/exdeep_transformer_sample.py
+-rw-r--r--   0        0        0     2907 2022-08-11 11:17:58.078311 ospark-0.1.4/ospark/samples/fots_sample.py
+-rw-r--r--   0        0        0     4571 2022-08-11 11:17:58.078462 ospark-0.1.4/ospark/samples/translator_sample.py
+-rw-r--r--   0        0        0     6190 2023-01-18 15:54:14.631940 ospark-0.1.4/ospark/trainer/__init__.py
+-rw-r--r--   0        0        0     1029 2023-01-18 15:54:14.632302 ospark-0.1.4/ospark/trainer/coca_trainer.py
+-rw-r--r--   0        0        0     5812 2023-01-18 15:54:14.632775 ospark-0.1.4/ospark/trainer/exdeep_transformer.py
+-rw-r--r--   0        0        0     5234 2023-01-18 15:54:14.633313 ospark-0.1.4/ospark/trainer/transformer_trainer.py
+-rw-r--r--   0        0        0        0 2022-08-11 11:17:58.079060 ospark-0.1.4/ospark/utility/__init__.py
+-rw-r--r--   0        0        0     1841 2022-08-11 11:17:58.079216 ospark-0.1.4/ospark/utility/non_max_suppression.py
+-rw-r--r--   0        0        0     3271 2022-08-11 11:17:58.079344 ospark-0.1.4/ospark/utility/padding_method.py
+-rw-r--r--   0        0        0    11438 2022-08-11 11:17:58.079621 ospark-0.1.4/ospark/utility/roi_rotate.py
+-rw-r--r--   0        0        0     2010 2022-08-13 11:56:06.896196 ospark-0.1.4/ospark/utility/weight_initializer.py
+-rw-r--r--   0        0        0        0 2023-01-18 15:54:14.633604 ospark-0.1.4/ospark/validator/__init__.py
+-rw-r--r--   0        0        0      965 2023-04-19 13:42:45.771301 ospark-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1022 2023-04-19 13:52:38.884923 ospark-0.1.4/setup.py
+-rw-r--r--   0        0        0      846 2023-04-19 13:52:38.885376 ospark-0.1.4/PKG-INFO
```

### Comparing `ospark-0.1.3/ospark/backbone/auto_encoder.py` & `ospark-0.1.4/ospark/backbone/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/backbone/backbone.py` & `ospark-0.1.4/ospark/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/backbone/builder.py` & `ospark-0.1.4/ospark/backbone/builder.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/backbone/resnet.py` & `ospark-0.1.4/ospark/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/backbone/u_net.py` & `ospark-0.1.4/ospark/backbone/u_net.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/backbone/vision_transformer.py` & `ospark-0.1.4/ospark/backbone/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/data_operator.py` & `ospark-0.1.4/ospark/data/data_operator.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/encoder.py` & `ospark-0.1.4/ospark/data/encoder.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/folder.py` & `ospark-0.1.4/ospark/data/folder.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/generator/__init__.py` & `ospark-0.1.4/ospark/data/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/generator/fots_data_generator.py` & `ospark-0.1.4/ospark/data/generator/fots_data_generator.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/generator/translate_data_generator.py` & `ospark-0.1.4/ospark/data/generator/translate_data_generator.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/data/path.py` & `ospark-0.1.4/ospark/data/path.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/builder.py` & `ospark-0.1.4/ospark/models/builder.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/coca.py` & `ospark-0.1.4/ospark/models/coca.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/exdeep_transformer.py` & `ospark-0.1.4/ospark/models/exdeep_transformer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/former.py` & `ospark-0.1.4/ospark/models/former.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/informer.py` & `ospark-0.1.4/ospark/models/informer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/pixel_wise.py` & `ospark-0.1.4/ospark/models/pixel_wise.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/text_recognition.py` & `ospark-0.1.4/ospark/models/text_recognition.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/models/transformer.py` & `ospark-0.1.4/ospark/models/transformer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/__init__.py` & `ospark-0.1.4/ospark/nn/block/__init__.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/connection_block.py` & `ospark-0.1.4/ospark/nn/block/connection_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/deep_transformer_block.py` & `ospark-0.1.4/ospark/nn/block/deep_transformer_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/informer_block.py` & `ospark-0.1.4/ospark/nn/block/informer_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/resnet_block.py` & `ospark-0.1.4/ospark/nn/block/resnet_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/transformer_block.py` & `ospark-0.1.4/ospark/nn/block/transformer_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/block/vgg_block.py` & `ospark-0.1.4/ospark/nn/block/vgg_block.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/cell/__init__.py` & `ospark-0.1.4/ospark/nn/cell/__init__.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/cell/resnet_cell.py` & `ospark-0.1.4/ospark/nn/cell/resnet_cell.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/component/basic_module.py` & `ospark-0.1.4/ospark/nn/component/basic_module.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/component/name_space.py` & `ospark-0.1.4/ospark/nn/component/name_space.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/component/weight.py` & `ospark-0.1.4/ospark/nn/component/weight.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/__init__.py` & `ospark-0.1.4/ospark/nn/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/activation.py` & `ospark-0.1.4/ospark/nn/layers/activation.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/connection_layer.py` & `ospark-0.1.4/ospark/nn/layers/connection_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/convolution_layer.py` & `ospark-0.1.4/ospark/nn/layers/convolution_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/deep_attention.py` & `ospark-0.1.4/ospark/nn/layers/deep_attention.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/deep_feed_forward.py` & `ospark-0.1.4/ospark/nn/layers/deep_feed_forward.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/dense_layer.py` & `ospark-0.1.4/ospark/nn/layers/dense_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/distilling_layer.py` & `ospark-0.1.4/ospark/nn/layers/distilling_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/embedding_layer.py` & `ospark-0.1.4/ospark/nn/layers/embedding_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/feed_forward.py` & `ospark-0.1.4/ospark/nn/layers/feed_forward.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/gated_linear_units.py` & `ospark-0.1.4/ospark/nn/layers/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/normalization.py` & `ospark-0.1.4/ospark/nn/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/pooling_layer.py` & `ospark-0.1.4/ospark/nn/layers/pooling_layer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/prob_sparse.py` & `ospark-0.1.4/ospark/nn/layers/prob_sparse.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/layers/self_attention.py` & `ospark-0.1.4/ospark/nn/layers/self_attention.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/balanced_loss.py` & `ospark-0.1.4/ospark/nn/loss_function/balanced_loss.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/contrastive_loss.py` & `ospark-0.1.4/ospark/nn/loss_function/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/cross_entropy.py` & `ospark-0.1.4/ospark/nn/loss_function/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/degree_loss.py` & `ospark-0.1.4/ospark/nn/loss_function/degree_loss.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/focal_loss.py` & `ospark-0.1.4/ospark/nn/loss_function/focal_loss.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/iou_loss.py` & `ospark-0.1.4/ospark/nn/loss_function/iou_loss.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/loss_function/sparse_categorical_cross_entropy.py` & `ospark-0.1.4/ospark/nn/loss_function/sparse_categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/metrics/confusion_matrix.py` & `ospark-0.1.4/ospark/nn/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/model.py` & `ospark-0.1.4/ospark/nn/model.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/nn/optimizer/learning_rate_schedule.py` & `ospark-0.1.4/ospark/nn/optimizer/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/ocr/fots.py` & `ospark-0.1.4/ospark/ocr/fots.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/predictor/fots_predictor.py` & `ospark-0.1.4/ospark/predictor/fots_predictor.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/predictor/translator.py` & `ospark-0.1.4/ospark/predictor/translator.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/samples/exdeep_transformer_sample.py` & `ospark-0.1.4/ospark/samples/exdeep_transformer_sample.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/samples/fots_sample.py` & `ospark-0.1.4/ospark/samples/fots_sample.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/samples/translator_sample.py` & `ospark-0.1.4/ospark/samples/translator_sample.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/trainer/__init__.py` & `ospark-0.1.4/ospark/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/trainer/coca_trainer.py` & `ospark-0.1.4/ospark/trainer/coca_trainer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/trainer/exdeep_transformer.py` & `ospark-0.1.4/ospark/trainer/exdeep_transformer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/trainer/transformer_trainer.py` & `ospark-0.1.4/ospark/trainer/transformer_trainer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/utility/non_max_suppression.py` & `ospark-0.1.4/ospark/utility/non_max_suppression.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/utility/padding_method.py` & `ospark-0.1.4/ospark/utility/padding_method.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/utility/roi_rotate.py` & `ospark-0.1.4/ospark/utility/roi_rotate.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/ospark/utility/weight_initializer.py` & `ospark-0.1.4/ospark/utility/weight_initializer.py`

 * *Files identical despite different names*

### Comparing `ospark-0.1.3/setup.py` & `ospark-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,19 +22,19 @@
  'ospark.utility',
  'ospark.validator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['tensorflow>=2.7.0,<3.0.0']
+['tensorflow>=2.12.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ospark',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Ospark is an opensource for quickly builder of former model series.',
     'long_description': None,
     'author': 'ospark-org',
     'author_email': 'donggicai1991@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ospark-0.1.3/PKG-INFO` & `ospark-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospark
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ospark is an opensource for quickly builder of former model series.
 License: Apache-2.0
 Keywords: text recognition,NLP,attention,tensorflow,transformer
 Author: ospark-org
 Author-email: donggicai1991@gmail.com
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -13,8 +13,8 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: tensorflow (>=2.7.0,<3.0.0)
+Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
```

