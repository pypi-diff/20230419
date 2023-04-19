# Comparing `tmp/laion_clap-1.1.3.tar.gz` & `tmp/laion_clap-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laion_clap-1.1.3.tar", last modified: Mon Apr 10 03:47:12 2023, max compression
+gzip compressed data, was "laion_clap-1.1.4.tar", last modified: Wed Apr 19 20:43:18 2023, max compression
```

## Comparing `laion_clap-1.1.3.tar` & `laion_clap-1.1.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.618166 laion_clap-1.1.3/
--rw-rw-r--   0 la        (1000) la        (1000)     7048 2023-02-28 19:23:25.000000 laion_clap-1.1.3/LICENSE
--rw-rw-r--   0 la        (1000) la        (1000)      203 2023-03-14 06:16:18.000000 laion_clap-1.1.3/MANIFEST.in
--rw-rw-r--   0 la        (1000) la        (1000)    23293 2023-04-10 03:47:12.618166 laion_clap-1.1.3/PKG-INFO
--rw-rw-r--   0 la        (1000) la        (1000)    14488 2023-04-10 03:33:21.000000 laion_clap-1.1.3/README.md
--rw-rw-r--   0 la        (1000) la        (1000)     1218 2023-04-10 03:46:52.000000 laion_clap-1.1.3/pyproject.toml
--rw-rw-r--   0 la        (1000) la        (1000)       38 2023-04-10 03:47:12.618166 laion_clap-1.1.3/setup.cfg
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/laion_clap/
--rw-rw-r--   0 la        (1000) la        (1000)      129 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/__init__.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/clap_module/
--rw-rw-r--   0 la        (1000) la        (1000)      568 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)     1215 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/bert.py
--rw-rw-r--   0 la        (1000) la        (1000)  1356917 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 la        (1000) la        (1000)    10593 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/factory.py
--rw-rw-r--   0 la        (1000) la        (1000)     7182 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/feature_fusion.py
--rw-rw-r--   0 la        (1000) la        (1000)    45110 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/htsat.py
--rw-rw-r--   0 la        (1000) la        (1000)     2204 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/linear_probe.py
--rw-rw-r--   0 la        (1000) la        (1000)    14405 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/loss.py
--rw-rw-r--   0 la        (1000) la        (1000)    32754 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-base.json
--rw-rw-r--   0 la        (1000) la        (1000)      498 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-large.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-tiny-win-1536.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-tiny.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-10.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-fmax-18k.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-fmax-8k-20s.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-tiny-transformer.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-win-1536.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14.json
--rw-rw-r--   0 la        (1000) la        (1000)      495 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-6.json
--rw-rw-r--   0 la        (1000) la        (1000)      388 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN101-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN101.json
--rw-rw-r--   0 la        (1000) la        (1000)      389 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50.json
--rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50x16.json
--rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50x4.json
--rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-16.json
--rw-rw-r--   0 la        (1000) la        (1000)      318 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-32-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-32.json
--rw-rw-r--   0 la        (1000) la        (1000)      296 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-L-14.json
--rw-rw-r--   0 la        (1000) la        (1000)     4724 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/openai.py
--rw-rw-r--   0 la        (1000) la        (1000)    21221 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/pann_model.py
--rw-rw-r--   0 la        (1000) la        (1000)     6212 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/pretrained.py
--rw-rw-r--   0 la        (1000) la        (1000)     4300 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/timm_model.py
--rw-rw-r--   0 la        (1000) la        (1000)     6204 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/tokenizer.py
--rw-rw-r--   0 la        (1000) la        (1000)      872 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/transform.py
--rw-rw-r--   0 la        (1000) la        (1000)    12988 2023-04-01 20:15:10.000000 laion_clap-1.1.3/src/laion_clap/clap_module/utils.py
--rw-rw-r--   0 la        (1000) la        (1000)       22 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/version.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/evaluate/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)     5455 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_dcase.py
--rw-rw-r--   0 la        (1000) la        (1000)    20038 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_linear_probe.py
--rw-rw-r--   0 la        (1000) la        (1000)     6718 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval.py
--rw-rw-r--   0 la        (1000) la        (1000)     9557 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval_main.py
--rw-rw-r--   0 la        (1000) la        (1000)     9769 2023-04-10 03:33:21.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_zeroshot_classification.py
--rw-rw-r--   0 la        (1000) la        (1000)     8767 2023-04-10 03:35:37.000000 laion_clap-1.1.3/src/laion_clap/hook.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/training/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)    84448 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/audioset_textmap.npy
--rw-rw-r--   0 la        (1000) la        (1000)    32641 2023-04-10 03:33:21.000000 laion_clap-1.1.3/src/laion_clap/training/data.py
--rw-rw-r--   0 la        (1000) la        (1000)     5078 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/distributed.py
--rw-rw-r--   0 la        (1000) la        (1000)    22135 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/imagenet_zeroshot_data.py
--rw-rw-r--   0 la        (1000) la        (1000)     3265 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/infer_demo.py
--rw-rw-r--   0 la        (1000) la        (1000)      899 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/logger.py
--rw-rw-r--   0 la        (1000) la        (1000)    25047 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/lp_main.py
--rw-rw-r--   0 la        (1000) la        (1000)    10645 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/lp_train.py
--rw-rw-r--   0 la        (1000) la        (1000)    22608 2023-04-01 20:31:07.000000 laion_clap-1.1.3/src/laion_clap/training/main.py
--rw-rw-r--   0 la        (1000) la        (1000)    17401 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/params.py
--rw-rw-r--   0 la        (1000) la        (1000)      659 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/scheduler.py
--rw-rw-r--   0 la        (1000) la        (1000)    35672 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/train.py
--rw-rw-r--   0 la        (1000) la        (1000)     3395 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/zero_shot.py
--rw-rw-r--   0 la        (1000) la        (1000)     2596 2023-04-01 20:34:21.000000 laion_clap-1.1.3/src/laion_clap/unit_test.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/laion_clap.egg-info/
--rw-rw-r--   0 la        (1000) la        (1000)    23293 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/PKG-INFO
--rw-rw-r--   0 la        (1000) la        (1000)     3095 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/SOURCES.txt
--rw-rw-r--   0 la        (1000) la        (1000)        1 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/dependency_links.txt
--rw-rw-r--   0 la        (1000) la        (1000)      160 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/requires.txt
--rw-rw-r--   0 la        (1000) la        (1000)       17 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/top_level.txt
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/tests/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)    56326 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/check_ckpt.py
--rw-rw-r--   0 la        (1000) la        (1000)     3295 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/check_tars.py
--rw-rw-r--   0 la        (1000) la        (1000)     2174 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/data_loader_test.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.964179 laion_clap-1.1.4/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     7048 2023-04-05 02:26:50.000000 laion_clap-1.1.4/LICENSE
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      203 2023-04-05 02:26:50.000000 laion_clap-1.1.4/MANIFEST.in
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    25816 2023-04-19 20:43:18.964179 laion_clap-1.1.4/PKG-INFO
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    17011 2023-04-19 20:16:17.000000 laion_clap-1.1.4/README.md
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     1218 2023-04-19 20:42:16.000000 laion_clap-1.1.4/pyproject.toml
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)       38 2023-04-19 20:43:18.964179 laion_clap-1.1.4/setup.cfg
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.956179 laion_clap-1.1.4/src/
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.956179 laion_clap-1.1.4/src/laion_clap/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      130 2023-04-19 20:21:51.000000 laion_clap-1.1.4/src/laion_clap/__init__.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.960179 laion_clap-1.1.4/src/laion_clap/clap_module/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      568 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/__init__.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     1215 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/bert.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)  1356917 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    10593 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/factory.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     7182 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/feature_fusion.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    45110 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/htsat.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     2204 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/linear_probe.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    14405 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/loss.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    32754 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.960179 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      497 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/HTSAT-base.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      498 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/HTSAT-large.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      496 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/HTSAT-tiny-win-1536.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      496 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/HTSAT-tiny.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      497 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-10.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      497 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-14-fmax-18k.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      496 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-14-fmax-8k-20s.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      496 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-14-tiny-transformer.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      497 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-14-win-1536.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      497 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-14.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      495 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/PANN-6.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      388 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN101-quickgelu.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      364 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN101.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      389 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN50-quickgelu.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      364 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN50.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      365 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN50x16.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      365 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/RN50x4.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      294 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/ViT-B-16.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      318 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      294 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/ViT-B-32.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      296 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/model_configs/ViT-L-14.json
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     4724 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/openai.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    21221 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/pann_model.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     6212 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/pretrained.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     4300 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/timm_model.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     6204 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/tokenizer.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      872 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/transform.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    12988 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/utils.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)       22 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/clap_module/version.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.964179 laion_clap-1.1.4/src/laion_clap/evaluate/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)        0 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/evaluate/__init__.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     5455 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/evaluate/eval_dcase.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    20038 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/evaluate/eval_linear_probe.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     6718 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/evaluate/eval_retrieval.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     9557 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/evaluate/eval_retrieval_main.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     9769 2023-04-19 20:16:17.000000 laion_clap-1.1.4/src/laion_clap/evaluate/eval_zeroshot_classification.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     8767 2023-04-19 20:16:17.000000 laion_clap-1.1.4/src/laion_clap/hook.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.964179 laion_clap-1.1.4/src/laion_clap/training/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)        0 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/__init__.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    84448 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/audioset_textmap.npy
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    32641 2023-04-19 20:16:17.000000 laion_clap-1.1.4/src/laion_clap/training/data.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     5078 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/distributed.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    22135 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/imagenet_zeroshot_data.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     3265 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/infer_demo.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      899 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/logger.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    25047 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/lp_main.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    10645 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/lp_train.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    22608 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/main.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    17401 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/params.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      659 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/scheduler.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    35672 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/train.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     3395 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/laion_clap/training/zero_shot.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     2597 2023-04-19 20:33:55.000000 laion_clap-1.1.4/src/laion_clap/unit_test.py
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.956179 laion_clap-1.1.4/src/laion_clap.egg-info/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    25816 2023-04-19 20:43:18.000000 laion_clap-1.1.4/src/laion_clap.egg-info/PKG-INFO
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     3095 2023-04-19 20:43:18.000000 laion_clap-1.1.4/src/laion_clap.egg-info/SOURCES.txt
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)        1 2023-04-19 20:43:18.000000 laion_clap-1.1.4/src/laion_clap.egg-info/dependency_links.txt
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)      160 2023-04-19 20:43:18.000000 laion_clap-1.1.4/src/laion_clap.egg-info/requires.txt
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)       17 2023-04-19 20:43:18.000000 laion_clap-1.1.4/src/laion_clap.egg-info/top_level.txt
+drwxrwxr-x   0 kechen    (1003) kechen    (1003)        0 2023-04-19 20:43:18.964179 laion_clap-1.1.4/src/tests/
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)        0 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/tests/__init__.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)    56326 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/tests/check_ckpt.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     3295 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/tests/check_tars.py
+-rw-rw-r--   0 kechen    (1003) kechen    (1003)     2174 2023-04-05 02:26:50.000000 laion_clap-1.1.4/src/tests/data_loader_test.py
```

### Comparing `laion_clap-1.1.3/LICENSE` & `laion_clap-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/PKG-INFO` & `laion_clap-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laion_clap
-Version: 1.1.3
+Version: 1.1.4
 Summary: Contrastive Language-Audio Pretraining Model from LAION
 Author: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Author-email: Ke Chen <knutchen@ucsd.edu>
 Maintainer: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Maintainer-email: Ke Chen <knutchen@ucsd.edu>
 License: Creative Commons Legal Code
         
@@ -136,37 +136,49 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLAP
-
-Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, similarly, the CLAP architecture is as follows.  
 <p align="center">
-  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/logo.PNG" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
 </p>
+<p align="center">
+  <a href="https://arxiv.org/abs/2211.06687"><img src="https://img.shields.io/badge/arXiv-2211.06687-brightgreen.svg?style=flat-square"/></a>
+  <a href="https://pypi.org/project/laion-clap"><img src="https://badge.fury.io/py/laion-clap.svg"/></a>
+  <a href="https://huggingface.co/docs/transformers/v4.27.2/en/model_doc/clap"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Transformers-blue"/></a>
+</p>
+ 
+### This repository provides representations of audios and texts via Contrastive Language-Audio Pretraining (CLAP)
 
+With CLAP, you can extract a latent representation of any given audio and text for your own model, or for different downstream tasks.
 
+All codes are comming officially with the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
+ - [Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
 
-The repository contains code for the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
- - [Large-scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
+**New Update: we release new CLAP pretrained checkpoints pretrained on music and speech data collecstions from [our dataset collection repo](https://github.com/LAION-AI/audio-dataset).**
 
 ## About this project
 
 This project is a project in [LAION](https://laion.ai/) that aims at learning better audio understanding and getting more audio data. 
 This is an opensource project. We adopt the codebase of [open_clip](https://github.com/mlfoundations/open_clip) for this project. 
-The major opensource contributers of this project are (in equal contribution): Yusong Wu, Tianyu Zhang, Ke Chen.
 
 many thanks to <a href="https://github.com/cfoster0/CLAP">@cfoster0</a> for allowing us to use his repo name.
 
+## Architecture
+Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, the CLAP architecture is as follows.  
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+</p>
+
 ## Quick Start 
-We provide the library for our CLAP model:
+We provide the PyPI library for our CLAP model:
 ```bash
-pip install laion_clap
+pip install laion-clap
 ```
 
 Then you can follow the below usage or refer to [unit_test.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/unit_test.py).
 
 For the documentation of the API, please refer to [hook.py](https://github.com/LAION-AI/CLAP/blob/main/src/laion_clap/hook.py).
 
 ```python
@@ -181,43 +193,43 @@
 
 
 def float32_to_int16(x):
     x = np.clip(x, a_min=-1., a_max=1.)
     return (x * 32767.).astype(np.int16)
 
 model = laion_clap.CLAP_Module(enable_fusion=False)
-model.load_ckpt()
+model.load_ckpt() # download the default pretrained checkpoint.
 
 # Directly get audio embeddings from audio files
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Directly get audio embeddings from audio files, but return torch tensor
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_data = torch.from_numpy(int16_to_float32(float32_to_int16(audio_data))).float() # quantize before send it in to the model
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get text embedings from texts:
@@ -230,14 +242,59 @@
 text_data = ["I love the contrastive learning", "I love the pretrain model"] 
 text_embed = model.get_text_embedding(text_data, use_tensor=True)
 print(text_embed)
 print(text_embed.shape)
 
 ```
 
+## Pretrained Models
+The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
+Please refer to the previous section for how to load and run the checkpoints.
+For the PyPI library, [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) and [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) are our default models (non-fusion and fusion)
+
+We further provide below pretrained models according to your usages:
+
+* For general audio less than 10-sec: [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) or [630k-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-best.pt)
+* For general audio with variable-length: [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) or [630k-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-fusion-best.pt)
+* For music: [music_audioset_epoch_15_esc_90.14.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_audioset_epoch_15_esc_90.14.pt)
+* For music and speech: [music_speech_epoch_15_esc_89.25.pt](https://huggingface.co/lukewys/laion_clap/blob/main/)
+* For speech, music and general audio: [music_speech_audioset_epoch_15_esc_89.98.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_speech_audioset_epoch_15_esc_89.98.pt)
+
+The checkpoints list here for each model setting is the one with the highest average mAP score in training.
+The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
+
+To use above pretrained models, you need to load the ckpt by yourself, as:
+
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
+We provide the CLAP's performance on audio classification tasks under the zero-shot setting or the supervised setting. More results can be found at our paper.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/clap-zeroshot.PNG" alt="Zero-shot Performance" width="100%"/>
+</p>
+
+
+
+
 ## Environment Installation
 If you want to check and reuse our model into your project instead of directly using the pip library, you need to install the same environment as we use, please run the following command:
 ```bash
 conda create env -n clap python=3.10
 conda activate clap
 git clone https://github.com/LAION-AI/CLAP.git
 cd CLAP
@@ -261,39 +318,14 @@
 To train on a single GPU machine, use `CUDA_VISIBLE_DEVICES=0 python -m ...` instead of `srun`.
 We use [Weights and Biases](https://wandb.ai/site) for experiment logging. You need to configure the weights and biases in your environment.
 To train on local dataset, please change the `--remotedata` in training scripts (see [experiment_scripts](./experiment_scripts) folder) with `--datasetpath <your dir to datasets>`.
 
 ## Core Code
 Please refer to [main.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/main.py), [train.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/train.py), [data.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/data.py),and [model.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/clap_module/model.py) to quicly get familiar with our model.
 
-## Pretrained Models
-The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
-Please refer to the previous section for how to load and run the checkpoints.
-
-The checkpoints list here for each model setting is the one with the highest average mAP score in training.
-The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
-
-Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
-
- - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
- - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
- - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
-
-The model uses a larger audio encoder. To load the model using the pip API:
-```python
-import laion_clap
-model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
-model.load_ckpt('checkpoint_path/checkpoint_name.pt')
-```
-
-Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
-We will release a more comprehensive version of the model with detailed experiments in the future.
-Please take your own risk when using this model.
-
-* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
 
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.3/README.md` & `laion_clap-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 # CLAP
-
-Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, similarly, the CLAP architecture is as follows.  
 <p align="center">
-  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/logo.PNG" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
 </p>
+<p align="center">
+  <a href="https://arxiv.org/abs/2211.06687"><img src="https://img.shields.io/badge/arXiv-2211.06687-brightgreen.svg?style=flat-square"/></a>
+  <a href="https://pypi.org/project/laion-clap"><img src="https://badge.fury.io/py/laion-clap.svg"/></a>
+  <a href="https://huggingface.co/docs/transformers/v4.27.2/en/model_doc/clap"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Transformers-blue"/></a>
+</p>
+ 
+### This repository provides representations of audios and texts via Contrastive Language-Audio Pretraining (CLAP)
 
+With CLAP, you can extract a latent representation of any given audio and text for your own model, or for different downstream tasks.
 
+All codes are comming officially with the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
+ - [Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
 
-The repository contains code for the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
- - [Large-scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
+**New Update: we release new CLAP pretrained checkpoints pretrained on music and speech data collecstions from [our dataset collection repo](https://github.com/LAION-AI/audio-dataset).**
 
 ## About this project
 
 This project is a project in [LAION](https://laion.ai/) that aims at learning better audio understanding and getting more audio data. 
 This is an opensource project. We adopt the codebase of [open_clip](https://github.com/mlfoundations/open_clip) for this project. 
-The major opensource contributers of this project are (in equal contribution): Yusong Wu, Tianyu Zhang, Ke Chen.
 
 many thanks to <a href="https://github.com/cfoster0/CLAP">@cfoster0</a> for allowing us to use his repo name.
 
+## Architecture
+Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, the CLAP architecture is as follows.  
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+</p>
+
 ## Quick Start 
-We provide the library for our CLAP model:
+We provide the PyPI library for our CLAP model:
 ```bash
-pip install laion_clap
+pip install laion-clap
 ```
 
 Then you can follow the below usage or refer to [unit_test.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/unit_test.py).
 
 For the documentation of the API, please refer to [hook.py](https://github.com/LAION-AI/CLAP/blob/main/src/laion_clap/hook.py).
 
 ```python
@@ -40,43 +52,43 @@
 
 
 def float32_to_int16(x):
     x = np.clip(x, a_min=-1., a_max=1.)
     return (x * 32767.).astype(np.int16)
 
 model = laion_clap.CLAP_Module(enable_fusion=False)
-model.load_ckpt()
+model.load_ckpt() # download the default pretrained checkpoint.
 
 # Directly get audio embeddings from audio files
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Directly get audio embeddings from audio files, but return torch tensor
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_data = torch.from_numpy(int16_to_float32(float32_to_int16(audio_data))).float() # quantize before send it in to the model
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get text embedings from texts:
@@ -89,14 +101,59 @@
 text_data = ["I love the contrastive learning", "I love the pretrain model"] 
 text_embed = model.get_text_embedding(text_data, use_tensor=True)
 print(text_embed)
 print(text_embed.shape)
 
 ```
 
+## Pretrained Models
+The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
+Please refer to the previous section for how to load and run the checkpoints.
+For the PyPI library, [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) and [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) are our default models (non-fusion and fusion)
+
+We further provide below pretrained models according to your usages:
+
+* For general audio less than 10-sec: [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) or [630k-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-best.pt)
+* For general audio with variable-length: [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) or [630k-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-fusion-best.pt)
+* For music: [music_audioset_epoch_15_esc_90.14.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_audioset_epoch_15_esc_90.14.pt)
+* For music and speech: [music_speech_epoch_15_esc_89.25.pt](https://huggingface.co/lukewys/laion_clap/blob/main/)
+* For speech, music and general audio: [music_speech_audioset_epoch_15_esc_89.98.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_speech_audioset_epoch_15_esc_89.98.pt)
+
+The checkpoints list here for each model setting is the one with the highest average mAP score in training.
+The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
+
+To use above pretrained models, you need to load the ckpt by yourself, as:
+
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
+We provide the CLAP's performance on audio classification tasks under the zero-shot setting or the supervised setting. More results can be found at our paper.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/clap-zeroshot.PNG" alt="Zero-shot Performance" width="100%"/>
+</p>
+
+
+
+
 ## Environment Installation
 If you want to check and reuse our model into your project instead of directly using the pip library, you need to install the same environment as we use, please run the following command:
 ```bash
 conda create env -n clap python=3.10
 conda activate clap
 git clone https://github.com/LAION-AI/CLAP.git
 cd CLAP
@@ -120,39 +177,14 @@
 To train on a single GPU machine, use `CUDA_VISIBLE_DEVICES=0 python -m ...` instead of `srun`.
 We use [Weights and Biases](https://wandb.ai/site) for experiment logging. You need to configure the weights and biases in your environment.
 To train on local dataset, please change the `--remotedata` in training scripts (see [experiment_scripts](./experiment_scripts) folder) with `--datasetpath <your dir to datasets>`.
 
 ## Core Code
 Please refer to [main.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/main.py), [train.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/train.py), [data.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/data.py),and [model.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/clap_module/model.py) to quicly get familiar with our model.
 
-## Pretrained Models
-The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
-Please refer to the previous section for how to load and run the checkpoints.
-
-The checkpoints list here for each model setting is the one with the highest average mAP score in training.
-The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
-
-Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
-
- - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
- - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
- - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
-
-The model uses a larger audio encoder. To load the model using the pip API:
-```python
-import laion_clap
-model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
-model.load_ckpt('checkpoint_path/checkpoint_name.pt')
-```
-
-Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
-We will release a more comprehensive version of the model with detailed experiments in the future.
-Please take your own risk when using this model.
-
-* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
 
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.3/pyproject.toml` & `laion_clap-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "laion_clap"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Ke Chen", email="knutchen@ucsd.edu" },
   { name="Yusong Wu" },
   { name="Tianyu Zhang" },
   { name="Yuchen Hui" }
 ]
 maintainers = [
```

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/__init__.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/__init__.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/bert.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/bert.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz` & `laion_clap-1.1.4/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/factory.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/factory.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/feature_fusion.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/htsat.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/htsat.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/linear_probe.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/linear_probe.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/loss.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/loss.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/model.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/openai.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/openai.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/pann_model.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/pann_model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/pretrained.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/pretrained.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/timm_model.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/timm_model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/tokenizer.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/tokenizer.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/transform.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/transform.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/clap_module/utils.py` & `laion_clap-1.1.4/src/laion_clap/clap_module/utils.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/evaluate/eval_dcase.py` & `laion_clap-1.1.4/src/laion_clap/evaluate/eval_dcase.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/evaluate/eval_linear_probe.py` & `laion_clap-1.1.4/src/laion_clap/evaluate/eval_linear_probe.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval.py` & `laion_clap-1.1.4/src/laion_clap/evaluate/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval_main.py` & `laion_clap-1.1.4/src/laion_clap/evaluate/eval_retrieval_main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/evaluate/eval_zeroshot_classification.py` & `laion_clap-1.1.4/src/laion_clap/evaluate/eval_zeroshot_classification.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/hook.py` & `laion_clap-1.1.4/src/laion_clap/hook.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/audioset_textmap.npy` & `laion_clap-1.1.4/src/laion_clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/data.py` & `laion_clap-1.1.4/src/laion_clap/training/data.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/distributed.py` & `laion_clap-1.1.4/src/laion_clap/training/distributed.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/imagenet_zeroshot_data.py` & `laion_clap-1.1.4/src/laion_clap/training/imagenet_zeroshot_data.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/infer_demo.py` & `laion_clap-1.1.4/src/laion_clap/training/infer_demo.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/logger.py` & `laion_clap-1.1.4/src/laion_clap/training/logger.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/lp_main.py` & `laion_clap-1.1.4/src/laion_clap/training/lp_main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/lp_train.py` & `laion_clap-1.1.4/src/laion_clap/training/lp_train.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/main.py` & `laion_clap-1.1.4/src/laion_clap/training/main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/params.py` & `laion_clap-1.1.4/src/laion_clap/training/params.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/scheduler.py` & `laion_clap-1.1.4/src/laion_clap/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/train.py` & `laion_clap-1.1.4/src/laion_clap/training/train.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/training/zero_shot.py` & `laion_clap-1.1.4/src/laion_clap/training/zero_shot.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/laion_clap/unit_test.py` & `laion_clap-1.1.4/src/laion_clap/unit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return (x / 32767.0).astype(np.float32)
 
 
 def float32_to_int16(x):
     x = np.clip(x, a_min=-1., a_max=1.)
     return (x * 32767.).astype(np.int16)
 
-model = laion_clap.CLAP_Module(enable_fusion=True)
+model = laion_clap.CLAP_Module(enable_fusion=False)
 model.load_ckpt()
 
 # Directly get audio embeddings from audio files
 audio_file = [
     '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
     '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
 ]
```

### Comparing `laion_clap-1.1.3/src/laion_clap.egg-info/PKG-INFO` & `laion_clap-1.1.4/src/laion_clap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laion-clap
-Version: 1.1.3
+Version: 1.1.4
 Summary: Contrastive Language-Audio Pretraining Model from LAION
 Author: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Author-email: Ke Chen <knutchen@ucsd.edu>
 Maintainer: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Maintainer-email: Ke Chen <knutchen@ucsd.edu>
 License: Creative Commons Legal Code
         
@@ -136,37 +136,49 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLAP
-
-Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, similarly, the CLAP architecture is as follows.  
 <p align="center">
-  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/logo.PNG" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
 </p>
+<p align="center">
+  <a href="https://arxiv.org/abs/2211.06687"><img src="https://img.shields.io/badge/arXiv-2211.06687-brightgreen.svg?style=flat-square"/></a>
+  <a href="https://pypi.org/project/laion-clap"><img src="https://badge.fury.io/py/laion-clap.svg"/></a>
+  <a href="https://huggingface.co/docs/transformers/v4.27.2/en/model_doc/clap"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Transformers-blue"/></a>
+</p>
+ 
+### This repository provides representations of audios and texts via Contrastive Language-Audio Pretraining (CLAP)
 
+With CLAP, you can extract a latent representation of any given audio and text for your own model, or for different downstream tasks.
 
+All codes are comming officially with the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
+ - [Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
 
-The repository contains code for the following paper, accepted by IEEE International Conference on Acoustics, Speech and Signal Processing, ICASSP 2023:
- - [Large-scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation](https://arxiv.org/abs/2211.06687)
+**New Update: we release new CLAP pretrained checkpoints pretrained on music and speech data collecstions from [our dataset collection repo](https://github.com/LAION-AI/audio-dataset).**
 
 ## About this project
 
 This project is a project in [LAION](https://laion.ai/) that aims at learning better audio understanding and getting more audio data. 
 This is an opensource project. We adopt the codebase of [open_clip](https://github.com/mlfoundations/open_clip) for this project. 
-The major opensource contributers of this project are (in equal contribution): Yusong Wu, Tianyu Zhang, Ke Chen.
 
 many thanks to <a href="https://github.com/cfoster0/CLAP">@cfoster0</a> for allowing us to use his repo name.
 
+## Architecture
+Contrastive Language-Audio Pretraining, known as CLAP. Referring to the CLIP (Contrastive Language-Image Pretraining) architecture, the CLAP architecture is as follows.  
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/audioclip-arch.png" alt="The Contrastive Language-Audio Pretraining Model Architecture" width="60%"/>
+</p>
+
 ## Quick Start 
-We provide the library for our CLAP model:
+We provide the PyPI library for our CLAP model:
 ```bash
-pip install laion_clap
+pip install laion-clap
 ```
 
 Then you can follow the below usage or refer to [unit_test.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/unit_test.py).
 
 For the documentation of the API, please refer to [hook.py](https://github.com/LAION-AI/CLAP/blob/main/src/laion_clap/hook.py).
 
 ```python
@@ -181,43 +193,43 @@
 
 
 def float32_to_int16(x):
     x = np.clip(x, a_min=-1., a_max=1.)
     return (x * 32767.).astype(np.int16)
 
 model = laion_clap.CLAP_Module(enable_fusion=False)
-model.load_ckpt()
+model.load_ckpt() # download the default pretrained checkpoint.
 
 # Directly get audio embeddings from audio files
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=False)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Directly get audio embeddings from audio files, but return torch tensor
 audio_file = [
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav',
-    '/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_long.wav'
+    '/home/data/test_clap_short.wav',
+    '/home/data/test_clap_long.wav'
 ]
 audio_embed = model.get_audio_embedding_from_filelist(x = audio_file, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get audio embeddings from audio data
-audio_data, _ = librosa.load('/home/la/kechen/Research/KE_CLAP/ckpt/test_clap_short.wav', sr=48000) # sample rate should be 48000
+audio_data, _ = librosa.load('/home/data/test_clap_short.wav', sr=48000) # sample rate should be 48000
 audio_data = audio_data.reshape(1, -1) # Make it (1,T) or (N,T)
 audio_data = torch.from_numpy(int16_to_float32(float32_to_int16(audio_data))).float() # quantize before send it in to the model
 audio_embed = model.get_audio_embedding_from_data(x = audio_data, use_tensor=True)
 print(audio_embed[:,-20:])
 print(audio_embed.shape)
 
 # Get text embedings from texts:
@@ -230,14 +242,59 @@
 text_data = ["I love the contrastive learning", "I love the pretrain model"] 
 text_embed = model.get_text_embedding(text_data, use_tensor=True)
 print(text_embed)
 print(text_embed.shape)
 
 ```
 
+## Pretrained Models
+The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
+Please refer to the previous section for how to load and run the checkpoints.
+For the PyPI library, [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) and [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) are our default models (non-fusion and fusion)
+
+We further provide below pretrained models according to your usages:
+
+* For general audio less than 10-sec: [630k-audioset-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-best.pt) or [630k-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-best.pt)
+* For general audio with variable-length: [630k-audioset-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-audioset-fusion-best.pt) or [630k-fusion-best.pt](https://huggingface.co/lukewys/laion_clap/blob/main/630k-fusion-best.pt)
+* For music: [music_audioset_epoch_15_esc_90.14.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_audioset_epoch_15_esc_90.14.pt)
+* For music and speech: [music_speech_epoch_15_esc_89.25.pt](https://huggingface.co/lukewys/laion_clap/blob/main/)
+* For speech, music and general audio: [music_speech_audioset_epoch_15_esc_89.98.pt](https://huggingface.co/lukewys/laion_clap/blob/main/music_speech_audioset_epoch_15_esc_89.98.pt)
+
+The checkpoints list here for each model setting is the one with the highest average mAP score in training.
+The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
+
+To use above pretrained models, you need to load the ckpt by yourself, as:
+
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
+We provide the CLAP's performance on audio classification tasks under the zero-shot setting or the supervised setting. More results can be found at our paper.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/LAION-AI/CLAP/main/assets/clap-zeroshot.PNG" alt="Zero-shot Performance" width="100%"/>
+</p>
+
+
+
+
 ## Environment Installation
 If you want to check and reuse our model into your project instead of directly using the pip library, you need to install the same environment as we use, please run the following command:
 ```bash
 conda create env -n clap python=3.10
 conda activate clap
 git clone https://github.com/LAION-AI/CLAP.git
 cd CLAP
@@ -261,39 +318,14 @@
 To train on a single GPU machine, use `CUDA_VISIBLE_DEVICES=0 python -m ...` instead of `srun`.
 We use [Weights and Biases](https://wandb.ai/site) for experiment logging. You need to configure the weights and biases in your environment.
 To train on local dataset, please change the `--remotedata` in training scripts (see [experiment_scripts](./experiment_scripts) folder) with `--datasetpath <your dir to datasets>`.
 
 ## Core Code
 Please refer to [main.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/main.py), [train.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/train.py), [data.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/training/data.py),and [model.py](https://github.com/LAION-AI/CLAP/blob/laion_clap_pip/src/laion_clap/clap_module/model.py) to quicly get familiar with our model.
 
-## Pretrained Models
-The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
-Please refer to the previous section for how to load and run the checkpoints.
-
-The checkpoints list here for each model setting is the one with the highest average mAP score in training.
-The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
-
-Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
-
- - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
- - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
- - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
-
-The model uses a larger audio encoder. To load the model using the pip API:
-```python
-import laion_clap
-model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
-model.load_ckpt('checkpoint_path/checkpoint_name.pt')
-```
-
-Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
-We will release a more comprehensive version of the model with detailed experiments in the future.
-Please take your own risk when using this model.
-
-* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
 
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.3/src/laion_clap.egg-info/SOURCES.txt` & `laion_clap-1.1.4/src/laion_clap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/tests/check_ckpt.py` & `laion_clap-1.1.4/src/tests/check_ckpt.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/tests/check_tars.py` & `laion_clap-1.1.4/src/tests/check_tars.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.3/src/tests/data_loader_test.py` & `laion_clap-1.1.4/src/tests/data_loader_test.py`

 * *Files identical despite different names*

