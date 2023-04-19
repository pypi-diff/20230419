# Comparing `tmp/textgen-0.2.3.tar.gz` & `tmp/textgen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.2.3.tar", last modified: Wed Apr 19 12:37:48 2023, max compression
+gzip compressed data, was "textgen-0.2.4.tar", last modified: Wed Apr 19 14:11:21 2023, max compression
```

## Comparing `textgen-0.2.3.tar` & `textgen-0.2.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.061799 textgen-0.2.3/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.3/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 12:37:48.062286 textgen-0.2.3/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.3/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-19 12:37:48.062972 textgen-0.2.3/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-19 12:37:28.000000 textgen-0.2.3/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.007411 textgen-0.2.3/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-19 12:37:28.000000 textgen-0.2.3/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.018701 textgen-0.2.3/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.3/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.3/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.3/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.3/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.3/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.3/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.022030 textgen-0.2.3/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.3/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    21986 2023-04-19 07:16:18.000000 textgen-0.2.3/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.3/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.024915 textgen-0.2.3/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.3/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    14505 2023-04-19 06:54:54.000000 textgen-0.2.3/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.026851 textgen-0.2.3/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.3/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.029345 textgen-0.2.3/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.3/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.3/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.032755 textgen-0.2.3/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.3/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.3/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.3/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.039215 textgen-0.2.3/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.3/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.3/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.3/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.3/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.3/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.042700 textgen-0.2.3/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.3/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    22688 2023-04-19 07:16:18.000000 textgen-0.2.3/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5741 2023-04-18 02:48:12.000000 textgen-0.2.3/textgen/llama/llama_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.051516 textgen-0.2.3/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.3/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.3/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.3/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.3/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.3/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.3/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.3/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.057929 textgen-0.2.3/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.3/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.3/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.3/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.3/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.3/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.060745 textgen-0.2.3/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.3/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.3/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.3/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 12:37:48.010712 textgen-0.2.3/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-19 12:37:47.000000 textgen-0.2.3/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.674785 textgen-0.2.4/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.4/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 14:11:21.675321 textgen-0.2.4/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.4/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-19 14:11:21.676265 textgen-0.2.4/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-19 14:11:02.000000 textgen-0.2.4/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.622178 textgen-0.2.4/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-19 14:11:02.000000 textgen-0.2.4/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.632125 textgen-0.2.4/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.4/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.4/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.4/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.4/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.4/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.4/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.636939 textgen-0.2.4/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.4/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    22085 2023-04-19 14:09:32.000000 textgen-0.2.4/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.4/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.640358 textgen-0.2.4/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.4/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14505 2023-04-19 06:54:54.000000 textgen-0.2.4/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.642195 textgen-0.2.4/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.4/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.645721 textgen-0.2.4/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.4/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.4/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.649093 textgen-0.2.4/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.4/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.4/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.655570 textgen-0.2.4/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.4/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.4/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.4/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.4/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.4/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.659754 textgen-0.2.4/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.4/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    22752 2023-04-19 14:10:06.000000 textgen-0.2.4/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5741 2023-04-18 02:48:12.000000 textgen-0.2.4/textgen/llama/llama_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.666469 textgen-0.2.4/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.4/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.4/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.4/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.4/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.4/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.4/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.4/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.671895 textgen-0.2.4/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.4/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.4/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.4/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.4/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.4/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.673844 textgen-0.2.4/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.4/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.4/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.4/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.625149 textgen-0.2.4/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.2.3/LICENSE` & `textgen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/PKG-INFO` & `textgen-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
```

### Comparing `textgen-0.2.3/README.md` & `textgen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/setup.py` & `textgen-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.2.3',
+    version='0.2.4',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
```

### Comparing `textgen-0.2.3/textgen/__init__.py` & `textgen-0.2.4/textgen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
```

### Comparing `textgen-0.2.3/textgen/augment/sentence_level_augment.py` & `textgen-0.2.4/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/augment/text_augment.py` & `textgen-0.2.4/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/augment/tokenizer.py` & `textgen-0.2.4/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/augment/translate_api.py` & `textgen-0.2.4/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/augment/word_level_augment.py` & `textgen-0.2.4/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/augment/word_vocab.py` & `textgen-0.2.4/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/chatglm/chatglm_model.py` & `textgen-0.2.4/textgen/chatglm/chatglm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,16 +370,19 @@
             keep_prompt: Whether to keep the prompt in the generated text.
             max_length: The maximum length of the generated text.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
+        if self.device == 'cpu':
+            self.model.float()
         if self.args.fp16:
             self.model.half()
+        self.model.to(self.device)
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
```

### Comparing `textgen-0.2.3/textgen/chatglm/chatglm_utils.py` & `textgen-0.2.4/textgen/chatglm/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/config/global_args.py` & `textgen-0.2.4/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/config/model_args.py` & `textgen-0.2.4/textgen/config/model_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/custom_models/models.py` & `textgen-0.2.4/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/data/HowNetPOSWord.txt` & `textgen-0.2.4/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/data/stopwords.txt` & `textgen-0.2.4/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_generation/language_generation_model.py` & `textgen-0.2.4/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_generation/language_generation_utils.py` & `textgen-0.2.4/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_modeling/language_modeling_model.py` & `textgen-0.2.4/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.2.4/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_modeling/songnet_model.py` & `textgen-0.2.4/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/language_modeling/songnet_utils.py` & `textgen-0.2.4/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/llama/llama_model.py` & `textgen-0.2.4/textgen/llama/llama_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,16 @@
             keep_prompt: Whether to keep the prompt in the generated text.
             max_length: The maximum length of the generated text.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
+        if self.device == 'cpu':
+            self.model.float()
         if self.args.fp16:
             self.model.half()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
```

### Comparing `textgen-0.2.3/textgen/llama/llama_utils.py` & `textgen-0.2.4/textgen/llama/llama_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.2.4/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.2.4/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.2.4/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/data_reader.py` & `textgen-0.2.4/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/seq2seq_model.py` & `textgen-0.2.4/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.2.4/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/t5/copyt5_model.py` & `textgen-0.2.4/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/t5/copyt5_utils.py` & `textgen-0.2.4/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/t5/t5_model.py` & `textgen-0.2.4/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/t5/t5_utils.py` & `textgen-0.2.4/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/unsup_generation/tgls_model.py` & `textgen-0.2.4/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen/unsup_generation/tgls_util.py` & `textgen-0.2.4/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.3/textgen.egg-info/PKG-INFO` & `textgen-0.2.4/textgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
```

### Comparing `textgen-0.2.3/textgen.egg-info/SOURCES.txt` & `textgen-0.2.4/textgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

