# Comparing `tmp/gpmap_tools-0.1.1.tar.gz` & `tmp/gpmap_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpmap_tools-0.1.1.tar", last modified: Tue Apr 18 18:48:02 2023, max compression
+gzip compressed data, was "gpmap_tools-0.1.2.tar", last modified: Wed Apr 19 17:04:12 2023, max compression
```

## Comparing `gpmap_tools-0.1.1.tar` & `gpmap_tools-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,62 @@
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.199070 gpmap_tools-0.1.1/
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1073 2021-12-23 08:41:34.000000 gpmap_tools-0.1.1/LICENSE
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)       17 2022-07-15 13:55:07.000000 gpmap_tools-0.1.1/MANIFEST.in
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      572 2023-04-18 18:48:02.199070 gpmap_tools-0.1.1/PKG-INFO
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     5048 2022-05-05 15:42:52.000000 gpmap_tools-0.1.1/README.md
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.191070 gpmap_tools-0.1.1/bin/
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2021-12-23 08:41:34.000000 gpmap_tools-0.1.1/bin/__init__.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1276 2022-12-01 03:59:36.000000 gpmap_tools-0.1.1/bin/calc_split_data_r2.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     5113 2022-04-12 13:31:08.000000 gpmap_tools-0.1.1/bin/calc_tpt.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     4698 2023-04-18 16:26:01.000000 gpmap_tools-0.1.1/bin/calc_visualization.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3736 2022-07-15 13:55:03.000000 gpmap_tools-0.1.1/bin/filter_genotypes.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     2828 2022-12-13 13:35:19.000000 gpmap_tools-0.1.1/bin/fit_seqdeft.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1226 2022-05-26 21:03:16.000000 gpmap_tools-0.1.1/bin/plot_relaxation_times.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     7909 2023-04-18 18:20:12.000000 gpmap_tools-0.1.1/bin/plot_visualization.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3751 2022-12-01 03:59:36.000000 gpmap_tools-0.1.1/bin/split_data.py
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3489 2023-03-25 17:57:41.000000 gpmap_tools-0.1.1/bin/vc_regression.py
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.191070 gpmap_tools-0.1.1/gpmap/
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2021-12-23 08:41:34.000000 gpmap_tools-0.1.1/gpmap/__init__.py
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.191070 gpmap_tools-0.1.1/gpmap/src/
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2022-04-21 15:30:00.000000 gpmap_tools-0.1.1/gpmap/src/__init__.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    12071 2023-04-18 16:18:36.000000 gpmap_tools-0.1.1/gpmap/src/genotypes.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    28015 2023-04-17 20:50:20.000000 gpmap_tools-0.1.1/gpmap/src/inference.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    11058 2023-04-06 13:54:44.000000 gpmap_tools-0.1.1/gpmap/src/kernel.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    15941 2023-04-17 19:48:55.000000 gpmap_tools-0.1.1/gpmap/src/linop.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    47989 2023-04-17 21:38:12.000000 gpmap_tools-0.1.1/gpmap/src/plot.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    32784 2023-04-18 15:51:54.000000 gpmap_tools-0.1.1/gpmap/src/randwalk.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    11655 2023-04-06 13:54:44.000000 gpmap_tools-0.1.1/gpmap/src/seq.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     1361 2022-11-02 13:28:13.000000 gpmap_tools-0.1.1/gpmap/src/settings.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    24969 2023-04-18 16:02:42.000000 gpmap_tools-0.1.1/gpmap/src/space.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    12441 2023-04-18 16:01:27.000000 gpmap_tools-0.1.1/gpmap/src/utils.py
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.195070 gpmap_tools-0.1.1/gpmap/test/
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2022-04-21 15:30:00.000000 gpmap_tools-0.1.1/gpmap/test/__init__.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     7665 2023-04-18 16:21:07.000000 gpmap_tools-0.1.1/gpmap/test/test_genotypes.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    10627 2023-04-17 17:16:48.000000 gpmap_tools-0.1.1/gpmap/test/test_inference.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     8398 2023-04-06 13:54:44.000000 gpmap_tools-0.1.1/gpmap/test/test_kernel.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    10871 2023-04-17 20:25:09.000000 gpmap_tools-0.1.1/gpmap/test/test_linops.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    19138 2023-04-06 14:37:02.000000 gpmap_tools-0.1.1/gpmap/test/test_plots.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    18332 2023-01-12 13:56:40.000000 gpmap_tools-0.1.1/gpmap/test/test_randwalk.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     6333 2022-11-02 13:32:48.000000 gpmap_tools-0.1.1/gpmap/test/test_seq.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     8168 2023-04-17 21:39:14.000000 gpmap_tools-0.1.1/gpmap/test/test_seqdeft.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    12851 2023-04-17 20:27:42.000000 gpmap_tools-0.1.1/gpmap/test/test_space.py
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     7411 2023-03-25 17:57:41.000000 gpmap_tools-0.1.1/gpmap/test/test_utils.py
-drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-18 18:48:02.199070 gpmap_tools-0.1.1/gpmap_tools.egg-info/
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      572 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/PKG-INFO
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      999 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        1 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      391 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/entry_points.txt
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      103 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/requires.txt
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)       10 2023-04-18 18:48:02.000000 gpmap_tools-0.1.1/gpmap_tools.egg-info/top_level.txt
--rw-rw-r--   0 cmarti    (1000) cmarti    (1000)       38 2023-04-18 18:48:02.199070 gpmap_tools-0.1.1/setup.cfg
--rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1837 2023-04-18 18:47:35.000000 gpmap_tools-0.1.1/setup.py
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.911983 gpmap_tools-0.1.2/
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1073 2021-12-23 08:41:34.000000 gpmap_tools-0.1.2/LICENSE
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)       17 2023-04-19 13:51:37.000000 gpmap_tools-0.1.2/MANIFEST.in
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      603 2023-04-19 17:04:12.911983 gpmap_tools-0.1.2/PKG-INFO
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     5048 2022-05-05 15:42:52.000000 gpmap_tools-0.1.2/README.md
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.887983 gpmap_tools-0.1.2/bin/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2021-12-23 08:41:34.000000 gpmap_tools-0.1.2/bin/__init__.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1276 2022-12-01 03:59:36.000000 gpmap_tools-0.1.2/bin/calc_split_data_r2.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     5113 2022-04-12 13:31:08.000000 gpmap_tools-0.1.2/bin/calc_tpt.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     4698 2023-04-18 16:26:01.000000 gpmap_tools-0.1.2/bin/calc_visualization.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3736 2022-07-15 13:55:03.000000 gpmap_tools-0.1.2/bin/filter_genotypes.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     2837 2023-04-19 00:41:19.000000 gpmap_tools-0.1.2/bin/fit_seqdeft.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     1226 2022-05-26 21:03:16.000000 gpmap_tools-0.1.2/bin/plot_relaxation_times.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     7909 2023-04-18 18:20:12.000000 gpmap_tools-0.1.2/bin/plot_visualization.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3751 2022-12-01 03:59:36.000000 gpmap_tools-0.1.2/bin/split_data.py
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     3444 2023-04-18 22:25:04.000000 gpmap_tools-0.1.2/bin/vc_regression.py
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.887983 gpmap_tools-0.1.2/gpmap/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2021-12-23 08:41:34.000000 gpmap_tools-0.1.2/gpmap/__init__.py
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.883983 gpmap_tools-0.1.2/gpmap/datasets/
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.895983 gpmap_tools-0.1.2/gpmap/datasets/data/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)  1696359 2023-04-18 21:31:29.000000 gpmap_tools-0.1.2/gpmap/datasets/data/f1u.pq
+-rw-r--r--   0 cmarti    (1000) cmarti    (1000)  2747275 2023-04-18 21:26:29.000000 gpmap_tools-0.1.2/gpmap/datasets/data/gb1.pq
+-rw-r--r--   0 cmarti    (1000) cmarti    (1000)   575862 2023-04-18 22:17:56.000000 gpmap_tools-0.1.2/gpmap/datasets/data/smn1.pq
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.899983 gpmap_tools-0.1.2/gpmap/datasets/landscapes/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)   927633 2023-04-18 21:30:22.000000 gpmap_tools-0.1.2/gpmap/datasets/landscapes/f1u.pq
+-rw-r--r--   0 cmarti    (1000) cmarti    (1000)  1874752 2023-04-18 21:26:41.000000 gpmap_tools-0.1.2/gpmap/datasets/landscapes/gb1.pq
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)   903407 2023-04-18 22:37:41.000000 gpmap_tools-0.1.2/gpmap/datasets/landscapes/smn1.pq
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.907983 gpmap_tools-0.1.2/gpmap/src/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2022-04-21 15:30:00.000000 gpmap_tools-0.1.2/gpmap/src/__init__.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     1166 2023-04-19 14:27:55.000000 gpmap_tools-0.1.2/gpmap/src/datasets.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    12071 2023-04-18 16:18:36.000000 gpmap_tools-0.1.2/gpmap/src/genotypes.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    28013 2023-04-18 20:38:32.000000 gpmap_tools-0.1.2/gpmap/src/inference.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    11058 2023-04-06 13:54:44.000000 gpmap_tools-0.1.2/gpmap/src/kernel.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    15879 2023-04-19 14:40:31.000000 gpmap_tools-0.1.2/gpmap/src/linop.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    47977 2023-04-19 13:25:27.000000 gpmap_tools-0.1.2/gpmap/src/plot.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    32792 2023-04-18 22:49:42.000000 gpmap_tools-0.1.2/gpmap/src/randwalk.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    11655 2023-04-06 13:54:44.000000 gpmap_tools-0.1.2/gpmap/src/seq.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     1511 2023-04-19 13:52:40.000000 gpmap_tools-0.1.2/gpmap/src/settings.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    25766 2023-04-19 00:54:18.000000 gpmap_tools-0.1.2/gpmap/src/space.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    12441 2023-04-18 16:01:27.000000 gpmap_tools-0.1.2/gpmap/src/utils.py
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.907983 gpmap_tools-0.1.2/gpmap/test/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        0 2022-04-21 15:30:00.000000 gpmap_tools-0.1.2/gpmap/test/__init__.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      949 2023-04-18 21:51:21.000000 gpmap_tools-0.1.2/gpmap/test/test_datasets.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     7665 2023-04-18 16:21:07.000000 gpmap_tools-0.1.2/gpmap/test/test_genotypes.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     8592 2023-04-19 14:49:11.000000 gpmap_tools-0.1.2/gpmap/test/test_inference.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     8398 2023-04-06 13:54:44.000000 gpmap_tools-0.1.2/gpmap/test/test_kernel.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    10931 2023-04-19 14:43:08.000000 gpmap_tools-0.1.2/gpmap/test/test_linops.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    19138 2023-04-19 16:36:52.000000 gpmap_tools-0.1.2/gpmap/test/test_plots.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    18311 2023-04-18 23:07:15.000000 gpmap_tools-0.1.2/gpmap/test/test_randwalk.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     6331 2023-04-19 00:01:23.000000 gpmap_tools-0.1.2/gpmap/test/test_seq.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     5571 2023-04-19 00:42:40.000000 gpmap_tools-0.1.2/gpmap/test/test_seqdeft.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)    13189 2023-04-19 14:30:40.000000 gpmap_tools-0.1.2/gpmap/test/test_space.py
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     7434 2023-04-18 23:56:14.000000 gpmap_tools-0.1.2/gpmap/test/test_utils.py
+drwxrwxr-x   0 cmarti    (1000) cmarti    (1000)        0 2023-04-19 17:04:12.911983 gpmap_tools-0.1.2/gpmap_tools.egg-info/
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      603 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)     1231 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)        1 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)      391 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)       93 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/requires.txt
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)       10 2023-04-19 17:04:12.000000 gpmap_tools-0.1.2/gpmap_tools.egg-info/top_level.txt
+-rw-rw-r--   0 cmarti    (1000) cmarti    (1000)       38 2023-04-19 17:04:12.911983 gpmap_tools-0.1.2/setup.cfg
+-rwxrwxr-x   0 cmarti    (1000) cmarti    (1000)     2012 2023-04-19 17:03:57.000000 gpmap_tools-0.1.2/setup.py
```

### Comparing `gpmap_tools-0.1.1/LICENSE` & `gpmap_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/PKG-INFO` & `gpmap_tools-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: gpmap_tools
-Version: 0.1.1
-Summary: Tools for inference and visualization of genotype-phenotype maps
+Version: 0.1.2
+Summary: Tools for inference and visualization of complex genotype-phenotype maps
 Home-page: https://bitbucket.org/cmartiga/gpmap_tools
-Author: Carlos Marti-Gomez
+Author: Carlos Martí-Gómez
 Author-email: martigo@cshl.edu
 License: MIT
 Keywords: genotype-phenotype maps,fitness landscape,exact gaussian process regression
 Platform: ALL
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3
 License-File: LICENSE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpmap_tools-0.1.1/README.md` & `gpmap_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/calc_split_data_r2.py` & `gpmap_tools-0.1.2/bin/calc_split_data_r2.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/calc_tpt.py` & `gpmap_tools-0.1.2/bin/calc_tpt.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/calc_visualization.py` & `gpmap_tools-0.1.2/bin/calc_visualization.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/filter_genotypes.py` & `gpmap_tools-0.1.2/bin/filter_genotypes.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/fit_seqdeft.py` & `gpmap_tools-0.1.2/bin/fit_seqdeft.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,27 @@
     
     # Load counts data
     log = LogTrack()
     log.write('Start analysis')
     data = pd.read_csv(counts_fpath, index_col=0)
 
     # Load annotation data
-    seqdeft = SeqDEFT(P, a=a_value, num_a=num_a)
+    seqdeft = SeqDEFT(P, a=a_value, num_reg=num_a)
     if get_a_values:
-        seqdeft.init(X=data.index.values)
+        seqdeft.init(genotypes=data.index.values)
         seqdeft.set_data(X=data.index.values, y=data['counts'].values)
         log.write('Calculating only a values')
         with open(out_fpath, 'w') as fhand:
             for a_value in seqdeft.get_a_values():
                 fhand.write('{}\n'.format(a_value))
     else:
         result = seqdeft.fit(X=data.index.values, y=data['counts'].values)
         result.to_csv(out_fpath)
         
-        fig = plot_SeqDEFT_summary(seqdeft.cv_log_L, result)
+        fig = plot_SeqDEFT_summary(seqdeft.logL_df, result)
         savefig(fig, out_fpath)
     
     log.finish()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gpmap_tools-0.1.1/bin/plot_relaxation_times.py` & `gpmap_tools-0.1.2/bin/plot_relaxation_times.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/plot_visualization.py` & `gpmap_tools-0.1.2/bin/plot_visualization.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/split_data.py` & `gpmap_tools-0.1.2/bin/split_data.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/bin/vc_regression.py` & `gpmap_tools-0.1.2/bin/vc_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 import argparse
 
 import numpy as np
-import pandas as pd
 
-from gpmap.src.utils import LogTrack
+from gpmap.src.utils import LogTrack, read_dataframe, write_dataframe
 from gpmap.src.inference import VCregression
 
         
 def main():
     description = 'Runs Variance Component regression using data from'
     description += ' quantitative phenotypes associated to their corresponding'
     description += ' sequences. If provided, the variance of the estimated '
@@ -18,24 +17,24 @@
     parser = argparse.ArgumentParser(description=description)
     input_group = parser.add_argument_group('Input')
     input_group.add_argument('data', help='CSV table with genotype-phenotype data')
 
     options_group = parser.add_argument_group('VC options')
     options_group.add_argument('--lambdas', default=None,
                                help='File containing known lambdas to use for prediction directly')
-    options_group.add_argument('-r', '--regularize',
-                               action='store_true', default=False,
-                               help='Regularize variance components to exponential decay through CV')
+    help_msg = 'Regularize variance components to exponential decay through CV'
+    options_group.add_argument('-r', '--regularize', action='store_true',
+                               default=False, help=help_msg)
 
     output_group = parser.add_argument_group('Output')
     output_group.add_argument('-o', '--output', required=True, help='Output file')
-    output_group.add_argument('-p', '--pred',
-                              help='File containing sequencse for predicting genotype')
-    output_group.add_argument('--var', action='store_true',
-                              help='Report also posterior variance for the predicted values')
+    help_msg = 'File containing sequences for predicting the associated phenotype'
+    output_group.add_argument('-p', '--pred', help=help_msg)
+    help_msg = 'Report also posterior variance for the predicted values'
+    output_group.add_argument('--var', action='store_true', help=help_msg)
 
     # Parse arguments
     parsed_args = parser.parse_args()
     data_fpath = parsed_args.data
     
     regularize = parsed_args.regularize
     lambdas_fpath = parsed_args.lambdas
@@ -43,16 +42,15 @@
     pred_fpath = parsed_args.pred
     out_fpath = parsed_args.output
     calc_variance = parsed_args.var
     
     # Load counts data
     log = LogTrack()
     log.write('Start analysis')
-    data = pd.read_csv(data_fpath, dtype=str)
-    data = data.set_index(data.columns[0]).astype(float)
+    data = read_dataframe(data_fpath)
     
     # Get processed data
     X = data.index.values
     y = data.values[:, 0]
     y_var = data.values[:, 1] if data.shape[1] > 1 else None 
     Xpred = [line.strip().strip('"')
              for line in open(pred_fpath)] if pred_fpath is not None else None
@@ -70,15 +68,15 @@
         
     log.write('Obtain phenotypic predictions')
     vc.set_data(X=X, y=y, y_var=y_var)
     vc.set_lambdas(lambdas)
     result = vc.predict(Xpred=Xpred, calc_variance=calc_variance)
     
     # Save output
-    result.to_csv(out_fpath)
+    write_dataframe(result, out_fpath)
     
     # Save lambdas
     prefix = '.'.join(out_fpath.split('.')[:-1])
     with open('{}.lambdas.txt'.format(prefix), 'w') as fhand:
         for l in lambdas:
             fhand.write('{}\n'.format(l))
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/genotypes.py` & `gpmap_tools-0.1.2/gpmap/src/genotypes.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/src/inference.py` & `gpmap_tools-0.1.2/gpmap/src/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             
             quad = calc_matrix_polynomial_quad(c_k, self.K.W.L, seq_values)
             cov[d] = reciprocal(quad, distance_class_ns[d])
             
         return(cov, distance_class_ns)
     
     def lambdas_to_variance(self, lambdas):
-        variance_components = (lambdas * self.W.L.lambdas_multiplicity)[1:]
+        variance_components = (lambdas * self.K.lambdas_multiplicity)[1:]
         variance_components = variance_components / variance_components.sum()
         return(variance_components)
     
     def set_lambdas(self, lambdas):
         self.lambdas = lambdas
         self.K.set_lambdas(lambdas=lambdas)
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/kernel.py` & `gpmap_tools-0.1.2/gpmap/src/kernel.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/src/linop.py` & `gpmap_tools-0.1.2/gpmap/src/linop.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         size = 1
         for k in range(self.l):
             size *= self.alpha
             if size >= self.max_size:
                 break
         return(k)
     
+    def todense(self):
+        return(self.dot(np.eye(self.shape[0])))
+    
     def quad(self, v):
         return(np.sum(v * self.dot(v)))
     
     def rayleigh_quotient(self, v, metric=None):
         return(self.quad(v) / inner_product(v, v, metric=metric))
 
 
@@ -55,15 +58,15 @@
             
         if max_size is None:
             self.calc_L()
             self.dot = self.dot0
         else:
             self.dot = self.dot1
             
-        self.calc_lambdas()
+        self.calc_lambdas(ps=ps)
         self.calc_lambdas_multiplicity()
         if ps is None:
             self.calc_W_kd_matrix()
     
     def set_ps(self, ps):
         self.variable_ps = ps is not None
         
@@ -71,16 +74,18 @@
             ps = [np.ones(self.alpha)] * self.l
         check_error(len(ps) == self.l, msg='Number of ps should be equal to length')
 
         # Normalize ps to have the eigenvalues in the right scale
         self.ps = np.vstack([p / p.sum() * self.alpha for p in ps])
         self.pi = calc_tensor_product([p.reshape((p.shape[0], 1)) for p in ps]).flatten()
     
-    def calc_lambdas(self):
+    def calc_lambdas(self, ps=None):
         self.lambdas = np.arange(self.l + 1) * self.alpha
+#         if ps is None:
+#             self.lambdas *= self.alpha
     
     def calc_Kn(self, p):
         Kn = np.vstack([p] * p.shape[0])
         np.fill_diagonal(Kn, np.zeros(Kn.shape[0]))
         return(Kn)
     
     def calc_Kns(self):
@@ -266,24 +271,14 @@
     def dot_square_norm(self, v):
         '''
         Note: we are calculating the squared D_pi-norm of the projection to be 
         able to do it directly through recursive product
         '''
         return(calc_tensor_product_quad(self.matrices, v1=self.pi * v, v2=v))
 
-
-def compute_vjs_norms(y, k, seq_length, n_alleles, L=None):
-    Pj = VjProjectionOperator(n_alleles, seq_length, L=L)
-    positions = np.arange(seq_length)
-    norms = {}
-    for j in combinations(positions, k):
-        Pj.set_j(np.array(j))
-        norms[j] = np.sqrt(Pj.quad(y))
-    return(norms) 
-
     
 class ProjectionOperator(LapDepOperator):
     def __init__(self, n_alleles=None, seq_length=None, L=None, max_L_size=None):
         super().__init__(n_alleles=n_alleles, seq_length=seq_length, L=L,
                          max_L_size=max_L_size)
         self.calc_eig_vandermonde_matrix()
         self.calc_polynomial_coeffs(numeric=False)
@@ -367,14 +362,18 @@
     def __init__(self, W):
         self.W = W
         self.D_sqrt_pi_inv = get_sparse_diag_matrix(1 / np.sqrt(W.L.pi))
         self.D_pi_inv = get_sparse_diag_matrix(1 / W.L.pi)
         self.n = W.n
         self.shape = (self.n, self.n)
         self.known_var = False
+    
+    @property
+    def lambdas_multiplicity(self):
+        return(self.W.L.lambdas_multiplicity)
         
     def set_y_var(self, y_var=None, obs_idx=None):
         
         if y_var is not None and obs_idx is not None:
             msg = 'y_var and obs_idx should have same dimension: {} vs {}'
             msg = msg.format(y_var.shape[0], obs_idx.shape[0])
             check_error(y_var.shape[0] == obs_idx.shape[0], msg=msg)
@@ -400,17 +399,17 @@
     def _dot(self, v):
         if self.W.L.variable_ps:
             return(self.W.dot(self.D_pi_inv.dot(v)))
         else:
             return(self.W.dot(v))
 
     def calc_gt_to_data_matrix(self, obs_idx):
-        self.gt2data = csr_matrix((np.ones(self.n_obs),
-                                   (obs_idx, np.arange(self.n_obs))),
-                                  shape=(self.n, self.n_obs))   
+        n_obs = obs_idx.shape[0]
+        self.gt2data = csr_matrix((np.ones(n_obs), (obs_idx, np.arange(n_obs))),
+                                  shape=(self.n, n_obs))   
     
     def dot(self, v, all_rows=False, add_y_var_diag=True, full_v=False):
         if full_v or not self.known_var:
             u = self._dot(v)
         else:
             u = self._dot(self.gt2data.dot(v))
             if add_y_var_diag:
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/plot.py` & `gpmap_tools-0.1.2/gpmap/src/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+import warnings
 import numpy as np
 import seaborn as sns
 import pandas as pd
 import matplotlib.patches as mpatches
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
@@ -11,22 +12,20 @@
 import holoviews as hv
 
 from matplotlib.collections import LineCollection
 from mpl_toolkits.mplot3d.art3d import Line3DCollection
 from holoviews.operation.datashader import datashade
 
 from gpmap.src.settings import PLOTS_FORMAT
+from gpmap.src.utils import check_error
 from gpmap.src.seq import guess_space_configuration
 from gpmap.src.genotypes import (get_edges_coords, get_nodes_df_highlight,
                                  minimize_nodes_distance)
-import warnings
-from gpmap.src.utils import check_error
 
 
-# Functions
 def init_fig(nrow=1, ncol=1, figsize=None, style='ticks',
              colsize=3, rowsize=3):
     sns.set_style(style)
     if figsize is None:
         figsize = (colsize * ncol, rowsize * nrow)
     fig, axes = plt.subplots(nrow, ncol, figsize=figsize)
     return(fig, axes)
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/randwalk.py` & `gpmap_tools-0.1.2/gpmap/src/randwalk.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         edges_format: str {'npz', 'csv'}
             Format to store the edges information. npz is more efficient but CSV
             can be used in smaller cases for plain text storage.
         
         '''
         self.decay_rates_df.to_csv('{}.decay_rates.csv'.format(prefix), index=False)
         
-        if nodes_format == 'parquet':
+        if nodes_format in ['parquet', 'pq']:
             self.nodes_df.to_parquet('{}.nodes.pq'.format(prefix))
         elif nodes_format == 'csv':
             self.nodes_df.to_csv('{}.nodes.csv'.format(prefix))
         else:
             msg = 'nodes_format can only take values ["parquet", "csv"]'
             raise ValueError(msg)
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/seq.py` & `gpmap_tools-0.1.2/gpmap/src/seq.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/src/settings.py` & `gpmap_tools-0.1.2/gpmap/src/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from os.path import join, abspath, dirname
 from Bio.Data import IUPACData
 
-VERSION = '0.1.0'
-
 # Directories
 BASE_DIR = abspath(join(dirname(__file__), '..'))
 BIN_DIR = join(BASE_DIR, '..', 'bin')
 TEST_DATA_DIR = join(BASE_DIR, 'test', 'data')
+DATASETS_DIR = join(BASE_DIR, 'datasets')
+RAW_DATA_DIR = join(DATASETS_DIR, 'data')
+LANDSCAPES_DIR = join(DATASETS_DIR, 'landscapes')
 
 # File paths
 PLOTS_FORMAT = 'png'
 
 
 ALPHABET = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J',
             'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T',
@@ -35,7 +36,9 @@
 MAX_STATES = 2e7
 U_MAX = 500
 PHI_UB, PHI_LB = 100, 0
 
 NUCLEOTIDES = ['A', 'U', 'G', 'C']
 COMPLEMENT = {'U': 'A', 'A': 'U', 'G': 'C', 'C': 'G', 'N': 'N',
               'T': 'A', '[': ']', ']': '['}
+
+DATASETS = ['gb1', 'f1u', 'smn1']
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/space.py` & `gpmap_tools-0.1.2/gpmap/src/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import warnings
 import numpy as np
 import pandas as pd
 
-from itertools import product
+from itertools import product, combinations
 from _collections import defaultdict
 
 from scipy.sparse.csr import csr_matrix
 from scipy.sparse._matrix_io import save_npz
 from scipy.sparse.extract import triu
 
 from gpmap.src.seq import (translate_seqs, guess_space_configuration,
@@ -15,15 +15,15 @@
                            get_product_states)
 from gpmap.src.utils import (get_sparse_diag_matrix, check_error,
                              calc_cartesian_product)
 from gpmap.src.settings import (DNA_ALPHABET, RNA_ALPHABET, PROTEIN_ALPHABET,
                                 ALPHABET, MAX_STATES, PROT_AMBIGUOUS_VALUES,
                                 DNA_AMBIGUOUS_VALUES, RNA_AMBIGUOUS_VALUES)
 from scipy.special._logsumexp import logsumexp
-from gpmap.src.linop import ProjectionOperator
+from gpmap.src.linop import ProjectionOperator, VjProjectionOperator
 
 
 class DiscreteSpace(object):
     '''
     Class to define an arbitrary discrete space characterized uniquely by the
     connectivity between the different states and optionally by the function
     e.g. fitness or energy at each state of the discrete space
@@ -410,28 +410,50 @@
         y = pd.Series(y, index=X)
         y = y.reindex(self.genotypes).values
             
         self.y = y
         self._check_y()
     
     def calc_variance_components(self):
+        '''
+        
+        '''
         if not hasattr(self, 'W'):
             n_alleles = np.unique(self.n_alleles)
             msg = 'Variance components can only be calculated for spaces'
             msg += ' with constant number of alleles across sites'
             check_error(n_alleles.shape[0] == 1, msg)
             n_alleles = n_alleles[0]
             self.W = ProjectionOperator(n_alleles=n_alleles,
                                         seq_length=self.seq_length)
         lambdas = []
         for k in np.arange(self.seq_length + 1):
             self.W.set_lambdas(k=k)
             ss = np.sum(self.W.dot(self.y) ** 2) / self.W.L.lambdas_multiplicity[k]
             lambdas.append(ss)
         return(np.array(lambdas))
+    
+    def calc_vjs_variance_components(self, k):
+        '''
+        
+        '''
+        if not hasattr(self, 'Pj'):
+            n_alleles = np.unique(self.n_alleles)
+            msg = 'Variance components can only be calculated for spaces'
+            msg += ' with constant number of alleles across sites'
+            check_error(n_alleles.shape[0] == 1, msg)
+            n_alleles = n_alleles[0]
+            self.Pj = VjProjectionOperator(n_alleles, self.seq_length)
+            
+        positions = np.arange(self.seq_length)
+        variances = {}
+        for j in combinations(positions, k):
+            self.Pj.set_j(np.array(j))
+            variances[j] = np.sum(self.Pj.dot(self.y) ** 2)
+        return(variances) 
         
     def to_nucleotide_space(self, codon_table='Standard', stop_y=None,
                             alphabet_type='dna'):
         '''
         Transforms a protein space into a nucleotide space using a codon table
         for translating the sequence
```

### Comparing `gpmap_tools-0.1.1/gpmap/src/utils.py` & `gpmap_tools-0.1.2/gpmap/src/utils.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_genotypes.py` & `gpmap_tools-0.1.2/gpmap/test/test_genotypes.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_inference.py` & `gpmap_tools-0.1.2/gpmap/test/test_inference.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 #!/usr/bin/env python
 import unittest
 import numpy as np
 import pandas as pd
 
 from os.path import join
-from itertools import combinations
-from timeit import timeit
 from subprocess import check_call
 
 from scipy.stats.mstats_basic import pearsonr
 from scipy.special._basic import comb
 
 from gpmap.src.inference import VCregression
 from gpmap.src.settings import TEST_DATA_DIR, BIN_DIR
-from gpmap.src.linop import (LaplacianOperator, ProjectionOperator,
-                             VjProjectionOperator)
-from gpmap.src.utils import get_sparse_diag_matrix
+from gpmap.src.linop import LaplacianOperator, ProjectionOperator
 from gpmap.src.space import SequenceSpace
 
 
 class VCTests(unittest.TestCase):
-    def test_get_gt_to_data_matrix(self):
+    def test_lambdas_to_variance_p(self):
         vc = VCregression()
         vc.init(3, 2)
-
-        m = vc.get_gt_to_data_matrix().todense()
-        assert(np.all(m == np.eye(8)))
-        
-        m = vc.get_gt_to_data_matrix(idx=np.array([0, 1, 2, 3])).todense()
-        assert(np.all(m[:4, :] == np.eye(4)))
-        assert(np.all(m[4:, :] == 0))
-        assert(m.shape == (8, 4))
+        lambdas = np.array([0, 1, 0.5, 0.1])
+        v = vc.lambdas_to_variance(lambdas)
+        assert(np.allclose(v, [3/4.6, 1.5/4.6, 0.1/4.6]))
     
     def test_simulate_vc(self):
         np.random.seed(1)
         sigma = 0.1
         l, a = 4, 4
         vc = VCregression()
         vc.init(l, a)
@@ -158,23 +149,14 @@
         # Ensure kernel alignment and calculation of variance components is the same
         space = SequenceSpace(X=data.index.values, y=data.y.values)
         lambdas1 = space.calc_variance_components()
         vc.fit(X=data.index.values, y=data.y.values)
         lambdas2 = vc.lambdas
         assert(np.allclose(lambdas2, lambdas1))
     
-    def test_vc_smn1(self):
-        data_fpath = join(TEST_DATA_DIR, 'smn1.0.train.csv')
-        out_fpath = join(TEST_DATA_DIR, 'smn1.0.out')
-        bin_fpath = join(BIN_DIR, 'vc_regression.py')
-        
-        # Perform regularization
-        cmd = [sys.executable, bin_fpath, data_fpath, '-o', out_fpath, '-r']
-        check_call(cmd)
-        
     def test_vc_predict(self):
         lambdas = np.array([0, 200, 20, 2, 0.2, 0.02])
         fpath = join(TEST_DATA_DIR, 'vc.data.csv')
         data = pd.read_csv(fpath, dtype={'seq': str}).set_index('seq')
         
         # Using the a priori known variance components
         vc = VCregression()
@@ -203,17 +185,16 @@
     
     def test_vc_predict_from_incomplete_data(self):
         np.random.seed(0)
         fpath = join(TEST_DATA_DIR, 'vc.data.csv')
         data = pd.read_csv(fpath, dtype={'seq': str}).set_index('seq')
         
         filtered = data.loc[np.random.choice(data.index, size=950), :]
-        vc = VCregression()
-        vc.fit(filtered.index, filtered['y'], y_var=filtered['var'], 
-               cross_validation=True)
+        vc = VCregression(cross_validation=True)
+        vc.fit(filtered.index, filtered['y'], y_var=filtered['var'])
         pred = vc.predict().sort_index()
         mse = np.mean((pred['ypred'] - data['y_true']) ** 2)
         rho = pearsonr(pred['ypred'], data['y_true'])[0]
         assert(rho > 0.95)
         assert(mse < 0.3)
     
     def test_vc_predict_max_L_size(self):
@@ -226,48 +207,14 @@
         vc.fit(filtered.index, filtered['y'], y_var=filtered['var'])
         pred = vc.predict().sort_index()
         mse = np.mean((pred['ypred'] - data['y_true']) ** 2)
         rho = pearsonr(pred['ypred'], data['y_true'])[0]
         assert(rho > 0.95)
         assert(mse < 0.3)
     
-    def test_skewed_VC(self):
-        ps = np.array([[0.4, 0.6],
-                       [0.3, 0.7]])
-        vc = VCregression()
-        vc.init(2, 2, ps=ps)
-        
-        # Ensure that we maintain the right eigenvalues
-        lambdas = np.linalg.eig(sk_vc.M.todense())[0]
-        assert(np.allclose(lambdas, [2, 1, 0, 1]))
-        
-        # Ensure that stationary frequencies add up to 1
-        assert(sk_vc.D_pi.data.sum() == 1)
-        
-        # Test projection into the constant subspace
-        f = np.random.normal(0, 1, size=sk_vc.n_genotypes)
-        sk_f_0 = sk_vc.project(f, k=0)
-        assert(np.allclose(sk_f_0, sk_f_0[0]))
-
-        # Test simulation and projection consistency
-        f = sk_vc.simulate(lambdas=[10, 5, 1])['y_true'].values
-        f_0 = sk_vc.project(f, k=0)
-        f_1 = sk_vc.project(f, k=1)
-        f_2 = sk_vc.project(f, k=2)
-        assert(np.allclose(f, f_0 + f_1 + f_2))
-        
-        # Ensure D_pi orthogonality of projections
-        assert(np.allclose(sk_vc.project(f_0, k=1), 0))
-        assert(np.allclose(sk_vc.project(f_0, k=2), 0))
-        assert(np.allclose(sk_vc.project(f_1, k=0), 0))
-        assert(np.allclose(sk_vc.project(f_1, k=2), 0))
-        assert(np.allclose(sk_vc.project(f_2, k=0), 0))
-        assert(np.allclose(sk_vc.project(f_2, k=1), 0))
-    
-    
     def test_vc_fit_bin(self):
         data_fpath = join(TEST_DATA_DIR, 'vc.data.csv')
         lambdas_fpath = join(TEST_DATA_DIR, 'vc.lambdas.csv')
         xpred_fpath = join(TEST_DATA_DIR, 'vc.xpred.txt')
         out_fpath = join(TEST_DATA_DIR, 'seqdeft.output.csv')
         bin_fpath = join(BIN_DIR, 'vc_regression.py')
         
@@ -287,9 +234,9 @@
         # Predict few sequences and their variances
         cmd = [sys.executable, bin_fpath, data_fpath, '-o', out_fpath, '-r',
                '--var', '-p', xpred_fpath]
         check_call(cmd)
         
         
 if __name__ == '__main__':
-    import sys;sys.argv = ['', 'VCTests.test_calculate_variance_components']
+    import sys;sys.argv = ['', 'VCTests']
     unittest.main()
```

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_kernel.py` & `gpmap_tools-0.1.2/gpmap/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_linops.py` & `gpmap_tools-0.1.2/gpmap/test/test_linops.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 #!/usr/bin/env python
 import unittest
 import numpy as np
-import pandas as pd
 
 from itertools import combinations
 from timeit import timeit
 
+from gpmap.src.settings import ALPHABET
+from gpmap.src.seq import generate_possible_sequences
+from gpmap.src.utils import get_sparse_diag_matrix
+from gpmap.src.kernel import VarianceComponentKernel
 from gpmap.src.linop import (LaplacianOperator, ProjectionOperator,
                              VjProjectionOperator, KernelOperator,
-                             compute_vjs_norms)
-from gpmap.src.kernel import VarianceComponentKernel
-from gpmap.src.settings import ALPHABET, TEST_DATA_DIR
-from gpmap.src.seq import generate_possible_sequences
-from os.path import join
+                             DeltaPOperator)
 
 
 class LinOpsTests(unittest.TestCase):
     def test_laplacian(self):
         L = LaplacianOperator(2, 2)
         
         v = np.ones(4)
         assert(np.allclose(L.dot(v), 0))
         assert(np.allclose(L.dot(2*v), 0))
         
         v = np.array([1, 2, 1, 0])
         u = np.array([-1, 3, 1, -3])
         assert(np.allclose(L.dot(v), u))
     
-    def test_laplacian_D_pi(self):
-        L = LaplacianOperator(2, 2)
-        assert(np.allclose(L.D_pi.data, 1))
-        
-        L = LaplacianOperator(2, 2, ps=np.array([[0.4, 0.6], [0.5, 0.5]]))
-        pi = np.array([0.2, 0.2, 0.3, 0.3])
-        assert(np.allclose(L.D_pi.data, pi))
-    
     def test_laplacian_eigenvalues(self):
         L = LaplacianOperator(2, 2)
         assert(np.allclose(L.lambdas, [0, 2, 4]))
         
         L = LaplacianOperator(2, 3)
         assert(np.allclose(L.lambdas, [0, 2, 4, 6]))
         
         L = LaplacianOperator(3, 2)
         assert(np.allclose(L.lambdas, [0, 3, 6]))
         
         ps = np.array([[0.4, 0.6], [0.5, 0.5]])
         L = LaplacianOperator(2, 2, ps=ps)
-        print(L.lambdas)
         assert(np.allclose(L.lambdas, [0, 1, 2]))
 
     def test_laplacian_split(self):
         L1 = LaplacianOperator(4, 7)
         L2 = LaplacianOperator(4, 7, max_size=500)
         
         for d in L2.Kns_shape:
@@ -224,108 +214,123 @@
         K.set_y_var(y_var=0.1 * np.ones(K.n), obs_idx=np.arange(K.n))
         K.set_lambdas(lambdas=np.append([0], 2-np.arange(l)))
         
         v = np.random.normal(size=K.n_obs)
         u = K.inv_dot(K.dot(v))
         assert(np.allclose(u, v))
     
-    def test_skewed_kernel_operator_big(self):
-        l, a = 4, 4
-        alleles = ALPHABET[:a]
-        ps = np.random.dirichlet(alpha=np.ones(a), size=l)
-        log_p = np.log(ps)
-        
-        # Define Laplacian based kernel
-        L = LaplacianOperator(a, l, ps=ps)
-        W = ProjectionOperator(L=L)
-        K1 = KernelOperator(W)
-        I = np.eye(K1.shape[0])
-        
-        # Define full kernel function
-        kernel = VarianceComponentKernel(l, a, use_p=True)
-        x = np.array([x for x in generate_possible_sequences(l, alleles)])
-        kernel.set_data(x1=x, alleles=alleles)
-        
-        # Test components
-        for k in range(l+1):
-            lambdas = np.zeros(l+1)
-            lambdas[k] = 1
-            K1.set_lambdas(lambdas)
-            k1 = K1.dot(I)
-            k2 = kernel(lambdas=lambdas, log_p=log_p)
-            assert(np.allclose(k1, k2))
-        
+    def test_kernel_opt_get_gt_to_data_matrix(self):
+        vc = KernelOperator(ProjectionOperator(2, 3))
+        obs_idx = np.arange(vc.n)
+        vc.calc_gt_to_data_matrix(obs_idx)
+        m = vc.gt2data.todense()
+        assert(np.all(m == np.eye(8)))
+        
+        vc.calc_gt_to_data_matrix(obs_idx=np.array([0, 1, 2, 3]))
+        m = vc.gt2data.todense()
+        assert(np.all(m[:4, :] == np.eye(4)))
+        assert(np.all(m[4:, :] == 0))
+        assert(m.shape == (8, 4))
+    
     def test_skewed_kernel_operator(self):
         ps = np.array([[0.3, 0.7], [0.5, 0.5]])
         log_p = np.log(ps)
         l, a = ps.shape
         
         # Define Laplacian based kernel
         L = LaplacianOperator(a, l, ps=ps)
         W = ProjectionOperator(L=L)
         K1 = KernelOperator(W)
-        I = np.eye(K1.shape[0])
         
         # Define full kernel function
         kernel = VarianceComponentKernel(l, a, use_p=True)
         x = np.array(['AA', 'AB', 'BA', 'BB'])
         kernel.set_data(x1=x, alleles=['A', 'B'])
         
         # Constant component
         lambdas = [1, 0, 0]
         K1.set_lambdas(lambdas)
-        k1 = K1.dot(I)
+        k1 = K1.todense()
         assert(np.allclose(k1, 1))
         
         K2 = kernel(lambdas=lambdas, log_p=log_p)
         assert(np.allclose(K2, 1))
         
         # Additive component
         lambdas = [0, 1, 0]
         K1.set_lambdas(lambdas)
-        k1 = K1.dot(I)
+        k1 = K1.todense()
         k2 = kernel(lambdas=lambdas, log_p=log_p)
         assert(np.allclose(k1, k2))
         
         # Pairwise component
         lambdas = [0, 0, 1]
         K1.set_lambdas(lambdas)
-        k1 = K1.dot(I)
+        k1 = K1.todense()
         k2 = kernel(lambdas=lambdas, log_p=log_p)
         assert(np.allclose(k1, k2))
     
-    def test_vj_projection_operator_ss(self):
-        vjp = VjProjectionOperator(4, 5)
-        v = np.random.normal(size=vjp.n)
+    def test_skewed_kernel_operator_big(self):
+        l, a = 4, 4
+        alleles = ALPHABET[:a]
+        ps = np.random.dirichlet(alpha=np.ones(a), size=l)
+        log_p = np.log(ps)
+        
+        # Define Laplacian based kernel
+        L = LaplacianOperator(a, l, ps=ps)
+        W = ProjectionOperator(L=L)
+        K1 = KernelOperator(W)
+        I = np.eye(K1.shape[0])
         
-        vjp.set_j([0, 2, 3])
-        print(timeit(lambda: vjp.quad(v), number=10))
-        print(timeit(lambda : vjp.dot_square_norm(v), number=10))
-        
-        # for k in range(1, 6):
-        #     for j in combinations(np.arange(vjp.l), k):
-        #         vjp.set_j(j)
-        #         u = vjp.dot(v)
-        #         ss1 = np.sum(u * u)
-        #         ss2 = vjp.dot_square_norm(v)
-        #         ss3 = vjp.quad(v) # only applies in equally weighted case
-        #         assert(np.allclose(ss1, ss2))
-        #         assert(np.allclose(ss1, ss3))
-    
-    def test_compute_vjs_squared_norms(self):
-        fpath = join(TEST_DATA_DIR, 'gb1.csv')
-        data = pd.read_csv(fpath, index_col=0)
-        
-        norms = compute_vjs_norms(data['log_binding'].values, k=1,
-                                  seq_length=4, n_alleles=20)
-        assert(norms[(2,)] > norms[(0,)])
-        assert(norms[(3,)] > norms[(1,)])
-        
-        norms = compute_vjs_norms(data['log_binding'].values, k=2,
-                                  seq_length=4, n_alleles=20)
-        for v in norms.values():
-            assert(norms[(2,3)] >= v)
+        # Define full kernel function
+        kernel = VarianceComponentKernel(l, a, use_p=True)
+        x = np.array([x for x in generate_possible_sequences(l, alleles)])
+        kernel.set_data(x1=x, alleles=alleles)
+        
+        # Test components
+        for k in range(l+1):
+            lambdas = np.zeros(l+1)
+            lambdas[k] = 1
+            K1.set_lambdas(lambdas)
+            k1 = K1.dot(I)
+            k2 = kernel(lambdas=lambdas, log_p=log_p)
+            assert(np.allclose(k1, k2))
     
+    def test_DeltaP_operator(self):
+        DP2 = DeltaPOperator(P=2, n_alleles=2, seq_length=3)
+        DP3 = DeltaPOperator(P=3, n_alleles=2, seq_length=3)
+
+        # Additive landscape        
+        v = np.array([0, 1, 1, 2,
+                      0, 1, 1, 2])
+        assert(DP2.quad(v) == 0)
+        assert(DP3.quad(v) == 0)
+        
+        # Pairwise landscape
+        v = np.array([0, 1, 1, 3,
+                      0, 1, 1, 3])
+        assert(DP2.quad(v) > 0)
+        assert(DP3.quad(v) == 0)
+    
+    def test_DP_calc_kernel_basis(self):
+        DP = DeltaPOperator(P=2, n_alleles=4, seq_length=5)
+        DP.calc_kernel_basis()
+        basis = DP.kernel_basis
+        
+        # Ensure basis is orthonormal
+        prod = basis.T.dot(basis)
+        identity = get_sparse_diag_matrix(np.ones(prod.shape[0]))
+        assert(np.allclose((prod - identity).todense(), 0))
+        
+        # Ensure basis is sparse
+        max_values = basis.shape[0] * basis.shape[1]
+        assert(basis.data.shape[0] < max_values) 
+        
+        # Ensure they generate good projection matrices
+        u = np.dot(basis, basis.T).dot(basis)
+        error = (basis - u).mean()
+        assert(np.allclose(error, 0))
+        
         
 if __name__ == '__main__':
     import sys;sys.argv = ['', 'LinOpsTests']
     unittest.main()
```

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_plots.py` & `gpmap_tools-0.1.2/gpmap/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_randwalk.py` & `gpmap_tools-0.1.2/gpmap/test/test_randwalk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 import unittest
 import sys
 
-from os.path import join
-from subprocess import check_call
-
 import numpy as np
 import pandas as pd
+
+from os.path import join
+from subprocess import check_call
+from itertools import product
+from tempfile import NamedTemporaryFile
 from scipy.sparse._matrix_io import load_npz
 
 from gpmap.src.settings import TEST_DATA_DIR, BIN_DIR
 from gpmap.src.space import CodonSpace
 from gpmap.src.randwalk import WMWSWalk
-from gpmap.src.plot import figure_Ns_grid
 from gpmap.src.utils import get_sparse_diag_matrix
-from itertools import product
 
 
 class RandomWalkTests(unittest.TestCase):
     def test_set_Ns(self):
         mc = WMWSWalk(CodonSpace(['S'], add_variation=True, seed=0))
 
         freqs = mc.calc_stationary_frequencies(Ns=0)
@@ -87,15 +87,14 @@
         mc.set_stationary_freqs(mc.calc_stationary_frequencies(Ns=1))
         mc.calc_rate_matrix(Ns=1)
         mc.calc_jump_matrix()
         times, path = mc.run_forward(time=1)
         assert(np.sum(times) == 1)
         assert(len(path) == len(times))
         
-    
     def calc_neutral_stat_freqs(self):
         mc = WMWSWalk(CodonSpace(['S'], add_variation=True, seed=0))
         
         sites_stat_freqs = [np.array([0.4, 0.6]), np.array([0.3, 0.7])]
         freqs = mc.calc_neutral_stat_freqs(sites_stat_freqs)
         assert(np.allclose(freqs, [0.12, 0.28, 0.18, 0.42]))
         
@@ -230,15 +229,14 @@
         # Check variable rates across sites
         site_mut_rates = np.array([1, 1, 2])
         mc.calc_model_neutral_rate_matrix(model='K80', site_mut_rates=site_mut_rates)
         assert(np.allclose(mc.neutral_stat_freqs, 1. / 64))
         assert(np.allclose(mc.neutral_rate_matrix.diagonal().sum(), -9))
         assert(np.unique(mc.neutral_rate_matrix.data).shape[0] > 2)
         
-        
     def test_stationary_frequencies(self):
         mc = WMWSWalk(CodonSpace(['S'], add_variation=True, seed=0))
         codons = ['AGC', 'AGT', 'TCA', 'TCC', 'TCG', 'TCT']
         codon_idxs = mc.space.get_state_idxs(codons)
         stop_codons = ['TGA', 'TAG', 'TAA']
         stop_codon_idxs = mc.space.get_state_idxs(stop_codons)
         
@@ -335,99 +333,99 @@
                                           exchange_rates={'a': 1, 'b': 2},
                                           stat_freqs={'A': 0.2, 'T': 0.2,
                                                       'C': 0.3, 'G': 0.3})
         mc.calc_visualization(Ns=1, n_components=20)
         nd2 = mc.nodes_df
         assert(not np.allclose(nd2['1'], nd1['1']))
     
-    def test_figure_Ns(self):
-        mc = WMWSWalk(CodonSpace(['S'], add_variation=True, seed=0))
-        fpath = join(TEST_DATA_DIR, 'serine.Ns_grid')
-        figure_Ns_grid(mc, fpath=fpath, nodes_color='function')
-    
     def test_write_visualization(self):
         mc = WMWSWalk(CodonSpace(['S'], add_variation=True, seed=0))
         mc.calc_visualization(Ns=1, n_components=20)
-        prefix = join(TEST_DATA_DIR, 'serine')
-        mc.write_tables(prefix, write_edges=True)
         
-        nodes_df = pd.read_csv('{}.nodes.csv'.format(prefix), index_col=0)
-        assert(np.allclose(nodes_df.values, mc.nodes_df.values))
+        with NamedTemporaryFile() as fhand:
+            prefix = fhand.name
+            mc.write_tables(prefix, write_edges=True, nodes_format='csv')
+            
+            nodes_df = pd.read_csv('{}.nodes.csv'.format(prefix), index_col=0)
+            assert(np.allclose(nodes_df.values, mc.nodes_df.values))
         
     def test_calc_visualization_bin_help(self):
         bin_fpath = join(BIN_DIR, 'calc_visualization.py')
     
         cmd = [sys.executable, bin_fpath, '-h']
         check_call(cmd)
     
     def test_calc_visualization_bin(self):
         bin_fpath = join(BIN_DIR, 'calc_visualization.py')
         fpath = join(TEST_DATA_DIR, 'serine.csv')
         
-        out_fpath = join(TEST_DATA_DIR, 'serine') 
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-p', '90', '-e']
-        check_call(cmd)
-        
-        df = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
-        assert(df.iloc[np.argmax(df['1']), :]['function'] > 1.5)
-        assert(df.iloc[np.argmin(df['1']), :]['function'] > 1.5)
-        
-        edges = load_npz('{}.edges.npz'.format(out_fpath))
-        assert(np.all(edges.shape == (64, 64)))
+        with NamedTemporaryFile() as fhand:
+            out_fpath = fhand.name
+            cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath,
+                   '-p', '90', '-e', '-nf', 'csv']
+            check_call(cmd)
+            
+            df = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
+            assert(df.iloc[np.argmax(df['1']), :]['function'] > 1.5)
+            assert(df.iloc[np.argmin(df['1']), :]['function'] > 1.5)
+            
+            edges = load_npz('{}.edges.npz'.format(out_fpath))
+            assert(np.all(edges.shape == (64, 64)))
     
     def test_calc_visualization_bin_guess_config(self):
         bin_fpath = join(BIN_DIR, 'calc_visualization.py')
         fpath = join(TEST_DATA_DIR, 'test.csv')
         
-        out_fpath = join(TEST_DATA_DIR, 'test') 
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-m', '0.5', '-e']
-        check_call(cmd)
+        with NamedTemporaryFile() as fhand:
+            cmd = [sys.executable, bin_fpath, fpath, '-o', fhand.name,
+                   '-m', '0.5', '-e']
+            check_call(cmd)
     
     def test_calc_visualization_codon_restricted(self):
         bin_fpath = join(BIN_DIR, 'calc_visualization.py')
         fpath = join(TEST_DATA_DIR, 'test.csv')
+        data = pd.read_csv(fpath, index_col=0)
+        cmd = [sys.executable, bin_fpath, fpath, '-m', '0.65', '-e', '-nf', 'csv']
         
         # run with standard genetic code
-        out_fpath = join(TEST_DATA_DIR, 'test') 
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-m', '0.65', '-e']
-        check_call(cmd)
-        edges1 = load_npz('{}.edges.npz'.format(out_fpath))
+        with NamedTemporaryFile() as fhand:
+            out_fpath = fhand.name
+            check_call(cmd + ['-o', out_fpath])
+            edges1 = load_npz('{}.edges.npz'.format(out_fpath))
         
         # run with bacterial genetic code 11
-        out_fpath = join(TEST_DATA_DIR, 'test.codon') 
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-m', '0.65',
-               '-e', '-c', '11']
-        check_call(cmd)
-        
-        df = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
-        data = pd.read_csv(fpath, index_col=0)
-        assert(df.shape[0] == data.shape[0])
-
-        # Ensure we have less edges when using codon restricted transitions        
-        edges2 = load_npz('{}.edges.npz'.format(out_fpath))
-        assert(edges1.sum() > edges2.sum())
+        with NamedTemporaryFile() as fhand:
+            out_fpath = fhand.name
+            check_call(cmd + ['-o', out_fpath, '-c', '11']) 
+            df = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
+            assert(df.shape[0] == data.shape[0])
+
+            # Ensure we have less edges when using codon restricted transitions        
+            edges2 = load_npz('{}.edges.npz'.format(out_fpath))
+            assert(edges1.sum() > edges2.sum())
 
     def test_calc_visualization_codon_bin(self):
         bin_fpath = join(BIN_DIR, 'calc_visualization.py')
         fpath = join(TEST_DATA_DIR, 'serine.protein.csv')
+        cmd = [sys.executable, bin_fpath, fpath, '-Ns', '1', 
+               '-e', '-C', '-nf', 'csv']
         
         # standard genetic code
-        out_fpath = join(TEST_DATA_DIR, 'serine.codon')
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-m', '0.65',
-               '-e', '-C', '-c', 'Standard']
-        check_call(cmd)
-        nodes = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
-        assert(nodes.shape[0] == 64)
+        with NamedTemporaryFile() as fhand:
+            out_fpath = fhand.name
+            check_call(cmd + ['-o', out_fpath, '-c', 'Standard'])
+            
+            nodes = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
+            assert(nodes.shape[0] == 64)
         
         # custom genetic code
-        out_fpath = join(TEST_DATA_DIR, 'serine.codon.custom')
-        codon_fpath = join(TEST_DATA_DIR, 'code_6037.csv')
-        cmd = [sys.executable, bin_fpath, fpath, '-o', out_fpath, '-m', '0.65',
-               '-e', '-C', '-c', codon_fpath]
-        check_call(cmd)
-        nodes = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
-        assert(nodes.shape[0] == 64)
+        with NamedTemporaryFile() as fhand:
+            out_fpath = fhand.name
+            codon_fpath = join(TEST_DATA_DIR, 'code_6037.csv')
+            check_call(cmd + ['-o', out_fpath, '-c', codon_fpath])
+            nodes = pd.read_csv('{}.nodes.csv'.format(out_fpath), index_col=0)
+            assert(nodes.shape[0] == 64)
         
         
 if __name__ == '__main__':
     sys.argv = ['', 'RandomWalkTests']
     unittest.main()
```

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_seq.py` & `gpmap_tools-0.1.2/gpmap/test/test_seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python
 import unittest
-
-from os.path import join
-
 import numpy as np
 import pandas as pd
 
+from os.path import join
 from gpmap.src.settings import TEST_DATA_DIR
 from gpmap.src.seq import (translate_seqs, guess_alphabet_type,
                            guess_space_configuration, get_custom_codon_table,
                            get_seqs_from_alleles, get_one_hot_from_alleles,
                            generate_freq_reduced_code, transcribe_seqs)
```

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_space.py` & `gpmap_tools-0.1.2/gpmap/test/test_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 import unittest
-
 import pandas as pd
 import numpy as np
 
-from gpmap.src.space import SequenceSpace, DiscreteSpace, CodonSpace,\
-    ProductSpace, GridSpace
-from scipy.sparse.csr import csr_matrix
-from gpmap.src.settings import TEST_DATA_DIR
 from os.path import join
 from tempfile import NamedTemporaryFile
+from scipy.sparse.csr import csr_matrix
+
+from gpmap.src.settings import TEST_DATA_DIR
+from gpmap.src.datasets import DataSet
+from gpmap.src.space import (SequenceSpace, DiscreteSpace, CodonSpace,
+                             ProductSpace, GridSpace)
 
 
 class SpaceTests(unittest.TestCase):
     def test_discrete_space_errors(self):
         # Fail when adjacency matrix is not well formed
         wrong_matrices = [np.array([0, 1]), 
                           np.array([[0, -1], [1, 0]]),
@@ -273,26 +274,36 @@
         np.random.shuffle(labels)
         data = data.loc[labels, :]
         
         s = SequenceSpace(X=data.index.values, y=data['y'].values)
         assert(np.all(sorted(s.state_labels[s.y > 1.5]) == sorted(codons)))
     
     def test_calculate_variance_components(self):
-        data = pd.read_csv(join(TEST_DATA_DIR, 'gb1.csv')).set_index('seq')
-        space = SequenceSpace(X=data.index.values, y=data.log_binding.values)
+        space = DataSet('gb1').to_sequence_space()
         lambdas = space.calc_variance_components()
         assert(np.all(lambdas > 0))
         
         data = pd.read_csv(join(TEST_DATA_DIR, 'negative_vc.tsv'),
                            index_col=0, sep='\t')
         data['y'] = np.log(data['Q_star'])
         space = SequenceSpace(X=data.index.values, y=data.y.values)
         lambdas = space.calc_variance_components()
         assert(np.all(lambdas > 0))
     
+    def test_calc_vjs_variance_components(self):
+        space = DataSet('gb1').to_sequence_space()
+        
+        vj1 = space.calc_vjs_variance_components(k=1)  
+        assert(vj1[(2,)] > vj1[(0,)])
+        assert(vj1[(3,)] > vj1[(1,)])
+        
+        vj2 = space.calc_vjs_variance_components(k=2)
+        for v in vj2.values():
+            assert(vj2[(2,3)] >= v)
+    
     def test_to_codon_space(self):
         fpath = join(TEST_DATA_DIR, 'serine.protein.csv')
         data = pd.read_csv(fpath, index_col=0)
         
         s = SequenceSpace(X=data.index.values, y=data['function'].values)
         s = s.to_nucleotide_space(codon_table='Standard', stop_y=0)
         assert(s.n_genotypes == 64)
```

### Comparing `gpmap_tools-0.1.1/gpmap/test/test_utils.py` & `gpmap_tools-0.1.2/gpmap/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 
 from os.path import join
 
-from gpmap.src.utils import calc_cartesian_product, get_CV_splits,\
-    calc_tensor_product, calc_cartesian_product_dot, calc_tensor_product_dot,\
-    calc_tensor_product_quad, quad
 from gpmap.src.settings import TEST_DATA_DIR
+from gpmap.src.utils import (calc_cartesian_product, get_CV_splits,
+                             calc_tensor_product, calc_cartesian_product_dot,
+                             calc_tensor_product_dot,
+                             calc_tensor_product_quad, quad)
 
 
 class UtilsTests(unittest.TestCase):
     def test_cartesian_product(self):
         # With adjacency matrices
         matrix = np.array([[0, 1],
                            [1, 0]])
@@ -139,18 +140,18 @@
         np.random.seed(0)
         nfolds = 3 
         X = np.array(['A', 'B', 'C'])
         y = np.array([1, 2, 2])
         
         splits = get_CV_splits(X, y, nfolds=3)
         for _, (x_train, y_train, _), (x_test, y_test, _) in splits:
-            assert(x_train.shape[0] == 1)
-            assert(y_train.shape[0] == 1)
-            assert(x_test.shape[0] == 2)
-            assert(y_test.shape[0] == 2)
+            assert(x_train.shape[0] == 2)
+            assert(y_train.shape[0] == 2)
+            assert(x_test.shape[0] == 1)
+            assert(y_test.shape[0] == 1)
             
         splits = list(get_CV_splits(X, y, nfolds=nfolds, count_data=True))
         assert(len(splits) == nfolds)
         for _, (x_train, y_train), (x_test, y_test) in splits:
             # Test total numbers are preserved
             assert(y_train.sum() + y_test.sum() == y.sum())
             
@@ -172,19 +173,17 @@
             pass
     
     def test_get_CV_splits_big_dataset(self):
         nfolds = 7
         data = pd.read_csv(join(TEST_DATA_DIR, 'seqdeft_counts.csv'),
                            index_col=0)
         X, y = data.index.values, data.iloc[:, 0].values
-        print(y.sum())
         splits = get_CV_splits(X, y, nfolds=nfolds, count_data=True)
         test_counts = {}
         for i, (x_train, y_train), (x_test, y_test) in splits:
-            print(y_train.sum())
             assert(y_train.sum() + y_test.sum() == y.sum())
             
             counts = {seq: c for seq, c in zip(x_train, y_train)}
             for seq, c in zip(x_test, y_test):
                 try:
                     counts[seq] += c
                 except KeyError:
```

### Comparing `gpmap_tools-0.1.1/gpmap_tools.egg-info/PKG-INFO` & `gpmap_tools-0.1.2/gpmap_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: gpmap-tools
-Version: 0.1.1
-Summary: Tools for inference and visualization of genotype-phenotype maps
+Version: 0.1.2
+Summary: Tools for inference and visualization of complex genotype-phenotype maps
 Home-page: https://bitbucket.org/cmartiga/gpmap_tools
-Author: Carlos Marti-Gomez
+Author: Carlos Martí-Gómez
 Author-email: martigo@cshl.edu
 License: MIT
 Keywords: genotype-phenotype maps,fitness landscape,exact gaussian process regression
 Platform: ALL
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3
 License-File: LICENSE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpmap_tools-0.1.1/setup.py` & `gpmap_tools-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 
 def main():
-    description = 'Tools for inference and visualization of genotype-phenotype'
-    description += ' maps'
+    description = 'Tools for inference and visualization of complex '
+    description += 'genotype-phenotype maps'
     setup(
         name='gpmap_tools',
         version=VERSION,
         license='MIT',
         description=description,
-        author='Carlos Marti-Gomez',
+        author='Carlos Martí-Gómez',
         author_email='martigo@cshl.edu',
         url='https://bitbucket.org/cmartiga/gpmap_tools',
         packages=find_packages(),
         include_package_data=True,
+        package_data = {'': ['datasets/*/gb1*',
+                             'datasets/*/f1u*',
+                             'datasets/*/smn1*']},
         entry_points={
             'console_scripts': [
                 'fit_SeqDEFT = bin.fit_seqdeft:main',
                 'vc_regression = bin.vc_regression:main',
                 'split_data = bin.split_data:main',
                 'calc_split_data_r2 = bin.calc_split_data_r2:main',
                 'calc_visualization = bin.calc_visualization:main',
                 'calc_tpt = bin.calc_tpt:main',
                 'plot_visualization = bin.plot_visualization:main',
                 'plot_decay_rates = bin.plot_decay_rates:main',
                 'filter_genotypes = bin.filter_genotypes:main',
             ]},
         install_requires=['biopython',
-                          'datashader', 'holoviews', 'plotly', 'logomaker',
+                          'datashader', 'holoviews', 'plotly',
                           'seaborn', 'matplotlib', 'tqdm',
                           'fastparquet', 'pandas', 'scipy', 'numpy'],
+        python_requires='>=3',
         platforms='ALL',
         keywords=['genotype-phenotype maps', 'fitness landscape',
                   'exact gaussian process regression'],
         classifiers=[
             "Programming Language :: Python :: 3",
             'Intended Audience :: Science/Research',
             "License :: OSI Approved :: MIT License",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

