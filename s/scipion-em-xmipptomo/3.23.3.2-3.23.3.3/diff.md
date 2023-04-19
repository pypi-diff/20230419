# Comparing `tmp/scipion-em-xmipptomo-3.23.3.2.tar.gz` & `tmp/scipion-em-xmipptomo-3.23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipptomo-3.23.3.2.tar", last modified: Tue Apr  4 10:14:37 2023, max compression
+gzip compressed data, was "scipion-em-xmipptomo-3.23.3.3.tar", last modified: Wed Apr 19 08:35:26 2023, max compression
```

## Comparing `scipion-em-xmipptomo-3.23.3.2.tar` & `scipion-em-xmipptomo-3.23.3.3.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.606464 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 10:14:37.000000 scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.606464 scipion-em-xmipptomo-3.23.3.2/xmipptomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_align_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_applyAlignmentTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_coords_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_crop_resize_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_crop_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_half_maps_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_phantom_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resizeTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_roiIJ.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_score_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_score_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_splitTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_subtomo_map_back.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_subtraction_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    29950 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_xmipptomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:14:37.610464 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/monotomo_tree_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_score_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-04 10:12:27.000000 scipion-em-xmipptomo-3.23.3.2/xmipptomo/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.769371 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.769371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_align_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_applyAlignmentTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_coords_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_resize_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_half_maps_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resizeTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_roiIJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_splitTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtomo_map_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtraction_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_xmipptomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/monotomo_tree_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_score_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/xmipp_logo.png
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/CHANGES.txt` & `scipion-em-xmipptomo-3.23.3.3/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+V3.23.03.3:
+ - Fit vesicles removed (moved to tomo)
+ -
 V3.23.03.2:
  - Mapback scales any reference to match the tomogram sampling.
 V3.23.03.1:
  - Subtomo projector compatible with hdf stacks. Test fixed. Projections keep orientation.
 
 V3.23.03.0:
  - New protocol and test extract_subtomos
@@ -47,18 +50,14 @@
       Protocol to crop tomograms using xmipp_transform_window.
       The protocol allows to change the size of a tomogram/s, by removing the
       borders defined by the users
 
    xmipptomo - Filter coordinates by map ( XmippProtFilterCoordinatesByMap ):
       Filter coordinate by map both given a mask or a resolucion map from a tomogram
 
-   xmipptomo - fit vesicles ( XmippProtFitEllipsoid ):
-      This protocol adjust a SetOfSubtomograms with coordinates assigned or a SetOfCoordinates3D, to a vesicle
-      (ellipsoid), defining regions of interest (SetOfMeshes) for each vesicle as output.
-
    xmipptomo - half maps ( XmippProtHalfMapsSubtomo ):
       Create half maps from a SetOfSubtomograms and its alignment
 
    xmipptomo - local Resolution MonoTomo ( XmippProtMonoTomo ):
       Given a tomogram the protocol assigns local resolutions to each voxel of the tomogram.
       To do that, thje protocol makes use of two half tomograms, called odd and even.
       These tomograms are reconstructed with the same alignment parameter but using the
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/LICENSE` & `scipion-em-xmipptomo-3.23.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.2
+Version: 3.23.3.3
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.2
+Version: 3.23.3.3
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/scipion_em_xmipptomo.egg-info/SOURCES.txt` & `scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 xmipptomo/protocols/protocol_cltomo.py
 xmipptomo/protocols/protocol_connected_components.py
 xmipptomo/protocols/protocol_coords_roi.py
 xmipptomo/protocols/protocol_crop_resize_base.py
 xmipptomo/protocols/protocol_crop_tomograms.py
 xmipptomo/protocols/protocol_extract_subtomos.py
 xmipptomo/protocols/protocol_filter_coordinates_by_map.py
-xmipptomo/protocols/protocol_fit_ellipsoid.py
 xmipptomo/protocols/protocol_flexalign.py
 xmipptomo/protocols/protocol_half_maps_subtomos.py
 xmipptomo/protocols/protocol_phantom_subtomo.py
 xmipptomo/protocols/protocol_phantom_tomo.py
 xmipptomo/protocols/protocol_project_top.py
 xmipptomo/protocols/protocol_resizeTS.py
 xmipptomo/protocols/protocol_resize_tomograms.py
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/setup.py` & `scipion-em-xmipptomo-3.23.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/__init__.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # **************************************************************************
 import xmipp3
 import subprocess, os
 import pyworkflow.utils as pwutils
 
 _logo = "xmipp_logo.png"
 _references = ['delaRosaTrevin2013']
-__version__ = "3.23.03.2" #X.YY.MM.sv
+__version__ = "3.23.03.3" #X.YY.MM.sv
         # X.Y.M = version of the xmipp release associated.
         # sv = Set this to ".0" on each xmipp  release.
         # For not release version (hotfix) increase it --> ".1", ".2", ...
 
 class Plugin(xmipp3.Plugin):
 
     @classmethod
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/bibtex.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/__init__.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from .protocol_applyAlignmentTS import XmippProtApplyTransformationMatrixTS
 from .protocol_cltomo import XmippProtCLTomo
 from .protocol_connected_components import XmippProtConnectedComponents
 from .protocol_coords_roi import XmippProtCCroi
 from .protocol_filter_coordinates_by_map import XmippProtFilterCoordinatesByMap
 from .protocol_crop_tomograms import XmippProtCropTomograms
 from .protocol_extract_subtomos import XmippProtExtractSubtomos
-from .protocol_fit_ellipsoid import XmippProtFitEllipsoid
 from .protocol_flexalign import XmippProtTsFlexAlign
 from .protocol_phantom_subtomo import XmippProtPhantomSubtomo
 from .protocol_phantom_tomo import XmippProtPhantomTomo
 from .protocol_project_top import XmippProtSubtomoProject
 from .protocol_resizeTS import XmippProtResizeTiltSeries
 from .protocol_resize_tomograms import XmippProtResizeTomograms
 from .protocol_resolution_local_monotomo import XmippProtMonoTomo
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_align_transform.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_align_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_applyAlignmentTS.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_applyAlignmentTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_apply_alignment_subtomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_apply_alignment_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_cltomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_connected_components.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_connected_components.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_coords_roi.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_coords_roi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_crop_resize_base.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_resize_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_crop_tomograms.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_filter_coordinates_by_map.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_filter_coordinates_by_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_fit_ellipsoid.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_project_top.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Estrella Fernandez Gimenez (me.fernandez@cnb.csic.es)
-# *
-# *  BCU, Centro Nacional de Biotecnologia, CSIC
+# * Authors:     David Herreros Calero (dherreros@cnb.csic.es)
+# *              Estrella Fernandez Gimenez (me.fernandez@cnb.csic.es)
 # *
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,183 +20,184 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import enum
 
-from os.path import basename, dirname, join
 import numpy as np
+from pwem.emlib.image import ImageHandler as ih
+from pwem.emlib import lib
+from pwem.objects import Particle, Volume, Transform, String, SetOfVolumes, SetOfParticles
+from pwem.protocols import ProtAnalysis3D
 from pyworkflow import BETA
-from pyworkflow.protocol.params import PointerParam
-import pyworkflow.utils as pwutlis
-from pwem.protocols import EMProtocol
-from tomo.protocols import ProtTomoBase
-from tomo.objects import MeshPoint, Ellipsoid, SubTomogram
-from tomo.utils import fit_ellipsoid, generatePointCloud
-import tomo.constants as const
-
-
-class XmippProtFitEllipsoid(EMProtocol, ProtTomoBase):
-    """ This protocol adjust a SetOfSubtomograms with coordinates assigned or a SetOfCoordinates3D, to a vesicle
-    (ellipsoid), defining regions of interest (SetOfMeshes) for each vesicle as output."""
+from pyworkflow.protocol.params import PointerParam, EnumParam, IntParam, BooleanParam
+from tomo.objects import SetOfSubTomograms
 
-    _label = 'fit vesicles'
+class SubtomoProjectOutput(enum.Enum):
+    particles = SetOfParticles
+    average = Particle
+
+class XmippProtSubtomoProject(ProtAnalysis3D):
+    """
+    Project a set of volumes or subtomograms to obtain their X, Y or Z projection of the desired range of slices.
+    """
+    _label = 'subtomo projection'
     _devStatus = BETA
+    _possibleOutputs = SubtomoProjectOutput
 
-    def __init__(self, **args):
-        EMProtocol.__init__(self, **args)
+    _dirChoices = ['X', 'Y', 'Z']
 
     # --------------------------- DEFINE param functions ------------------------
     def _defineParams(self, form):
-        form.addSection(label='Input')
-        form.addParam('input', PointerParam, pointerClass="SetOfSubTomograms, SetOfCoordinates3D",
-                      label='Subtomograms/Coordinates3D',
-                      help='Subtomograms or coordinates3D picked in vesicles. If there are more than one vesicle per '
-                           'tomogram, input subtomograms or coordinates should have assigned groupId.')
-        form.addParam('inputTomos', PointerParam, label="Tomograms", pointerClass='SetOfTomograms',
-                      help='Select tomograms from which subtomograms come.')
+        form.addSection(label='General parameters')
+        form.addParam('input', PointerParam, pointerClass=[SetOfSubTomograms, SetOfVolumes],
+                      label='Input Volumes', help='This protocol can *not* work with .em files *if* the input is a set'
+                                                  ' of tomograms or a set of volumes, ')
+        form.addParam('radAvg', BooleanParam, default=False, label='Compute radial average?',
+                      help='Compute the radial average with respect to Z of the input volumes and from them, '
+                           'it computes their projections in the desired direction')
+        form.addParam('dirParam', EnumParam, choices=self._dirChoices, default=2, display=EnumParam.DISPLAY_HLIST,
+                      label='Projection direction', condition='radAvg == False')
+        form.addParam('rangeParam', EnumParam, choices=['All', 'Range'], default=0, display=EnumParam.DISPLAY_HLIST,
+                      label='Range of slices', condition='radAvg == False',
+                      help='Range of slices used to compute the projection, where 0 is the central slice.')
+        form.addParam('cropParam', IntParam, default=10, label='Slices', condition="rangeParam == 1",
+                      help='Crop this amount of voxels in each side of the selected direction.')
 
-    # --------------------------- INSERT steps functions --------------------------------------------
+    # --------------------------- INSERT steps functions ------------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep('fitEllipsoidStep')
-        self._insertFunctionStep('createOutputStep')
+
+        self._insertFunctionStep(self.projectStep)
+        self._insertFunctionStep(self.createOutputStep)
 
     # --------------------------- STEPS functions -------------------------------
-    def fitEllipsoidStep(self):
+    def projectStep(self):
         input = self.input.get()
-        inputTomos = self.inputTomos.get()
-        self.outSet = self._createSetOfMeshes(inputTomos)
-        totalMeshes = 0
-        for tomo in inputTomos.iterItems(iterate=False):
-            vesicleList = []
-            vesicleIdList = []
-            tomoName = basename(tomo.getFileName())
-            tomoDim = [float(d) for d in tomo.getDim()]
-            firstItem = input.getFirstItem()
-            if self._getInputisSubtomo(firstItem):
-                dirName = dirname(firstItem.getVolName())
-                for item in input.iterItems(where="_volName='%s'" % join(dirName, tomoName)):
-                    vesicleId = self._getVesicleId(item)
-                    if vesicleId not in vesicleIdList:
-                        vesicleIdList.append(vesicleId)
-                        vesicle = self._createSetOfSubTomograms('_' + pwutlis.removeBaseExt(tomoName) +
-                                                                '_vesicle_' + str(vesicleId))
-                        vesicleList.append(vesicle)
-                    idx = vesicleIdList.index(vesicleId)
-                    vesicleList[idx].append(item)
+        x, y, z = input.getDim()
+
+        print("Dimensions (x,y,z) are: %s, %s, %s." % (x,y,z))
+
+
+        dir = self.dirParam.get()
+        partialProjection = self.rangeParam.get() == 1
+
+        if partialProjection:
+            bottomSlice = int(x/2 - self.cropParam.get())
+            topSlice = int(x/2 + self.cropParam.get())
+
 
+        fnProj = self._getExtraPath("projections.mrcs")
+        lib.createEmptyFile(fnProj, x, y, 1, input.getSize())
+
+        tmpOrientedSubtomoFn = self._getExtraPath("oriented.mrc")
+
+        for subtomo in input.iterItems():
+
+            fn = "%s@%s" % subtomo.getLocation()
+            if fn.endswith('.mrc'):
+                fn += ':mrc'
+
+            if subtomo.hasTransform():
+
+                ih().rotateVolume(fn, tmpOrientedSubtomoFn, subtomo.getTransform())
+                fn = tmpOrientedSubtomoFn
+
+            vol = ih().read(fn)
+            img = ih().createImage()
+
+            if self.radAvg.get():
+                img = vol.radialAverageAxis()
             else:
-                for item in input.iterCoordinates(volume=tomo):
-                    vesicleId = self._getVesicleId(item)
-                    if vesicleId not in vesicleIdList:
-                        vesicleIdList.append(vesicleId)
-                        vesicle = self._createSetOfCoordinates3D(inputTomos, '_' + pwutlis.removeBaseExt(tomoName)
-                                                                 + '_vesicle_' + str(vesicleId))
-                        vesicleList.append(vesicle)
-                    idx = vesicleIdList.index(vesicleId)
-                    vesicleList[idx].append(item)
-
-            totalMeshes += len(vesicleList)
-
-            for vesicle in vesicleList:
-                x = []
-                y = []
-                z = []
-
-                if self._getInputisSubtomo(input.getFirstItem()):
-                    for item in vesicle.iterItems():
-                        coord = self._getCoor(item)
-                        x.append(float(coord.getX(const.BOTTOM_LEFT_CORNER)) / tomoDim[0])
-                        y.append(float(coord.getY(const.BOTTOM_LEFT_CORNER)) / tomoDim[1])
-                        z.append(float(coord.getZ(const.BOTTOM_LEFT_CORNER)) / tomoDim[2])
-                else:
-                    for item in vesicle.iterCoordinates(volume=tomo):
-                        coord = self._getCoor(item)
-                        x.append(float(coord.getX(const.BOTTOM_LEFT_CORNER)) / tomoDim[0])
-                        y.append(float(coord.getY(const.BOTTOM_LEFT_CORNER)) / tomoDim[1])
-                        z.append(float(coord.getZ(const.BOTTOM_LEFT_CORNER)) / tomoDim[2])
-
-                [center, radii, v, _, chi2] = fit_ellipsoid(np.array(x), np.array(y), np.array(z))
-                algDesc = '%f*x*x + %f*y*y + %f*z*z + 2*%f*x*y + 2*%f*x*z + 2*%f*y*z + 2*%f*x + 2*%f*y + 2*%f*z + %f ' \
-                          '= 0' % (v[0], v[1], v[2], v[3], v[4], v[5], v[6], v[7], v[8], v[9])
-                adjEllipsoid = Ellipsoid()
-                adjEllipsoid.setAlgebraicDesc(algDesc)
-                adjEllipsoid.setCenter(str(center))
-                adjEllipsoid.setRadii(str(radii))
-                print(algDesc)
-                print('Chi2: ', chi2)
-                pointCloud = generatePointCloud(v, tomo.getDim())
-                if not pointCloud:
-                    raise Exception("It does not seem like any output is produced!")
-
-                for point in pointCloud:
-                    meshPoint = MeshPoint()
-                    meshPoint.setVolume(tomo.clone())
-                    meshPoint.setX(point[0], const.BOTTOM_LEFT_CORNER)
-                    meshPoint.setY(point[1], const.BOTTOM_LEFT_CORNER)
-                    meshPoint.setZ(point[2], const.BOTTOM_LEFT_CORNER)
-                    meshPoint.setGroupId(self._getVesicleId(item))
-                    meshPoint.setDescription(adjEllipsoid)
-                    meshPoint.setVolumeName(basename(tomo.getFileName()))
-                    self.outSet.append(meshPoint)
-        self.outSet.setPrecedents(inputTomos)
-        self.outSet.setNumberOfMeshes(totalMeshes)
+                volData = vol.getData()
 
-    def createOutputStep(self):
-        self._defineOutputs(outputMeshes=self.outSet)
-        self._defineSourceRelation(self.inputTomos.get(), self.outSet)
+                proj = np.empty([x, y])
 
-    # --------------------------- INFO functions --------------------------------
-    def _validate(self):
-        validateMsgs = []
-        input = self.input.get()
-        if input.getSize() < 9:
-            validateMsgs.append('At least 9 subtomograms/coordinates are required to fit a unique ellipsoid')
-        if self._getInputisSubtomo(self.input.get().getFirstItem()):
-            if not input.getFirstItem().hasCoordinate3D():
-                validateMsgs.append('Subtomograms should have coordinates')
-        return validateMsgs
+                # X axis
+                if dir == 0:
+                    if partialProjection:
+                        volData = volData[:, :, bottomSlice:topSlice]
+                    for zi in range(z):
+                        for yi in range(y):
+                            proj[yi, zi] = np.sum(volData[zi, yi, :])
+                # Y axis
+                elif dir == 1:
+                    if partialProjection:
+                        volData = volData[:, bottomSlice:topSlice, :]
+                    for zi in range(z):
+                        for xi in range(x):
+                            proj[zi, xi] = np.sum(volData[zi, :, xi])
+                # Z axis
+                elif dir == 2:
+                    if partialProjection:
+                        volData = volData[bottomSlice:topSlice, :, :]
+                    for xi in range(x):
+                        for yi in range(y):
+                            proj[yi, xi] = np.sum(volData[:, yi, xi])
 
-    def _summary(self):
-        summary = []
-        if not self.isFinished():
-            summary.append("Output vesicles not ready yet.")
-        else:
-            summary.append("%d subtomograms/coordinates3D from %d tomograms\n%d vesicles adjusted" %
-                           (self.input.get().getSize(), self.inputTomos.get().getSize(),
-                            self.outputMeshes.getNumberOfMeshes()))
-        return summary
+                # Make the projection to be the image data
+                img.setData(proj)
+
+            # Write the image at a specific slice
+            img.write('%d@%s' % (subtomo.getObjId(), fnProj))
+
+    def createOutputStep(self):
+        input = self.input.get()
+        imgSetOut = self._createSetOfParticles()
+        imgSetOut.setSamplingRate(input.getSamplingRate())
+        imgSetOut.setAlignmentProj()
+
+        # Input could be SetOfVolumes or SetOfSubtomograms
+        for item in input.iterItems():
+            idx = item.getObjId()
+            p = Particle()
+            p.setLocation(ih._convertToLocation((idx, self._getExtraPath("projections.mrcs"))))
+            p._subtomogramID = String(idx)
+
+            if item.hasTransform():
+                transform = Transform()
+                transform.setMatrix(item.getTransform().getMatrix())
+                p.setTransform(transform)
+            imgSetOut.append(p)
+
+        self._defineOutputs(**{SubtomoProjectOutput.particles.name:imgSetOut})
+        self._defineSourceRelation(self.input, imgSetOut)
+
+        if self.radAvg.get():
+            avgFile = self._getExtraPath("average.xmp")
+            imgh = ih()
+            avgImage = imgh.computeAverage(imgSetOut)
+            avgImage.write(avgFile)
+            avg = Particle()
+            avg.setLocation(1, avgFile)
+            avg.copyInfo(imgSetOut)
+            self._defineOutputs(**{SubtomoProjectOutput.average.name:avg})
+            self._defineSourceRelation(self.input, avg)
 
+    # --------------------------- INFO functions ------------------------------
     def _methods(self):
-        if not self.isFinished():
-            return ["Protocol not finished yet"]
-        else:
-            return ["Fit an ellipsoid and compute a 3D set of points (mesh) for each of the %d vesicles adjusted." %
-                self.outputMeshes.getNumberOfMeshes()]
+        vols = self.input.get()
 
-    # --------------------------- UTILS functions --------------------------------------------
-    def _getInputisSubtomo(self, item):
-        if isinstance(item, SubTomogram):
-            return True
+        methods=[]
+        if self.radAvg:
+            methods.append("Radial average computed for %d volumes with dimensions %s were obtained." % (vols.getSize(), vols.getDimensions()))
         else:
-            return False
+            methods.append("Projections on the %s axis of %d volumes with dimensions %s were obtained using %s slices."
+                       % (self._dirChoices[self.dirParam.get()], vols.getSize(), vols.getDimensions(),
+                          "all" if self.rangeParam.get() == 0 else self.cropParam.get()))
+        return methods
 
-    def _getCoor(self, item):
-        if self._getInputisSubtomo(item):
-            coor = item.getCoordinate3D()
-        else:
-            coor = item
-        return coor
 
-    def _getVesicleId(self, item):
-        coor = self._getCoor(item)
-        if coor.hasGroupId():
-            vesicleId = coor.getGroupId()
+    def _summary(self):
+        summary = []
+
+        if self.radAvg:
+            summary.append("Radial average: %s" % self.radAvg)
         else:
-            vesicleId = '1'  # For now it works with several vesicles in the same tomo just for subtomos with groupId
-        return vesicleId
 
-    def _evaluateQuadric(self, v, x, y, z):
-        return v[0]*x*x + v[1]*y*y + v[2]*z*z + 2*v[3]*x*y + 2*v[4]*x*z + 2*v[5]*y*z + 2*v[6]*x + 2*v[7]*y + 2*v[8]*z +\
-               v[9]
+            summary.append("Projections direction: %s" % self._dirChoices[self.dirParam.get()])
+            summary.append("Number: %s" % ("All" if self.rangeParam.get() == 0 else self.cropParam.get()))
+
+        return summary
+
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_flexalign.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_flexalign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_half_maps_subtomos.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_half_maps_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_phantom_tomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resizeTS.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resizeTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resize_tomograms.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resize_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_roiIJ.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_roiIJ.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_score_coordinates.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_score_transform.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_splitTS.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_splitTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_subtomo_map_back.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtomo_map_back.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols/protocol_subtraction_subtomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtraction_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/protocols.conf` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols.conf`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 	    ]}
 	]},
 	{"tag": "section", "text": "Particles", "children": [
 	    {"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": [
 	        {"tag": "protocol", "value": "XmippProtConnectedComponents", "text": "default"},
 	        {"tag": "protocol", "value": "XmippProtRoiIJ",   "text": "default"},
 		    {"tag": "protocol", "value": "XmippProtCCroi",   "text": "default"},
-            {"tag": "protocol", "value": "XmippProtFitEllipsoid",   "text": "default"},
             {"tag": "protocol", "value": "XmippProtScoreCoordinates",   "text": "default"}
             ]}
         ]},
 	{"tag": "section", "text": "Subtomogram averaging", "children": [
 	    {"tag": "section", "text": "Preprocessing", "children": [
             {"tag": "protocol", "value": "XmippProtSubtomoProject", "text": "default"},
             {"tag": "protocol", "value": "XmippProtApplyTransformSubtomo", "text": "default"}
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/__init__.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_extract_subtomos.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,30 @@
                                               samplingRate=5)
 
         self.launchProtocol(protImportTomogram)
 
         protImportCoordinates3d = self.newProtocol(tomo.protocols.ProtImportCoordinates3D,
                                                    auto=IMPORT_FROM_EMAN,
                                                    filesPath=self.coords3D,
-                                                   importTomograms=protImportTomogram.outputTomograms,
+                                                   importTomograms=protImportTomogram.Tomograms,
                                                    filesPattern='', boxSize=32,
                                                    samplingRate=5)
 
         self.launchProtocol(protImportCoordinates3d)
-        self.assertSetSize(protImportTomogram.outputTomograms, 1,
+        self.assertSetSize(protImportTomogram.Tomograms, 1,
                            "There was a problem with tomogram output")
         self.assertSetSize(protImportCoordinates3d.outputCoordinates, 5,
                            "There was a problem with coordinates 3d output")
         return protImportCoordinates3d, protImportTomogram
 
     def _runXmippTomoExtraction(self, doInvert=False, boxSize=32, differenttomogram = False):
         protImportCoordinates3d, protImportTomogram = self._runImportCoordinatesAndTomograms()
         if differenttomogram:
             protTomoExtraction = self.newProtocol(XmippProtExtractSubtomos,
-                                                  tomograms=protImportTomogram.outputTomograms,
+                                                  tomograms=protImportTomogram.Tomograms,
                                                   coords=protImportCoordinates3d.outputCoordinates,
                                                   invertContrast=doInvert,
                                                   boxSize=boxSize)
         else:
             protTomoExtraction = self.newProtocol(XmippProtExtractSubtomos,
                                                   coords=protImportCoordinates3d.outputCoordinates,
                                                   invertContrast=doInvert,
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_monotomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_monotomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         TestMonoTomoBase.setData()
         cls.protImportHalf1 = cls.runImportTomograms(cls.odd, 16.14)
         cls.protImportHalf2 = cls.runImportTomograms(cls.even, 16.14)
 
     def testMonoTomo(self):
         MonoTomo = self.newProtocol(XmippProtMonoTomo,
                                     objLabel='two halves monotomo',
-                                    oddTomograms=self.protImportHalf1.outputTomograms,
-                                    evenTomograms=self.protImportHalf2.outputTomograms,
+                                    oddTomograms=self.protImportHalf1.Tomograms,
+                                    evenTomograms=self.protImportHalf2.Tomograms,
                                     useMask=False,
                                     minRes=1,
                                     maxRes=150,
                                     )
         self.launchProtocol(MonoTomo)
         self.assertTrue(exists(MonoTomo._getExtraPath('tomo_1/fullTomogram_1.mrc')),
                         "MonoTomo has failed creating the resolution tomogram")
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_crop.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         TestReSizeBase.setData()
         cls.protImportTomos = cls.runImportTomograms(cls.tomos, 16.14)
 
     def testCropTomogramsSamplingRate(self):
         Rrb = XmippProtCropTomograms()
         crop = self.newProtocol(XmippProtCropTomograms,
                                     objLabel='crop tomos',
-                                    inputSet=self.protImportTomos.outputTomograms,
+                                    inputSet=self.protImportTomos.Tomograms,
                                     xcrop0=100,
                                     xcropF=900,
                                     ycrop0=100,
                                     ycropF=900,
                                     zcrop0=10,
                                     zcropF=100)
         self.launchProtocol(crop)
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_resize.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_resize.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,43 +55,43 @@
         TestReSizeBase.setData()
         cls.protImportTomos = cls.runImportTomograms(cls.tomos, 16.14)
 
     def testReSizeTomogramsSamplingRate(self):
         Rrb = XmippProtResizeTomograms()
         reSize = self.newProtocol(XmippProtResizeTomograms,
                                     objLabel='Resize tomos',
-                                    inputSet=self.protImportTomos.outputTomograms,
+                                    inputSet=self.protImportTomos.Tomograms,
                                     resizeOption = Rrb.RESIZE_SAMPLINGRATE,
                                     resizeSamplingRate = 32.28)
         self.launchProtocol(reSize)
         self.assertTrue(reSize)
         self.assertSetSize(reSize.outputSetOfTomograms, 2,
                            "resize has failed in the samplingrate option probably related with the use "
                            "of a SetOfTomograms (processing the second tomogram)")
 
 
     def testReSizeTomogramsFactor(self):
         Rrb = XmippProtResizeTomograms()
         reSize = self.newProtocol(XmippProtResizeTomograms,
                                     objLabel='Resize tomos',
-                                    inputSet=self.protImportTomos.outputTomograms,
+                                    inputSet=self.protImportTomos.Tomograms,
                                     resizeOption = Rrb.RESIZE_FACTOR,
                                     resizeFactor = 0.5)
         self.launchProtocol(reSize)
         self.assertTrue(reSize)
         self.assertSetSize(reSize.outputSetOfTomograms, 2,
                            "resize has failed in the Factor option probably related with the use "
                            "of a SetOfTomograms (processing the second tomogram)")
 
 
     def testReSizeTomogramsPiramid(self):
         Rrb = XmippProtResizeTomograms()
         reSize = self.newProtocol(XmippProtResizeTomograms,
                                     objLabel='Resize tomos',
-                                    inputSet=self.protImportTomos.outputTomograms,
+                                    inputSet=self.protImportTomos.Tomograms,
                                     resizeOption = Rrb.RESIZE_PYRAMID,
                                     resizeLevel = 0)
         self.launchProtocol(reSize)
         self.assertTrue(reSize)
         self.assertSetSize(reSize.outputSetOfTomograms, 2,
                            "Resize has failed in the pyramid option probably related with the use "
                            "of a SetOfTomograms (processing the second tomogram)")
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/tests/test_protocols_xmipptomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_xmipptomo.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 from pwem.protocols import ProtUnionSet
 from pwem.emlib.image import ImageHandler
 from pyworkflow.tests import BaseTest, setupTestProject
 from tomo.tests import DataSet
 from tomo.protocols import (ProtImportCoordinates3D,
                             ProtImportTomograms,
                             ProtImportSubTomograms,
-                            ProtImportTs)
+                            ProtImportTs, TomoProtFitEllipsoid)
 
 
 from xmipptomo.protocols import XmippProtSubtomoProject, XmippProtConnectedComponents, XmippProtApplyTransformSubtomo, \
-    XmippProtSubtomoMapBack, XmippProtPhantomSubtomo, XmippProtScoreCoordinates, XmippProtScoreTransform, \
-    XmippProtHalfMapsSubtomo, XmippProtPhantomTomo, XmippProtSubtractionSubtomo, XmippProtCCroi, XmippProtFitEllipsoid, XmippProtSplitTiltSeries
+    XmippProtSubtomoMapBack, XmippProtPhantomSubtomo, XmippProtScoreCoordinates, \
+    XmippProtHalfMapsSubtomo, XmippProtPhantomTomo, XmippProtSubtractionSubtomo, XmippProtCCroi, XmippProtSplitTiltSeries
 
 from xmipptomo.protocols.protocol_phantom_tomo import OutputPhantomTomos
 from xmipptomo.protocols.protocol_project_top import SubtomoProjectOutput
 
 
 class TestXmipptomoProtCC(BaseTest):
     """ This class check if the protocol to compute connected components works
@@ -60,19 +60,19 @@
     def _runPreviousProtocols(self):
         protImportTomogram = self.newProtocol(ProtImportTomograms,
                                               filesPath=self.tomogram,
                                               samplingRate=5)
         self.launchProtocol(protImportTomogram)
         protImportCoordinates3d = self.newProtocol(ProtImportCoordinates3D,
                                                    filesPath=self.coords3D,
-                                                   importTomograms=protImportTomogram.outputTomograms,
+                                                   importTomograms=protImportTomogram.Tomograms,
                                                    boxSize=32,
                                                    samplingRate=5)
         self.launchProtocol(protImportCoordinates3d)
-        self.assertIsNotNone(protImportTomogram.outputTomograms,
+        self.assertIsNotNone(protImportTomogram.Tomograms,
                              "There was a problem with tomogram output")
         self.assertIsNotNone(protImportCoordinates3d.outputCoordinates,
                              "There was a problem with coordinates 3d output")
         return protImportCoordinates3d
 
     def test_cc(self):
         protImport = self._runPreviousProtocols()
@@ -204,23 +204,23 @@
         cls.coords3D = cls.dataset.getFile('overview_wbp.txt')
 
     def _runPreviousProtocols(self):
         protImportTomogram = self.newProtocol(ProtImportTomograms,
                                               filesPath=self.tomogram,
                                               samplingRate=5)
         self.launchProtocol(protImportTomogram)
-        self.assertIsNotNone(protImportTomogram.outputTomograms,
+        self.assertIsNotNone(protImportTomogram.Tomograms,
                              "There was a problem with tomogram output")
 
         protPhantom = self.newProtocol(XmippProtPhantomSubtomo,
                                        option=1,
                                        sampling=4,
                                        nsubtomos=5,
                                        coords=True,
-                                       tomos=protImportTomogram.outputTomograms)
+                                       tomos=protImportTomogram.Tomograms)
         self.launchProtocol(protPhantom)
         self.assertIsNotNone(protPhantom.outputSubtomograms,
                              "There was a problem with subtomograms output")
 
         return protImportTomogram, protPhantom
 
     def test_mapback(self):
@@ -273,23 +273,22 @@
 
     def _runPreviousProtocols(self):
         protImportTomogram = self.newProtocol(ProtImportTomograms,
                                               filesPath=self.tomogram,
                                               samplingRate=2,
                                               objLabel='Import Tomogram')
         self.launchProtocol(protImportTomogram)
-        output = getattr(protImportTomogram, 'outputTomograms', None)
-        self.assertIsNotNone(output,
+        self.assertSetSize(protImportTomogram.Tomograms, size=1, msg=
                              "There was a problem with import tomograms output")
 
         protImportCoordinates3d = self.newProtocol(ProtImportCoordinates3D,
                                                    objLabel='Import Coordinates - TXT',
                                                    auto=0,
                                                    filesPath=self.dataset.getPath(),
-                                                   importTomograms=protImportTomogram.outputTomograms,
+                                                   importTomograms=protImportTomogram.Tomograms,
                                                    filesPattern='*.txt', boxSize=32,
                                                    samplingRate=5)
         self.launchProtocol(protImportCoordinates3d)
         output = getattr(protImportCoordinates3d, 'outputCoordinates', None)
         self.assertIsNotNone(output,
                              "There was a problem with import coordinates output")
 
@@ -439,116 +438,60 @@
         self.launchProtocol(subtraction)
         self.assertIsNotNone(subtraction.outputSubtomograms,
                              "There was a problem with subtracted subtomograms output")
         self.assertSetSize(subtraction.outputSubtomograms, 10, "There was a problem with particles output")
         self.assertTrue(subtraction.outputSubtomograms.getSamplingRate() == 1.0)
         self.assertTrue(subtraction.outputSubtomograms.getFirstItem().getDim() == (40, 40, 40))
 
-
-class TestXmipptomoProtFitVesicles(BaseTest):
-    """ This class check if the protocol fit vesicles works properly."""
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet('tomo-em')
-        cls.tomogram = cls.dataset.getFile('tomo1')
-        cls.coords3D = cls.dataset.getFile('overview_wbp.txt')
-
-    def _runPreviousProtocols(self):
-        protImportTomogram = self.newProtocol(ProtImportTomograms,
-                                              filesPath=self.tomogram,
-                                              samplingRate=5)
-        self.launchProtocol(protImportTomogram)
-        self.assertIsNotNone(protImportTomogram.outputTomograms,
-                             "There was a problem with tomogram output")
-
-        protImportCoordinates3d = self.newProtocol(ProtImportCoordinates3D,
-                                                   filesPath=self.coords3D,
-                                                   importTomograms=protImportTomogram.outputTomograms,
-                                                   boxSize=32,
-                                                   samplingRate=5)
-        self.launchProtocol(protImportCoordinates3d)
-        self.assertIsNotNone(protImportCoordinates3d.outputCoordinates,
-                             "There was a problem with coordinates 3d output")
-
-        protImportCoordinates3d_2 = self.newProtocol(ProtImportCoordinates3D,
-                                                     filesPath=self.coords3D,
-                                                     importTomograms=protImportTomogram.outputTomograms,
-                                                     boxSize=32,
-                                                     samplingRate=5)
-        self.launchProtocol(protImportCoordinates3d_2)
-        self.assertIsNotNone(protImportCoordinates3d_2.outputCoordinates,
-                             "There was a problem with coordinates 3d output 2")
-
-        protJoinCoordinates = self.newProtocol(ProtUnionSet,
-                                               inputSets=[protImportCoordinates3d.outputCoordinates,
-                                                          protImportCoordinates3d_2.outputCoordinates])
-        self.launchProtocol(protJoinCoordinates)
-        self.assertIsNotNone(protJoinCoordinates.outputSet,
-                             "There was a problem with join coordinates output")
-
-        return protJoinCoordinates, protImportTomogram
-
-    def test_fitEllipsoid(self):
-        protJoinCoordinates, protImportTomogram = self._runPreviousProtocols()
-        protFitVesicles = self.newProtocol(XmippProtFitEllipsoid,
-                                           input=protJoinCoordinates.outputSet,
-                                           inputTomos=protImportTomogram.outputTomograms)
-        self.launchProtocol(protFitVesicles)
-        self.assertIsNotNone(protFitVesicles.outputMeshes, "There was a problem with output vesicles (SetOfMeshes)")
-        self.assertEqual(protFitVesicles.outputMeshes.getSize(), 11184)
-        return protFitVesicles
-
-
 class TestXmipptomoProtCCtoROI(BaseTest):
-    """ This class check if the protocol connected componnents to ROIs works properly."""
+    """ This class check if the protocol connected components to ROIs works properly."""
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('tomo-em')
         cls.tomogram = cls.dataset.getFile('tomo1')
         cls.coords3D = cls.dataset.getFile('overview_wbp.txt')
 
     def _runPreviousProtocols(self):
         protImportTomogram = self.newProtocol(ProtImportTomograms,
                                               filesPath=self.tomogram,
                                               samplingRate=5)
         self.launchProtocol(protImportTomogram)
-        self.assertIsNotNone(protImportTomogram.outputTomograms,
+        self.assertIsNotNone(protImportTomogram.Tomograms,
                              "There was a problem with tomogram output")
 
         protImportCoordinates3d = self.newProtocol(ProtImportCoordinates3D,
                                                    filesPath=self.coords3D,
-                                                   importTomograms=protImportTomogram.outputTomograms,
+                                                   importTomograms=protImportTomogram.Tomograms,
                                                    boxSize=32,
                                                    samplingRate=5)
         self.launchProtocol(protImportCoordinates3d)
         self.assertIsNotNone(protImportCoordinates3d.outputCoordinates,
                              "There was a problem with coordinates 3d output")
 
         protImportCoordinates3d_2 = self.newProtocol(ProtImportCoordinates3D,
                                                      filesPath=self.coords3D,
-                                                     importTomograms=protImportTomogram.outputTomograms,
+                                                     importTomograms=protImportTomogram.Tomograms,
                                                      boxSize=32,
                                                      samplingRate=5)
         self.launchProtocol(protImportCoordinates3d_2)
         self.assertIsNotNone(protImportCoordinates3d_2.outputCoordinates,
                              "There was a problem with coordinates 3d output 2")
 
         protJoinCoordinates = self.newProtocol(ProtUnionSet,
                                                inputSets=[protImportCoordinates3d.outputCoordinates,
                                                           protImportCoordinates3d_2.outputCoordinates])
         self.launchProtocol(protJoinCoordinates)
         self.assertIsNotNone(protJoinCoordinates.outputSet,
                              "There was a problem with join coordinates output")
 
-        protFitVesicles = self.newProtocol(XmippProtFitEllipsoid,
+        protFitVesicles = self.newProtocol(TomoProtFitEllipsoid,
                                            input=protJoinCoordinates.outputSet,
-                                           inputTomos=protImportTomogram.outputTomograms)
+                                           inputTomos=protImportTomogram.Tomograms)
         self.launchProtocol(protFitVesicles)
         self.assertIsNotNone(protFitVesicles.outputMeshes, "There was a problem with output vesicles (SetOfMeshes)")
         return protFitVesicles, protJoinCoordinates
 
     def test_CCtoROIs(self):
         protFitVesicles, protJoinCoordinates = self._runPreviousProtocols()
         protCCtoROI = self.newProtocol(XmippProtCCroi,
```

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/utils.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/__init__.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/monotomo_tree_provider.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/monotomo_tree_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_cltomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_phantom_create.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/viewers/viewer_score_subtomos.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_score_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/wizards.py` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.2/xmipptomo/xmipp_logo.png` & `scipion-em-xmipptomo-3.23.3.3/xmipptomo/xmipp_logo.png`

 * *Files identical despite different names*

