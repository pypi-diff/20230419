# Comparing `tmp/xturing-0.1.0.tar.gz` & `tmp/xturing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.0.tar", last modified: Tue Apr 18 12:33:56 2023, max compression
+gzip compressed data, was "xturing-0.1.1.tar", last modified: Wed Apr 19 13:02:09 2023, max compression
```

## Comparing `xturing-0.1.0.tar` & `xturing-0.1.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.512836 xturing-0.1.0/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    11357 2023-03-20 07:53:44.000000 xturing-0.1.0/LICENSE
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       34 2023-03-29 09:34:15.000000 xturing-0.1.0/MANIFEST.in
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-18 12:33:56.512284 xturing-0.1.0/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7162 2023-04-18 12:33:45.000000 xturing-0.1.0/README.md
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2203 2023-04-18 12:33:45.000000 xturing-0.1.0/pyproject.toml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       38 2023-04-18 12:33:56.512979 xturing-0.1.0/setup.cfg
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.456961 xturing-0.1.0/src/
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.463750 xturing-0.1.0/src/xturing/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       22 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/__about__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      438 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/__init__.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.469370 xturing-0.1.0/src/xturing/cli/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      561 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2042 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/api.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      989 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/chat.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      131 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/cli/ui.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.472261 xturing-0.1.0/src/xturing/config/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      569 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/config/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      972 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/config/config_data_classes.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2701 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/config/finetuning_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2739 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/config/generation_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1862 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/config/read_config.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.476892 xturing-0.1.0/src/xturing/datasets/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      436 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      199 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     8179 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/datasets/instruction_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      222 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/text2image_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/datasets/text_dataset.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.483206 xturing-0.1.0/src/xturing/engines/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3182 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      272 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/engines/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1871 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/bloom_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6746 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1923 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/cerebras_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      804 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/distilgpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1755 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/galactica_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1446 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/gpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2885 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/gptj_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.484177 xturing-0.1.0/src/xturing/engines/gptj_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/engines/gptj_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7690 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/engines/gptj_utils/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6256 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/llama_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.485311 xturing-0.1.0/src/xturing/engines/llama_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       65 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/engines/llama_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    44486 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/engines/llama_utils/llama.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.487872 xturing-0.1.0/src/xturing/engines/lora_engine/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       73 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/lora_engine/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    42467 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/lora_engine/lora.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3556 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/lora_engine/save_and_load.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/lora_engine/test.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/opt_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.489720 xturing-0.1.0/src/xturing/engines/quant_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       59 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6803 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/custom_autotune.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    23551 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/quant.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.492493 xturing-0.1.0/src/xturing/model_apis/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      864 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1827 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/ai21.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      573 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1847 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/cohere.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4600 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/openai.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.498464 xturing-0.1.0/src/xturing/models/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2566 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/models/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2067 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/models/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1084 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/bloom.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7132 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1135 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/cerebras.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      579 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/distilgpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1152 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/galactica.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1033 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/gpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1067 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2100 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/models/llama.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1050 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/opt.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      542 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/models/stable_diffusion.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.500499 xturing-0.1.0/src/xturing/preprocessors/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      137 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/preprocessors/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      484 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/preprocessors/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4582 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/preprocessors/instruction_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2252 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/preprocessors/text_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      642 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/registry.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.503058 xturing-0.1.0/src/xturing/self_instruct/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     9891 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/bootstrap_instructions.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     5490 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/generate_instances.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3737 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/identify_if_classification.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    14280 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2198 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.504210 xturing-0.1.0/src/xturing/self_instruct/templates/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3580 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/templates/clf_task_template.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    12674 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.505864 xturing-0.1.0/src/xturing/trainers/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       78 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/trainers/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      233 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/trainers/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     5983 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/trainers/lightning_trainer.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.506795 xturing-0.1.0/src/xturing/ui/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/ui/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    13646 2023-04-03 17:19:47.000000 xturing-0.1.0/src/xturing/ui/playground.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.511469 xturing-0.1.0/src/xturing/utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      215 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/external_loggers.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3075 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/utils/hub.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      304 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/utils/interactive.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2147 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/logging.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      621 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/utils/loss_fns.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1366 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/notebooks.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6886 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/utils/text_splitter.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3803 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/utils/utils.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.467361 xturing-0.1.0/src/xturing.egg-info/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3201 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/SOURCES.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        1 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/dependency_links.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       48 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/entry_points.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      237 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/requires.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        8 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/top_level.txt
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.248906 xturing-0.1.1/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    11357 2023-03-20 07:53:44.000000 xturing-0.1.1/LICENSE
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       34 2023-03-29 09:34:15.000000 xturing-0.1.1/MANIFEST.in
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-19 13:02:09.248351 xturing-0.1.1/PKG-INFO
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7162 2023-04-18 12:33:45.000000 xturing-0.1.1/README.md
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2203 2023-04-19 13:01:46.000000 xturing-0.1.1/pyproject.toml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       38 2023-04-19 13:02:09.249064 xturing-0.1.1/setup.cfg
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.194814 xturing-0.1.1/src/
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.202283 xturing-0.1.1/src/xturing/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       22 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/__about__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      438 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/__init__.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.207892 xturing-0.1.1/src/xturing/cli/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      561 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2042 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/api.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      989 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/chat.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      131 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/cli/ui.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.211762 xturing-0.1.1/src/xturing/config/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      569 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/config/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      972 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/config/config_data_classes.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2701 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/config/finetuning_config.yaml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2739 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/config/generation_config.yaml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1862 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/config/read_config.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.214383 xturing-0.1.1/src/xturing/datasets/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      436 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      199 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     8179 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/datasets/instruction_dataset.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      222 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/text2image_dataset.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/datasets/text_dataset.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.218672 xturing-0.1.1/src/xturing/engines/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3182 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      272 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/engines/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1871 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/bloom_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6746 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/causal.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1923 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/cerebras_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      804 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/distilgpt2_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1755 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/galactica_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1446 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/gpt2_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2885 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/gptj_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.219527 xturing-0.1.1/src/xturing/engines/gptj_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/engines/gptj_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7690 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/engines/gptj_utils/gptj.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6256 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/llama_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.220496 xturing-0.1.1/src/xturing/engines/llama_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       65 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/engines/llama_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    44486 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/engines/llama_utils/llama.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.222578 xturing-0.1.1/src/xturing/engines/lora_engine/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       73 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/lora_engine/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    42467 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/lora_engine/lora.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3556 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/lora_engine/save_and_load.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/lora_engine/test.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/opt_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.224038 xturing-0.1.1/src/xturing/engines/quant_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       59 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/quant_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6803 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    28505 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/engines/quant_utils/quant.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.226862 xturing-0.1.1/src/xturing/model_apis/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      864 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1827 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/ai21.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      573 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1847 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/cohere.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     4600 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/openai.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.232201 xturing-0.1.1/src/xturing/models/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2566 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/models/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2067 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/models/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1084 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/bloom.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7132 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/causal.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1135 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/cerebras.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      579 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/distilgpt2.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1152 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/galactica.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1033 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/gpt2.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1067 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/gptj.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2100 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/models/llama.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1050 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/opt.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      542 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/models/stable_diffusion.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.234366 xturing-0.1.1/src/xturing/preprocessors/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      137 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/preprocessors/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      484 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/preprocessors/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     4582 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/preprocessors/instruction_collator.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2252 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/preprocessors/text_collator.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      642 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/registry.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.237815 xturing-0.1.1/src/xturing/self_instruct/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     9891 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     5490 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/generate_instances.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3737 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/identify_if_classification.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    14280 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2198 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.239038 xturing-0.1.1/src/xturing/self_instruct/templates/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3580 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    12674 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.241073 xturing-0.1.1/src/xturing/trainers/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       78 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/trainers/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      233 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/trainers/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6049 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/trainers/lightning_trainer.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.242192 xturing-0.1.1/src/xturing/ui/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/ui/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    13646 2023-04-03 17:19:47.000000 xturing-0.1.1/src/xturing/ui/playground.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.247081 xturing-0.1.1/src/xturing/utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      215 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/external_loggers.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3075 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/utils/hub.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      304 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/utils/interactive.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2147 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/logging.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      621 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/utils/loss_fns.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1366 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/notebooks.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6886 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/utils/text_splitter.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3803 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/utils/utils.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.205715 xturing-0.1.1/src/xturing.egg-info/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/PKG-INFO
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3201 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/SOURCES.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        1 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/dependency_links.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       48 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/entry_points.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      237 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/requires.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        8 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.0/LICENSE` & `xturing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/PKG-INFO` & `xturing-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.0/README.md` & `xturing-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/pyproject.toml` & `xturing-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.0"
+version = "0.1.1"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
```

### Comparing `xturing-0.1.0/src/xturing/cli/__init__.py` & `xturing-0.1.1/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/cli/api.py` & `xturing-0.1.1/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/cli/chat.py` & `xturing-0.1.1/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/config/__init__.py` & `xturing-0.1.1/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/config/config_data_classes.py` & `xturing-0.1.1/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.1/src/xturing/config/finetuning_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/config/generation_config.yaml` & `xturing-0.1.1/src/xturing/config/generation_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/config/read_config.py` & `xturing-0.1.1/src/xturing/config/read_config.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.1/src/xturing/datasets/instruction_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/datasets/text_dataset.py` & `xturing-0.1.1/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/__init__.py` & `xturing-0.1.1/src/xturing/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/bloom_engine.py` & `xturing-0.1.1/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/causal.py` & `xturing-0.1.1/src/xturing/engines/causal.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.1/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.1/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/galactica_engine.py` & `xturing-0.1.1/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.1/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/gptj_engine.py` & `xturing-0.1.1/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.1/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/llama_engine.py` & `xturing-0.1.1/src/xturing/engines/llama_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.1/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.1/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.1/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/opt_engine.py` & `xturing-0.1.1/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.1/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.1/src/xturing/engines/quant_utils/quant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,49 @@
+import math
+
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.cuda.amp import custom_bwd, custom_fwd
-import math
+
 
 def quantize(x, scale, zero, maxq):
     if maxq < 0:
         return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
     q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
     return scale * (q - zero)
 
-class Quantizer(nn.Module):
 
+class Quantizer(nn.Module):
     def __init__(self, shape=1):
         super(Quantizer, self).__init__()
-        self.register_buffer('maxq', torch.tensor(0))
-        self.register_buffer('scale', torch.zeros(shape))
-        self.register_buffer('zero', torch.zeros(shape))
+        self.register_buffer("maxq", torch.tensor(0))
+        self.register_buffer("scale", torch.zeros(shape))
+        self.register_buffer("zero", torch.zeros(shape))
 
     def configure(
         self,
-        bits, perchannel=False, sym=True, 
-        mse=False, norm=2.4, grid=100, maxshrink=.8,
-        trits=False
-        ):
-        
-        self.maxq = torch.tensor(2 ** bits - 1)
+        bits,
+        perchannel=False,
+        sym=True,
+        mse=False,
+        norm=2.4,
+        grid=100,
+        maxshrink=0.8,
+        trits=False,
+    ):
+        self.maxq = torch.tensor(2**bits - 1)
         self.perchannel = perchannel
         self.sym = sym
         self.mse = mse
         self.norm = norm
         self.grid = grid
-        self.maxshrink = maxshrink 
+        self.maxshrink = maxshrink
         if trits:
-            self.maxq = torch.tensor(-1) 
+            self.maxq = torch.tensor(-1)
 
     def find_params(self, x, weight=False):
         dev = x.device
         self.maxq = self.maxq.to(dev)
 
         shape = x.shape
         if self.perchannel:
@@ -74,17 +80,17 @@
             self.scale = (xmax - xmin) / self.maxq
             if self.sym:
                 self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
             else:
                 self.zero = torch.round(-xmin / self.scale)
 
         if self.mse:
-            best = torch.full([x.shape[0]], float('inf'), device=dev)
+            best = torch.full([x.shape[0]], float("inf"), device=dev)
             for i in range(int(self.maxshrink * self.grid)):
-                p = 1 - i / self.grid 
+                p = 1 - i / self.grid
                 xmin1 = p * xmin
                 xmax1 = p * xmax
                 scale1 = (xmax1 - xmin1) / self.maxq
                 zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
                 q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
                 q -= x
                 q.abs_()
@@ -109,75 +115,209 @@
             self.zero = self.zero.reshape(shape)
             return
         if len(shape) == 4:
             self.scale = self.scale.reshape((1, -1, 1, 1))
             self.zero = self.zero.reshape((1, -1, 1, 1))
         if len(shape) == 3:
             self.scale = self.scale.reshape((1, 1, -1))
-            self.zero = self.zero.reshape((1, 1, -1)) 
+            self.zero = self.zero.reshape((1, 1, -1))
         if len(shape) == 2:
             self.scale = self.scale.unsqueeze(0)
             self.zero = self.zero.unsqueeze(0)
 
     def quantize(self, x):
         if self.ready():
             return quantize(x, self.scale, self.zero, self.maxq)
         return x
 
     def enabled(self):
         return self.maxq > 0
 
     def ready(self):
         return torch.all(self.scale != 0)
-    
+
+
 try:
     import triton
     import triton.language as tl
+
     from . import custom_autotune
 
     # code based https://github.com/fpgaminer/GPTQ-triton
     @custom_autotune.autotune(
         configs=[
-            triton.Config({'BLOCK_SIZE_M': 256, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 256, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 256,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 256,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_N": 128,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 128,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_N": 32,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
             # These provided a benefit on a 3090
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "BLOCK_SIZE_K": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "BLOCK_SIZE_K": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_N": 64,
+                    "BLOCK_SIZE_K": 128,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
         ],
-        key=['M', 'N'],
+        key=["M", "N"],
         nearest_power_of_two=True,
     )
-    
     @triton.jit
-    def matmul_248_kernel(a_ptr, b_ptr, c_ptr,
-                          scales_ptr, zeros_ptr, g_ptr,
-                          M, N, K, bits, maxq,
-                          stride_am, stride_ak,
-                          stride_bk, stride_bn,
-                          stride_cm, stride_cn,
-                          stride_scales, stride_zeros,
-                          BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-                          GROUP_SIZE_M: tl.constexpr):
+    def matmul_248_kernel(
+        a_ptr,
+        b_ptr,
+        c_ptr,
+        scales_ptr,
+        zeros_ptr,
+        g_ptr,
+        M,
+        N,
+        K,
+        bits,
+        maxq,
+        stride_am,
+        stride_ak,
+        stride_bk,
+        stride_bn,
+        stride_cm,
+        stride_cn,
+        stride_scales,
+        stride_zeros,
+        BLOCK_SIZE_M: tl.constexpr,
+        BLOCK_SIZE_N: tl.constexpr,
+        BLOCK_SIZE_K: tl.constexpr,
+        GROUP_SIZE_M: tl.constexpr,
+    ):
         """
         Compute the matrix multiplication C = A x B.
         A is of shape (M, K) float16
         B is of shape (K//8, N) int32
         C is of shape (M, N) float16
         scales is of shape (G, N) float16
         zeros is of shape (G, N) float16
-        g_ptr is of shape (K) int32 
+        g_ptr is of shape (K) int32
         """
         infearure_per_bits = 32 // bits
 
         pid = tl.program_id(axis=0)
         num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
         num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
         num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
@@ -187,94 +327,235 @@
         group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
         pid_m = first_pid_m + (pid % group_size_m)
         pid_n = (pid % num_pid_in_group) // group_size_m
 
         offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
         offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
         offs_k = tl.arange(0, BLOCK_SIZE_K)
-        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)   # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-        a_mask = (offs_am[:, None] < M)
+        a_ptrs = a_ptr + (
+            offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak
+        )  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+        a_mask = offs_am[:, None] < M
         # b_ptrs is set up such that it repeats elements along the K axis 8 times
-        b_ptrs = b_ptr + ((offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn)   # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+        b_ptrs = b_ptr + (
+            (offs_k[:, None] // infearure_per_bits) * stride_bk
+            + offs_bn[None, :] * stride_bn
+        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
         g_ptrs = g_ptr + offs_k
         # shifter is used to extract the N bits of each element in the 32-bit word from B
         scales_ptrs = scales_ptr + offs_bn[None, :]
-        zeros_ptrs = zeros_ptr + (offs_bn[None, :]// infearure_per_bits) 
-        
+        zeros_ptrs = zeros_ptr + (offs_bn[None, :] // infearure_per_bits)
+
         shifter = (offs_k % infearure_per_bits) * bits
         zeros_shifter = (offs_bn % infearure_per_bits) * bits
         accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
-                
+
         for k in range(0, num_pid_k):
             g_idx = tl.load(g_ptrs)
 
             # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-            scales = tl.load(scales_ptrs + g_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            zeros = tl.load(zeros_ptrs + g_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            
+            scales = tl.load(
+                scales_ptrs + g_idx[:, None] * stride_scales
+            )  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            zeros = tl.load(
+                zeros_ptrs + g_idx[:, None] * stride_zeros
+            )  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+
             zeros = (zeros >> zeros_shifter[None, :]) & maxq
-            zeros = (zeros + 1)
-            
-            a = tl.load(a_ptrs, mask=a_mask, other=0.)   # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-            b = tl.load(b_ptrs)   # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+            zeros = zeros + 1
+
+            a = tl.load(a_ptrs, mask=a_mask, other=0.0)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
 
             # Now we need to unpack b (which is N-bit values) into 32-bit values
             b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
             b = (b - zeros) * scales  # Scale and shift
 
             accumulator += tl.dot(a, b)
             a_ptrs += BLOCK_SIZE_K
             b_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
             g_ptrs += BLOCK_SIZE_K
 
         c = accumulator.to(tl.float16)
         c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
         c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
         tl.store(c_ptrs, accumulator, mask=c_mask)
-        
+
     # code based https://github.com/fpgaminer/GPTQ-triton
     @custom_autotune.autotune(
         configs=[
-            triton.Config({'BLOCK_SIZE_M': 256, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 256, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_K': 128, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 128, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_K': 32, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 256,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 256,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_K": 128,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 128,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 128,
+                    "BLOCK_SIZE_K": 32,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
             # These provided a benefit on a 3090
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 32, 'BLOCK_SIZE_N': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_K': 32, 'BLOCK_SIZE_N': 64, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
-            triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_K': 64, 'BLOCK_SIZE_N': 128, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "BLOCK_SIZE_N": 32,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 64,
+                    "BLOCK_SIZE_K": 32,
+                    "BLOCK_SIZE_N": 64,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
+            triton.Config(
+                {
+                    "BLOCK_SIZE_M": 32,
+                    "BLOCK_SIZE_K": 64,
+                    "BLOCK_SIZE_N": 128,
+                    "GROUP_SIZE_M": 8,
+                },
+                num_stages=4,
+                num_warps=4,
+            ),
         ],
-        key=['M', 'K'],
+        key=["M", "K"],
         nearest_power_of_two=True,
     )
-    
     @triton.jit
-    def trans_matmul_248_kernel(a_ptr, b_ptr, c_ptr,
-                                scales_ptr, zeros_ptr, g_ptr,
-                                M, N, K, bits, maxq,
-                                stride_am, stride_ak,
-                                stride_bk, stride_bn,
-                                stride_cm, stride_cn,
-                                stride_scales, stride_zeros,
-                                BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-                                GROUP_SIZE_M: tl.constexpr):
+    def trans_matmul_248_kernel(
+        a_ptr,
+        b_ptr,
+        c_ptr,
+        scales_ptr,
+        zeros_ptr,
+        g_ptr,
+        M,
+        N,
+        K,
+        bits,
+        maxq,
+        stride_am,
+        stride_ak,
+        stride_bk,
+        stride_bn,
+        stride_cm,
+        stride_cn,
+        stride_scales,
+        stride_zeros,
+        BLOCK_SIZE_M: tl.constexpr,
+        BLOCK_SIZE_N: tl.constexpr,
+        BLOCK_SIZE_K: tl.constexpr,
+        GROUP_SIZE_M: tl.constexpr,
+    ):
         """
         Compute the matrix multiplication C = A x B.
         A is of shape (M, N) float16
         B is of shape (K//8, N) int32
         C is of shape (M, K) float16
         scales is of shape (G, N) float16
         zeros is of shape (G, N) float16
-        g_ptr is of shape (K) int32 
+        g_ptr is of shape (K) int32
         """
         infearure_per_bits = 32 // bits
 
         pid = tl.program_id(axis=0)
         num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
         num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
         num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
@@ -284,213 +565,327 @@
         group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
         pid_m = first_pid_m + (pid % group_size_m)
         pid_k = (pid % num_pid_in_group) // group_size_m
 
         offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
         offs_bk = pid_k * BLOCK_SIZE_K + tl.arange(0, BLOCK_SIZE_K)
         offs_n = tl.arange(0, BLOCK_SIZE_N)
-        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak)   # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-        a_mask = (offs_am[:, None] < M)
+        a_ptrs = a_ptr + (
+            offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak
+        )  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+        a_mask = offs_am[:, None] < M
         # b_ptrs is set up such that it repeats elements along the K axis 8 times
-        b_ptrs = b_ptr + ((offs_bk[:, None] // infearure_per_bits) * stride_bk + offs_n[None, :] * stride_bn)   # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+        b_ptrs = b_ptr + (
+            (offs_bk[:, None] // infearure_per_bits) * stride_bk
+            + offs_n[None, :] * stride_bn
+        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
         g_ptrs = g_ptr + offs_bk
         g_idx = tl.load(g_ptrs)
-        
+
         # shifter is used to extract the N bits of each element in the 32-bit word from B
-        scales_ptrs = scales_ptr + offs_n[None, :]  + g_idx[:, None] * stride_scales
-        zeros_ptrs = zeros_ptr + (offs_n[None, :]// infearure_per_bits) + g_idx[:, None] * stride_zeros
-        
+        scales_ptrs = scales_ptr + offs_n[None, :] + g_idx[:, None] * stride_scales
+        zeros_ptrs = (
+            zeros_ptr
+            + (offs_n[None, :] // infearure_per_bits)
+            + g_idx[:, None] * stride_zeros
+        )
+
         shifter = (offs_bk % infearure_per_bits) * bits
         zeros_shifter = (offs_n % infearure_per_bits) * bits
         accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_K), dtype=tl.float32)
-        
+
         for k in range(0, num_pid_n):
             # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
             scales = tl.load(scales_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
             zeros = tl.load(zeros_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            
+
             zeros = (zeros >> zeros_shifter[None, :]) & maxq
-            zeros = (zeros + 1)
-            
-            a = tl.load(a_ptrs, mask=a_mask, other=0.)   # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-            b = tl.load(b_ptrs)   # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+            zeros = zeros + 1
+
+            a = tl.load(a_ptrs, mask=a_mask, other=0.0)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
 
             # Now we need to unpack b (which is N-bit values) into 32-bit values
             b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
             b = (b - zeros) * scales  # Scale and shift
             b = tl.trans(b)
 
             accumulator += tl.dot(a, b)
             a_ptrs += BLOCK_SIZE_N
             b_ptrs += BLOCK_SIZE_N
             scales_ptrs += BLOCK_SIZE_N
-            zeros_ptrs += (BLOCK_SIZE_N // infearure_per_bits)
-            
+            zeros_ptrs += BLOCK_SIZE_N // infearure_per_bits
+
         c = accumulator.to(tl.float16)
         c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bk[None, :]
         c_mask = (offs_am[:, None] < M) & (offs_bk[None, :] < K)
         tl.store(c_ptrs, accumulator, mask=c_mask)
+
 except:
-    print('trioton not installed.')
+    print("triton not installed.")
+
 
 def matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
-    output = torch.empty((input.shape[0], qweight.shape[1]), device='cuda', dtype=torch.float16)
-    grid = lambda META: (triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),)
-    matmul_248_kernel[grid](input, qweight, output,
-                            scales, qzeros, g_idx,
-                            input.shape[0], qweight.shape[1], input.shape[1], bits, maxq,
-                            input.stride(0), input.stride(1),
-                            qweight.stride(0), qweight.stride(1),
-                            output.stride(0), output.stride(1),
-                            scales.stride(0), qzeros.stride(0))
+    output = torch.empty(
+        (input.shape[0], qweight.shape[1]), device="cuda", dtype=torch.float16
+    )
+    grid = lambda META: (
+        triton.cdiv(input.shape[0], META["BLOCK_SIZE_M"])
+        * triton.cdiv(qweight.shape[1], META["BLOCK_SIZE_N"]),
+    )
+    matmul_248_kernel[grid](
+        input,
+        qweight,
+        output,
+        scales,
+        qzeros,
+        g_idx,
+        input.shape[0],
+        qweight.shape[1],
+        input.shape[1],
+        bits,
+        maxq,
+        input.stride(0),
+        input.stride(1),
+        qweight.stride(0),
+        qweight.stride(1),
+        output.stride(0),
+        output.stride(1),
+        scales.stride(0),
+        qzeros.stride(0),
+    )
     return output
 
+
 def transpose_matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
     output_dim = (qweight.shape[0] * 32) // bits
-    output = torch.empty((input.shape[0], output_dim), device='cuda', dtype=torch.float16)
-    grid = lambda META: (triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
-    trans_matmul_248_kernel[grid](input, qweight, output,
-                                      scales, qzeros, g_idx,
-                                      input.shape[0], qweight.shape[1], output_dim, bits, maxq,
-                                      input.stride(0), input.stride(1),
-                                      qweight.stride(0), qweight.stride(1),
-                                      output.stride(0), output.stride(1),
-                                      scales.stride(0), qzeros.stride(0))
+    output = torch.empty(
+        (input.shape[0], output_dim), device="cuda", dtype=torch.float16
+    )
+    grid = lambda META: (
+        triton.cdiv(input.shape[0], META["BLOCK_SIZE_M"])
+        * triton.cdiv(output_dim, META["BLOCK_SIZE_K"]),
+    )
+    trans_matmul_248_kernel[grid](
+        input,
+        qweight,
+        output,
+        scales,
+        qzeros,
+        g_idx,
+        input.shape[0],
+        qweight.shape[1],
+        output_dim,
+        bits,
+        maxq,
+        input.stride(0),
+        input.stride(1),
+        qweight.stride(0),
+        qweight.stride(1),
+        output.stride(0),
+        output.stride(1),
+        scales.stride(0),
+        qzeros.stride(0),
+    )
     return output
 
+
 class QuantLinearFunction(torch.autograd.Function):
     @staticmethod
     @custom_fwd(cast_inputs=torch.float16)
     def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
         output = matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq)
         ctx.save_for_backward(qweight, scales, qzeros, g_idx)
-        ctx.bits,ctx.maxq = bits, maxq
+        ctx.bits, ctx.maxq = bits, maxq
         return output
-    
+
     @staticmethod
     @custom_bwd
     def backward(ctx, grad_output):
         qweight, scales, qzeros, g_idx = ctx.saved_tensors
         bits, maxq = ctx.bits, ctx.maxq
         grad_input = None
 
         if ctx.needs_input_grad[0]:
-            grad_input = transpose_matmul248(grad_output, qweight, scales, qzeros, g_idx, bits, maxq)
+            grad_input = transpose_matmul248(
+                grad_output, qweight, scales, qzeros, g_idx, bits, maxq
+            )
         return grad_input, None, None, None, None, None, None
-    
-class QuantLinear(nn.Module): 
+
+
+class QuantLinear(nn.Module):
     def __init__(self, bits, groupsize, infeatures, outfeatures, bias):
         super().__init__()
-        if bits not in [2,4,8]:
+        if bits not in [2, 4, 8]:
             raise NotImplementedError("Only 2,4,8 bits are supported.")
         self.infeatures = infeatures
         self.outfeatures = outfeatures
         self.bits = bits
-        self.maxq = 2 ** self.bits - 1
+        self.maxq = 2**self.bits - 1
         self.groupsize = groupsize if groupsize != -1 else infeatures
-        
-        self.register_buffer('qweight', torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32))
-        self.register_buffer('qzeros', torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32))
-        self.register_buffer('scales', torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16))
-        self.register_buffer('g_idx', torch.tensor([i // self.groupsize  for i in range(infeatures)], dtype = torch.int32))
+
+        self.register_buffer(
+            "qweight",
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32),
+        )
+        self.register_buffer(
+            "qzeros",
+            torch.zeros(
+                (math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits),
+                dtype=torch.int32,
+            ),
+        )
+        self.register_buffer(
+            "scales",
+            torch.zeros(
+                (math.ceil(infeatures / self.groupsize), outfeatures),
+                dtype=torch.float16,
+            ),
+        )
+        self.register_buffer(
+            "g_idx",
+            torch.tensor(
+                [i // self.groupsize for i in range(infeatures)], dtype=torch.int32
+            ),
+        )
         if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures),dtype=torch.float16))
+            self.register_buffer(
+                "bias", torch.zeros((outfeatures), dtype=torch.float16)
+            )
         else:
             self.bias = None
-        
-    def pack(self, linear, scales, zeros, g_idx = None):
+
+    def pack(self, linear, scales, zeros, g_idx=None):
         self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-        
+
         scales = scales.t().contiguous()
         zeros = zeros.t().contiguous()
         scale_zeros = zeros * scales
         self.scales = scales.clone().half()
         if linear.bias is not None:
             self.bias = linear.bias.clone().half()
-            
+
         intweight = []
         for idx in range(self.infeatures):
-            intweight.append(torch.round((linear.weight.data[:,idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]).to(torch.int)[:,None])
-        intweight = torch.cat(intweight,dim=1)
+            intweight.append(
+                torch.round(
+                    (linear.weight.data[:, idx] + scale_zeros[self.g_idx[idx]])
+                    / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
         intweight = intweight.t().contiguous()
         intweight = intweight.numpy().astype(np.uint32)
-        qweight = np.zeros((intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32)
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
         i = 0
         row = 0
         while row < qweight.shape[0]:
-            if self.bits in [2,4,8]:
-                for j in range(i, i + (32//self.bits)):
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
                     qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32//self.bits
+                i += 32 // self.bits
                 row += 1
             else:
                 raise NotImplementedError("Only 2,4,8 bits are supported.")
-                
+
         qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight) 
-        
-        zeros -= 1;
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
         zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        qzeros = np.zeros(
+            (zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32
+        )
         i = 0
         col = 0
         while col < qzeros.shape[1]:
-            if self.bits in [2,4,8]:
-                for j in range(i, i + (32//self.bits)):
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
                     qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32//self.bits
+                i += 32 // self.bits
                 col += 1
             else:
                 raise NotImplementedError("Only 2,4,8 bits are supported.")
-                
+
         qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros) 
-        
+        self.qzeros = torch.from_numpy(qzeros)
+
     def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures, )
-        out = QuantLinearFunction.apply(x.reshape(-1,x.shape[-1]), self.qweight, self.scales, 
-                                        self.qzeros, self.g_idx, self.bits, self.maxq)
-        out = out + self.bias if self.bias is not None else out  
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        out = QuantLinearFunction.apply(
+            x.reshape(-1, x.shape[-1]),
+            self.qweight,
+            self.scales,
+            self.qzeros,
+            self.g_idx,
+            self.bits,
+            self.maxq,
+        )
+        out = out + self.bias if self.bias is not None else out
         return out.reshape(out_shape)
-        
-def autotune_warmup(model, transpose = False):
+
+
+def autotune_warmup(model, transpose=False):
     """
     Pre-tunes the quantized kernel
     """
     from tqdm import tqdm
 
     n_values = {}
 
     for _, m in model.named_modules():
         if not isinstance(m, QuantLinear):
             continue
 
         k = m.infeatures
         n = m.outfeatures
-        
+
         if n not in n_values:
-            n_values[n] = (k, m.qweight.cuda(), m.scales.cuda(), m.qzeros.cuda(), m.g_idx.cuda(), m.bits, m.maxq)
+            n_values[n] = (
+                k,
+                m.qweight.cuda(),
+                m.scales.cuda(),
+                m.qzeros.cuda(),
+                m.g_idx.cuda(),
+                m.bits,
+                m.maxq,
+            )
 
-    print(f'Found {len(n_values)} unique N values.')
+    print(f"Found {len(n_values)} unique N values.")
 
-    print('Warming up autotune cache ...')
+    print("Warming up autotune cache ...")
     for m in tqdm(range(0, 12)):
-        m = 2 ** m   # [1, 2048]
+        m = 2**m  # [1, 2048]
         for n, (k, qweight, scales, qzeros, g_idx, bits, maxq) in n_values.items():
-            a = torch.randn(m, k, dtype=torch.float16, device='cuda')
+            a = torch.randn(m, k, dtype=torch.float16, device="cuda")
             matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
             if transpose:
-                a = torch.randn(m, n, dtype=torch.float16, device='cuda')
+                a = torch.randn(m, n, dtype=torch.float16, device="cuda")
                 transpose_matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
     del n_values
-        
-def make_quant(module, names, bits, groupsize, name=''):
+
+
+def make_quant(module, names, bits, groupsize, name=""):
     if isinstance(module, QuantLinear):
         return
     for attr in dir(module):
         tmp = getattr(module, attr)
-        name1 = name + '.' + attr if name != '' else attr
+        name1 = name + "." + attr if name != "" else attr
         if name1 in names:
             delattr(module, attr)
-            setattr(module, attr, QuantLinear(bits, groupsize, tmp.in_features, tmp.out_features, tmp.bias is not None))
+            setattr(
+                module,
+                attr,
+                QuantLinear(
+                    bits,
+                    groupsize,
+                    tmp.in_features,
+                    tmp.out_features,
+                    tmp.bias is not None,
+                ),
+            )
     for name1, child in module.named_children():
-        make_quant(child, names, bits, groupsize, name + '.' + name1 if name != '' else name1)
+        make_quant(
+            child, names, bits, groupsize, name + "." + name1 if name != "" else name1
+        )
```

### Comparing `xturing-0.1.0/src/xturing/model_apis/__init__.py` & `xturing-0.1.1/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/model_apis/ai21.py` & `xturing-0.1.1/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/model_apis/base.py` & `xturing-0.1.1/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/model_apis/cohere.py` & `xturing-0.1.1/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/model_apis/openai.py` & `xturing-0.1.1/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/__init__.py` & `xturing-0.1.1/src/xturing/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/base.py` & `xturing-0.1.1/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/bloom.py` & `xturing-0.1.1/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/causal.py` & `xturing-0.1.1/src/xturing/models/causal.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/cerebras.py` & `xturing-0.1.1/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/distilgpt2.py` & `xturing-0.1.1/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/galactica.py` & `xturing-0.1.1/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/gpt2.py` & `xturing-0.1.1/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/gptj.py` & `xturing-0.1.1/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/llama.py` & `xturing-0.1.1/src/xturing/models/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/opt.py` & `xturing-0.1.1/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/models/stable_diffusion.py` & `xturing-0.1.1/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.1/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.1/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/registry.py` & `xturing-0.1.1/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.1/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.1/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.1/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.1/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.1/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.1/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.1/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.1/src/xturing/trainers/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,19 @@
         if max_training_time_in_secs is not None:
             training_callbacks.append(
                 callbacks.Timer(
                     duration=datetime.timedelta(seconds=max_training_time_in_secs)
                 )
             )
         model_engine.model.train()
-        model_engine.model.print_trainable_parameters()
+
+        try:
+            model_engine.model.print_trainable_parameters()
+        except AttributeError:
+            pass
 
         if DEFAULT_DEVICE.type == "cpu":
             self.trainer = Trainer(
                 num_nodes=1,
                 accelerator="cpu",
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
```

### Comparing `xturing-0.1.0/src/xturing/ui/playground.py` & `xturing-0.1.1/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/hub.py` & `xturing-0.1.1/src/xturing/utils/hub.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/logging.py` & `xturing-0.1.1/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/loss_fns.py` & `xturing-0.1.1/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/notebooks.py` & `xturing-0.1.1/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/text_splitter.py` & `xturing-0.1.1/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing/utils/utils.py` & `xturing-0.1.1/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.0/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.1/src/xturing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.0/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.1/src/xturing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

