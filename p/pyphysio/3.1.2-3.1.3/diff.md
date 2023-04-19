# Comparing `tmp/pyphysio-3.1.2.tar.gz` & `tmp/pyphysio-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphysio-3.1.2.tar", last modified: Wed Apr  5 14:37:18 2023, max compression
+gzip compressed data, was "pyphysio-3.1.3.tar", last modified: Wed Apr 19 12:20:22 2023, max compression
```

## Comparing `pyphysio-3.1.2.tar` & `pyphysio-3.1.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.704673 pyphysio-3.1.2/
--rwx------   0 bizzego   (1000) bizzego   (1000)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.2/LICENSE
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      879 2023-04-05 14:37:18.700673 pyphysio-3.1.2/PKG-INFO
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.2/README.md
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.692673 pyphysio-3.1.2/pyphysio/
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.2/pyphysio/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    12620 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/_base_algorithm.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/artefacts.py
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.2/pyphysio/filters.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.692673 pyphysio-3.1.2/pyphysio/generators/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/generators/__init__.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/indicators/
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.2/pyphysio/indicators/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/indicators/frequencydomain.py
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/indicators/nonlinear.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    13240 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/indicators/peaks.py
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/indicators/timedomain.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     7554 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/interactive.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/loaders/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/loaders/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/loaders/_load_nirx.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    13169 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/segmenters.py
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)    17230 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/signal.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.688673 pyphysio-3.1.2/pyphysio/specialized/
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/activity/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/activity/_presets.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/eda/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     6862 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/specialized/eda/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.2/pyphysio/specialized/eda/_presets.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/eeg/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/eeg/_presets.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/emg/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/emg/_presets.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/fnirs/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/fnirs/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/fnirs/_convert.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/fnirs/_data.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.2/pyphysio/specialized/fnirs/_dl_sqi.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.696673 pyphysio-3.1.2/pyphysio/specialized/heart/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    27262 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/specialized/heart/__init__.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/specialized/heart/_presets.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.700673 pyphysio-3.1.2/pyphysio/specialized/resp/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.2/pyphysio/specialized/resp/_presets.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.2/pyphysio/sqi.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.700673 pyphysio-3.1.2/pyphysio/test_data/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.2/pyphysio/test_data/info_medical
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.2/pyphysio/test_data/medical.txt.bz2
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)    33962 2023-04-05 14:15:40.000000 pyphysio-3.1.2/pyphysio/utils.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.692673 pyphysio-3.1.2/pyphysio.egg-info/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      879 2023-04-05 14:37:18.000000 pyphysio-3.1.2/pyphysio.egg-info/PKG-INFO
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1355 2023-04-05 14:37:18.000000 pyphysio-3.1.2/pyphysio.egg-info/SOURCES.txt
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)        1 2023-04-05 14:37:18.000000 pyphysio-3.1.2/pyphysio.egg-info/dependency_links.txt
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)       54 2023-04-05 14:37:18.000000 pyphysio-3.1.2/pyphysio.egg-info/requires.txt
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)        9 2023-04-05 14:37:18.000000 pyphysio-3.1.2/pyphysio.egg-info/top_level.txt
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)       38 2023-04-05 14:37:18.704673 pyphysio-3.1.2/setup.cfg
--rwxrwxr-x   0 bizzego   (1000) bizzego   (1000)     2290 2023-04-05 14:36:15.000000 pyphysio-3.1.2/setup.py
-drwxrwxr-x   0 bizzego   (1000) bizzego   (1000)        0 2023-04-05 14:37:18.700673 pyphysio-3.1.2/tests/
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     7896 2023-04-05 14:15:40.000000 pyphysio-3.1.2/tests/test_eda_methods.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_filters.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_fnirs.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_get_sampling_freq.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      520 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_ibi_estimators.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.2/tests/test_segmenters.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_signal.py
--rw-rw-r--   0 bizzego   (1000) bizzego   (1000)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.2/tests/test_tools.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.3/LICENSE
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-04-19 12:20:22.884463 pyphysio-3.1.3/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.3/README.md
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.876463 pyphysio-3.1.3/pyphysio/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    12620 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/_base_algorithm.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/artefacts.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.3/pyphysio/filters.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/generators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/generators/__init__.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/indicators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.3/pyphysio/indicators/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/indicators/frequencydomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/indicators/nonlinear.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    17342 2023-04-14 08:49:08.000000 pyphysio-3.1.3/pyphysio/indicators/peaks.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/indicators/timedomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     7580 2023-04-19 07:35:54.000000 pyphysio-3.1.3/pyphysio/interactive.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/loaders/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/loaders/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/loaders/_load_nirx.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    13169 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    17232 2023-04-06 12:32:55.000000 pyphysio-3.1.3/pyphysio/signal.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.876463 pyphysio-3.1.3/pyphysio/specialized/
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/activity/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/activity/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/eda/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     6887 2023-04-13 12:45:40.000000 pyphysio-3.1.3/pyphysio/specialized/eda/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/specialized/eda/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/eeg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/eeg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/emg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/emg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/fnirs/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_convert.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_data.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_dl_sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/heart/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    27262 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/specialized/heart/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/specialized/heart/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/resp/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.3/pyphysio/specialized/resp/_presets.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.3/pyphysio/sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/pyphysio/test_data/
+-rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/test_data/info_medical
+-rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/test_data/medical.txt.bz2
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34172 2023-04-13 12:44:09.000000 pyphysio-3.1.3/pyphysio/utils.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio.egg-info/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1355 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/SOURCES.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/dependency_links.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)       54 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/requires.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/top_level.txt
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-04-19 12:20:22.884463 pyphysio-3.1.3/setup.cfg
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2290 2023-04-19 12:18:04.000000 pyphysio-3.1.3/setup.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/tests/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8337 2023-04-13 12:55:10.000000 pyphysio-3.1.3/tests/test_eda_methods.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_filters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_fnirs.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_get_sampling_freq.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.3/tests/test_ibi_estimators.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.3/tests/test_segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_signal.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_tools.py
```

### Comparing `pyphysio-3.1.2/LICENSE` & `pyphysio-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/PKG-INFO` & `pyphysio-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.2/README.md` & `pyphysio-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/__init__.py` & `pyphysio-3.1.3/pyphysio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/_base_algorithm.py` & `pyphysio-3.1.3/pyphysio/_base_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/artefacts.py` & `pyphysio-3.1.3/pyphysio/artefacts.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/filters.py` & `pyphysio-3.1.3/pyphysio/filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/generators/__init__.py` & `pyphysio-3.1.3/pyphysio/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/indicators/frequencydomain.py` & `pyphysio-3.1.3/pyphysio/indicators/frequencydomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/indicators/nonlinear.py` & `pyphysio-3.1.3/pyphysio/indicators/nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/indicators/peaks.py` & `pyphysio-3.1.3/pyphysio/indicators/peaks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # coding=utf-8
 # from __future__ import division
 # 
 # from abc import abstractmethod as _abstract, ABCMeta as _ABCMeta
 
 import numpy as _np
+import xarray as _xr
 from .._base_algorithm import _Algorithm
 from ..utils import PeakDetection as _PeakDetection,\
-    PeakSelection as _Algorithmelection, Durations as _Durations,\
-    Slopes as _Slopes
+    PeakSelection as _PeakSelection
 
 # __author__ = 'AleB'
 
+#TODO: create just one function for duration and slopes
 
 class PeaksMax(_Algorithm):
     """
     Return the maximum amplitude of detected peaks.
 
     Parameters
     ----------
-    delta : float, >0
-        Minimum amplitude of peaks to be selected
+    peaks : numpy array
+        values of the result of PeakSelection
+        
     
     Returns
     -------
     mx : float
         Maximum amplitude of detected peaks
     
     """
     def __init__(self, delta, **kwargs):
-        assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         _Algorithm.__init__(self, delta=delta, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
         params = self._params
-        
         delta = params['delta']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-
-        if len(idx_maxs) == 0:
-            print("No peak found")
-            return _np.nan
-        else:
-            return _np.nanmax(val_maxs)
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        signal_values = signal.p.get_values()
+        
+        if len(idx_peaks) == 0:
+            out = _np.nan * _np.max(signal_values, keepdims=True)
+            return out
+            
+        return _np.max(signal_values[idx_peaks], keepdims=True)
 
 
 class PeaksMin(_Algorithm):
     """
     Return the minimum amplitude of detected peaks.
 
     Parameters
@@ -57,28 +60,30 @@
     Returns
     -------
     mn : float
         Minimum amplitude of detected peaks
     
     """
     def __init__(self, delta, **kwargs):
-        assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         _Algorithm.__init__(self, delta=delta, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
         params = self._params
         delta = params['delta']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-
-        if len(idx_maxs) == 0:
-            print("No peak found, returning numpy.nan")
-            return _np.nan
-        else:
-            return _np.nanmin(val_maxs)
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        signal_values = signal.p.get_values()
+        
+        if len(idx_peaks) == 0:
+            out = _np.nan * _np.min(signal_values, keepdims=True)
+            return out
+            
+        return _np.min(signal_values[idx_peaks], keepdims=True)
 
 
 class PeaksMean(_Algorithm):
     """
     Return the average amplitude of detected peaks.
 
     Parameters
@@ -89,28 +94,31 @@
     Returns
     -------
     av : float
         Average amplitude of detected peaks
     
     """
     def __init__(self, delta, **kwargs):
-        assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         _Algorithm.__init__(self, delta=delta, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
         params = self._params
+        
         delta = params['delta']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-
-        if len(idx_maxs) == 0:
-            print("No peak found")
-            return _np.nan
-        else:
-            return _np.nanmean(val_maxs)
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        signal_values = signal.p.get_values()
+        
+        if len(idx_peaks) == 0:
+            out = _np.nan * _np.mean(signal_values, keepdims=True)
+            return out
+            
+        return _np.mean(signal_values[idx_peaks], keepdims=True)
 
 
 class PeaksNum(_Algorithm):
     """
     Return the number of detected peaks.
 
     Parameters
@@ -121,28 +129,24 @@
     Returns
     -------
     n : float
         Number of detected peaks
     
     """
     def __init__(self, delta, **kwargs):
-        assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         _Algorithm.__init__(self, delta=delta, **kwargs)
-
+        self.dimensions = {'time' : 1}
+    
     def algorithm(self, signal):
         params = self._params
         delta = params['delta']
-        
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        return _np.array([len(idx_peaks)])
 
-        if len(idx_maxs) == 0:
-            print("No peak found")
-            return _np.nan
-        else:
-            return len(idx_maxs)
 
 class DurationMin(_Algorithm):
     """
     Return the minimum duration of detected peaks.
 
     Parameters
     ----------
@@ -155,39 +159,55 @@
         
     Returns
     -------
     mn : float
         Minimum duration of detected peaks
     
     """
-    def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
-        assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
+    def __init__(self, delta, win_pre, win_post, **kwargs):
+        assert delta > 0, 'delta must be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
-
+        self.dimensions = {'time' : 1}
+        
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        
+        durations = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            durations.append((i_sp - i_st)/fsamp)
+        
+        return(_np.array([_np.min(durations)]))
+        
 
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            durations = _Durations(starts=idxs_start, stops=idxs_stop)(signal)
-            return _np.nanmin(_np.array(durations))
+        
 
 
 class DurationMax(_Algorithm):
     """
     Return the maximum duration of detected peaks.
 
     Parameters
@@ -201,40 +221,52 @@
         
     Returns
     -------
     mx : float
         Maximum duration of detected peaks
     
     """
-    def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
+    def __init__(self, delta, win_pre, win_post, **kwargs):
         assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
-
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            durations = _Durations(starts=idxs_start, stops=idxs_stop)(signal)
-            return _np.nanmax(_np.array(durations))
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        
+        durations = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            durations.append((i_sp - i_st)/fsamp)
+        
+        return(_np.array([_np.max(durations)]))
 
 
 class DurationMean(_Algorithm):
     """
     Return the average duration of detected peaks.
 
     Parameters
@@ -253,34 +285,47 @@
     
     """
     def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
         assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            durations = _Durations(starts=idxs_start, stops=idxs_stop)(signal)
-            return _np.nanmean(_np.array(durations))
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        
+        durations = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            durations.append((i_sp - i_st)/fsamp)
+        
+        return(_np.array([_np.mean(durations)]))
 
 
 class SlopeMin(_Algorithm):
     """
     Return the minimum slope of detected peaks.
 
     Parameters
@@ -294,39 +339,54 @@
         
     Returns
     -------
     mn : float
         Minimum slope of detected peaks
     
     """
-    def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
+    def __init__(self, delta, win_pre, win_post, **kwargs):
         assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-        
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            slopes = _Slopes(starts=idxs_start, peaks=idx_maxs)(signal)
-            return _np.nanmin(_np.array(slopes))
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        signal_values = signal.p.get_values().ravel()
+        slopes = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            if (i_sp-i_st)>1:
+                slopes.append(fsamp*_np.max(_np.diff(signal_values[i_st:i_sp])))
+            
+        
+        return(_np.array([_np.min(slopes)]))
 
 
 class SlopeMax(_Algorithm):
     """
     Return the maximum slope of detected peaks.
 
     Parameters
@@ -345,34 +405,49 @@
     
     """
     def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
         assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
+        self.dimensions = {'time' : 1}
 
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-        
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            slopes = _Slopes(starts=idxs_start, peaks=idx_maxs)(signal)
-            return _np.nanmax(_np.array(slopes))
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        signal_values = signal.p.get_values().ravel()
+        slopes = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            if (i_sp-i_st)>1:
+                slopes.append(fsamp*_np.max(_np.diff(signal_values[i_st:i_sp])))
+            
+        
+        return(_np.array([_np.max(slopes)]))
 
 
 class SlopeMean(_Algorithm):
     """
     Return the average slope of detected peaks.
 
     Parameters
@@ -391,27 +466,42 @@
     
     """
     def __init__(self, delta, win_pre=1, win_post=1, **kwargs):
         assert delta > 0, 'Parameter delta, i.e. amplitude of the minimum peak, has to be > 0'
         assert win_pre > 0, 'win_pre must be > 0'
         assert win_post > 0, 'win_post must be > 0'
         _Algorithm.__init__(self, delta=delta, win_pre=win_pre, win_post=win_post, **kwargs)
+        self.dimensions = {'time' : 1}
 
-    
     def algorithm(self, signal):
+        fsamp = signal.p.get_sampling_freq()
         params = self._params
         delta = params['delta']
         win_pre = params['win_pre']
         win_post = params['win_post']
-
-        idx_maxs, idx_mins, val_maxs, val_mins = _PeakDetection(delta=delta)(signal)
-        if len(idx_maxs) == 0:
-            print("No peaks found")
-            return _np.nan
-
-        idxs_start, idxs_stop = _Algorithmelection(indices=idx_maxs, win_pre=win_pre, win_post=win_post)(signal)
-        if len(idxs_start) == 0:
-            print("Unable to detect the start of the peaks")
-            return _np.nan
-        else:
-            slopes = _Slopes(starts=idxs_start, peaks=idx_maxs)(signal)
-            return _np.nanmean(_np.array(slopes))
+        
+        peaks = _PeakDetection(delta = delta)(signal)
+        idx_peaks = _np.where(~_np.isnan(peaks.p.get_values()))[0].ravel()
+        
+        if len(idx_peaks) == 0:
+            return _np.array([_np.nan])
+            
+        peaks_area = _PeakSelection(idx_peaks, win_pre, win_post)(signal).p.get_values().ravel()
+        
+        idx_start_peaks = _np.where(_np.diff(peaks_area) ==1)[0]
+        idx_stop_peaks = _np.where(_np.diff(peaks_area) == -1)[0]
+        
+        if idx_start_peaks[0] > idx_stop_peaks[0]: #start with a peak
+            idx_start_peaks = _np.insert(idx_start_peaks, 0, 0)
+            
+        if idx_start_peaks[-1] > idx_stop_peaks[-1]: #stop with a peak
+            idx_stop_peaks = _np.insert(idx_stop_peaks, 
+                                        len(idx_stop_peaks), 
+                                        len(peaks_area))
+        signal_values = signal.p.get_values().ravel()
+        slopes = []
+        for i_st, i_sp in zip(idx_start_peaks, idx_stop_peaks):
+            if (i_sp-i_st)>1:
+                slopes.append(fsamp*_np.max(_np.diff(signal_values[i_st:i_sp])))
+            
+        
+        return(_np.array([_np.mean(slopes)]))
```

### Comparing `pyphysio-3.1.2/pyphysio/indicators/timedomain.py` & `pyphysio-3.1.3/pyphysio/indicators/timedomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/loaders/_load_nirx.py` & `pyphysio-3.1.3/pyphysio/loaders/_load_nirx.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/segmenters.py` & `pyphysio-3.1.3/pyphysio/segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/signal.py` & `pyphysio-3.1.3/pyphysio/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
                 signal = self.da.dropna(dim = 'time')
                 signal.attrs['sampling_freq'] = 'unevenly'
                 return(signal)
         else:
             print('No nans in the signal, no action performed')
             return(self.da)
     
-    def plot(self, marker=None, ncols=4, sharey=True):
+    def plot(self, marker=None, ncols=4, sharey=False):
         fig = _gcf()
         t_ = self.get_times()
         v_ = self.get_values()
         linestyle='solid'
         
         n_ch = self.get_nchannels()
         n_comp = self.get_ncomponents()
@@ -468,11 +468,11 @@
         processed_da = da.p.process_na(na_action)
         processed_dataset = self.ds
         processed_dataset[main_signal] = processed_da
         if na_action != 'keep':
             processed_dataset = processed_dataset.dropna('time')
         return(processed_dataset)
         
-    def plot(self, marker=None, ncols=4, sharey=True):
+    def plot(self, marker=None, ncols=4, sharey=False):
         self.main_signal.p.plot(marker=marker,
                                 ncols=ncols,
                                 sharey=sharey)
```

### Comparing `pyphysio-3.1.2/pyphysio/specialized/activity/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/activity/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/eda/__init__.py` & `pyphysio-3.1.3/pyphysio/specialized/eda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ... import create_signal
 from ..._base_algorithm import _Algorithm
 # from ...signal import create_signal
 from ...filters import DeConvolutionalFilter as _DeConvolutionalFilter, \
     ConvolutionalFilter as _ConvolutionalFilter
 from ...utils import PeakDetection as _PeakDetection, PeakSelection as _PeakSelection
 
+from ._presets import *
+
 # PHASIC ESTIMATION
 class DriverEstim(_Algorithm):
     """
     Estimates the driver of an EDA signal according to (see Notes)
 
     The estimation uses a deconvolution using a Bateman function as Impulsive Response Function.
     The version of the Bateman function here adopted is:
```

### Comparing `pyphysio-3.1.2/pyphysio/specialized/eda/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/eda/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/eeg/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/eeg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/emg/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/emg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/fnirs/__init__.py` & `pyphysio-3.1.3/pyphysio/specialized/fnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/fnirs/_convert.py` & `pyphysio-3.1.3/pyphysio/specialized/fnirs/_convert.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/fnirs/_data.py` & `pyphysio-3.1.3/pyphysio/specialized/fnirs/_data.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/fnirs/_dl_sqi.py` & `pyphysio-3.1.3/pyphysio/specialized/fnirs/_dl_sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/heart/__init__.py` & `pyphysio-3.1.3/pyphysio/specialized/heart/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/heart/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/heart/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/specialized/resp/_presets.py` & `pyphysio-3.1.3/pyphysio/specialized/resp/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/sqi.py` & `pyphysio-3.1.3/pyphysio/sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/test_data/medical.txt.bz2` & `pyphysio-3.1.3/pyphysio/test_data/medical.txt.bz2`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/pyphysio/utils.py` & `pyphysio-3.1.3/pyphysio/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -739,142 +739,142 @@
     def algorithm(self, signal):
         params = self._params
         max_alg = Maxima(**params) 
         result = -1*max_alg.algorithm(-signal)
         return(result)
 
 #TODO from here
-class BootstrapEstimation(_Algorithm):
-    """
-    Perform a bootstrapped estimation of given statistical indicator
-    
-    Parameters
-    ----------
-    func : numpy function
-        Function to use in the bootstrapping. Must accept data as input
+# class BootstrapEstimation(_Algorithm):
+#     """
+#     Perform a bootstrapped estimation of given statistical indicator
+    
+#     Parameters
+#     ----------
+#     func : numpy function
+#         Function to use in the bootstrapping. Must accept data as input
         
-    Optional parameters
-    -------------------
-    
-    n : int, >0, default = 100
-        Number of iterations
-    k : float, (0,1), default = 0.5
-        Portion of data to be used at each iteration
-    
-    Returns
-    -------
-    estim : float
-        Bootstrapped estimate
-    
-    """
-
-    def __init__(self, func, n=100, k=0.5):
-        from types import FunctionType as Func
-        assert isinstance(func, Func), "Parameter function should be a function (types.FunctionType)"
-        assert n > 0, "n should be positive"
-        assert 0 < k <= 1, "k should be between (0 and 1]"
-        _Algorithm.__init__(self, func=func, n=n, k=k)
-
-    
-    def algorithm(self, signal):
-        params = self._params
-        signal = _np.asarray(signal)
-        l = len(signal)
-        func = params['func']
-        niter = int(params['n'])
-        k = params['k']
-
-        estim = []
-        for i in range(niter):
-            ixs = _np.arange(l)
-            ixs_p = _np.random.permutation(ixs)
-            sampled_data = signal[ixs_p[:int(round(k * l))]]
-            curr_est = func(sampled_data)
-            estim.append(curr_est)
-        estim = _np.sort(estim)
-        return estim[int(len(estim) / 2)]
-
-class Durations(_Algorithm):
-    """
-    Compute durations of events starting from their start and stop indexes
-
-    Parameters:
-    -----------
-    starts : array
-        Start indexes along the data
-    stops : array
-        Stop indexes along the data
-
-    Return:
-    -------
-    durations : array
-        durations of the events
-    """
-
-    def __init__(self, starts, stops):
-        starts = _np.array(starts)
-        assert starts.ndim == 1
-        stops = _np.array(stops)
-        assert stops.ndim == 1
-        _Algorithm.__init__(self, starts=starts, stops=stops)
-
+#     Optional parameters
+#     -------------------
     
-    def algorithm(self, signal):
-        params = self._params
-        starts = params["starts"]
-        stops = params["stops"]
-
-        fsamp = signal.get_sampling_freq()
-        durations = []
-        for I in range(len(starts)):
-            if (stops[I] > 0) & (starts[I] >= 0):
-                durations.append((stops[I] - starts[I]) / fsamp)
-            else:
-                durations.append(_np.nan)
-        return durations
-
-class Slopes(_Algorithm):
-    """
-    Compute rising slope of peaks
-
-    Parameters:
-    -----------
-    starts : array
-        Start of the peaks indexes
-    peaks : array
-        Peaks indexes
-
-    Return:
-    -------
-    slopes : array
-        Rising slopes the peaks
-    """
-
-    def __init__(self, starts, peaks):
-        starts = _np.array(starts)
-        assert starts.ndim == 1
-        peaks = _np.array(peaks)
-        assert peaks.ndim == 1
-        _Algorithm.__init__(self, starts=starts, peaks=peaks)
-
-    
-    def algorithm(cls, data, params):
-        starts = params["starts"]
-        peaks = params["peaks"]
-
-        fsamp = data.get_sampling_freq()
-        slopes = []
-        for I in range(len(starts)):
-            if peaks[I] > 0 & starts[I] >= 0:
-                dy = data[peaks[I]] - data[starts[I]]
-                dt = (peaks[I] - starts[I]) / fsamp
-                slopes.append(dy / dt)
-            else:
-                slopes.append(_np.nan)
-        return slopes
+#     n : int, >0, default = 100
+#         Number of iterations
+#     k : float, (0,1), default = 0.5
+#         Portion of data to be used at each iteration
+    
+#     Returns
+#     -------
+#     estim : float
+#         Bootstrapped estimate
+    
+#     """
+
+#     def __init__(self, func, n=100, k=0.5):
+#         from types import FunctionType as Func
+#         assert isinstance(func, Func), "Parameter function should be a function (types.FunctionType)"
+#         assert n > 0, "n should be positive"
+#         assert 0 < k <= 1, "k should be between (0 and 1]"
+#         _Algorithm.__init__(self, func=func, n=n, k=k)
+
+    
+#     def algorithm(self, signal):
+#         params = self._params
+#         signal = _np.asarray(signal)
+#         l = len(signal)
+#         func = params['func']
+#         niter = int(params['n'])
+#         k = params['k']
+
+#         estim = []
+#         for i in range(niter):
+#             ixs = _np.arange(l)
+#             ixs_p = _np.random.permutation(ixs)
+#             sampled_data = signal[ixs_p[:int(round(k * l))]]
+#             curr_est = func(sampled_data)
+#             estim.append(curr_est)
+#         estim = _np.sort(estim)
+#         return estim[int(len(estim) / 2)]
+
+# class Durations(_Algorithm):
+#     """
+#     Compute durations of events starting from their start and stop indexes
+
+#     Parameters:
+#     -----------
+#     starts : array
+#         Start indexes along the data
+#     stops : array
+#         Stop indexes along the data
+
+#     Return:
+#     -------
+#     durations : array
+#         durations of the events
+#     """
+
+#     def __init__(self, starts, stops):
+#         starts = _np.array(starts)
+#         assert starts.ndim == 1
+#         stops = _np.array(stops)
+#         assert stops.ndim == 1
+#         _Algorithm.__init__(self, starts=starts, stops=stops)
+
+    
+#     def algorithm(self, signal):
+#         params = self._params
+#         starts = params["starts"]
+#         stops = params["stops"]
+
+#         fsamp = signal.get_sampling_freq()
+#         durations = []
+#         for I in range(len(starts)):
+#             if (stops[I] > 0) & (starts[I] >= 0):
+#                 durations.append((stops[I] - starts[I]) / fsamp)
+#             else:
+#                 durations.append(_np.nan)
+#         return durations
+
+# class Slopes(_Algorithm):
+#     """
+#     Compute rising slope of peaks
+
+#     Parameters:
+#     -----------
+#     starts : array
+#         Start of the peaks indexes
+#     peaks : array
+#         Peaks indexes
+
+#     Return:
+#     -------
+#     slopes : array
+#         Rising slopes the peaks
+#     """
+
+#     def __init__(self, starts, peaks):
+#         starts = _np.array(starts)
+#         assert starts.ndim == 1
+#         peaks = _np.array(peaks)
+#         assert peaks.ndim == 1
+#         _Algorithm.__init__(self, starts=starts, peaks=peaks)
+
+    
+#     def algorithm(cls, data, params):
+#         starts = params["starts"]
+#         peaks = params["peaks"]
+
+#         fsamp = data.get_sampling_freq()
+#         slopes = []
+#         for I in range(len(starts)):
+#             if peaks[I] > 0 & starts[I] >= 0:
+#                 dy = data[peaks[I]] - data[starts[I]]
+#                 dt = (peaks[I] - starts[I]) / fsamp
+#                 slopes.append(dy / dt)
+#             else:
+#                 slopes.append(_np.nan)
+#         return slopes
 
 class PeakSelection(_Algorithm):
     """
     Identify the start and the end indexes of each peak in the signal, using derivatives.
 
     Parameters
     ----------
```

### Comparing `pyphysio-3.1.2/pyphysio.egg-info/PKG-INFO` & `pyphysio-3.1.3/pyphysio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.2/pyphysio.egg-info/SOURCES.txt` & `pyphysio-3.1.3/pyphysio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/setup.py` & `pyphysio-3.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
               'pyphysio.specialized.fnirs',
               'pyphysio.specialized.heart',
               'pyphysio.specialized.resp',
               'pyphysio.indicators',
               'pyphysio.generators'],
     package_data={'pyphysio': ['test_data/*']},
     # data_files={'test_data_out': ['info_medical', 'medical.txt.bz2']},
-    version='3.1.2',
+    version='3.1.3',
     description='Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)',
     author='a.bizzego',
     author_email='andrea.bizzego@unitn.it',
     url='https://gitlab.com/a.bizzego/pyphysio',
     keywords=['eda', 'gsr', 'ecg', 'bvp', 'fnirs', 'signal', 
               'analysis', 'physiological', 'psychopysiology', 'neuroscience'],
     classifiers=[
```

### Comparing `pyphysio-3.1.2/tests/test_eda_methods.py` & `pyphysio-3.1.3/tests/test_eda_methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,39 @@
 
 # driver.p.plot()
 # driver_.p.plot()
 
 phasic = eda_tools.PhasicEstim(0.005, win_pre=3, win_post=3)(driver)
 tonic = eda_tools.PhasicEstim(0.005, win_pre=3, win_post=3, return_phasic=False)(driver)
 
+#%%
+# driver.p.plot()
+# tonic.p.plot()
+# phasic.p.plot()
+# plt.show()
+
+
+#%%
+import pyphysio.indicators.peaks as pk
+
+pks_max = pk.PeaksMax(delta=0.005)(phasic)
+
+pks_num = pk.PeaksNum(delta=0.005)(phasic)
+
+dur_mean = pk.DurationMean(0.005, 2, 2)(phasic)
+
+slope = pk.SlopeMin(0.005, 2, 2)(phasic)
+
+#%%
+phasic_indicators = eda_tools.preset_phasic(delta=0.005)
 
+indicators = []
+for ind in phasic_indicators:
+    indicators.append(ind(phasic))
+#%%
 # #%%
 # #%
 # # fig, axes = plt.subplots(3,1,sharex=True)
 # # plt.sca(axes[0])
 # # signal.p.plot()
 
 # # plt.sca(axes[1])
```

### Comparing `pyphysio-3.1.2/tests/test_filters.py` & `pyphysio-3.1.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/tests/test_fnirs.py` & `pyphysio-3.1.3/tests/test_fnirs.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/tests/test_get_sampling_freq.py` & `pyphysio-3.1.3/tests/test_get_sampling_freq.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/tests/test_ibi_estimators.py` & `pyphysio-3.1.3/tests/test_ibi_estimators.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 ecg_data = TestData().ecg()
 
 signal = create_signal(ecg_data, sampling_freq=2048)
 
 ibi = heart.BeatFromECG()(signal)
 
 #%%
+
+
+from pyphysio.interactive import Annotate
+
+annotator = Annotate(signal, ibi)
+
 bvp_data = TestData().bvp() 
 
 signal = create_signal(bvp_data, sampling_freq=2048)
 
 ibi = heart.BeatFromBP()(signal)
 
 ibi_rco = heart.BeatOptimizer()(ibi)
```

### Comparing `pyphysio-3.1.2/tests/test_segmenters.py` & `pyphysio-3.1.3/tests/test_segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/tests/test_signal.py` & `pyphysio-3.1.3/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.2/tests/test_tools.py` & `pyphysio-3.1.3/tests/test_tools.py`

 * *Files identical despite different names*

