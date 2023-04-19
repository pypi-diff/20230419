# Comparing `tmp/fastsim-2.0.18.tar.gz` & `tmp/fastsim-2.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsim-2.0.18.tar", last modified: Wed Apr 12 20:40:54 2023, max compression
+gzip compressed data, was "fastsim-2.0.19.tar", last modified: Wed Apr 19 19:24:11 2023, max compression
```

## Comparing `fastsim-2.0.18.tar` & `fastsim-2.0.19.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 20:40:39.000000 fastsim-2.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 20:40:39.000000 fastsim-2.0.18/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-12 20:40:39.000000 fastsim-2.0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-12 20:40:54.491536 fastsim-2.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-04-12 20:40:39.000000 fastsim-2.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.423535 fastsim-2.0.18/fastsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    37910 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.431535 fastsim-2.0.18/fastsim/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/2017_Ford_F150_thermal_val.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/accel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/demo_abc_drag_coef_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/demo_eu_vehicle_wltp.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/fastsim-icon-web-131x172.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/fusion_thermal_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/fusion_thermal_cal_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/fusion_thermal_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/mp_parallel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/stop_start_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/time_dilation_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/docs/wltc_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/inspect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.431535 fastsim-2.0.18/fastsim/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/FASTSim_py_veh_db.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.439535 fastsim-2.0.18/fastsim/resources/cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/NREL13.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/accel.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.419535 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.439535 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.439535 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/
--rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
--rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.443535 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4105836_2/
--rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.447536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/
--rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.451536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/
--rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.455536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/
--rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.459536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/
--rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.459536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/
--rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.459536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/
--rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
--rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.463536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4113492_1/
--rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.463536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4114555_1/
--rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.463536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_1/
--rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.463536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_2/
--rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.467536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115957_1/
--rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.467536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115985_1/
--rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.467536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116361_1/
--rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.467536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116721_2/
--rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.467536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116728_1/
--rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.471536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_1/
--rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.471536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_2/
--rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.471536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116880_1/
--rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.471536 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/
--rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/ftpmc1b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/hwfet.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/longHaulDriveCycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/udds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/us06.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_extra_high3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_high3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_high3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_low3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_med3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_med3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wmtc_all.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wmtc_part1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wmtc_part2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/cycles/wmtc_part3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/longparams.json
--rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/master_benchmark_vars.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/res_excel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.479536 fastsim-2.0.18/fastsim/resources/vehdb/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Focus.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Focus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Fusion.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Class_4_Box_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Line_Haul_Conv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Line_Haul_Conv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/fail_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/fail_overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/legacy_template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/legacy_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/test_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/test_overrides.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.479536 fastsim-2.0.18/fastsim/resources/vehdb/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/rustext.py
--rw-r--r--   0 runner    (1001) docker     (123)   116204 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/simdrivelabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.483536 fastsim-2.0.18/fastsim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_coasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_eco_cruise.py
--rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_following.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_simdrive_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_soc_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/tests/test_vs_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-12 20:40:39.000000 fastsim-2.0.18/fastsim/vehicle_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.427535 fastsim-2.0.18/fastsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 20:40:54.000000 fastsim-2.0.18/fastsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 20:40:39.000000 fastsim-2.0.18/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.483536 fastsim-2.0.18/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.487536 fastsim-2.0.18/rust/fastsim-core/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.487536 fastsim-2.0.18/rust/fastsim-core/proc-macros/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.487536 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/proc-macros/src/utilities.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/rust/fastsim-core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/air.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/cycle.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/rust/fastsim-core/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/html/docs-header.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/macros.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/pyo3imports.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/rust/fastsim-core/src/simdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/simdrive/cyc_mods.rs
--rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/simdrive/simdrive_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/simdrive.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/simdrivelabel.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/vehicle.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/vehicle_thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-core/src/vehicle_utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/rust/fastsim-py/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:40:54.491536 fastsim-2.0.18/rust/fastsim-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 20:40:39.000000 fastsim-2.0.18/rust/fastsim-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:40:54.491536 fastsim-2.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 20:40:39.000000 fastsim-2.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-19 19:24:00.000000 fastsim-2.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-19 19:24:00.000000 fastsim-2.0.19/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 19:24:00.000000 fastsim-2.0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-19 19:24:10.207713 fastsim-2.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-04-19 19:24:00.000000 fastsim-2.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.163712 fastsim-2.0.19/fastsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37910 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.167712 fastsim-2.0.19/fastsim/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/2017_Ford_F150_thermal_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/accel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/demo_abc_drag_coef_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/demo_eu_vehicle_wltp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/fastsim-icon-web-131x172.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/fusion_thermal_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/fusion_thermal_cal_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/fusion_thermal_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/mp_parallel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/stop_start_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/time_dilation_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/docs/wltc_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/inspect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.167712 fastsim-2.0.19/fastsim/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/FASTSim_py_veh_db.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.171712 fastsim-2.0.19/fastsim/resources/cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/NREL13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/accel.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.159711 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.171712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.175712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/
+-rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.175712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4105836_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.179712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.183712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/
+-rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.183712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.187712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.187712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.187712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.187712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4113492_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4114555_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115957_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115985_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.191712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116361_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116721_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116728_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116880_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.195712 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/ftpmc1b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/hwfet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/longHaulDriveCycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/udds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/us06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_extra_high3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_high3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_high3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_low3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_med3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_med3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wmtc_all.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wmtc_part1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wmtc_part2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/cycles/wmtc_part3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/longparams.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/master_benchmark_vars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/res_excel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/fastsim/resources/vehdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Focus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Focus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Fusion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Class_4_Box_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Line_Haul_Conv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Line_Haul_Conv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/fail_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/fail_overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/legacy_template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/legacy_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/test_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/test_overrides.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/fastsim/resources/vehdb/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/rustext.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116204 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/simdrivelabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/fastsim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_coasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_eco_cruise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_simdrive_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_soc_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/tests/test_vs_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-19 19:24:00.000000 fastsim-2.0.19/fastsim/vehicle_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.163712 fastsim-2.0.19/fastsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 19:24:10.000000 fastsim-2.0.19/fastsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-19 19:24:00.000000 fastsim-2.0.19/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/rust/fastsim-core/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.203713 fastsim-2.0.19/rust/fastsim-core/proc-macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/proc-macros/src/utilities.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/air.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/cycle.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-core/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/html/docs-header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/pyo3imports.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-core/src/simdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/simdrive/cyc_mods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/simdrive/simdrive_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/simdrive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41715 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/simdrivelabel.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    59542 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/vehicle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/vehicle_thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-core/src/vehicle_utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:24:10.207713 fastsim-2.0.19/rust/fastsim-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-19 19:24:00.000000 fastsim-2.0.19/rust/fastsim-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 19:24:10.211713 fastsim-2.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-19 19:24:00.000000 fastsim-2.0.19/setup.py
```

### Comparing `fastsim-2.0.18/LICENSE` & `fastsim-2.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/LICENSE.md` & `fastsim-2.0.19/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/PKG-INFO` & `fastsim-2.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.18
+Version: 2.0.19
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -122,15 +122,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
-2.0.11 - 2.0.18 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
+2.0.11 - 2.0.19 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`
```

### Comparing `fastsim-2.0.18/README.md` & `fastsim-2.0.19/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
-2.0.11 - 2.0.18 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
+2.0.11 - 2.0.19 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`
```

### Comparing `fastsim-2.0.18/fastsim/__init__.py` & `fastsim-2.0.19/fastsim/__init__.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/auxiliaries.py` & `fastsim-2.0.19/fastsim/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/calibration.py` & `fastsim-2.0.19/fastsim/calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/cycle.py` & `fastsim-2.0.19/fastsim/cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/2017_Ford_F150_thermal_val.py` & `fastsim-2.0.19/fastsim/docs/2017_Ford_F150_thermal_val.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/accel_demo.py` & `fastsim-2.0.19/fastsim/docs/accel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/cav_demo.py` & `fastsim-2.0.19/fastsim/docs/cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/cav_sweep.py` & `fastsim-2.0.19/fastsim/docs/cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/demo.py` & `fastsim-2.0.19/fastsim/docs/demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/demo_abc_drag_coef_conv.py` & `fastsim-2.0.19/fastsim/docs/demo_abc_drag_coef_conv.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/demo_eu_vehicle_wltp.py` & `fastsim-2.0.19/fastsim/docs/demo_eu_vehicle_wltp.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/fastsim-icon-web-131x172.jpg` & `fastsim-2.0.19/fastsim/docs/fastsim-icon-web-131x172.jpg`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/fusion_thermal_cal.py` & `fastsim-2.0.19/fastsim/docs/fusion_thermal_cal.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/fusion_thermal_cal_post.py` & `fastsim-2.0.19/fastsim/docs/fusion_thermal_cal_post.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/fusion_thermal_demo.py` & `fastsim-2.0.19/fastsim/docs/fusion_thermal_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/mp_parallel_demo.py` & `fastsim-2.0.19/fastsim/docs/mp_parallel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/stop_start_demo.py` & `fastsim-2.0.19/fastsim/docs/stop_start_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/time_dilation_demo.py` & `fastsim-2.0.19/fastsim/docs/time_dilation_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/docs/wltc_calibration.py` & `fastsim-2.0.19/fastsim/docs/wltc_calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/inspect_utils.py` & `fastsim-2.0.19/fastsim/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/parameters.py` & `fastsim-2.0.19/fastsim/parameters.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resample.py` & `fastsim-2.0.19/fastsim/resample.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/FASTSim_py_veh_db.csv` & `fastsim-2.0.19/fastsim/resources/FASTSim_py_veh_db.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/HHDDTCruiseSmooth.csv` & `fastsim-2.0.19/fastsim/resources/cycles/HHDDTCruiseSmooth.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/NREL13.csv` & `fastsim-2.0.19/fastsim/resources/cycles/NREL13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv` & `fastsim-2.0.19/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/accel.csv` & `fastsim-2.0.19/fastsim/resources/cycles/accel.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv` & `fastsim-2.0.19/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/ftpmc1b.csv` & `fastsim-2.0.19/fastsim/resources/cycles/ftpmc1b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/hwfet.csv` & `fastsim-2.0.19/fastsim/resources/cycles/hwfet.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/longHaulDriveCycle.csv` & `fastsim-2.0.19/fastsim/resources/cycles/longHaulDriveCycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/udds.csv` & `fastsim-2.0.19/fastsim/resources/cycles/udds.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/us06.csv` & `fastsim-2.0.19/fastsim/resources/cycles/us06.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_extra_high3.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_extra_high3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_high3a.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_high3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_high3b.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_high3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_low3.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_low3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_med3a.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_med3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wltc_class3_med3b.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wltc_class3_med3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wmtc_all.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wmtc_all.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wmtc_part1.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wmtc_part1.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wmtc_part2.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wmtc_part2.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/cycles/wmtc_part3.csv` & `fastsim-2.0.19/fastsim/resources/cycles/wmtc_part3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/longparams.json` & `fastsim-2.0.19/fastsim/resources/longparams.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/master_benchmark_vars.csv` & `fastsim-2.0.19/fastsim/resources/master_benchmark_vars.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/res_excel.json` & `fastsim-2.0.19/fastsim/resources/res_excel.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Focus.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Focus.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Focus.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Focus.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Fusion.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Fusion.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2012_Ford_Fusion.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2012_Ford_Fusion.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Class_4_Box_Truck.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/Class_4_Box_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Class_4_Box_Truck.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/Class_4_Box_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Line_Haul_Conv.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/Line_Haul_Conv.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Line_Haul_Conv.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/Line_Haul_Conv.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/fail_overrides.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/fail_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/fail_overrides.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/fail_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/legacy_template.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/legacy_template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/legacy_template.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/legacy_template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/template.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/template.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/test_overrides.csv` & `fastsim-2.0.19/fastsim/resources/vehdb/test_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/test_overrides.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/test_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml` & `fastsim-2.0.19/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/simdrive.py` & `fastsim-2.0.19/fastsim/simdrive.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/simdrivelabel.py` & `fastsim-2.0.19/fastsim/simdrivelabel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_auxiliaries.py` & `fastsim-2.0.19/fastsim/tests/test_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_cav_demo.py` & `fastsim-2.0.19/fastsim/tests/test_cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_cav_sweep.py` & `fastsim-2.0.19/fastsim/tests/test_cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_coasting.py` & `fastsim-2.0.19/fastsim/tests/test_coasting.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_copy.py` & `fastsim-2.0.19/fastsim/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_cycle.py` & `fastsim-2.0.19/fastsim/tests/test_cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_demo.py` & `fastsim-2.0.19/fastsim/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_eco_cruise.py` & `fastsim-2.0.19/fastsim/tests/test_eco_cruise.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_following.py` & `fastsim-2.0.19/fastsim/tests/test_following.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_logging.py` & `fastsim-2.0.19/fastsim/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_rust.py` & `fastsim-2.0.19/fastsim/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_simdrive.py` & `fastsim-2.0.19/fastsim/tests/test_simdrive.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_simdrive_sweep.py` & `fastsim-2.0.19/fastsim/tests/test_simdrive_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_soc_correction.py` & `fastsim-2.0.19/fastsim/tests/test_soc_correction.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_vehicle.py` & `fastsim-2.0.19/fastsim/tests/test_vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/tests/test_vs_excel.py` & `fastsim-2.0.19/fastsim/tests/test_vs_excel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/utilities.py` & `fastsim-2.0.19/fastsim/utilities.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/vehicle.py` & `fastsim-2.0.19/fastsim/vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim/vehicle_base.py` & `fastsim-2.0.19/fastsim/vehicle_base.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/fastsim.egg-info/PKG-INFO` & `fastsim-2.0.19/fastsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.18
+Version: 2.0.19
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -122,15 +122,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
-2.0.11 - 2.0.18 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
+2.0.11 - 2.0.19 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`
```

### Comparing `fastsim-2.0.18/fastsim.egg-info/SOURCES.txt` & `fastsim-2.0.19/fastsim.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 fastsim/__init__.py
 fastsim/auxiliaries.py
 fastsim/calibration.py
 fastsim/cycle.py
 fastsim/inspect_utils.py
 fastsim/parameters.py
```

### Comparing `fastsim-2.0.18/pyproject.toml` & `fastsim-2.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "setuptools-rust>=0.11.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastsim"
-version = "2.0.18"
+version = "2.0.19"
 authors = [{ name = "NREL/MTES/CIMS/MBAP Group", email = "fastsim@nrel.gov" }]
 description = "Tool for modeling vehicle powertrains"
 readme = "README.md"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fastsim-2.0.18/rust/Cargo.toml` & `fastsim-2.0.19/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/Cargo.toml` & `fastsim-2.0.19/rust/fastsim-core/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,16 @@
 proc-macros = { path = "proc-macros" }
 serde_json = "1.0.81"
 bincode = "1.3.3"
 log = "0.4.17"
 polynomial = "0.2.4"
 argmin = "0.7.0"
 argmin-math = { version = "0.2.1", features = ["ndarray_latest-nolinalg-serde"] }
+validator = { version = "0.16", features = ["derive"] }
+lazy_static = "1.4.0"
+regex = "1.7.1"
 
 [package.metadata.docs.rs]
 rustdoc-args = [ "--html-in-header", "./src/html/docs-header.html" ]
 
 [features]
 pyo3 = ["dep:pyo3"]
```

### Comparing `fastsim-2.0.18/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs` & `fastsim-2.0.19/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs` & `fastsim-2.0.19/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/proc-macros/src/history_vec_derive.rs` & `fastsim-2.0.19/rust/fastsim-core/proc-macros/src/history_vec_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/proc-macros/src/lib.rs` & `fastsim-2.0.19/rust/fastsim-core/proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/proc-macros/src/utilities.rs` & `fastsim-2.0.19/rust/fastsim-core/proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/air.rs` & `fastsim-2.0.19/rust/fastsim-core/src/air.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/cycle.rs` & `fastsim-2.0.19/rust/fastsim-core/src/cycle.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/html/docs-header.html` & `fastsim-2.0.19/rust/fastsim-core/src/html/docs-header.html`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/lib.rs` & `fastsim-2.0.19/rust/fastsim-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/macros.rs` & `fastsim-2.0.19/rust/fastsim-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/params.rs` & `fastsim-2.0.19/rust/fastsim-core/src/params.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/simdrive/cyc_mods.rs` & `fastsim-2.0.19/rust/fastsim-core/src/simdrive/cyc_mods.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/simdrive/simdrive_impl.rs` & `fastsim-2.0.19/rust/fastsim-core/src/simdrive/simdrive_impl.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/simdrive.rs` & `fastsim-2.0.19/rust/fastsim-core/src/simdrive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/simdrivelabel.rs` & `fastsim-2.0.19/rust/fastsim-core/src/simdrivelabel.rs`

 * *Files 1% similar despite different names*

```diff
@@ -846,15 +846,16 @@
             17000.0,
             33170.0,
             RustPhysicalProperties::default(),
             500.0,
             0.99,
             None,
             None,
-        );
+        )
+        .unwrap();
 
         let (mut label_fe, _) = get_label_fe(&veh, None, None).unwrap();
         // For some reason, RustVehicle::mock_vehicle() != RustVehicle::mock_vehicle()
         // Therefore, veh field in both structs replaced with Default for comparison purposes
         label_fe.veh = vehicle::RustVehicle::default();
         // TODO: Figure out why net_accel values are different
         println!("Calculated net accel: {}", label_fe.net_accel);
```

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/thermal.rs` & `fastsim-2.0.19/rust/fastsim-core/src/thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/traits.rs` & `fastsim-2.0.19/rust/fastsim-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/utils.rs` & `fastsim-2.0.19/rust/fastsim-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/vehicle.rs` & `fastsim-2.0.19/rust/fastsim-core/src/vehicle.rs`

 * *Files 18% similar despite different names*

```diff
@@ -3,29 +3,41 @@
 // local
 use crate::imports::*;
 use crate::params::*;
 use crate::proc_macros::{add_pyo3_api, ApproxEq};
 #[cfg(feature = "pyo3")]
 use crate::pyo3imports::*;
 
+use lazy_static::lazy_static;
+use regex::Regex;
+use validator::Validate;
+
+// veh_pt_type options
 pub const CONV: &str = "Conv";
 pub const HEV: &str = "HEV";
 pub const PHEV: &str = "PHEV";
 pub const BEV: &str = "BEV";
 pub const VEH_PT_TYPES: [&str; 4] = [CONV, HEV, PHEV, BEV];
+lazy_static! {
+    static ref VEH_PT_TYPE_OPTIONS_REGEX: Regex = Regex::new("Conv|HEV|PHEV|BEV").unwrap();
+}
 
+// fc_eff_type options
 pub const SI: &str = "SI";
 pub const ATKINSON: &str = "Atkinson";
 pub const DIESEL: &str = "Diesel";
 pub const H2FC: &str = "H2FC";
 pub const HD_DIESEL: &str = "HD_Diesel";
-
 pub const FC_EFF_TYPES: [&str; 5] = [SI, ATKINSON, DIESEL, H2FC, HD_DIESEL];
+lazy_static! {
+    static ref FC_EFF_TYPE_OPTIONS_REGEX: Regex =
+        Regex::new("SI|Atkinson|Diesel|H2FC|HD_Diesel").unwrap();
+}
 
-#[derive(Default, Serialize, Deserialize, Clone, Debug, PartialEq, ApproxEq)]
+#[derive(Default, Serialize, Deserialize, Clone, Debug, PartialEq, ApproxEq, Validate)]
 #[add_pyo3_api(
     #[allow(clippy::too_many_arguments)]
     #[new]
     pub fn __new__(
         scenario_name: String,
         selection: u32,
         veh_year: u32,
@@ -131,15 +143,15 @@
         //ess_mass_kg: f64,
         //mc_mass_kg: f64,
         //fc_mass_kg: f64,
         //fs_mass_kg: f64,
         //mc_perc_out_array: Option<Vec<f64>>,
         fc_peak_eff_override: Option<f64>,
         mc_peak_eff_override: Option<f64>,
-    ) -> Self {
+    ) -> Result<Self, anyhow::Error> {
         Self::new(
             scenario_name,
             selection,
             veh_year,
             veh_pt_type,
             drag_coef,
             frontal_area_m2,
@@ -336,189 +348,245 @@
     #[serde(skip)]
     pub selection: u32,
     /// Vehicle year
     #[serde(alias = "vehModelYear")]
     pub veh_year: u32,
     /// Vehicle powertrain type, one of \[[CONV](CONV), [HEV](HEV), [PHEV](PHEV), [BEV](BEV)\]
     #[serde(alias = "vehPtType")]
+    #[validate(regex(
+        path = "VEH_PT_TYPE_OPTIONS_REGEX",
+        message = "must be one of [\"Conv\", \"HEV\", \"PHEV\", \"BEV\"]"
+    ))]
     pub veh_pt_type: String,
     /// Aerodynamic drag coefficient
     #[serde(alias = "dragCoef")]
+    #[validate(range(min = 0))]
     pub drag_coef: f64,
     /// Frontal area, $m^2$
     #[serde(alias = "frontalAreaM2")]
+    #[validate(range(min = 0))]
     pub frontal_area_m2: f64,
     /// Vehicle mass excluding cargo, passengers, and powertrain components, $kg$
     #[serde(alias = "gliderKg")]
+    #[validate(range(min = 0))]
     pub glider_kg: f64,
     /// Vehicle center of mass height, $m$  
     /// **NOTE:** positive for FWD, negative for RWD, AWD, 4WD
     #[serde(alias = "vehCgM")]
     pub veh_cg_m: f64,
     /// Fraction of weight on the drive axle while stopped
     #[serde(alias = "driveAxleWeightFrac")]
+    #[validate(range(min = 0, max = 1))]
     pub drive_axle_weight_frac: f64,
     /// Wheelbase, $m$
     #[serde(alias = "wheelBaseM")]
+    #[validate(range(min = 0))]
     pub wheel_base_m: f64,
     /// Cargo mass including passengers, $kg$
     #[serde(alias = "cargoKg")]
+    #[validate(range(min = 0))]
     pub cargo_kg: f64,
     /// Total vehicle mass, overrides mass calculation, $kg$
     #[serde(alias = "vehOverrideKg")]
+    #[validate(range(min = 0))]
     pub veh_override_kg: f64,
     /// Component mass multiplier for vehicle mass calculation
     #[serde(alias = "compMassMultiplier")]
+    #[validate(range(min = 0))]
     pub comp_mass_multiplier: f64,
     /// Fuel storage max power output, $kW$
     #[serde(alias = "maxFuelStorKw")]
+    #[validate(range(min = 0))]
     pub fs_max_kw: f64,
     /// Fuel storage time to peak power, $s$
     #[serde(alias = "fuelStorSecsToPeakPwr")]
+    #[validate(range(min = 0))]
     pub fs_secs_to_peak_pwr: f64,
     /// Fuel storage energy capacity, $kWh$
     #[serde(alias = "fuelStorKwh")]
+    #[validate(range(min = 0))]
     pub fs_kwh: f64,
     /// Fuel specific energy, $\frac{kWh}{kg}$
     #[serde(alias = "fuelStorKwhPerKg")]
+    #[validate(range(min = 0))]
     pub fs_kwh_per_kg: f64,
     /// Fuel converter peak continuous power, $kW$
     #[serde(alias = "maxFuelConvKw")]
+    #[validate(range(min = 0))]
     pub fc_max_kw: f64,
     /// Fuel converter output power percentage map, x-values of [fc_eff_map](RustVehicle::fc_eff_map)
     #[serde(alias = "fcPwrOutPerc")]
     pub fc_pwr_out_perc: Array1<f64>,
     /// Fuel converter efficiency map
     #[serde(default)]
     pub fc_eff_map: Array1<f64>,
     /// Fuel converter efficiency type, one of \[[SI](SI), [ATKINSON](ATKINSON), [DIESEL](DIESEL), [H2FC](H2FC), [HD_DIESEL](HD_DIESEL)\]  
     /// Used for calculating [fc_eff_map](RustVehicle::fc_eff_map), and other calculations if H2FC
     #[serde(alias = "fcEffType")]
+    #[validate(regex(
+        path = "FC_EFF_TYPE_OPTIONS_REGEX",
+        message = "must be one of [\"SI\", \"Atkinson\", \"Diesel\", \"H2FC\", \"HD_Diesel\"]"
+    ))]
     pub fc_eff_type: String,
     /// Fuel converter time to peak power, $s$
     #[serde(alias = "fuelConvSecsToPeakPwr")]
+    #[validate(range(min = 0))]
     pub fc_sec_to_peak_pwr: f64,
     /// Fuel converter base mass, $kg$
     #[serde(alias = "fuelConvBaseKg")]
+    #[validate(range(min = 0))]
     pub fc_base_kg: f64,
     /// Fuel converter specific power (power-to-weight ratio), $\frac{kW}{kg}$
     #[serde(alias = "fuelConvKwPerKg")]
+    #[validate(range(min = 0))]
     pub fc_kw_per_kg: f64,
     /// Minimum time fuel converter must be on before shutoff (for HEV, PHEV)
     #[serde(alias = "minFcTimeOn")]
+    #[validate(range(min = 0))]
     pub min_fc_time_on: f64,
     /// Fuel converter idle power, $kW$
     #[serde(alias = "idleFcKw")]
+    #[validate(range(min = 0))]
     pub idle_fc_kw: f64,
     /// Peak continuous electric motor power, $kW$
     #[serde(alias = "mcMaxElecInKw")]
+    #[validate(range(min = 0))]
     pub mc_max_kw: f64,
     /// Electric motor output power percentage map, x-values of [mc_eff_map](RustVehicle::mc_eff_map)
     #[serde(alias = "mcPwrOutPerc")]
     pub mc_pwr_out_perc: Array1<f64>,
     /// Electric motor efficiency map
     #[serde(alias = "mcEffArray")]
     pub mc_eff_map: Array1<f64>,
     /// Electric motor time to peak power, $s$
     #[serde(alias = "motorSecsToPeakPwr")]
+    #[validate(range(min = 0))]
     pub mc_sec_to_peak_pwr: f64,
     /// Motor power electronics mass per power output, $\frac{kg}{kW}$
     #[serde(alias = "mcPeKgPerKw")]
+    #[validate(range(min = 0))]
     pub mc_pe_kg_per_kw: f64,
     /// Motor power electronics base mass, $kg$
     #[serde(alias = "mcPeBaseKg")]
+    #[validate(range(min = 0))]
     pub mc_pe_base_kg: f64,
     /// Traction battery maximum power output, $kW$
     #[serde(alias = "maxEssKw")]
+    #[validate(range(min = 0))]
     pub ess_max_kw: f64,
     /// Traction battery energy capacity, $kWh$
     #[serde(alias = "maxEssKwh")]
+    #[validate(range(min = 0))]
     pub ess_max_kwh: f64,
     /// Traction battery mass per energy, $\frac{kg}{kWh}$
     #[serde(alias = "essKgPerKwh")]
+    #[validate(range(min = 0))]
     pub ess_kg_per_kwh: f64,
     /// Traction battery base mass, $kg$
     #[serde(alias = "essBaseKg")]
+    #[validate(range(min = 0))]
     pub ess_base_kg: f64,
     /// Traction battery round-trip efficiency
     #[serde(alias = "essRoundTripEff")]
+    #[validate(range(min = 0, max = 1))]
     pub ess_round_trip_eff: f64,
     /// Traction battery cycle life coefficient A, see [reference](https://web.archive.org/web/20090529194442/http://www.ocean.udel.edu/cms/wkempton/Kempton-V2G-pdfFiles/PDF%20format/Duvall-V2G-batteries-June05.pdf)
     #[serde(alias = "essLifeCoefA")]
     pub ess_life_coef_a: f64,
     /// Traction battery cycle life coefficient B, see [reference](https://web.archive.org/web/20090529194442/http://www.ocean.udel.edu/cms/wkempton/Kempton-V2G-pdfFiles/PDF%20format/Duvall-V2G-batteries-June05.pdf)
     #[serde(alias = "essLifeCoefB")]
     pub ess_life_coef_b: f64,
     /// Traction battery minimum state of charge
     #[serde(alias = "minSoc")]
+    #[validate(range(min = 0, max = 1))]
     pub min_soc: f64,
     /// Traction battery maximum state of charge
     #[serde(alias = "maxSoc")]
+    #[validate(range(min = 0, max = 1))]
     pub max_soc: f64,
     /// ESS discharge effort toward max FC efficiency
     #[serde(alias = "essDischgToFcMaxEffPerc")]
+    #[validate(range(min = 0, max = 1))]
     pub ess_dischg_to_fc_max_eff_perc: f64,
     /// ESS charge effort toward max FC efficiency
     #[serde(alias = "essChgToFcMaxEffPerc")]
+    #[validate(range(min = 0, max = 1))]
     pub ess_chg_to_fc_max_eff_perc: f64,
     /// Mass moment of inertia per wheel, $kg \cdot m^2$
     #[serde(alias = "wheelInertiaKgM2")]
+    #[validate(range(min = 0))]
     pub wheel_inertia_kg_m2: f64,
     /// Number of wheels
     #[serde(alias = "numWheels")]
-    pub num_wheels: f64,
+    #[validate(range(min = 0))]
+    pub num_wheels: f64, // TODO: Shouldn't this just be a unsigned integer? u8 would work fine.
     /// Rolling resistance coefficient
     #[serde(alias = "wheelRrCoef")]
+    #[validate(range(min = 0))]
     pub wheel_rr_coef: f64,
     /// Wheel radius, $m$
     #[serde(alias = "wheelRadiusM")]
+    #[validate(range(min = 0))]
     pub wheel_radius_m: f64,
     /// Wheel coefficient of friction
     #[serde(alias = "wheelCoefOfFric")]
+    #[validate(range(min = 0))]
     pub wheel_coef_of_fric: f64,
     /// Speed where the battery reserved for accelerating is zero
     #[serde(alias = "maxAccelBufferMph")]
+    #[validate(range(min = 0))]
     pub max_accel_buffer_mph: f64,
     /// Percent of usable battery energy reserved to help accelerate
     #[serde(alias = "maxAccelBufferPercOfUseableSoc")]
+    #[validate(range(min = 0, max = 1))]
     pub max_accel_buffer_perc_of_useable_soc: f64,
     /// Percent SOC buffer for high accessory loads during cycles with long idle time
     #[serde(alias = "percHighAccBuf")]
+    #[validate(range(min = 0))]
     pub perc_high_acc_buf: f64,
     /// Speed at which the fuel converter must turn on, $mph$
     #[serde(alias = "mphFcOn")]
+    #[validate(range(min = 0))]
     pub mph_fc_on: f64,
     /// Power demand above which to require fuel converter on, $kW$
     #[serde(alias = "kwDemandFcOn")]
+    #[validate(range(min = 0))]
     pub kw_demand_fc_on: f64,
     /// Maximum brake regeneration efficiency
     #[serde(alias = "maxRegen")]
+    #[validate(range(min = 0, max = 1))]
     pub max_regen: f64,
     /// Stop/start micro-HEV flag
     pub stop_start: bool,
     /// Force auxiliary power load to come from fuel converter
     #[serde(alias = "forceAuxOnFC")]
     pub force_aux_on_fc: bool,
     /// Alternator efficiency
     #[serde(alias = "altEff")]
+    #[validate(range(min = 0, max = 1))]
     pub alt_eff: f64,
     /// Charger efficiency
     #[serde(alias = "chgEff")]
+    #[validate(range(min = 0, max = 1))]
     pub chg_eff: f64,
     /// Auxiliary load power, $kW$
     #[serde(alias = "auxKw")]
+    #[validate(range(min = 0))]
     pub aux_kw: f64,
     /// Transmission mass, $kg$
     #[serde(alias = "transKg")]
+    #[validate(range(min = 0))]
     pub trans_kg: f64,
     /// Transmission efficiency
     #[serde(alias = "transEff")]
+    #[validate(range(min = 0, max = 1))]
     pub trans_eff: f64,
-    /// Maximum acceptable overall change in ESS energy relative to energy from fuel (HEV SOC balancing only), $\frac{\Delta E_{ESS}}{\Delta E_{fuel}}$
+    /// Maximum acceptable ratio of change in ESS energy to expended fuel energy (used in hybrid SOC balancing), $\frac{\Delta E_{ESS}}{\Delta E_{fuel}}$
     #[serde(alias = "essToFuelOkError")]
+    #[validate(range(min = 0))]
     pub ess_to_fuel_ok_error: f64,
     #[doc(hidden)]
     #[serde(skip)]
     pub small_motor_power_kw: f64,
     #[doc(hidden)]
     #[serde(skip)]
     pub large_motor_power_kw: f64,
@@ -649,17 +717,19 @@
     #[serde(skip)]
     pub val_veh_base_cost: f64,
     #[doc(hidden)]
     #[serde(skip)]
     pub val_msrp: f64,
     /// Fuel converter efficiency peak override, scales entire curve
     #[serde(skip)]
+    #[validate(range(min = 0, max = 1))]
     pub fc_peak_eff_override: Option<f64>,
     /// Motor efficiency peak override, scales entire curve
     #[serde(skip)]
+    #[validate(range(min = 0, max = 1))]
     pub mc_peak_eff_override: Option<f64>,
     #[serde(skip)]
     #[doc(hidden)]
     pub orphaned: bool,
 }
 
 /// RustVehicle rust methods
@@ -748,15 +818,15 @@
         val_veh_base_cost: f64,
         val_msrp: f64,
         props: RustPhysicalProperties,
         regen_a: f64,
         regen_b: f64,
         fc_peak_eff_override: Option<f64>,
         mc_peak_eff_override: Option<f64>,
-    ) -> Self {
+    ) -> Result<Self, anyhow::Error> {
         let fc_pwr_out_perc = Array::from_vec(fc_pwr_out_perc);
         let fc_eff_map = Array::from_vec(fc_eff_map);
         let mc_pwr_out_perc = Array::from_vec(mc_pwr_out_perc);
         let mc_eff_map: Array1<f64> =
             Array::from_vec(mc_eff_map.unwrap_or_else(|| vec![0.0; LARGE_BASELINE_EFF.len()]));
         let veh_override_kg: f64 = veh_override_kg.unwrap_or(0.0);
 
@@ -867,16 +937,20 @@
             fc_mass_kg: 0.0,
             fs_mass_kg: 0.0,
             mc_perc_out_array: Default::default(),
             fc_peak_eff_override,
             mc_peak_eff_override,
             orphaned: false,
         };
+        match veh.validate() {
+            Ok(_) => (),
+            Err(e) => bail!(e),
+        };
         veh.set_derived();
-        veh
+        Ok(veh)
     }
 
     /// Calculate total vehicle mass. Sum up component masses if
     /// positive real number is not specified for self.veh_override_kg
     #[allow(clippy::neg_cmp_op_on_partial_ord)]
     pub fn set_veh_mass(&mut self) {
         let mut ess_mass_kg = 0.0;
@@ -1393,14 +1467,15 @@
             //mc_mass_kg,
             //fc_mass_kg,
             //fs_mass_kg,
             //None,
             None,
             None,
         )
+        .unwrap()
     }
 
     pub fn from_file(filename: &str) -> Result<Self, anyhow::Error> {
         let extension = Path::new(filename)
             .extension()
             .and_then(OsStr::to_str)
             .unwrap_or("");
@@ -1420,14 +1495,226 @@
         veh_res
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use validator::ValidationErrors;
 
     #[test]
     fn test_set_derived_via_new() {
         let veh = RustVehicle::mock_vehicle();
         assert!(veh.veh_kg > 0.0);
     }
+
+    // test input validation by providing bad inputs, then checking
+    // the produced error for the offending field names
+    #[test]
+    fn test_input_validation() {
+        // set up vehicle input parameters
+        let scenario_name = String::from("2016 FORD Escape 4cyl 2WD");
+        let selection: u32 = 5;
+        let veh_year: u32 = 2016;
+        let veh_pt_type = String::from("whoops"); // bad input
+        let drag_coef: f64 = 0.355;
+        let frontal_area_m2: f64 = 3.066;
+        let glider_kg: f64 = -50.0; // bad input
+        let veh_cg_m: f64 = 0.53;
+        let drive_axle_weight_frac: f64 = 0.59;
+        let wheel_base_m: f64 = 2.6;
+        let cargo_kg: f64 = 136.0;
+        let veh_override_kg: Option<f64> = None;
+        let comp_mass_multiplier: f64 = 1.4;
+        let fs_max_kw: f64 = 2000.0;
+        let fs_secs_to_peak_pwr: f64 = 1.0;
+        let fs_kwh: f64 = 504.0;
+        let fs_kwh_per_kg: f64 = 9.89;
+        let fc_max_kw: f64 = -60.0; // bad input
+        let fc_pwr_out_perc: Vec<f64> = vec![
+            0.0, 0.005, 0.015, 0.04, 0.06, 0.1, 0.14, 0.2, 0.4, 0.6, 0.8, 1.0,
+        ];
+        let fc_eff_map: Vec<f64> = vec![
+            0.1, 0.12, 0.16, 0.22, 0.28, 0.33, 0.35, 0.36, 0.35, 0.34, 0.32, 0.3,
+        ];
+        let fc_eff_type: String = String::from("SI");
+        let fc_sec_to_peak_pwr: f64 = 6.0;
+        let fc_base_kg: f64 = 61.0;
+        let fc_kw_per_kg: f64 = 2.13;
+        let min_fc_time_on: f64 = 30.0;
+        let idle_fc_kw: f64 = 2.5;
+        let mc_max_kw: f64 = 0.0;
+        let mc_pwr_out_perc: Vec<f64> =
+            vec![0.0, 0.02, 0.04, 0.06, 0.08, 0.1, 0.2, 0.4, 0.6, 0.8, 1.0];
+        let mc_eff_map: Vec<f64> = vec![
+            0.12, 0.16, 0.21, 0.29, 0.35, 0.42, 0.75, 0.92, 0.93, 0.93, 0.92,
+        ];
+        let mc_sec_to_peak_pwr: f64 = 4.0;
+        let mc_pe_kg_per_kw: f64 = 0.833;
+        let mc_pe_base_kg: f64 = 21.6;
+        let ess_max_kw: f64 = 0.0;
+        let ess_max_kwh: f64 = 0.0;
+        let ess_kg_per_kwh: f64 = 8.0;
+        let ess_base_kg: f64 = 75.0;
+        let ess_round_trip_eff: f64 = 0.97;
+        let ess_life_coef_a: f64 = 110.0;
+        let ess_life_coef_b: f64 = -0.6811;
+        let min_soc: f64 = -0.5; // bad input
+        let max_soc: f64 = 1.5; // bad input
+        let ess_dischg_to_fc_max_eff_perc: f64 = 0.0;
+        let ess_chg_to_fc_max_eff_perc: f64 = 0.0;
+        let wheel_inertia_kg_m2: f64 = 0.815;
+        let num_wheels: f64 = 4.0;
+        let wheel_rr_coef: f64 = 0.006;
+        let wheel_radius_m: f64 = 0.336;
+        let wheel_coef_of_fric: f64 = 0.7;
+        let max_accel_buffer_mph: f64 = 60.0;
+        let max_accel_buffer_perc_of_useable_soc: f64 = 0.2;
+        let perc_high_acc_buf: f64 = 0.0;
+        let mph_fc_on: f64 = 30.0;
+        let kw_demand_fc_on: f64 = 100.0;
+        let max_regen: f64 = 0.98;
+        let stop_start: bool = false;
+        let force_aux_on_fc: bool = true;
+        let alt_eff: f64 = 1.0;
+        let chg_eff: f64 = 0.86;
+        let aux_kw: f64 = 0.7;
+        let trans_kg: f64 = 114.0;
+        let trans_eff: f64 = 0.92;
+        let ess_to_fuel_ok_error: f64 = 0.005;
+        let val_udds_mpgge: f64 = 23.0;
+        let val_hwy_mpgge: f64 = 32.0;
+        let val_comb_mpgge: f64 = 26.0;
+        let val_udds_kwh_per_mile: f64 = f64::NAN;
+        let val_hwy_kwh_per_mile: f64 = f64::NAN;
+        let val_comb_kwh_per_mile: f64 = f64::NAN;
+        let val_cd_range_mi: f64 = f64::NAN;
+        let val_const65_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const60_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const55_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const45_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_unadj_udds_kwh_per_mile: f64 = f64::NAN;
+        let val_unadj_hwy_kwh_per_mile: f64 = f64::NAN;
+        let val0_to60_mph: f64 = 9.9;
+        let val_ess_life_miles: f64 = f64::NAN;
+        let val_range_miles: f64 = f64::NAN;
+        let val_veh_base_cost: f64 = f64::NAN;
+        let val_msrp: f64 = f64::NAN;
+        let props = RustPhysicalProperties::default();
+        let regen_a: f64 = 500.0;
+        let regen_b: f64 = 0.99;
+        let fc_peak_eff_override: Option<f64> = None;
+        let mc_peak_eff_override: Option<f64> = Some(-0.50); // bad input
+
+        // instantiate vehicle result
+        let veh_result = RustVehicle::new(
+            scenario_name,
+            selection,
+            veh_year,
+            veh_pt_type, // bad input
+            drag_coef,
+            frontal_area_m2,
+            glider_kg, // bad input
+            veh_cg_m,
+            drive_axle_weight_frac,
+            wheel_base_m,
+            cargo_kg,
+            veh_override_kg,
+            comp_mass_multiplier,
+            fs_max_kw,
+            fs_secs_to_peak_pwr,
+            fs_kwh,
+            fs_kwh_per_kg,
+            fc_max_kw, // bad input
+            fc_pwr_out_perc,
+            fc_eff_map,
+            fc_eff_type,
+            fc_sec_to_peak_pwr,
+            fc_base_kg,
+            fc_kw_per_kg,
+            min_fc_time_on,
+            idle_fc_kw,
+            mc_max_kw,
+            mc_pwr_out_perc,
+            Some(mc_eff_map),
+            mc_sec_to_peak_pwr,
+            mc_pe_kg_per_kw,
+            mc_pe_base_kg,
+            ess_max_kw,
+            ess_max_kwh,
+            ess_kg_per_kwh,
+            ess_base_kg,
+            ess_round_trip_eff,
+            ess_life_coef_a,
+            ess_life_coef_b,
+            min_soc, // bad input
+            max_soc, // bad input
+            ess_dischg_to_fc_max_eff_perc,
+            ess_chg_to_fc_max_eff_perc,
+            wheel_inertia_kg_m2,
+            num_wheels,
+            wheel_rr_coef,
+            wheel_radius_m,
+            wheel_coef_of_fric,
+            max_accel_buffer_mph,
+            max_accel_buffer_perc_of_useable_soc,
+            perc_high_acc_buf,
+            mph_fc_on,
+            kw_demand_fc_on,
+            max_regen,
+            stop_start,
+            force_aux_on_fc,
+            alt_eff,
+            chg_eff,
+            aux_kw,
+            trans_kg,
+            trans_eff,
+            ess_to_fuel_ok_error,
+            val_udds_mpgge,
+            val_hwy_mpgge,
+            val_comb_mpgge,
+            val_udds_kwh_per_mile,
+            val_hwy_kwh_per_mile,
+            val_comb_kwh_per_mile,
+            val_cd_range_mi,
+            val_const65_mph_kwh_per_mile,
+            val_const60_mph_kwh_per_mile,
+            val_const55_mph_kwh_per_mile,
+            val_const45_mph_kwh_per_mile,
+            val_unadj_udds_kwh_per_mile,
+            val_unadj_hwy_kwh_per_mile,
+            val0_to60_mph,
+            val_ess_life_miles,
+            val_range_miles,
+            val_veh_base_cost,
+            val_msrp,
+            props,
+            regen_a,
+            regen_b,
+            fc_peak_eff_override,
+            mc_peak_eff_override, // bad input
+        );
+
+        // hard-coded fields where bad inputs were provided above
+        let bad_fields = [
+            "veh_pt_type",
+            "glider_kg",
+            "fc_max_kw",
+            "min_soc",
+            "max_soc",
+            "mc_peak_eff_override",
+        ];
+        // downcast anyhow::error back into validator::ValidationErrors
+        // this test will fail on the unwrap() if the error is not downcastable to ValidationErrors
+        // e.g. if the error was not from input validation
+        let validation_errs = veh_result
+            .unwrap_err()
+            .downcast::<ValidationErrors>()
+            .unwrap();
+        let validation_errs_hashmap = validation_errs.errors();
+        // assert that specified bad fields were caught
+        assert!(validation_errs_hashmap
+            .keys()
+            .all(|key| bad_fields.contains(key)));
+        assert!(validation_errs_hashmap.len() == bad_fields.len());
+    }
 }
```

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/vehicle_thermal.rs` & `fastsim-2.0.19/rust/fastsim-core/src/vehicle_thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-core/src/vehicle_utils.rs` & `fastsim-2.0.19/rust/fastsim-core/src/vehicle_utils.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-py/Cargo.toml` & `fastsim-2.0.19/rust/fastsim-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/rust/fastsim-py/src/lib.rs` & `fastsim-2.0.19/rust/fastsim-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.18/setup.py` & `fastsim-2.0.19/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""PyPI setup script.  To use it, run `python setup.py sdist bdist_wheel` from this directory."""
+"""
+PyPI setup script.  To use it, run `python setup.py sdist bdist_wheel` from this directory.
+"""
 
 import setuptools
 from setuptools_rust import RustExtension, Binding
 
 import os
 import sys
 develop_mode = os.environ.get("DEVELOP_MODE", False)
@@ -15,15 +17,18 @@
             "fastsimrust",
             "rust/fastsim-py/Cargo.toml",
             binding=Binding.PyO3,
             py_limited_api=True,
         ),
     ]
 
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # rust extension
     rust_extensions=rust_extensions,
+    include_package_data=True,
+    package_data={
+        "fastsim": ["README.md", "LICENSE.md", "rust/*"],
+    },
 )
```

