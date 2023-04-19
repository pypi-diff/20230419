# Comparing `tmp/textgen-0.2.2.tar.gz` & `tmp/textgen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.2.2.tar", last modified: Mon Apr 17 14:32:15 2023, max compression
+gzip compressed data, was "textgen-0.2.3.tar", last modified: Wed Apr 19 12:37:48 2023, max compression
```

## Comparing `textgen-0.2.2.tar` & `textgen-0.2.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.105381 textgen-0.2.2/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.2/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-17 14:32:15.105904 textgen-0.2.2/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.2/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-17 14:32:15.106668 textgen-0.2.2/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-17 14:02:51.000000 textgen-0.2.2/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.047149 textgen-0.2.2/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-17 13:39:14.000000 textgen-0.2.2/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.055964 textgen-0.2.2/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.2/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.2/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.2/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.2/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.2/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.2/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.058842 textgen-0.2.2/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.2/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    31478 2023-04-17 14:30:17.000000 textgen-0.2.2/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.2/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.062480 textgen-0.2.2/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.2/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    14497 2023-04-14 05:57:19.000000 textgen-0.2.2/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.064526 textgen-0.2.2/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.2/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.068106 textgen-0.2.2/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.2/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.2/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.071986 textgen-0.2.2/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.2/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.2/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.079396 textgen-0.2.2/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.2/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.2/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.2/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.2/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.2/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.084416 textgen-0.2.2/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.2/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    23156 2023-04-17 04:08:29.000000 textgen-0.2.2/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5753 2023-04-13 14:13:30.000000 textgen-0.2.2/textgen/llama/llama_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.093358 textgen-0.2.2/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.2/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.2/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.2/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.2/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.2/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.2/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.2/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.101326 textgen-0.2.2/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.2/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.2/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.2/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.2/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.2/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.103988 textgen-0.2.2/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.2/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.2/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.2/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.050098 textgen-0.2.2/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.061799 textgen-0.2.3/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.3/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 12:37:48.062286 textgen-0.2.3/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.3/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-19 12:37:48.062972 textgen-0.2.3/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-19 12:37:28.000000 textgen-0.2.3/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.007411 textgen-0.2.3/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-19 12:37:28.000000 textgen-0.2.3/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.018701 textgen-0.2.3/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.3/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.3/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.3/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.3/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.3/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.3/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.022030 textgen-0.2.3/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.3/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    21986 2023-04-19 07:16:18.000000 textgen-0.2.3/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.3/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.024915 textgen-0.2.3/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.3/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14505 2023-04-19 06:54:54.000000 textgen-0.2.3/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.026851 textgen-0.2.3/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.3/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.029345 textgen-0.2.3/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.3/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.3/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.032755 textgen-0.2.3/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.3/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.3/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.039215 textgen-0.2.3/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.3/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.3/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.3/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.3/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.3/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.042700 textgen-0.2.3/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.3/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    22688 2023-04-19 07:16:18.000000 textgen-0.2.3/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5741 2023-04-18 02:48:12.000000 textgen-0.2.3/textgen/llama/llama_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.051516 textgen-0.2.3/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.3/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.3/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.3/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.3/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.3/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.3/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.3/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.057929 textgen-0.2.3/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.3/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.3/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.3/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.3/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.3/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.060745 textgen-0.2.3/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.3/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.3/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.3/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.010712 textgen-0.2.3/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.2.2/LICENSE` & `textgen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/PKG-INFO` & `textgen-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.2
+Version: 0.2.3
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
```

### Comparing `textgen-0.2.2/README.md` & `textgen-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/setup.py` & `textgen-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.2.2',
+    version='0.2.3',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
```

### Comparing `textgen-0.2.2/textgen/__init__.py` & `textgen-0.2.3/textgen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
```

### Comparing `textgen-0.2.2/textgen/augment/sentence_level_augment.py` & `textgen-0.2.3/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/augment/text_augment.py` & `textgen-0.2.3/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/augment/tokenizer.py` & `textgen-0.2.3/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/augment/translate_api.py` & `textgen-0.2.3/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/augment/word_level_augment.py` & `textgen-0.2.3/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/augment/word_vocab.py` & `textgen-0.2.3/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/chatglm/chatglm_model.py` & `textgen-0.2.3/textgen/chatglm/chatglm_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @author:XuMing(xuming624@qq.com)
 @description:
 """
 import os
 import random
 import re
 import sys
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import List, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from loguru import logger
 from peft import (
     get_peft_model,
@@ -24,21 +24,14 @@
 from tqdm.auto import tqdm
 from transformers import Trainer, TrainingArguments, AutoTokenizer, AutoModel, AutoConfig
 from transformers.trainer import TRAINING_ARGS_NAME
 
 from textgen.chatglm.chatglm_utils import load_hf_dataset, ChatGlmDataset
 from textgen.config.model_args import ChatGlmArgs
 
-try:
-    import wandb
-
-    wandb_available = True
-except ImportError:
-    wandb_available = False
-
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
     "chatglm": (AutoConfig, AutoModel, AutoTokenizer),
 }
@@ -129,17 +122,22 @@
         self.args.model_type = model_type
         if model_name is None:
             self.args.model_name = "ChatGLM_from_scratch"
         else:
             self.args.model_name = model_name
 
         self.lora_name = lora_name
-        self.lora_loaded = False
+        if self.args.use_lora:
+            self.load_lora()
+
+        if torch.__version__ >= "2" and sys.platform != "win32":
+            self.model = torch.compile(self.model)
 
     def data_collator(self, batch):
+        """Data collator that will dynamically pad the inputs received."""
         len_ids = [len(example) for example in batch]
         longest = max(len_ids)
         input_ids = []
         labels_list = []
         for ids_l, example in sorted(zip(len_ids, batch), key=lambda x: -x[0]):
             ids = list(example)
             seq_len = ids.index(self.tokenizer.bos_token_id) + 1  # is equal to prompt length
@@ -240,18 +238,16 @@
                     logger.info(f"Restarting from {checkpoint_name}")
                     adapters_weights = torch.load(checkpoint_name)
                     self.model = set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
-            self.lora_loaded = True
         else:
-            logger.error("only impl lora fine-tune, set `use_lora=True` for train.")
-            raise ValueError("set `use_lora=True` for train.")
+            logger.warning("Now full model params fine-tune, which is slow, set `use_lora=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
 
         # load dataset
         train_dataset = self.load_and_cache_examples(train_data)
         if verbose:
             logger.debug(f"train_dataset len: {len(train_dataset)}, train_dataset[0]: {train_dataset[0]}")
         eval_dataset = None
@@ -335,58 +331,53 @@
             logger.info(f"  {key} = {metrics[key]}")
         output_file = os.path.join(output_dir, f"{split}_results.txt")
         with open(output_file, "w") as writer:
             for key in sorted(metrics.keys()):
                 writer.write("{} = {}\n".format(key, str(metrics[key])))
 
     def load_lora(self):
-        if self.args.use_lora:
-            if self.lora_name:
-                self.model = PeftModel.from_pretrained(self.model, self.lora_name)
-                logger.info(f"Loaded lora model from {self.lora_name}")
-                self.lora_loaded = True
-            else:
-                lora_path = os.path.join(self.args.output_dir, self.args.lora_name)
-                if lora_path and os.path.exists(lora_path):
-                    self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
-                    logger.info(f"Loaded lora model from {lora_path}")
-                    self.lora_loaded = True
-            if torch.__version__ >= "2" and sys.platform != "win32":
-                self.model = torch.compile(self.model)
+        """Load lora model."""
+        if self.lora_name:
+            self.model = PeftModel.from_pretrained(self.model, self.lora_name)
+            logger.info(f"Loaded lora model from {self.lora_name}")
+        else:
+            lora_path = os.path.join(self.args.output_dir, self.args.lora_bin_name)
+            if lora_path and os.path.exists(lora_path):
+                self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
+                logger.info(f"Loaded lora model from {lora_path}")
 
     def process_response(self, response):
+        """Process response text."""
         response = response.strip().replace("[[训练时间]]", "2023年")
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
             [";", "；"],
-            ["\?", "？"],
+            ["\\?", "？"],
         ]
         for item in punkts:
             response = re.sub(r"([\u4e00-\u9fff])%s" % item[0], r"\1%s" % item[1], response)
             response = re.sub(r"%s([\u4e00-\u9fff])" % item[0], r"%s\1" % item[1], response)
         return response
 
     @torch.no_grad()
-    def predict(self, sentences, keep_prompt=False, max_length=None, **kwargs):
+    def predict(self, sentences: List[str], keep_prompt: bool = False, max_length: int = None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
             sentences: A python list of text (str) to be sent to the model for prediction. 
             keep_prompt: Whether to keep the prompt in the generated text.
             max_length: The maximum length of the generated text.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
-        if not self.lora_loaded:
-            self.load_lora()
         if self.args.fp16:
             self.model.half()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
@@ -419,15 +410,15 @@
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
         return all_outputs
 
     @torch.no_grad()
     def chat(self, query: str, history: List[Tuple[str, str]] = None,
-             keep_prompt=False, max_length=128, **kwargs):
+             keep_prompt: bool = False, max_length: int = 128, **kwargs):
         """
         Chat with the model
         :param query:
         :param history:
         :param keep_prompt:
         :param max_length:
         :param kwargs:
@@ -479,14 +470,15 @@
                 data,
                 mode,
             )
 
     def save_model(
             self, output_dir=None, optimizer=None, scheduler=None, model=None, results=None
     ):
+        """Save the model and the tokenizer to the `output_dir`."""
         if not output_dir:
             output_dir = self.args.output_dir
         os.makedirs(output_dir, exist_ok=True)
 
         if model and not self.args.no_save:
             # Take care of distributed/parallel training
             model_to_save = model.module if hasattr(model, "module") else model
@@ -510,223 +502,28 @@
     def _load_model_args(self, input_dir):
         args = ChatGlmArgs()
         args.load(input_dir)
         return args
 
 
 class FinetuneTrainer(Trainer):
+    """Finetune trainer for ChatGlmModel"""
+
     def compute_loss(self, model, inputs, return_outputs=False):
+        """Computes the loss."""
         return model(
             input_ids=inputs["input_ids"],
             labels=inputs["labels"],
         ).loss
 
-    def evaluate(
-            self,
-            eval_dataset=None,
-            ignore_keys=None,
-            metric_key_prefix: str = "eval",
-            **gen_kwargs
-    ):
-        """
-        Run evaluation and returns metrics.
-
-        The calling script will be responsible for providing a method to compute metrics, as they are task-dependent
-        (pass it to the init `compute_metrics` argument).
-
-        You can also subclass and override this method to inject custom behavior.
-
-        Args:
-            eval_dataset (`Dataset`, *optional*):
-                Pass a dataset if you wish to override `self.eval_dataset`. If it is an [`~datasets.Dataset`], columns
-                not accepted by the `model.forward()` method are automatically removed. It must implement the `__len__`
-                method.
-            ignore_keys (`List[str]`, *optional*):
-                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
-                gathering predictions.
-            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
-                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
-                "eval_bleu" if the prefix is `"eval"` (default)
-            gen_kwargs:
-                Additional `generate` specific kwargs.
-
-        Returns:
-            A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
-            dictionary also contains the epoch number which comes from the training state.
-        """
-
-        gen_kwargs = gen_kwargs.copy()
-        self._gen_kwargs = gen_kwargs
-        return super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
-
-    def predict(
-            self,
-            test_dataset,
-            ignore_keys: Optional[List[str]] = None,
-            metric_key_prefix: str = "test",
-            **gen_kwargs
-    ):
-        """
-        Run prediction and returns predictions and potential metrics.
-
-        Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
-        will also return metrics, like in `evaluate()`.
-
-        Args:
-            test_dataset (`Dataset`):
-                Dataset to run the predictions on. If it is a [`~datasets.Dataset`], columns not accepted by the
-                `model.forward()` method are automatically removed. Has to implement the method `__len__`
-            ignore_keys (`List[str]`, *optional*):
-                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
-                gathering predictions.
-            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
-                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
-                "eval_bleu" if the prefix is `"eval"` (default)
-            max_length (`int`, *optional*):
-                The maximum target length to use when predicting with the generate method.
-            num_beams (`int`, *optional*):
-                Number of beams for beam search that will be used when predicting with the generate method. 1 means no
-                beam search.
-            gen_kwargs:
-                Additional `generate` specific kwargs.
-
-        <Tip>
-
-        If your predictions or labels have different sequence lengths (for instance because you're doing dynamic
-        padding in a token classification task) the predictions will be padded (on the right) to allow for
-        concatenation into one array. The padding index is -100.
-
-        </Tip>
-
-        Returns: *NamedTuple* A namedtuple with the following keys:
-
-            - predictions (`np.ndarray`): The predictions on `test_dataset`.
-            - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
-            - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
-              labels).
-        """
-
-        gen_kwargs = gen_kwargs.copy()
-        self._gen_kwargs = gen_kwargs
-
-        return super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
-
-    def prediction_step(
-            self,
-            model: nn.Module,
-            inputs: Dict[str, Union[torch.Tensor, Any]],
-            prediction_loss_only: bool,
-            ignore_keys: Optional[List[str]] = None,
-    ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
-        """
-        Perform an evaluation step on `model` using `inputs`.
-
-        Subclass and override to inject custom behavior.
-
-        Args:
-            model (`nn.Module`):
-                The model to evaluate.
-            inputs (`Dict[str, Union[torch.Tensor, Any]]`):
-                The inputs and targets of the model.
-
-                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
-                argument `labels`. Check your model's documentation for all accepted arguments.
-            prediction_loss_only (`bool`):
-                Whether or not to return the loss only.
-            ignore_keys (`List[str]`, *optional*): Ignore the keys in the output of your model (if it is a dictionary)
-        Return:
-            Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss, logits and
-            labels (each being optional).
-        """
-
-        if prediction_loss_only:
-            return super().prediction_step(
-                model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
-            )
-
-        has_labels = "labels" in inputs
-        inputs = self._prepare_inputs(inputs)
-
-        # XXX: adapt synced_gpus for fairscale as well
-        gen_kwargs = self._gen_kwargs.copy()
-        if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
-            gen_kwargs["max_length"] = self.model.config.max_length
-        gen_kwargs["num_beams"] = (
-            gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.model.config.num_beams
-        )
-        default_synced_gpus = False
-        gen_kwargs["synced_gpus"] = (
-            gen_kwargs["synced_gpus"] if gen_kwargs.get("synced_gpus") is not None else default_synced_gpus
-        )
-
-        if "attention_mask" in inputs:
-            gen_kwargs["attention_mask"] = inputs.get("attention_mask", None)
-        if "position_ids" in inputs:
-            gen_kwargs["position_ids"] = inputs.get("position_ids", None)
-        if "global_attention_mask" in inputs:
-            gen_kwargs["global_attention_mask"] = inputs.get("global_attention_mask", None)
-
-        # prepare generation inputs
-        # some encoder-decoder models can have varying encoder's and thus
-        # varying model input names
-        if hasattr(self.model, "encoder") and self.model.encoder.main_input_name != self.model.main_input_name:
-            generation_inputs = inputs[self.model.encoder.main_input_name]
-        else:
-            generation_inputs = inputs[self.model.main_input_name]
-
-        gen_kwargs["input_ids"] = generation_inputs
-        generated_tokens = self.model.generate(**gen_kwargs)
-        generated_tokens = generated_tokens[:, generation_inputs.size()[-1]:]
-
-        # in case the batch is shorter than max length, the output should be padded
-        if gen_kwargs.get("max_length") is not None and generated_tokens.shape[-1] < gen_kwargs["max_length"]:
-            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_length"])
-        elif gen_kwargs.get("max_new_tokens") is not None and generated_tokens.shape[-1] < (
-                gen_kwargs["max_new_tokens"] + 1
-        ):
-            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_new_tokens"] + 1)
-
-        loss = None
-
-        if self.args.prediction_loss_only:
-            return loss, None, None
-
-        if has_labels:
-            labels = inputs["labels"]
-            if gen_kwargs.get("max_length") is not None and labels.shape[-1] < gen_kwargs["max_length"]:
-                labels = self._pad_tensors_to_max_len(labels, gen_kwargs["max_length"])
-            elif gen_kwargs.get("max_new_tokens") is not None and labels.shape[-1] < (
-                    gen_kwargs["max_new_tokens"] + 1
-            ):
-                labels = self._pad_tensors_to_max_len(labels, (gen_kwargs["max_new_tokens"] + 1))
-        else:
-            labels = None
-
-        return loss, generated_tokens, labels
-
-    def _pad_tensors_to_max_len(self, tensor, max_length):
-        if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
-            # If PAD token is not defined at least EOS token has to be defined
-            pad_token_id = (
-                self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
-            )
-        else:
-            if self.model.config.pad_token_id is not None:
-                pad_token_id = self.model.config.pad_token_id
-            else:
-                raise ValueError("Pad_token_id must be set in the configuration of the model, in order to pad tensors")
-
-        padded_tensor = pad_token_id * torch.ones(
-            (tensor.shape[0], max_length), dtype=tensor.dtype, device=tensor.device
-        )
-        padded_tensor[:, : tensor.shape[-1]] = tensor
-        return padded_tensor
-
     def save_model(self, output_dir=None, _internal_call=False):
+        """Save the LoRA model"""
         os.makedirs(output_dir, exist_ok=True)
         torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
         self.model.save_pretrained(output_dir)
 
 
 class CastOutputToFloat(nn.Sequential):
+    """Cast the output of the model to float"""
+
     def forward(self, x):
         return super().forward(x).to(torch.float32)
```

### Comparing `textgen-0.2.2/textgen/chatglm/chatglm_utils.py` & `textgen-0.2.3/textgen/chatglm/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/config/global_args.py` & `textgen-0.2.3/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/config/model_args.py` & `textgen-0.2.3/textgen/config/model_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     temperature: float = 0.95
     special_tokens_list: list = field(default_factory=list)
     top_k: float = None
     top_p: float = 0.7
     model_name_or_path: Optional[str] = field(default="THUDM/chatglm-6b")
     dataset_name_or_path: Optional[str] = field(default="shibing624/alpaca-zh")
     use_lora: bool = True
-    lora_name: str = field(default="adapter_model.bin")
+    lora_bin_name: str = field(default="adapter_model.bin")
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
     lora_target_modules = ["query_key_value"]
     lora_bias = "none"
     only_lora_state_dict: bool = False
     num_train_epochs = 1
@@ -418,15 +418,15 @@
     repetition_penalty: float = 1.0
     temperature: float = 0.95
     special_tokens_list: list = field(default_factory=list)
     top_k: float = 30
     top_p: float = 0.7
     model_name_or_path: Optional[str] = field(default="decapoda-research/llama-7b-hf")
     use_lora: bool = True
-    lora_name: str = field(default="adapter_model.bin")
+    lora_bin_name: str = field(default="adapter_model.bin")
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
     lora_target_modules = ["q_proj", "k_proj", "v_proj", "o_proj"]
     lora_bias = "none"
     only_lora_state_dict: bool = True
     num_train_epochs = 3
```

### Comparing `textgen-0.2.2/textgen/custom_models/models.py` & `textgen-0.2.3/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/data/HowNetPOSWord.txt` & `textgen-0.2.3/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/data/stopwords.txt` & `textgen-0.2.3/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_generation/language_generation_model.py` & `textgen-0.2.3/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_generation/language_generation_utils.py` & `textgen-0.2.3/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_modeling/language_modeling_model.py` & `textgen-0.2.3/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.2.3/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_modeling/songnet_model.py` & `textgen-0.2.3/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/language_modeling/songnet_utils.py` & `textgen-0.2.3/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/llama/llama_model.py` & `textgen-0.2.3/textgen/llama/llama_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,14 @@
 from transformers import LlamaForCausalLM, LlamaTokenizer
 from transformers import Trainer, TrainingArguments, AutoConfig
 from transformers.trainer import TRAINING_ARGS_NAME
 
 from textgen.config.model_args import LlamaArgs
 from textgen.llama.llama_utils import load_hf_dataset, LlamaDataset
 
-try:
-    import wandb
-
-    wandb_available = True
-except ImportError:
-    wandb_available = False
-
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
     "llama": (AutoConfig, LlamaForCausalLM, LlamaTokenizer),
 }
@@ -127,29 +120,32 @@
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
             self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name)
         else:
             self.tokenizer = tokenizer_class.from_pretrained(model_name)
             self.args.tokenizer_name = self.args.model_name
 
-        self.tokenizer.pad_token_id = (
-            0  # unk. we want this to be different from the eos token
-        )
-        self.model.config.pad_token_id = 0  # unk
-        self.model.config.bos_token_id = 1
-        self.model.config.eos_token_id = 2
-        self.tokenizer.padding_side = "left"  # Allow batched inference
         self.args.model_type = model_type
         if model_name is None:
             self.args.model_name = "Llama_from_scratch"
         else:
             self.args.model_name = model_name
 
         self.lora_name = lora_name
-        self.lora_loaded = False
+        if self.args.use_lora:
+            self.load_lora()
+
+        # unwind broken decapoda-research config
+        self.tokenizer.padding_side = "left"
+        self.tokenizer.pad_token_id = 0  # unk. we want this to be different from the eos token
+        self.model.config.pad_token_id = 0  # unk
+        self.model.config.bos_token_id = 1
+        self.model.config.eos_token_id = 2
+        if torch.__version__ >= "2" and sys.platform != "win32":
+            self.model = torch.compile(self.model)
 
     def train_model(
             self,
             train_data,
             output_dir=None,
             args=None,
             eval_data=None,
@@ -235,18 +231,16 @@
                     logger.info(f"Restarting from {checkpoint_name}")
                     adapters_weights = torch.load(checkpoint_name)
                     self.model = set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
-            self.lora_loaded = True
         else:
-            logger.error("only impl lora fine-tune, set `use_lora=True` for train.")
-            raise ValueError("set `use_lora=True` for train.")
+            logger.warning("Now full model params fine-tune, which is slow, set `use_lora=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
 
         # load dataset
         train_dataset = self.load_and_cache_examples(train_data)
         if verbose:
             logger.debug(f"train_dataset len: {len(train_dataset)}, train_dataset[0]: {train_dataset[0]}")
         eval_dataset = None
@@ -353,60 +347,48 @@
             logger.info(f"  {key} = {metrics[key]}")
         output_file = os.path.join(output_dir, f"{split}_results.txt")
         with open(output_file, "w") as writer:
             for key in sorted(metrics.keys()):
                 writer.write("{} = {}\n".format(key, str(metrics[key])))
 
     def load_lora(self):
-        if self.args.use_lora:
-            if self.lora_name:
-                if os.path.isdir(self.lora_name) and os.path.exists(
-                        os.path.join(self.lora_name, "tokenizer_config.json")):
-                    update_tokenizer = True
-                else:
-                    update_tokenizer = False
-                if "ziqingyang/chinese" in self.lora_name or update_tokenizer:
-                    self.tokenizer = LlamaTokenizer.from_pretrained(self.lora_name)
-                    self.model.resize_token_embeddings(len(self.tokenizer))
-                    assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
-                    logger.debug(f"Tokenizer updated, vocabulary size: {len(self.tokenizer)}")
-                self.model = PeftModel.from_pretrained(self.model, self.lora_name)
-                logger.info(f"Loaded lora model from {self.lora_name}")
-                self.lora_loaded = True
+        """Load lora model"""
+        if self.lora_name:
+            if os.path.isdir(self.lora_name) and os.path.exists(
+                    os.path.join(self.lora_name, "tokenizer_config.json")):
+                update_tokenizer = True
             else:
-                lora_path = os.path.join(self.args.output_dir, self.args.lora_name)
-                if lora_path and os.path.exists(lora_path):
-                    self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
-                    logger.info(f"Loaded lora model from {lora_path}")
-                    self.lora_loaded = True
-
-            # unwind broken decapoda-research config
-            self.tokenizer.padding_side = "left"
-            self.model.config.pad_token_id = self.tokenizer.pad_token_id = 0  # unk
-            self.model.config.bos_token_id = 1
-            self.model.config.eos_token_id = 2
-            if torch.__version__ >= "2" and sys.platform != "win32":
-                self.model = torch.compile(self.model)
+                update_tokenizer = False
+            if "ziqingyang/chinese" in self.lora_name or update_tokenizer:
+                self.tokenizer = LlamaTokenizer.from_pretrained(self.lora_name)
+                self.model.resize_token_embeddings(len(self.tokenizer))
+                assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
+                logger.debug(f"Tokenizer updated, vocabulary size: {len(self.tokenizer)}")
+            self.model = PeftModel.from_pretrained(self.model, self.lora_name)
+            logger.info(f"Loaded lora model from {self.lora_name}")
+        else:
+            lora_path = os.path.join(self.args.output_dir, self.args.lora_bin_name)
+            if lora_path and os.path.exists(lora_path):
+                self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
+                logger.info(f"Loaded lora model from {lora_path}")
 
     @torch.no_grad()
-    def predict(self, sentences, keep_prompt=False, max_length=None, **kwargs):
+    def predict(self, sentences: List[str], keep_prompt: bool = False, max_length: int = None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
             sentences: A python list of text (str) to be sent to the model for prediction. Note that the prefix should be prepended to the text.
             keep_prompt: Whether to keep the prompt in the generated text.
             max_length: The maximum length of the generated text.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
-        if not self.lora_loaded:
-            self.load_lora()
         if self.args.fp16:
             self.model.half()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
@@ -442,15 +424,15 @@
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
         return all_outputs
 
     @torch.no_grad()
     def chat(self, query: str, history: List[Tuple[str, str]] = None,
-             keep_prompt=False, max_length=128, **kwargs):
+             keep_prompt: bool = False, max_length: int = 128, **kwargs):
         """
         Chat with the model
         :param query:
         :param history:
         :param keep_prompt:
         :param max_length:
         :param kwargs:
@@ -502,14 +484,15 @@
                 data,
                 mode,
             )
 
     def save_model(
             self, output_dir=None, optimizer=None, scheduler=None, model=None, results=None
     ):
+        """Save the model and the tokenizer."""
         if not output_dir:
             output_dir = self.args.output_dir
         os.makedirs(output_dir, exist_ok=True)
 
         if model and not self.args.no_save:
             # Take care of distributed/parallel training
             model_to_save = model.module if hasattr(model, "module") else model
@@ -533,11 +516,16 @@
     def _load_model_args(self, input_dir):
         args = LlamaArgs()
         args.load(input_dir)
         return args
 
 
 class FinetuneTrainer(Trainer):
+    """
+    Trainer for finetuning models
+    """
+
     def save_model(self, output_dir=None, _internal_call=False):
+        """Save the LoRA model."""
         os.makedirs(output_dir, exist_ok=True)
         torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
         self.model.save_pretrained(output_dir)
```

### Comparing `textgen-0.2.2/textgen/llama/llama_utils.py` & `textgen-0.2.3/textgen/llama/llama_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from loguru import logger
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
 
 PROMPT_DICT = {
     "prompt_input": (
         "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
-        "### Instruction:\n{instruction}\n### Input:\n{input_text}\n\n### Response:"
+        "### Instruction:\n{instruction}\n{input_text}\n\n### Response:"
     ),
     "prompt_no_input": (
         "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
         "### Instruction:\n{instruction}\n\n### Response:"
     ),
 }
```

### Comparing `textgen-0.2.2/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.2.3/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.2.3/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.2.3/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/seq2seq/data_reader.py` & `textgen-0.2.3/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/seq2seq/seq2seq_model.py` & `textgen-0.2.3/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.2.3/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/t5/copyt5_model.py` & `textgen-0.2.3/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/t5/copyt5_utils.py` & `textgen-0.2.3/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/t5/t5_model.py` & `textgen-0.2.3/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/t5/t5_utils.py` & `textgen-0.2.3/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/unsup_generation/tgls_model.py` & `textgen-0.2.3/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen/unsup_generation/tgls_util.py` & `textgen-0.2.3/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.2/textgen.egg-info/PKG-INFO` & `textgen-0.2.3/textgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.2
+Version: 0.2.3
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
```

### Comparing `textgen-0.2.2/textgen.egg-info/SOURCES.txt` & `textgen-0.2.3/textgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

