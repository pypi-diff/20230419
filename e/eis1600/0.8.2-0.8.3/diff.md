# Comparing `tmp/eis1600-0.8.2.tar.gz` & `tmp/eis1600-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.2.tar", last modified: Mon Apr 17 11:47:28 2023, max compression
+gzip compressed data, was "eis1600-0.8.3.tar", last modified: Wed Apr 19 08:15:32 2023, max compression
```

## Comparing `eis1600-0.8.2.tar` & `eis1600-0.8.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.294513 eis1600-0.8.2/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.2/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-17 11:47:28.294513 eis1600-0.8.2/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.2/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.278513 eis1600-0.8.2/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.2/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.282513 eis1600-0.8.2/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.2/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.2/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.2/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.2/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.282513 eis1600-0.8.2/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.2/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.2/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.2/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.282513 eis1600-0.8.2/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.2/eis1600/gazetteers/data/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.286513 eis1600-0.8.2/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.2/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.2/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.2/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.286513 eis1600-0.8.2/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.2/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      374 2023-04-05 10:09:07.000000 eis1600-0.8.2/eis1600/helper/entity_tags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.2/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.2/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.2/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3723 2023-04-14 12:34:00.000000 eis1600-0.8.2/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.2/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-13 08:15:00.000000 eis1600-0.8.2/eis1600/helper/my_json_ecoder.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.2/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-13 08:57:43.000000 eis1600-0.8.2/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.286513 eis1600-0.8.2/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.2/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.2/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.2/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.2/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13026 2023-04-13 10:26:19.000000 eis1600-0.8.2/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.2/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.2/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.290513 eis1600-0.8.2/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.2/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6622 2023-04-14 12:11:46.000000 eis1600-0.8.2/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.2/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.2/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.2/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.2/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6008 2023-04-17 08:45:53.000000 eis1600-0.8.2/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.290513 eis1600-0.8.2/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.2/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.2/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.2/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.2/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.290513 eis1600-0.8.2/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.2/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1201 2023-04-17 07:58:03.000000 eis1600-0.8.2/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10081 2023-04-17 11:47:02.000000 eis1600-0.8.2/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.2/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.290513 eis1600-0.8.2/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.2/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.2/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.2/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.290513 eis1600-0.8.2/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.2/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.2/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.2/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 11:47:28.282513 eis1600-0.8.2/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1749 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       52 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-17 11:47:28.000000 eis1600-0.8.2/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-17 11:47:28.294513 eis1600-0.8.2/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2138 2023-04-17 11:47:18.000000 eis1600-0.8.2/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.592384 eis1600-0.8.3/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.3/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-19 08:15:32.592384 eis1600-0.8.3/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.3/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.580385 eis1600-0.8.3/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.3/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.580385 eis1600-0.8.3/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.3/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.3/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.3/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.3/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.580385 eis1600-0.8.3/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.3/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.3/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.3/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.580385 eis1600-0.8.3/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.3/eis1600/gazetteers/data/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.584385 eis1600-0.8.3/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.3/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.3/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.3/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.584385 eis1600-0.8.3/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.3/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      374 2023-04-05 10:09:07.000000 eis1600-0.8.3/eis1600/helper/entity_tags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.3/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.3/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.3/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3723 2023-04-14 12:34:00.000000 eis1600-0.8.3/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.3/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-13 08:15:00.000000 eis1600-0.8.3/eis1600/helper/my_json_ecoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.3/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-13 08:57:43.000000 eis1600-0.8.3/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.588384 eis1600-0.8.3/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.3/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.3/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.3/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13026 2023-04-13 10:26:19.000000 eis1600-0.8.3/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.3/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.3/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.588384 eis1600-0.8.3/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.3/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6622 2023-04-14 12:11:46.000000 eis1600-0.8.3/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.3/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.3/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.3/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.3/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6008 2023-04-17 08:45:53.000000 eis1600-0.8.3/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.588384 eis1600-0.8.3/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.3/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.3/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.3/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.3/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.592384 eis1600-0.8.3/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.3/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1201 2023-04-17 07:58:03.000000 eis1600-0.8.3/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10081 2023-04-17 11:47:02.000000 eis1600-0.8.3/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.3/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.592384 eis1600-0.8.3/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.3/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.3/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.3/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.592384 eis1600-0.8.3/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.3/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.3/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.3/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:15:32.580385 eis1600-0.8.3/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1749 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       99 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-19 08:15:32.000000 eis1600-0.8.3/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-19 08:15:32.592384 eis1600-0.8.3/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2277 2023-04-19 08:14:49.000000 eis1600-0.8.3/setup.py
```

### Comparing `eis1600-0.8.2/LICENSE` & `eis1600-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/PKG-INFO` & `eis1600-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.2
+Version: 0.8.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.2/README.md` & `eis1600-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/dates/Date.py` & `eis1600-0.8.3/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/dates/date_patterns.py` & `eis1600-0.8.3/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/dates/methods.py` & `eis1600-0.8.3/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/gazetteers/Onomastics.py` & `eis1600-0.8.3/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/gazetteers/Toponyms.py` & `eis1600-0.8.3/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/Singleton.py` & `eis1600-0.8.3/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/ar_normalization.py` & `eis1600-0.8.3/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.8.3/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/markdown_methods.py` & `eis1600-0.8.3/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/markdown_patterns.py` & `eis1600-0.8.3/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/miu_random_revisions.py` & `eis1600-0.8.3/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/repo.py` & `eis1600-0.8.3/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/helper/yml_to_json.py` & `eis1600-0.8.3/eis1600/helper/yml_to_json.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/UIDs.py` & `eis1600-0.8.3/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.8.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/insert_uids.py` & `eis1600-0.8.3/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/methods.py` & `eis1600-0.8.3/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/update_uids.py` & `eis1600-0.8.3/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.8.3/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/HeadingTracker.py` & `eis1600-0.8.3/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/YAMLHandler.py` & `eis1600-0.8.3/eis1600/miu/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.8.3/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/methods.py` & `eis1600-0.8.3/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.8.3/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/miu/yml_handling.py` & `eis1600-0.8.3/eis1600/miu/yml_handling.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/nlp/cameltools.py` & `eis1600-0.8.3/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.8.3/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/nlp/utils.py` & `eis1600-0.8.3/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/onomastics/annotation.py` & `eis1600-0.8.3/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/onomastics/methods.py` & `eis1600-0.8.3/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/onomastics/re_pattern.py` & `eis1600-0.8.3/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/processing/postprocessing.py` & `eis1600-0.8.3/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/processing/preprocessing.py` & `eis1600-0.8.3/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/stats/methods.py` & `eis1600-0.8.3/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600/stats/miu_stats.py` & `eis1600-0.8.3/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600.egg-info/PKG-INFO` & `eis1600-0.8.3/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.2
+Version: 0.8.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.2/eis1600.egg-info/SOURCES.txt` & `eis1600-0.8.3/eis1600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/eis1600.egg-info/entry_points.txt` & `eis1600-0.8.3/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.2/setup.py` & `eis1600-0.8.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.2',
+      version='0.8.3',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
@@ -27,15 +27,22 @@
                   'reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main',
                   'update_uids = eis1600.markdown.update_uids:main',
                   'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main',
                   'yml_to_json = eis1600.helper.yml_to_json:main'
           ],
       },
       python_requires='>=3.7, <3.9',
-      install_requires=['openiti', 'pandas', 'numpy', 'tqdm', 'p_tqdm'],
+      install_requires=[
+              'openiti',
+              'pandas',
+              'numpy',
+              'tqdm',
+              'p_tqdm',
+              'importlib_resources; python_version < "3.8"'
+      ],
       extras_require={'NER': ['camel-tools']},
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent',
                    'Development Status :: 1 - Planning',
                    'Intended Audience :: Science/Research']
       )
```

