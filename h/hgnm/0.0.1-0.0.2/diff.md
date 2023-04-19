# Comparing `tmp/HGNM-0.0.1.tar.gz` & `tmp/hgnm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\magnu\OneDrive\Dokumente\Karlsruher Institut f\374r Technologie\Hiwi ALR\DAVIS_Library\HGNM\dist\.tmp-3ah59ba3\HGNM-0.0.1", last modified: Thu Apr 13 13:59:53 2023, max compression
+gzip compressed data, was "C:\Users\magnu\OneDrive\Dokumente\Karlsruher Institut f\374r Technologie\Hiwi ALR\DAVIS_Library\HGNM\dist\.tmp-dck90pqs\hgnm-0.0.2", last modified: Wed Apr 19 07:56:30 2023, max compression
```

## Comparing `HGNM-0.0.1.tar` & `hgnm-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:53.000000 HGNM-0.0.1/
--rw-rw-rw-   0        0        0     1111 2023-03-30 09:55:00.000000 HGNM-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1130 2023-04-13 13:59:53.000000 HGNM-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-03-30 10:03:02.000000 HGNM-0.0.1/README.md
--rw-rw-rw-   0        0        0     1579 2023-04-13 13:52:08.000000 HGNM-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 13:59:53.000000 HGNM-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM/
--rw-rw-rw-   0        0        0     1473 2023-04-11 13:59:57.000000 HGNM-0.0.1/src/HGNM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM/modules/
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:52.000000 HGNM-0.0.1/src/HGNM/modules/abstract/
--rw-rw-rw-   0        0        0     2045 2023-04-12 09:24:10.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractBlock.py
--rw-rw-rw-   0        0        0     2357 2023-04-12 09:21:00.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractGraphAssertions.py
--rw-rw-rw-   0        0        0     2260 2023-04-12 09:13:07.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractInputEmbedding.py
--rw-rw-rw-   0        0        0     7529 2023-04-12 12:25:29.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractMessagePassingBase.py
--rw-rw-rw-   0        0        0     2393 2023-04-04 09:20:24.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractModules.py
--rw-rw-rw-   0        0        0     6452 2023-04-12 12:18:21.000000 HGNM-0.0.1/src/HGNM/modules/abstract/AbstractStack.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/abstract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:52.000000 HGNM-0.0.1/src/HGNM/modules/common/
--rw-rw-rw-   0        0        0     2522 2023-04-12 09:10:41.000000 HGNM-0.0.1/src/HGNM/modules/common/Embedding.py
--rw-rw-rw-   0        0        0     6771 2023-04-12 09:09:20.000000 HGNM-0.0.1/src/HGNM/modules/common/LatentMLP.py
--rw-rw-rw-   0        0        0     2420 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/common/UtilityModules.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/common/__init__.py
--rw-rw-rw-   0        0        0    11642 2023-04-12 09:22:02.000000 HGNM-0.0.1/src/HGNM/modules/common/hmpn_util.py
--rw-rw-rw-   0        0        0     3825 2023-04-05 06:38:40.000000 HGNM-0.0.1/src/HGNM/modules/get_message_passing_base.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:52.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/
--rw-rw-rw-   0        0        0     3853 2023-04-12 12:19:30.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousBlock.py
--rw-rw-rw-   0        0        0     4457 2023-04-12 12:13:54.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousGraphAssertions.py
--rw-rw-rw-   0        0        0     3374 2023-04-12 12:16:40.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousInputEmbedding.py
--rw-rw-rw-   0        0        0     6708 2023-04-12 12:27:20.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousMessagePassingBase.py
--rw-rw-rw-   0        0        0    11820 2023-04-12 12:12:17.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousModules.py
--rw-rw-rw-   0        0        0     9627 2023-04-12 12:13:20.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousStack.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:52.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/mock/
--rw-rw-rw-   0        0        0    13233 2023-04-12 15:11:09.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/mock/MockHeteroBase.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/heterogeneous/mock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:52.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/
--rw-rw-rw-   0        0        0     4317 2023-04-12 15:19:41.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousBlock.py
--rw-rw-rw-   0        0        0     3027 2023-04-12 15:16:32.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousGraphAssertions.py
--rw-rw-rw-   0        0        0     2782 2023-04-12 15:17:11.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousInputEmbedding.py
--rw-rw-rw-   0        0        0     6330 2023-04-12 15:21:47.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousMessagePassingBase.py
--rw-rw-rw-   0        0        0     6758 2023-04-12 15:17:47.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousModules.py
--rw-rw-rw-   0        0        0     3433 2023-04-12 15:18:25.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousStack.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/modules/homogeneous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:53.000000 HGNM-0.0.1/src/HGNM/util/
--rw-rw-rw-   0        0        0     2295 2023-04-03 09:18:46.000000 HGNM-0.0.1/src/HGNM/util/Keys.py
--rw-rw-rw-   0        0        0      843 2023-04-03 09:00:48.000000 HGNM-0.0.1/src/HGNM/util/Types.py
--rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 HGNM-0.0.1/src/HGNM/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1711 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-13 13:59:51.000000 HGNM-0.0.1/src/HGNM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/
+-rw-rw-rw-   0        0        0     1111 2023-03-30 09:55:00.000000 hgnm-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1130 2023-04-19 07:56:30.000000 hgnm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-04-19 07:44:31.000000 hgnm-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1579 2023-04-19 07:44:22.000000 hgnm-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:56:30.000000 hgnm-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/
+-rw-rw-rw-   0        0        0     1393 2023-04-18 19:43:12.000000 hgnm-0.0.2/src/HGNM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/abstract/
+-rw-rw-rw-   0        0        0     2037 2023-04-18 15:28:08.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractBlock.py
+-rw-rw-rw-   0        0        0     2353 2023-04-18 15:28:23.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractGraphAssertions.py
+-rw-rw-rw-   0        0        0     2252 2023-04-18 19:40:11.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractInputEmbedding.py
+-rw-rw-rw-   0        0        0     7501 2023-04-18 19:40:26.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractMessagePassingBase.py
+-rw-rw-rw-   0        0        0     2393 2023-04-04 09:20:24.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractModules.py
+-rw-rw-rw-   0        0        0     6444 2023-04-18 19:40:39.000000 hgnm-0.0.2/src/HGNM/modules/abstract/AbstractStack.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/abstract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/common/
+-rw-rw-rw-   0        0        0     2510 2023-04-18 19:40:58.000000 hgnm-0.0.2/src/HGNM/modules/common/Embedding.py
+-rw-rw-rw-   0        0        0     6767 2023-04-18 19:41:41.000000 hgnm-0.0.2/src/HGNM/modules/common/LatentMLP.py
+-rw-rw-rw-   0        0        0     2420 2023-04-18 19:41:52.000000 hgnm-0.0.2/src/HGNM/modules/common/UtilityModules.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/common/__init__.py
+-rw-rw-rw-   0        0        0    11630 2023-04-18 19:41:32.000000 hgnm-0.0.2/src/HGNM/modules/common/hmpn_util.py
+-rw-rw-rw-   0        0        0     3825 2023-04-05 06:38:40.000000 hgnm-0.0.2/src/HGNM/modules/get_message_passing_base.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/
+-rw-rw-rw-   0        0        0     3833 2023-04-18 15:22:08.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousBlock.py
+-rw-rw-rw-   0        0        0     4453 2023-04-18 15:24:46.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousGraphAssertions.py
+-rw-rw-rw-   0        0        0     3358 2023-04-18 15:25:06.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousInputEmbedding.py
+-rw-rw-rw-   0        0        0     6680 2023-04-18 15:25:27.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousMessagePassingBase.py
+-rw-rw-rw-   0        0        0    11808 2023-04-18 15:25:44.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousModules.py
+-rw-rw-rw-   0        0        0     9603 2023-04-18 15:25:59.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousStack.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/mock/
+-rw-rw-rw-   0        0        0    13213 2023-04-18 15:24:28.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/mock/MockHeteroBase.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/heterogeneous/mock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/
+-rw-rw-rw-   0        0        0     4301 2023-04-18 15:26:35.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousBlock.py
+-rw-rw-rw-   0        0        0     3019 2023-04-18 15:26:53.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousGraphAssertions.py
+-rw-rw-rw-   0        0        0     2770 2023-04-18 15:27:03.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousInputEmbedding.py
+-rw-rw-rw-   0        0        0     6302 2023-04-18 15:27:19.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousMessagePassingBase.py
+-rw-rw-rw-   0        0        0     6742 2023-04-18 15:27:40.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousModules.py
+-rw-rw-rw-   0        0        0     3421 2023-04-18 15:27:50.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousStack.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/modules/homogeneous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM/util/
+-rw-rw-rw-   0        0        0     2295 2023-04-03 09:18:46.000000 hgnm-0.0.2/src/HGNM/util/Keys.py
+-rw-rw-rw-   0        0        0      843 2023-04-03 09:00:48.000000 hgnm-0.0.2/src/HGNM/util/Types.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 14:33:36.000000 hgnm-0.0.2/src/HGNM/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:56:30.000000 hgnm-0.0.2/src/HGNM.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-04-19 07:56:29.000000 hgnm-0.0.2/src/HGNM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2023-04-19 07:56:29.000000 hgnm-0.0.2/src/HGNM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:56:29.000000 hgnm-0.0.2/src/HGNM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 07:56:29.000000 hgnm-0.0.2/src/HGNM.egg-info/top_level.txt
```

### Comparing `HGNM-0.0.1/LICENSE` & `hgnm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/PKG-INFO` & `hgnm-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: HGNM
-Version: 0.0.1
+Name: hgnm
+Version: 0.0.2
 Summary: A small library for the HGNM project. It contains the implementation of the HGNM model. 
-Author-email: Niklas Freimuth <niklas.freimuth@kit.edu>, Philipp Dahlinger <philipp.dahlinger@kit.edu>, Magnus Landwehr <magnus.landwehr@student.kit.edu>
+Author-email: Magnus Landwehr <magnus.landwehr@student.kit.edu>, Niklas Freimuth <niklas.freimuth@kit.edu>, Philipp Dahlinger <philipp.dahlinger@kit.edu>
 Maintainer-email: Niklas Freimuth <niklas.freimuth@kit.edu>
 Project-URL: Homepage, https://github.com/sungsy/HGNM
 Project-URL: Bug Tracker, https://github.com/sungsy/HGNM/issues
 Project-URL: Institute, https://alr.anthropomatik.kit.edu/index.php
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,13 +15,13 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.0
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Version 0.1.0
+Version 0.0.2
 
 
 # HGNM
 Pypi library for DAVIS - ALR - KIT
```

### Comparing `HGNM-0.0.1/pyproject.toml` & `hgnm-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 00000170: 2020 2320 226e 756d 7079 222c 0d0a 2020    # "numpy",..  
 00000180: 2020 2274 6f72 6368 222c 0d0a 2020 2020    "torch",..    
 00000190: 2274 6f72 6368 5f67 656f 6d65 7472 6963  "torch_geometric
 000001a0: 222c 0d0a 2020 2020 5d0d 0a62 7569 6c64  ",..    ]..build
 000001b0: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 000001c0: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 000001d0: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
-000001e0: 0a6e 616d 6520 3d20 2248 474e 4d22 0d0a  .name = "HGNM"..
-000001f0: 7665 7273 696f 6e20 3d20 2230 2e30 2e31  version = "0.0.1
+000001e0: 0a6e 616d 6520 3d20 2268 676e 6d22 0d0a  .name = "hgnm"..
+000001f0: 7665 7273 696f 6e20 3d20 2230 2e30 2e32  version = "0.0.2
 00000200: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
-00000210: 2020 7b20 6e61 6d65 3d22 4e69 6b6c 6173    { name="Niklas
-00000220: 2046 7265 696d 7574 6822 2c20 656d 6169   Freimuth", emai
-00000230: 6c3d 226e 696b 6c61 732e 6672 6569 6d75  l="niklas.freimu
-00000240: 7468 406b 6974 2e65 6475 2220 7d2c 0d0a  th@kit.edu" },..
-00000250: 2020 7b20 6e61 6d65 3d22 5068 696c 6970    { name="Philip
-00000260: 7020 4461 686c 696e 6765 7222 2c20 656d  p Dahlinger", em
-00000270: 6169 6c3d 2270 6869 6c69 7070 2e64 6168  ail="philipp.dah
-00000280: 6c69 6e67 6572 406b 6974 2e65 6475 227d  linger@kit.edu"}
-00000290: 2c0d 0a20 207b 206e 616d 653d 224d 6167  ,..  { name="Mag
-000002a0: 6e75 7320 4c61 6e64 7765 6872 222c 2065  nus Landwehr", e
-000002b0: 6d61 696c 3d22 6d61 676e 7573 2e6c 616e  mail="magnus.lan
-000002c0: 6477 6568 7240 7374 7564 656e 742e 6b69  dwehr@student.ki
+00000210: 2020 7b20 6e61 6d65 3d22 4d61 676e 7573    { name="Magnus
+00000220: 204c 616e 6477 6568 7222 2c20 656d 6169   Landwehr", emai
+00000230: 6c3d 226d 6167 6e75 732e 6c61 6e64 7765  l="magnus.landwe
+00000240: 6872 4073 7475 6465 6e74 2e6b 6974 2e65  hr@student.kit.e
+00000250: 6475 227d 2c0d 0a20 207b 206e 616d 653d  du"},..  { name=
+00000260: 224e 696b 6c61 7320 4672 6569 6d75 7468  "Niklas Freimuth
+00000270: 222c 2065 6d61 696c 3d22 6e69 6b6c 6173  ", email="niklas
+00000280: 2e66 7265 696d 7574 6840 6b69 742e 6564  .freimuth@kit.ed
+00000290: 7522 207d 2c0d 0a20 207b 206e 616d 653d  u" },..  { name=
+000002a0: 2250 6869 6c69 7070 2044 6168 6c69 6e67  "Philipp Dahling
+000002b0: 6572 222c 2065 6d61 696c 3d22 7068 696c  er", email="phil
+000002c0: 6970 702e 6461 686c 696e 6765 7240 6b69  ipp.dahlinger@ki
 000002d0: 742e 6564 7522 7d0d 0a5d 0d0a 6d61 696e  t.edu"}..]..main
 000002e0: 7461 696e 6572 7320 3d20 5b0d 0a20 2020  tainers = [..   
 000002f0: 207b 206e 616d 653d 224e 696b 6c61 7320   { name="Niklas 
 00000300: 4672 6569 6d75 7468 222c 2065 6d61 696c  Freimuth", email
 00000310: 3d22 6e69 6b6c 6173 2e66 7265 696d 7574  ="niklas.freimut
 00000320: 6840 6b69 742e 6564 7522 207d 2c0d 0a5d  h@kit.edu" },..]
 00000330: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description =
```

### Comparing `HGNM-0.0.1/src/HGNM/__init__.py` & `hgnm-0.0.2/src/HGNM/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# # make import easier 
+# make import easier 
 
 
-# # abstract modules
-# from src.HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding as AbInputEmbedding
-# from src.HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase as AbMessagePassingBase
-# from src.HGNM.modules.abstract.AbstractStack import AbstractStack as AbStack
-# from src.HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions as AbGraphAssertions
+# abstract modules
+from HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding as AbInputEmbedding
+from HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase as AbMessagePassingBase
+from HGNM.modules.abstract.AbstractStack import AbstractStack as AbStack
+from HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions as AbGraphAssertions
 
-# # heterogeneous modules
-# from src.HGNM.modules.heterogeneous.HeterogeneousInputEmbedding import HeterogeneousInputEmbedding as HeteroInputEmbedding
-# from src.HGNM.modules.heterogeneous.HeterogeneousMessagePassingBase import HeterogeneousMessagePassingBase as HeteroMessagePassingBase
-# from src.HGNM.modules.heterogeneous.HeterogeneousStack import HeterogeneousStack as HeteroStack
-# from src.HGNM.modules.heterogeneous.HeterogeneousGraphAssertions import HeterogeneousGraphAssertions as HeteroGraphAssertions
+# heterogeneous modules
+from HGNM.modules.heterogeneous.HeterogeneousInputEmbedding import HeterogeneousInputEmbedding as HeteroInputEmbedding
+from HGNM.modules.heterogeneous.HeterogeneousMessagePassingBase import HeterogeneousMessagePassingBase as HeteroMessagePassingBase
+from HGNM.modules.heterogeneous.HeterogeneousStack import HeterogeneousStack as HeteroStack
+from HGNM.modules.heterogeneous.HeterogeneousGraphAssertions import HeterogeneousGraphAssertions as HeteroGraphAssertions
 
-# # homogeneous modules
-# from src.HGNM.modules.homogeneous.HomogeneousInputEmbedding import HomogeneousInputEmbedding as HomoInputEmbedding
-# from src.HGNM.modules.homogeneous.HomogeneousMessagePassingBase import HomogeneousMessagePassingBase as HomoMessagePassingBase
-# from src.HGNM.modules.homogeneous.HomogeneousStack import HomogeneousStack as HomoStack
-# from src.HGNM.modules.homogeneous.HomogeneousGraphAssertions import HomogeneousGraphAssertions as HomoGraphAssertions
+# homogeneous modules
+from HGNM.modules.homogeneous.HomogeneousInputEmbedding import HomogeneousInputEmbedding as HomoInputEmbedding
+from HGNM.modules.homogeneous.HomogeneousMessagePassingBase import HomogeneousMessagePassingBase as HomoMessagePassingBase
+from HGNM.modules.homogeneous.HomogeneousStack import HomogeneousStack as HomoStack
+from HGNM.modules.homogeneous.HomogeneousGraphAssertions import HomogeneousGraphAssertions as HomoGraphAssertions
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractBlock.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractBlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from typing import Optional
 from torch import nn
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.hmpn_util import noop
+from HGNM.util.Types import *
+from HGNM.modules.common.hmpn_util import noop
 
 
 class AbstractBlock(nn.Module, abc.ABC):
     """
      Defines a single Message Passing Block that takes an observation graph and updates its node and edge
      features using different modules described in implementations of this abstract class.
      It first updates the edge-features. The node-features are updated next using the new edge-features. Finally,
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractGraphAssertions.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractGraphAssertions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 from typing import Dict, Optional, Tuple, Union
 from torch_geometric.data.data import BaseData
-from src.HGNM.modules.common.hmpn_util import noop
+from HGNM.modules.common.hmpn_util import noop
 
 class AbstractGraphAssertions(abc.ABC):
     """
     Asserts that the input graph has the correct shape.
     """
     def __init__(self, *,
                  in_node_features: Union[int, Dict[str, int]],
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractInputEmbedding.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractInputEmbedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 # from torch import nn
 from typing import Optional
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.Embedding import Embedding
+from HGNM.util.Types import *
+from HGNM.modules.common.Embedding import Embedding
 
 
 class AbstractInputEmbedding(torch.nn.Module):
     """
     Parent class to heterogeneous and homogeneous input embeddings. Embeds global features.
     """
     def __init__(self,
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractMessagePassingBase.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractMessagePassingBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import abc
 import torch
 # from torch import nn
 from typing import Optional, Tuple, Callable
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.hmpn_util import get_scatter_reducers, get_create_copy
-from src.HGNM.modules.common.hmpn_util import noop
-from src.HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
-from src.HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
-from src.HGNM.modules.abstract.AbstractStack import AbstractStack
-from src.HGNM.util.Keys import AGENT
+from HGNM.util.Types import *
+from HGNM.modules.common.hmpn_util import get_scatter_reducers, get_create_copy
+from HGNM.modules.common.hmpn_util import noop
+from HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
+from HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
+from HGNM.modules.abstract.AbstractStack import AbstractStack
+from HGNM.util.Keys import AGENT
 
 
 class AbstractMessagePassingBase(torch.nn.Module, abc.ABC):
     """
     The Message Passing base contains the feature embedding as well as all the message passing blocks.
     Its output is a graph or a tuple of node_features, edge_features, global_features, batch_indices with
     feature dimension of latent_dimension.
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractModules.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractModules.py`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/src/HGNM/modules/abstract/AbstractStack.py` & `hgnm-0.0.2/src/HGNM/modules/abstract/AbstractStack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import copy
 import torch.nn as nn
 from typing import Optional
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.hmpn_util import noop
+from HGNM.util.Types import *
+from HGNM.modules.common.hmpn_util import noop
 
 
 class AbstractStack(nn.Module, abc.ABC):
     """
     Message Passing module that acts on both node and edge features used for observation graphs.
     Internally stacks multiple instances of MessagePassingBlock.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/common/Embedding.py` & `hgnm-0.0.2/src/HGNM/modules/common/Embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from torch import nn
 from typing import Optional
-from src.HGNM.modules.common.UtilityModules import EmptyLinear
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.LatentMLP import LatentMLP
+from HGNM.modules.common.UtilityModules import EmptyLinear
+from HGNM.util.Types import *
+from HGNM.modules.common.LatentMLP import LatentMLP
 
 
 class Embedding(nn.Module):
     """
     Linear Embedding module. Essentially a learned matrix multiplication (and a bias) to make input dimension of tokens
     compatible with the "main" architecture that uses them.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/common/LatentMLP.py` & `hgnm-0.0.2/src/HGNM/modules/common/LatentMLP.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from torch import nn as nn
 import torch
 from torch.nn import utils
 import numpy as np
-from src.HGNM.util.Types import *
+from HGNM.util.Types import *
 
 
 class SwiGlu(nn.Module):
     def __init__(self, in_features, out_features):
         super(SwiGlu, self).__init__()
         self.l1 = nn.Linear(in_features, out_features)
         self.l2 = nn.Linear(in_features, out_features)
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/common/UtilityModules.py` & `hgnm-0.0.2/src/HGNM/modules/common/UtilityModules.py`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/src/HGNM/modules/common/hmpn_util.py` & `hgnm-0.0.2/src/HGNM/modules/common/hmpn_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import Counter
 from typing import Dict, Tuple
 
 import torch
 import torch_geometric
 import copy
 
-from src.HGNM.util.Types import *
-from src.HGNM.util import Keys, Keys as Keys
-from src.HGNM.util.Keys import AGGR_AGGR, CONCAT_AGGR, AGENT
+from HGNM.util.Types import *
+from HGNM.util import Keys, Keys as Keys
+from HGNM.util.Keys import AGGR_AGGR, CONCAT_AGGR, AGENT
 
 
 def get_default_edge_relation(sender_node_type: str, receiver_node_type: str,
                               include_nodes: bool = True) -> Union[str, Tuple[str, str, str]]:
     """
     Wrapper function for uniform edge identifiers. Builds a string 'sender_node_type+"2"+receiver_node_type'
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/get_message_passing_base.py` & `hgnm-0.0.2/src/HGNM/modules/get_message_passing_base.py`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousBlock.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousBlock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from torch import nn
 from typing import Callable
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.abstract.AbstractBlock import AbstractBlock
-from src.HGNM.modules.heterogeneous.HeterogeneousModules import HeterogeneousEdgeModule, \
+from HGNM.util.Types import *
+from HGNM.modules.abstract.AbstractBlock import AbstractBlock
+from HGNM.modules.heterogeneous.HeterogeneousModules import HeterogeneousEdgeModule, \
     HeterogeneousNodeModule, HeterogeneousGlobalModule
-from src.HGNM.modules.common.hmpn_util import noop
-from src.HGNM.modules.common.LatentMLP import LatentMLP
+from HGNM.modules.common.hmpn_util import noop
+from HGNM.modules.common.LatentMLP import LatentMLP
 
 
 class HeterogeneousBlock(AbstractBlock):
     """
          Defines a single Message Passing Block that takes a heterogeneous observation graph and updates its node and edge
          features using different modules (Edge, Node, Global).
          It first updates the edge-features. The node-features are updated next using the new edge-features. Finally,
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousGraphAssertions.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousGraphAssertions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional, Tuple
 from torch_geometric.data import Batch
 
-from src.HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
+from HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
 
 
 class HeterogeneousGraphAssertions(AbstractGraphAssertions):
 
     def __init__(self, *,
                  in_node_features: Dict[str, int],
                  in_edge_features: Dict[Tuple[str, str, str], int],
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousInputEmbedding.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousInputEmbedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from torch import nn
 from typing import Optional, Tuple
 import torch
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.Embedding import Embedding
-from src.HGNM.modules.common.hmpn_util import tuple_to_string
-from src.HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
+from HGNM.util.Types import *
+from HGNM.modules.common.Embedding import Embedding
+from HGNM.modules.common.hmpn_util import tuple_to_string
+from HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
 
 
 class HeterogeneousInputEmbedding(AbstractInputEmbedding):
     """
     Input feature embedding for Heterogeneous Graphs.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousMessagePassingBase.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousMessagePassingBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
 import torch
 import torch.nn as nn
 from typing import Optional, Tuple
 
-from src.HGNM.util.Types import *
-from src.HGNM.util.Keys import AGENT
+from HGNM.util.Types import *
+from HGNM.util.Keys import AGENT
 
-from src.HGNM.modules.heterogeneous.HeterogeneousInputEmbedding import HeterogeneousInputEmbedding
-from src.HGNM.modules.heterogeneous.HeterogeneousStack import HeterogeneousStack
-from src.HGNM.modules.heterogeneous.HeterogeneousGraphAssertions import HeterogeneousGraphAssertions
-from src.HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase
-from src.HGNM.modules.common.hmpn_util import noop, unpack_heterogeneous_features
+from HGNM.modules.heterogeneous.HeterogeneousInputEmbedding import HeterogeneousInputEmbedding
+from HGNM.modules.heterogeneous.HeterogeneousStack import HeterogeneousStack
+from HGNM.modules.heterogeneous.HeterogeneousGraphAssertions import HeterogeneousGraphAssertions
+from HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase
+from HGNM.modules.common.hmpn_util import noop, unpack_heterogeneous_features
 
 
 class HeterogeneousMessagePassingBase(AbstractMessagePassingBase):
     """
         Graph Neural Network (GNN) Base module processes the graph observations of the environment.
         It uses a stack of GNN Blocks. Each block defines a single GNN pass.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousModules.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousModules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch.nn as nn
 import torch
 from typing import Callable
 
-from src.HGNM.modules.abstract.AbstractModules import AbstractMetaModule
-from src.HGNM.util.Types import *
-from src.HGNM.util.Keys import AGGR_AGGR
+from HGNM.modules.abstract.AbstractModules import AbstractMetaModule
+from HGNM.util.Types import *
+from HGNM.util.Keys import AGGR_AGGR
 
 
 
 class HeterogeneousMetaModule(AbstractMetaModule):
     """
     Base class for the heterogeneous modules used in the GNN.
     They are used for updating node-, edge-, and global features.
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/HeterogeneousStack.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/HeterogeneousStack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from torch import nn
 from typing import Callable, Tuple
 
-from src.HGNM.modules.common.hmpn_util import count_in_node_features
-from src.HGNM.util.Types import *
-from src.HGNM.modules.abstract.AbstractStack import AbstractStack
-from src.HGNM.modules.heterogeneous.HeterogeneousBlock import HeterogeneousBlock
-from src.HGNM.modules.common.LatentMLP import LatentMLP
-from src.HGNM.util.Keys import AGGR_AGGR
+from HGNM.modules.common.hmpn_util import count_in_node_features
+from HGNM.util.Types import *
+from HGNM.modules.abstract.AbstractStack import AbstractStack
+from HGNM.modules.heterogeneous.HeterogeneousBlock import HeterogeneousBlock
+from HGNM.modules.common.LatentMLP import LatentMLP
+from HGNM.util.Keys import AGGR_AGGR
 
 
 class HeterogeneousStack(AbstractStack):
     """
     Message Passing module that acts on both node and edge features.
     Internally stacks multiple instances of MessagePassingBlocks.
     This implementation is used for heterogeneous observation graphs.
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/heterogeneous/mock/MockHeteroBase.py` & `hgnm-0.0.2/src/HGNM/modules/heterogeneous/mock/MockHeteroBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import torch_geometric
 from typing import Optional, Tuple
 
-from src.HGNM.util.Types import *
-from src.HGNM.util.Keys import AGENT
-from src.HGNM.modules.common.hmpn_util import noop, unpack_heterogeneous_features
-from src.HGNM.modules.common.hmpn_util import get_create_copy
-from src.HGNM.modules.homogeneous.HomogeneousMessagePassingBase import HomogeneousMessagePassingBase
+from HGNM.util.Types import *
+from HGNM.util.Keys import AGENT
+from HGNM.modules.common.hmpn_util import noop, unpack_heterogeneous_features
+from HGNM.modules.common.hmpn_util import get_create_copy
+from HGNM.modules.homogeneous.HomogeneousMessagePassingBase import HomogeneousMessagePassingBase
 
 
 class MockHeteroBase(HomogeneousMessagePassingBase):
     """
     Calls like a heterogeneous base but uses a homogeneous base with broad input features that get sparsely populated.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousBlock.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousBlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.HGNM.util.Types import *
-from src.HGNM.modules.abstract.AbstractBlock import AbstractBlock
-from src.HGNM.modules.homogeneous.HomogeneousModules import HomogeneousEdgeModule, \
+from HGNM.util.Types import *
+from HGNM.modules.abstract.AbstractBlock import AbstractBlock
+from HGNM.modules.homogeneous.HomogeneousModules import HomogeneousEdgeModule, \
     HomogeneousNodeModule, HomogeneousGlobalModule
-from src.HGNM.modules.common.hmpn_util import noop
+from HGNM.modules.common.hmpn_util import noop
 
 
 class HomogeneousBlock(AbstractBlock):
     """
          Defines a single MessagePassingLayer that takes a homogeneous observation graph and updates its node and edge
          features using different modules (Edge, Node, Global).
          It first updates the edge-features. The node-features are updated next using the new edge-features. Finally,
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousGraphAssertions.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousGraphAssertions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Tuple
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
+from HGNM.util.Types import *
+from HGNM.modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
 
 
 class HomogeneousGraphAssertions(AbstractGraphAssertions):
 
     def __init__(self, *,
                  in_node_features: Dict[str, int],
                  in_edge_features: Dict[Tuple[str, str, str], int],
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousInputEmbedding.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousInputEmbedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 import torch
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.Embedding import Embedding
-from src.HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
+from HGNM.util.Types import *
+from HGNM.modules.common.Embedding import Embedding
+from HGNM.modules.abstract.AbstractInputEmbedding import AbstractInputEmbedding
 
 
 class HomogeneousInputEmbedding(AbstractInputEmbedding):
     def __init__(self,
                  *,
                  in_node_features: int,
                  in_edge_features: int,
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousMessagePassingBase.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousMessagePassingBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 from typing import Optional
 
 # from modules.abstract.AbstractGraphAssertions import AbstractGraphAssertions
-from src.HGNM.util.Types import *
-from src.HGNM.util.Keys import AGENT
-from src.HGNM.modules.homogeneous.HomogeneousInputEmbedding import HomogeneousInputEmbedding
-from src.HGNM.modules.homogeneous.HomogeneousStack import HomogeneousStack
-from src.HGNM.modules.homogeneous.HomogeneousGraphAssertions import HomogeneousGraphAssertions
-from src.HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase
-from src.HGNM.modules.common.hmpn_util import noop, unpack_homogeneous_features
+from HGNM.util.Types import *
+from HGNM.util.Keys import AGENT
+from HGNM.modules.homogeneous.HomogeneousInputEmbedding import HomogeneousInputEmbedding
+from HGNM.modules.homogeneous.HomogeneousStack import HomogeneousStack
+from HGNM.modules.homogeneous.HomogeneousGraphAssertions import HomogeneousGraphAssertions
+from HGNM.modules.abstract.AbstractMessagePassingBase import AbstractMessagePassingBase
+from HGNM.modules.common.hmpn_util import noop, unpack_homogeneous_features
 
 
 class HomogeneousMessagePassingBase(AbstractMessagePassingBase):
     """
     # todo write nice comments
 
         Graph Neural Network (GNN) Base module processes the graph observations of the environment.
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousModules.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousModules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch.nn as nn
 import torch
 from torch_geometric.data import Batch
 from typing import Callable
 
-from src.HGNM.modules.abstract.AbstractModules import AbstractMetaModule
-from src.HGNM.util.Types import *
-from src.HGNM.modules.common.LatentMLP import LatentMLP
-from src.HGNM.modules.common.hmpn_util import noop
+from HGNM.modules.abstract.AbstractModules import AbstractMetaModule
+from HGNM.util.Types import *
+from HGNM.modules.common.LatentMLP import LatentMLP
+from HGNM.modules.common.hmpn_util import noop
 
 
 class HomogeneousMetaModule(AbstractMetaModule):
     """
     Base class for the homogeneous modules used in the GNN.
     They are used for updating node-, edge-, and global features.
     """
```

### Comparing `HGNM-0.0.1/src/HGNM/modules/homogeneous/HomogeneousStack.py` & `hgnm-0.0.2/src/HGNM/modules/homogeneous/HomogeneousStack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from torch import nn
 from typing import Callable
 
-from src.HGNM.util.Types import *
-from src.HGNM.modules.abstract.AbstractStack import AbstractStack
-from src.HGNM.modules.homogeneous.HomogeneousBlock import HomogeneousBlock
+from HGNM.util.Types import *
+from HGNM.modules.abstract.AbstractStack import AbstractStack
+from HGNM.modules.homogeneous.HomogeneousBlock import HomogeneousBlock
 
 
 class HomogeneousStack(AbstractStack):
     """
     Message Passing module that acts on both node and edge features.
     Internally stacks multiple instances of MessagePassingBlocks.
     This implementation is used for homogeneous observation graphs.
```

### Comparing `HGNM-0.0.1/src/HGNM/util/Keys.py` & `hgnm-0.0.2/src/HGNM/util/Keys.py`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/src/HGNM/util/Types.py` & `hgnm-0.0.2/src/HGNM/util/Types.py`

 * *Files identical despite different names*

### Comparing `HGNM-0.0.1/src/HGNM.egg-info/PKG-INFO` & `hgnm-0.0.2/src/HGNM.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: HGNM
-Version: 0.0.1
+Name: hgnm
+Version: 0.0.2
 Summary: A small library for the HGNM project. It contains the implementation of the HGNM model. 
-Author-email: Niklas Freimuth <niklas.freimuth@kit.edu>, Philipp Dahlinger <philipp.dahlinger@kit.edu>, Magnus Landwehr <magnus.landwehr@student.kit.edu>
+Author-email: Magnus Landwehr <magnus.landwehr@student.kit.edu>, Niklas Freimuth <niklas.freimuth@kit.edu>, Philipp Dahlinger <philipp.dahlinger@kit.edu>
 Maintainer-email: Niklas Freimuth <niklas.freimuth@kit.edu>
 Project-URL: Homepage, https://github.com/sungsy/HGNM
 Project-URL: Bug Tracker, https://github.com/sungsy/HGNM/issues
 Project-URL: Institute, https://alr.anthropomatik.kit.edu/index.php
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,13 +15,13 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.0
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Version 0.1.0
+Version 0.0.2
 
 
 # HGNM
 Pypi library for DAVIS - ALR - KIT
```

### Comparing `HGNM-0.0.1/src/HGNM.egg-info/SOURCES.txt` & `hgnm-0.0.2/src/HGNM.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,12 @@
 src/HGNM/modules/homogeneous/HomogeneousInputEmbedding.py
 src/HGNM/modules/homogeneous/HomogeneousMessagePassingBase.py
 src/HGNM/modules/homogeneous/HomogeneousModules.py
 src/HGNM/modules/homogeneous/HomogeneousStack.py
 src/HGNM/modules/homogeneous/__init__.py
 src/HGNM/util/Keys.py
 src/HGNM/util/Types.py
-src/HGNM/util/__init__.py
+src/HGNM/util/__init__.py
+src/hgnm.egg-info/PKG-INFO
+src/hgnm.egg-info/SOURCES.txt
+src/hgnm.egg-info/dependency_links.txt
+src/hgnm.egg-info/top_level.txt
```

