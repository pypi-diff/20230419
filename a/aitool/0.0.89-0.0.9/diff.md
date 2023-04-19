# Comparing `tmp/aitool-0.0.89.tar.gz` & `tmp/aitool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitool-0.0.89.tar", last modified: Tue Feb 21 13:24:00 2023, max compression
+gzip compressed data, was "dist/aitool-0.0.9.tar", last modified: Thu Jul 22 09:08:31 2021, max compression
```

## Comparing `aitool-0.0.89.tar` & `aitool-0.0.9.tar`

### file list

```diff
@@ -1,95 +1,31 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.477083 aitool-0.0.89/
--rw-r--r--   0 bytedance   (501) staff       (20)     1084 2020-10-22 11:16:54.000000 aitool-0.0.89/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)     2091 2023-02-21 13:24:00.476922 aitool-0.0.89/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     1612 2022-01-08 14:42:45.000000 aitool-0.0.89/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.463736 aitool-0.0.89/aitool/
--rw-r--r--   0 bytedance   (501) staff       (20)     5542 2023-02-21 13:22:34.000000 aitool-0.0.89/aitool/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.467984 aitool-0.0.89/aitool/basic_function/
--rw-r--r--   0 bytedance   (501) staff       (20)       81 2021-03-10 06:22:12.000000 aitool-0.0.89/aitool/basic_function/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3687 2023-02-15 13:08:54.000000 aitool-0.0.89/aitool/basic_function/basic.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3022 2022-01-04 12:20:56.000000 aitool-0.0.89/aitool/basic_function/cache.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2229 2022-01-20 13:24:39.000000 aitool-0.0.89/aitool/basic_function/deduplication.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.468522 aitool-0.0.89/aitool/basic_function/download/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2021-08-05 12:13:13.000000 aitool-0.0.89/aitool/basic_function/download/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3106 2022-05-19 07:58:54.000000 aitool-0.0.89/aitool/basic_function/download/classtest.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1680 2022-05-19 08:14:59.000000 aitool-0.0.89/aitool/basic_function/download/download.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5670 2020-10-22 15:05:02.000000 aitool-0.0.89/aitool/basic_function/download/utils.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1063 2021-07-23 08:28:19.000000 aitool-0.0.89/aitool/basic_function/exe_time.py
--rw-r--r--   0 bytedance   (501) staff       (20)    16705 2023-02-21 03:44:04.000000 aitool-0.0.89/aitool/basic_function/file.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9376 2023-02-13 07:09:00.000000 aitool-0.0.89/aitool/basic_function/format_data.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11165 2022-01-11 14:07:11.000000 aitool-0.0.89/aitool/basic_function/multi.py
--rw-r--r--   0 bytedance   (501) staff       (20)      770 2022-05-19 07:36:16.000000 aitool-0.0.89/aitool/basic_function/path.py
--rw-r--r--   0 bytedance   (501) staff       (20)      986 2022-05-23 08:36:46.000000 aitool-0.0.89/aitool/basic_function/random.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2466 2021-07-23 09:42:23.000000 aitool-0.0.89/aitool/basic_function/retry.py
--rw-r--r--   0 bytedance   (501) staff       (20)      843 2021-09-29 07:42:59.000000 aitool-0.0.89/aitool/basic_function/security.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1035 2021-08-02 08:56:02.000000 aitool-0.0.89/aitool/basic_function/singleton.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2039 2022-01-20 13:26:31.000000 aitool-0.0.89/aitool/basic_function/string.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4358 2022-01-10 12:11:55.000000 aitool-0.0.89/aitool/basic_function/time.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3615 2021-07-23 08:34:21.000000 aitool-0.0.89/aitool/basic_function/tmp.py
--rw-r--r--   0 bytedance   (501) staff       (20)      109 2023-02-21 12:49:59.000000 aitool-0.0.89/aitool/basic_function/tmp10.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1068 2021-08-06 12:17:58.000000 aitool-0.0.89/aitool/basic_function/tmp2.py
--rw-r--r--   0 bytedance   (501) staff       (20)      866 2021-10-27 06:16:38.000000 aitool-0.0.89/aitool/basic_function/tmp3.py
--rw-r--r--   0 bytedance   (501) staff       (20)      985 2022-01-04 11:05:46.000000 aitool-0.0.89/aitool/basic_function/tmp4.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6055 2022-01-07 15:55:11.000000 aitool-0.0.89/aitool/basic_function/tmp5.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1088 2022-01-07 11:08:27.000000 aitool-0.0.89/aitool/basic_function/tmp6.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2212 2022-01-07 15:48:04.000000 aitool-0.0.89/aitool/basic_function/tmp7.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2999 2022-01-08 15:21:07.000000 aitool-0.0.89/aitool/basic_function/tmp8.py
--rw-r--r--   0 bytedance   (501) staff       (20)      352 2022-01-08 16:04:16.000000 aitool-0.0.89/aitool/basic_function/tmp9.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1665 2022-02-28 09:34:54.000000 aitool-0.0.89/aitool/basic_function/word.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.468758 aitool-0.0.89/aitool/basic_function/words/
--rw-r--r--   0 bytedance   (501) staff       (20)      751 2022-02-28 09:20:28.000000 aitool-0.0.89/aitool/basic_function/words/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9348 2022-02-28 09:27:33.000000 aitool-0.0.89/aitool/basic_function/words/morTrans.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.468909 aitool-0.0.89/aitool/data_structure/
--rw-r--r--   0 bytedance   (501) staff       (20)       79 2020-10-26 07:20:05.000000 aitool-0.0.89/aitool/data_structure/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.469418 aitool-0.0.89/aitool/data_structure/graph/
--rw-r--r--   0 bytedance   (501) staff       (20)       79 2020-10-26 07:20:46.000000 aitool-0.0.89/aitool/data_structure/graph/__init__.py
--rw-rw-rw-   0 bytedance   (501) staff       (20)    10586 2020-11-16 12:36:51.000000 aitool-0.0.89/aitool/data_structure/graph/chain_forward_stars.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.473919 aitool-0.0.89/aitool/datasets/
--rw-r--r--   0 bytedance   (501) staff       (20)      123 2021-08-05 07:43:14.000000 aitool-0.0.89/aitool/datasets/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1856 2023-02-15 12:51:53.000000 aitool-0.0.89/aitool/datasets/deny.txt
--rw-r--r--   0 bytedance   (501) staff       (20)  5673839 2023-02-15 17:52:08.000000 aitool-0.0.89/aitool/datasets/keyword.pkl
--rw-r--r--   0 bytedance   (501) staff       (20)   136533 2015-12-28 02:19:04.000000 aitool-0.0.89/aitool/datasets/negative.txt
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.474074 aitool-0.0.89/aitool/datasets/nlp/
--rw-r--r--   0 bytedance   (501) staff       (20)       79 2020-10-22 11:26:54.000000 aitool-0.0.89/aitool/datasets/nlp/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    77415 2015-12-28 02:19:04.000000 aitool-0.0.89/aitool/datasets/positive.txt
--rw-r--r--   0 bytedance   (501) staff       (20)    23257 2023-02-20 03:51:42.000000 aitool-0.0.89/aitool/datasets/stopwords.txt
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.474204 aitool-0.0.89/aitool/nlp/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2021-09-14 03:58:57.000000 aitool-0.0.89/aitool/nlp/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.474564 aitool-0.0.89/aitool/nlp/basic/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2021-09-14 03:59:04.000000 aitool-0.0.89/aitool/nlp/basic/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2033 2022-01-20 13:15:41.000000 aitool-0.0.89/aitool/nlp/basic/conditional_probability.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2456 2021-09-28 13:15:39.000000 aitool-0.0.89/aitool/nlp/basic/split_sentence.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.474966 aitool-0.0.89/aitool/nlp/sentiment_analysis/
--rw-r--r--   0 bytedance   (501) staff       (20)      695 2023-02-13 03:40:33.000000 aitool-0.0.89/aitool/nlp/sentiment_analysis/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1184 2023-02-13 06:50:39.000000 aitool-0.0.89/aitool/nlp/sentiment_analysis/dict_match.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1484 2023-02-13 03:58:49.000000 aitool-0.0.89/aitool/nlp/sentiment_analysis/use_snownlp.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.475085 aitool-0.0.89/aitool/nlp/string_matching/
--rw-r--r--   0 bytedance   (501) staff       (20)      751 2021-11-22 04:20:00.000000 aitool-0.0.89/aitool/nlp/string_matching/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.475374 aitool-0.0.89/aitool/nlp/string_matching/ac_automation/
--rw-r--r--   0 bytedance   (501) staff       (20)      751 2021-11-22 04:29:09.000000 aitool-0.0.89/aitool/nlp/string_matching/ac_automation/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4345 2021-11-22 04:39:25.000000 aitool-0.0.89/aitool/nlp/string_matching/ac_automation/ac_automation.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.475495 aitool-0.0.89/aitool/nlp/string_recall/
--rw-r--r--   0 bytedance   (501) staff       (20)      751 2021-11-22 04:20:00.000000 aitool-0.0.89/aitool/nlp/string_recall/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.476101 aitool-0.0.89/aitool/nlp/string_recall/bktree/
--rw-r--r--   0 bytedance   (501) staff       (20)      751 2021-11-22 04:20:00.000000 aitool-0.0.89/aitool/nlp/string_recall/bktree/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2130 2021-03-10 04:24:22.000000 aitool-0.0.89/aitool/nlp/string_recall/bktree/bktree-wenri.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4159 2022-03-31 11:17:32.000000 aitool-0.0.89/aitool/nlp/string_recall/bktree/bktree.py
--rw-r--r--   0 bytedance   (501) staff       (20)      302 2021-04-22 03:16:55.000000 aitool-0.0.89/aitool/nlp/string_recall/bktree/cppbktree.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6416 2021-04-09 03:11:00.000000 aitool-0.0.89/aitool/nlp/string_recall/bktree/evaluation.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.476220 aitool-0.0.89/aitool/task_customized/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2021-07-26 12:30:52.000000 aitool-0.0.89/aitool/task_customized/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.476450 aitool-0.0.89/aitool/task_customized/ip_enhance/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2021-07-26 12:31:04.000000 aitool-0.0.89/aitool/task_customized/ip_enhance/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11256 2023-02-20 12:08:50.000000 aitool-0.0.89/aitool/task_customized/ip_enhance/filter.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.476701 aitool-0.0.89/aitool/task_customized/keyword_mining/
--rw-r--r--   0 bytedance   (501) staff       (20)      688 2023-02-10 08:13:44.000000 aitool-0.0.89/aitool/task_customized/keyword_mining/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15223 2023-02-21 13:22:40.000000 aitool-0.0.89/aitool/task_customized/keyword_mining/keyword.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1021 2022-05-23 08:32:39.000000 aitool-0.0.89/aitool/tmp.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-02-21 13:24:00.464376 aitool-0.0.89/aitool.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)     2091 2023-02-21 13:24:00.000000 aitool-0.0.89/aitool.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     2503 2023-02-21 13:24:00.000000 aitool-0.0.89/aitool.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-02-21 13:24:00.000000 aitool-0.0.89/aitool.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)      270 2023-02-21 13:24:00.000000 aitool-0.0.89/aitool.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        7 2023-02-21 13:24:00.000000 aitool-0.0.89/aitool.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-02-21 13:24:00.477136 aitool-0.0.89/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1362 2023-02-20 03:34:14.000000 aitool-0.0.89/setup.py
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/
+-rw-r--r--   0 apricot    (501) staff       (20)     2175 2021-07-22 09:08:31.000000 aitool-0.0.9/PKG-INFO
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/data_structure/
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/data_structure/graph/
+-rw-r--r--   0 apricot    (501) staff       (20)       79 2020-10-26 07:20:46.000000 aitool-0.0.9/aitool/data_structure/graph/__init__.py
+-rw-rw-rw-   0 apricot    (501) staff       (20)    10586 2020-11-16 12:36:51.000000 aitool-0.0.9/aitool/data_structure/graph/chain_forward_stars.py
+-rw-r--r--   0 apricot    (501) staff       (20)       79 2020-10-26 07:20:05.000000 aitool-0.0.9/aitool/data_structure/__init__.py
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/datasets/
+-rw-r--r--   0 apricot    (501) staff       (20)       79 2020-10-22 11:26:53.000000 aitool-0.0.9/aitool/datasets/__init__.py
+-rw-r--r--   0 apricot    (501) staff       (20)     5670 2020-10-22 15:05:02.000000 aitool-0.0.9/aitool/datasets/utils.py
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/datasets/nlp/
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/datasets/nlp/classification/
+-rw-r--r--   0 apricot    (501) staff       (20)      114 2020-10-23 08:16:20.000000 aitool-0.0.9/aitool/datasets/nlp/classification/__init__.py
+-rw-r--r--   0 apricot    (501) staff       (20)     3149 2020-10-23 08:40:58.000000 aitool-0.0.9/aitool/datasets/nlp/classification/classtest.py
+-rw-r--r--   0 apricot    (501) staff       (20)       79 2020-10-22 11:26:54.000000 aitool-0.0.9/aitool/datasets/nlp/__init__.py
+-rw-r--r--   0 apricot    (501) staff       (20)      875 2021-07-22 09:04:24.000000 aitool-0.0.9/aitool/__init__.py
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool/basic_function/
+-rw-r--r--   0 apricot    (501) staff       (20)     1721 2021-07-22 09:02:37.000000 aitool-0.0.9/aitool/basic_function/file_function.py
+-rw-r--r--   0 apricot    (501) staff       (20)       81 2021-03-10 06:22:12.000000 aitool-0.0.9/aitool/basic_function/__init__.py
+-rw-r--r--   0 apricot    (501) staff       (20)      841 2021-07-05 10:05:43.000000 aitool-0.0.9/aitool/basic_function/singleton.py
+-rw-r--r--   0 apricot    (501) staff       (20)     1061 2021-03-10 07:53:24.000000 aitool-0.0.9/aitool/basic_function/time_function.py
+-rw-r--r--   0 apricot    (501) staff       (20)     1412 2020-10-28 15:58:01.000000 aitool-0.0.9/README.md
+-rw-r--r--   0 apricot    (501) staff       (20)     1237 2021-07-05 06:43:08.000000 aitool-0.0.9/setup.py
+drwxr-xr-x   0 apricot    (501) staff       (20)        0 2021-07-22 09:08:31.000000 aitool-0.0.9/aitool.egg-info/
+-rw-r--r--   0 apricot    (501) staff       (20)     2175 2021-07-22 09:08:30.000000 aitool-0.0.9/aitool.egg-info/PKG-INFO
+-rw-r--r--   0 apricot    (501) staff       (20)      638 2021-07-22 09:08:30.000000 aitool-0.0.9/aitool.egg-info/SOURCES.txt
+-rw-r--r--   0 apricot    (501) staff       (20)       37 2021-07-22 09:08:30.000000 aitool-0.0.9/aitool.egg-info/requires.txt
+-rw-r--r--   0 apricot    (501) staff       (20)        7 2021-07-22 09:08:30.000000 aitool-0.0.9/aitool.egg-info/top_level.txt
+-rw-r--r--   0 apricot    (501) staff       (20)        1 2021-07-22 09:08:30.000000 aitool-0.0.9/aitool.egg-info/dependency_links.txt
+-rw-r--r--   0 apricot    (501) staff       (20)       38 2021-07-22 09:08:31.000000 aitool-0.0.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aitool-0.0.89/PKG-INFO` & `aitool-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,52 @@
 Metadata-Version: 2.1
 Name: aitool
-Version: 0.0.89
+Version: 0.0.9
 Summary: Summarize the algorithms and data of nlp
 Home-page: https://github.com/deepgameai/aitool.git
 Author: xiangyuejia
 Author-email: xiangyuejia@qq.com
 License: UNKNOWN
+Description: [![AITool logo](https://raw.githubusercontent.com/deepgameai/aitool/main/docs/logo/logo.png)](https://deepgameai.github.io/2020-02-28-test-markdown/)
+        
+        --------------------------------------------------------------------------------
+        
+        [![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/)
+        [![stars](https://img.shields.io/github/stars/deepgameai/aitool?style=social)]()
+        
+        AITool is a Python package that provides two high-level features:
+        - 封装了有百种算法（包括动态规划、统计模型、深度学习等等）
+        - 每种算法都自带数据，便于验证和使用
+        - Encapsulates hundreds of algorithms. (Including dynamic programming, statistical models, deep learning, etc.)
+        - Each algorithm comes with its own data for easy verification and use.
+        
+        aitool - 
+        [官方主页](https://deepgameai.github.io/2020-02-28-test-markdown/) - 
+        [文档](https://aitool20201028.readthedocs.io/en/latest/)
+        
+        - [Motivation](#motivation)
+        - [Installation](#installation)
+        - [Getting Started](#getting-started)
+        - [Communication](#communication)
+        - [Releases and Contributing](#releases-and-contributing)
+        - [The Team](#the-team)
+        
+        ## Motivation
+        
+        ## Installation
+        
+        ## Getting Started
+        
+        ## Communication
+        
+        ## Releases and Contributing
+        
+        ## The Team
+        
+        ## 授权许可
+        本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![AITool logo](https://raw.githubusercontent.com/deepgameai/aitool/main/docs/logo/logo.png)](https://deepgameai.github.io/2020-02-28-test-markdown/)
-
---------------------------------------------------------------------------------
-
-[![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/).
-[![stars](https://img.shields.io/github/stars/deepgameai/aitool?style=social)]()
-
-AITool 工具致力于提高开发效率
-> 待完善，预计2022年6月完成1.0版本
-
-AITool is a Python package that provides:
-- 百种工具函数（数据处理、多进程、计时器等）
-- 百种算法（包括动态规划、统计模型、深度学习等等）
-- 每种算法都自带数据，便于验证和使用。
-- Encapsulates hundreds of algorithms. (Including dynamic programming, statistical models, deep learning, etc.)
-- Each algorithm comes with its own data for easy verification and use
-
-aitool - 
-[官方主页](https://deepgameai.github.io/2020-02-28-test-markdown/) - 
-[文档](https://aitool20201028.readthedocs.io/en/latest/)
-
-- [Motivation](#motivation)
-- [Installation](#installation)
-- [Getting Started](#getting-started)
-- [Communication](#communication)
-- [Releases and Contributing](#releases-and-contributing)
-- [The Team](#the-team)
-
-## Motivation
-
-## Installation
-```shell script
-pip install aitool --upgrade
-```
-
-
-## Getting Started
-```shell script
-# Todo
-```
-
-## Communication
-
-## Releases and Contributing
-
-## The Team
-
-## 授权许可
-本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
-
-
```

### Comparing `aitool-0.0.89/README.md` & `aitool-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 [![AITool logo](https://raw.githubusercontent.com/deepgameai/aitool/main/docs/logo/logo.png)](https://deepgameai.github.io/2020-02-28-test-markdown/)
 
 --------------------------------------------------------------------------------
 
-[![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/).
+[![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/)
 [![stars](https://img.shields.io/github/stars/deepgameai/aitool?style=social)]()
 
-AITool 工具致力于提高开发效率
-> 待完善，预计2022年6月完成1.0版本
-
-AITool is a Python package that provides:
-- 百种工具函数（数据处理、多进程、计时器等）
-- 百种算法（包括动态规划、统计模型、深度学习等等）
-- 每种算法都自带数据，便于验证和使用。
+AITool is a Python package that provides two high-level features:
+- 封装了有百种算法（包括动态规划、统计模型、深度学习等等）
+- 每种算法都自带数据，便于验证和使用
 - Encapsulates hundreds of algorithms. (Including dynamic programming, statistical models, deep learning, etc.)
-- Each algorithm comes with its own data for easy verification and use
+- Each algorithm comes with its own data for easy verification and use.
 
 aitool - 
 [官方主页](https://deepgameai.github.io/2020-02-28-test-markdown/) - 
 [文档](https://aitool20201028.readthedocs.io/en/latest/)
 
 - [Motivation](#motivation)
 - [Installation](#installation)
@@ -25,25 +21,18 @@
 - [Communication](#communication)
 - [Releases and Contributing](#releases-and-contributing)
 - [The Team](#the-team)
 
 ## Motivation
 
 ## Installation
-```shell script
-pip install aitool --upgrade
-```
-
 
 ## Getting Started
-```shell script
-# Todo
-```
 
 ## Communication
 
 ## Releases and Contributing
 
 ## The Team
 
 ## 授权许可
-本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
+本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
```

### Comparing `aitool-0.0.89/aitool/basic_function/download/__init__.py` & `aitool-0.0.9/aitool/basic_function/singleton.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,10 +9,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-
+A decorator to make single class
 """
-from typing import Dict, Union, List, Any, NoReturn
+
+
+def singleton(cls):
+    _instance = {}
+
+    def inner():
+        if cls not in _instance:
+            _instance[cls] = cls()
+        return _instance[cls]
+    return inner
```

### Comparing `aitool-0.0.89/aitool/basic_function/download/classtest.py` & `aitool-0.0.9/aitool/datasets/nlp/classification/classtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: UTF-8 -*-
 # @Time    : 2020/10/22
 # @Author  : xiangyuejia@qq.com
-from typing import Any, Tuple
+import os
+import aitool.datasets.utils
+from typing import Any, Callable, Optional, Tuple
 
-from aitool.basic_function.download.utils import check_integrity, download_and_extract_archive
+from aitool.datasets.utils import check_integrity, download_and_extract_archive
 
 
 class ClassTest1:
     base_folder = 'cifar-10-batches-py'
     url = 'https://raw.githubusercontent.com/deepgameai/datasets/main/NLP/classifier/test.txt'
     filename = 'test.txt'
     tgz_md5 = '749b1843d4c4be33afc4ba7f1158fc33'
@@ -87,13 +89,12 @@
             print('Files already downloaded and verified')
             return
         download_and_extract_archive(self.url, self.root, filename=self.filename, md5=self.tgz_md5)
 
     def extra_repr(self) -> str:
         return "Split: {}".format("Train" if self.train is True else "Test")
 
-
 if __name__ == '__main__':
     import os
     os.environ["HTTPS_PROXY"] = "http://127.0.0.1:12639"
     data = ClassTest1('.', train=True, download=True)
     ccc = 1
```

### Comparing `aitool-0.0.89/aitool/basic_function/download/utils.py` & `aitool-0.0.9/aitool/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `aitool-0.0.89/aitool/basic_function/exe_time.py` & `aitool-0.0.9/aitool/basic_function/time_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: UTF-8 -*-
 # @Time    : 2021/3/10
 # @Author  : xiangyuejia@qq.com
 # Apache License
 # Copyright©2020-2021 xiangyuejia@qq.com All Rights Reserved
 import time
 
-
 def exe_time(print_time=False, detail=False):
     def wrapper(func):
         def decorate(*args, **kw):
             t0 = time.time()
             if detail:
                 print("@%s, {%s} start" % (time.strftime("%X", time.localtime()), func.__name__))
             back = func(*args, **kw)
@@ -17,15 +16,14 @@
                 print("@%s, {%s} finish" % (time.strftime("%X", time.localtime()), func.__name__))
             if print_time:
                 print("@%.3fs taken for {%s}" % (time.time() - t0, func.__name__))
             return back
         return decorate
     return wrapper
 
-
 if __name__ == '__main__':
     @exe_time()
     def test1():
         print('i am from england')
 
 
     @exe_time(print_time=True)
```

### Comparing `aitool-0.0.89/aitool/data_structure/graph/chain_forward_stars.py` & `aitool-0.0.9/aitool/data_structure/graph/chain_forward_stars.py`

 * *Files identical despite different names*

### Comparing `aitool-0.0.89/aitool.egg-info/PKG-INFO` & `aitool-0.0.9/aitool.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,52 @@
 Metadata-Version: 2.1
 Name: aitool
-Version: 0.0.89
+Version: 0.0.9
 Summary: Summarize the algorithms and data of nlp
 Home-page: https://github.com/deepgameai/aitool.git
 Author: xiangyuejia
 Author-email: xiangyuejia@qq.com
 License: UNKNOWN
+Description: [![AITool logo](https://raw.githubusercontent.com/deepgameai/aitool/main/docs/logo/logo.png)](https://deepgameai.github.io/2020-02-28-test-markdown/)
+        
+        --------------------------------------------------------------------------------
+        
+        [![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/)
+        [![stars](https://img.shields.io/github/stars/deepgameai/aitool?style=social)]()
+        
+        AITool is a Python package that provides two high-level features:
+        - 封装了有百种算法（包括动态规划、统计模型、深度学习等等）
+        - 每种算法都自带数据，便于验证和使用
+        - Encapsulates hundreds of algorithms. (Including dynamic programming, statistical models, deep learning, etc.)
+        - Each algorithm comes with its own data for easy verification and use.
+        
+        aitool - 
+        [官方主页](https://deepgameai.github.io/2020-02-28-test-markdown/) - 
+        [文档](https://aitool20201028.readthedocs.io/en/latest/)
+        
+        - [Motivation](#motivation)
+        - [Installation](#installation)
+        - [Getting Started](#getting-started)
+        - [Communication](#communication)
+        - [Releases and Contributing](#releases-and-contributing)
+        - [The Team](#the-team)
+        
+        ## Motivation
+        
+        ## Installation
+        
+        ## Getting Started
+        
+        ## Communication
+        
+        ## Releases and Contributing
+        
+        ## The Team
+        
+        ## 授权许可
+        本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![AITool logo](https://raw.githubusercontent.com/deepgameai/aitool/main/docs/logo/logo.png)](https://deepgameai.github.io/2020-02-28-test-markdown/)
-
---------------------------------------------------------------------------------
-
-[![version](https://badgen.net/badge/version/0.0.1/blue)](https://aitool20201028.readthedocs.io/en/latest/).
-[![stars](https://img.shields.io/github/stars/deepgameai/aitool?style=social)]()
-
-AITool 工具致力于提高开发效率
-> 待完善，预计2022年6月完成1.0版本
-
-AITool is a Python package that provides:
-- 百种工具函数（数据处理、多进程、计时器等）
-- 百种算法（包括动态规划、统计模型、深度学习等等）
-- 每种算法都自带数据，便于验证和使用。
-- Encapsulates hundreds of algorithms. (Including dynamic programming, statistical models, deep learning, etc.)
-- Each algorithm comes with its own data for easy verification and use
-
-aitool - 
-[官方主页](https://deepgameai.github.io/2020-02-28-test-markdown/) - 
-[文档](https://aitool20201028.readthedocs.io/en/latest/)
-
-- [Motivation](#motivation)
-- [Installation](#installation)
-- [Getting Started](#getting-started)
-- [Communication](#communication)
-- [Releases and Contributing](#releases-and-contributing)
-- [The Team](#the-team)
-
-## Motivation
-
-## Installation
-```shell script
-pip install aitool --upgrade
-```
-
-
-## Getting Started
-```shell script
-# Todo
-```
-
-## Communication
-
-## Releases and Contributing
-
-## The Team
-
-## 授权许可
-本项目采用 MIT 开源授权许可证，完整的授权说明已放置在 [LICENSE](LICENSE) 文件中。
-
-
```

### Comparing `aitool-0.0.89/setup.py` & `aitool-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,17 +28,14 @@
   author='xiangyuejia',
   author_email='xiangyuejia@qq.com',
   description='Summarize the algorithms and data of nlp',
   long_description=LONG_DESCRIPTION,
   long_description_content_type='text/markdown',
   url='https://github.com/deepgameai/aitool.git',
   packages=find_packages(),
-  package_data={
-      'aitool.datasets': ['stopwords.txt', 'negative.txt', 'positive.txt', 'keyword.pkl', 'deny.txt'],
-  },
   classifiers=[
       'Programming Language :: Python :: 3',
       'License :: OSI Approved :: MIT License',
       'Operating System :: OS Independent',
   ],
   install_requires=[] + INSTALL_REQUIRES,
   python_requires='>=3.6, <4',
```

