# Comparing `tmp/floodmodeller_api-0.4.1.tar.gz` & `tmp/floodmodeller_api-0.4.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floodmodeller_api-0.4.1.tar", last modified: Fri Mar 10 16:11:52 2023, max compression
+gzip compressed data, was "floodmodeller_api-0.4.1.post1.tar", last modified: Wed Apr 19 11:32:29 2023, max compression
```

## Comparing `floodmodeller_api-0.4.1.tar` & `floodmodeller_api-0.4.1.post1.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.865107 floodmodeller_api-0.4.1/
--rw-rw-rw-   0        0        0      190 2023-03-10 15:50:08.000000 floodmodeller_api-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4296 2023-03-10 16:11:52.864109 floodmodeller_api-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3324 2023-03-10 11:38:46.000000 floodmodeller_api-0.4.1/README.md
--rw-rw-rw-   0        0        0     4751 2022-05-18 11:19:34.000000 floodmodeller_api-0.4.1/code-of-conduct.md
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.289679 floodmodeller_api-0.4.1/floodmodeller_api/
--rw-rw-rw-   0        0        0      247 2022-09-05 15:46:08.000000 floodmodeller_api-0.4.1/floodmodeller_api/__init__.py
--rw-rw-rw-   0        0        0     7805 2023-03-10 14:34:14.000000 floodmodeller_api-0.4.1/floodmodeller_api/_base.py
--rw-rw-rw-   0        0        0    11795 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/backup.py
--rw-rw-rw-   0        0        0    35053 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/dat.py
--rw-rw-rw-   0        0        0     4936 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/diff.py
--rw-rw-rw-   0        0        0    12892 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/ied.py
--rw-rw-rw-   0        0        0    27159 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/ief.py
--rw-rw-rw-   0        0        0    11562 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/ief_flags.py
--rw-rw-rw-   0        0        0    12118 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/inp.py
--rw-rw-rw-   0        0        0  1721680 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1/floodmodeller_api/libifcoremd.dll
--rw-rw-rw-   0        0        0  4458832 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1/floodmodeller_api/libmmd.dll
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.328543 floodmodeller_api-0.4.1/floodmodeller_api/logs/
--rw-rw-rw-   0        0        0       76 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/logs/__init__.py
--rw-rw-rw-   0        0        0    11006 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/logs/lf.py
--rw-rw-rw-   0        0        0     9863 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/logs/lf_helpers.py
--rw-rw-rw-   0        0        0    15807 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/logs/lf_params.py
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.367438 floodmodeller_api-0.4.1/floodmodeller_api/test/
--rw-rw-rw-   0        0        0       85 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/__init__.py
--rw-rw-rw-   0        0        0      153 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/conftest.py
--rw-rw-rw-   0        0        0     4306 2023-03-10 15:27:46.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_backup.py
--rw-rw-rw-   0        0        0     3284 2023-03-10 14:00:10.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_dat.py
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.718499 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/
--rw-rw-rw-   0        0        0    33666 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/All Units 4_6.DAT
--rw-rw-rw-   0        0        0    33666 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/All Units 4_6.feb
--rw-rw-rw-   0        0        0    32682 2022-05-23 13:45:26.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/BRIDGE.DAT
--rw-rw-rw-   0        0        0     1473 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.dat
--rw-rw-rw-   0        0        0     1473 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.feb
--rw-rw-rw-   0        0        0     2157 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakADI.xml
--rw-rw-rw-   0        0        0     2373 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakFAST.xml
--rw-rw-rw-   0        0        0     2138 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakFAST_dy.xml
--rw-rw-rw-   0        0        0     2183 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakTVD.xml
--rw-rw-rw-   0        0        0     2248 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreach.xml
--rw-rw-rw-   0        0        0     2403 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreachFAST.xml
--rw-rw-rw-   0        0        0     2169 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreachFAST_dy.xml
--rw-rw-rw-   0        0        0     2604 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1+2_QH.xml
--rw-rw-rw-   0        0        0     1463 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_H.xml
--rw-rw-rw-   0        0        0     1472 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q.xml
--rw-rw-rw-   0        0        0     1771 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q_FAST.xml
--rw-rw-rw-   0        0        0     1779 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q_FAST_dy.xml
--rw-rw-rw-   0        0        0     1475 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_W.xml
--rw-rw-rw-   0        0        0    22430 2021-12-14 12:06:23.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.DAT
--rw-rw-rw-   0        0        0     1685 2021-12-14 11:50:12.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.ext
--rw-rw-rw-   0        0        0    23132 2021-12-14 11:49:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.feb
--rw-rw-rw-   0        0        0     1685 2021-12-14 12:06:23.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.gxy
--rw-rw-rw-   0        0        0    14395 2021-12-10 17:29:13.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.DAT
--rw-rw-rw-   0        0        0     3449 2021-12-10 17:29:13.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.ext
--rw-rw-rw-   0        0        0    14395 2021-12-10 18:13:32.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.feb
--rw-rw-rw-   0        0        0    11795 2015-01-30 20:38:06.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX18.DAT
--rw-rw-rw-   0        0        0     7346 2015-01-30 12:55:52.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX2.DAT
--rw-rw-rw-   0        0        0    32692 2021-10-06 15:55:52.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX3.DAT
--rw-rw-rw-   0        0        0    56320 2021-12-10 19:43:48.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.DAT
--rw-rw-rw-   0        0        0    11125 2021-12-10 19:42:52.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.ext
--rw-rw-rw-   0        0        0    56276 2021-12-10 19:42:21.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.feb
--rw-rw-rw-   0        0        0     9303 2021-12-10 17:50:14.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.DAT
--rw-rw-rw-   0        0        0     1721 2021-12-10 17:49:24.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.ext
--rw-rw-rw-   0        0        0     9303 2021-12-10 18:13:34.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.feb
--rw-rw-rw-   0        0        0     2190 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2D.xml
--rw-rw-rw-   0        0        0     2300 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2DFAST.xml
--rw-rw-rw-   0        0        0     2067 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2DFAST_dy.xml
--rw-rw-rw-   0        0        0     1397 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.dat
--rw-rw-rw-   0        0        0      538 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.ext
--rw-rw-rw-   0        0        0      278 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.feb
--rw-rw-rw-   0        0        0      921 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.gxy
--rw-rw-rw-   0        0        0     6607 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.dat
--rw-rw-rw-   0        0        0      536 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.ext
--rw-rw-rw-   0        0        0      278 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.feb
--rw-rw-rw-   0        0        0     2450 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.fmpx
--rw-rw-rw-   0        0        0     1057 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.gxy
--rw-rw-rw-   0        0        0      381 2022-09-05 15:46:08.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex3.ief
--rw-rw-rw-   0        0        0    94378 2022-09-07 12:44:27.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex3.lf1
--rw-rw-rw-   0        0        0    47074 2015-01-30 19:36:38.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex4.DAT
--rw-rw-rw-   0        0        0    84885 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex4_changed.DAT
--rw-rw-rw-   0        0        0    17968 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example1.inp
--rw-rw-rw-   0        0        0     7422 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example2.inp
--rw-rw-rw-   0        0        0    17690 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example3.inp
--rw-rw-rw-   0        0        0    19479 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example4.inp
--rw-rw-rw-   0        0        0     5633 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example5.inp
--rw-rw-rw-   0        0        0     6428 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example6.inp
--rw-rw-rw-   0        0        0     4913 2015-01-30 20:28:40.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/jump.dat
--rw-rw-rw-   0        0        0    84297 2021-07-08 14:24:13.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.dat
--rw-rw-rw-   0        0        0      538 2021-07-08 14:32:20.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.ext
--rw-rw-rw-   0        0        0       86 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.exy
--rw-rw-rw-   0        0        0      926 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.feb
--rw-rw-rw-   0        0        0      926 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.ied
--rw-rw-rw-   0        0        0      351 2021-07-08 14:36:52.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.ief
--rw-rw-rw-   0        0        0     5633 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.inp
--rw-rw-rw-   0        0        0     8600 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.mmm
--rw-rw-rw-   0        0        0      713 2021-07-08 14:32:48.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.pxy
--rw-rw-rw-   0        0        0        0 2021-07-08 14:36:34.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.uic
--rw-rw-rw-   0        0        0     4824 2021-07-08 14:37:06.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzd
--rw-rw-rw-   0        0        0     2176 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzl
--rw-rw-rw-   0        0        0   373584 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzn
--rw-rw-rw-   0        0        0        0 2021-07-08 14:36:37.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzu
--rw-rw-rw-   0        0        0   311556 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzx
--rw-rw-rw-   0        0        0     3302 2021-07-12 12:02:06.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network_from_tabularCSV.csv
--rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.dat
--rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.ext
--rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.feb
--rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.gxy
--rw-rw-rw-   0        0        0     3415 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.dat
--rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.ext
--rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.feb
--rw-rw-rw-   0        0        0     2433 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.fmpx
--rw-rw-rw-   0        0        0      611 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.gxy
--rw-rw-rw-   0        0        0     4475 2023-03-10 15:23:33.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/test_output.csv
--rw-rw-rw-   0        0        0      516 2022-05-11 10:13:09.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/unit checks.dat
--rw-rw-rw-   0        0        0      820 2023-03-10 14:00:10.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_ied.py
--rw-rw-rw-   0        0        0      539 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_ief.py
--rw-rw-rw-   0        0        0     1534 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_inp.py
--rw-rw-rw-   0        0        0     1361 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_logs_lf.py
--rw-rw-rw-   0        0        0     1575 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_xml2d.py
--rw-rw-rw-   0        0        0     1141 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/test/test_zzn.py
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.787314 floodmodeller_api-0.4.1/floodmodeller_api/units/
--rw-rw-rw-   0        0        0       22 2022-06-15 09:09:07.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/__init__.py
--rw-rw-rw-   0        0        0     3515 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/_base.py
--rw-rw-rw-   0        0        0    20183 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/boundaries.py
--rw-rw-rw-   0        0        0     9212 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/conduits.py
--rw-rw-rw-   0        0        0     4335 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/helpers.py
--rw-rw-rw-   0        0        0     3790 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/iic.py
--rw-rw-rw-   0        0        0    12646 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/losses.py
--rw-rw-rw-   0        0        0    14371 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/sections.py
--rw-rw-rw-   0        0        0    71393 2023-03-10 14:34:17.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/structures.py
--rw-rw-rw-   0        0        0     6235 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/units.py
--rw-rw-rw-   0        0        0     2029 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/units/unsupported.py
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.841173 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/
--rw-rw-rw-   0        0        0       27 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/_base.py
--rw-rw-rw-   0        0        0     3931 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/conduits.py
--rw-rw-rw-   0        0        0     2056 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/general_parameters.py
--rw-rw-rw-   0        0        0     3363 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/junctions.py
--rw-rw-rw-   0        0        0     3228 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/losses.py
--rw-rw-rw-   0        0        0     4751 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/outfalls.py
--rw-rw-rw-   0        0        0     4644 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/raingauges.py
--rw-rw-rw-   0        0        0     3323 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/subsections.py
--rw-rw-rw-   0        0        0     5697 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/urban1d/xsections.py
--rw-rw-rw-   0        0        0     1079 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/util.py
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.859124 floodmodeller_api-0.4.1/floodmodeller_api/validation/
--rw-rw-rw-   0        0        0       39 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/validation/__init__.py
--rw-rw-rw-   0        0        0    15545 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/validation/parameters.py
--rw-rw-rw-   0        0        0    12322 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/validation/urban_parameters.py
--rw-rw-rw-   0        0        0     4340 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/validation/validation.py
--rw-rw-rw-   0        0        0       23 2023-03-10 16:09:56.000000 floodmodeller_api-0.4.1/floodmodeller_api/version.py
--rw-rw-rw-   0        0        0    28238 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/xml2d.py
--rw-rw-rw-   0        0        0     1847 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1/floodmodeller_api/xml2d_template.py
--rw-rw-rw-   0        0        0    16560 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/floodmodeller_api/zzn.py
--rw-rw-rw-   0        0        0    76800 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1/floodmodeller_api/zzn_read.dll
-drwxrwxrwx   0        0        0        0 2023-03-10 16:11:52.312610 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/
--rw-rw-rw-   0        0        0     4296 2023-03-10 16:11:51.000000 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6195 2023-03-10 16:11:51.000000 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 16:11:51.000000 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-10 16:11:51.000000 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-10 16:11:51.000000 floodmodeller_api-0.4.1/floodmodeller_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      933 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1/license.txt
--rw-rw-rw-   0        0        0       40 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 16:11:52.866104 floodmodeller_api-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1192 2023-03-10 15:29:53.000000 floodmodeller_api-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:29.501863 floodmodeller_api-0.4.1.post1/
+-rw-rw-rw-   0        0        0      190 2023-03-10 15:50:08.000000 floodmodeller_api-0.4.1.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4590 2023-04-19 11:32:29.499869 floodmodeller_api-0.4.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     3588 2023-04-19 10:53:34.000000 floodmodeller_api-0.4.1.post1/README.md
+-rw-rw-rw-   0        0        0     4751 2022-05-18 11:19:34.000000 floodmodeller_api-0.4.1.post1/code-of-conduct.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:27.640484 floodmodeller_api-0.4.1.post1/floodmodeller_api/
+-rw-rw-rw-   0        0        0      247 2022-09-05 15:46:08.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/__init__.py
+-rw-rw-rw-   0        0        0     7805 2023-03-10 14:34:14.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/_base.py
+-rw-rw-rw-   0        0        0    11795 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/backup.py
+-rw-rw-rw-   0        0        0    35053 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/dat.py
+-rw-rw-rw-   0        0        0     4936 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/diff.py
+-rw-rw-rw-   0        0        0    12892 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/ied.py
+-rw-rw-rw-   0        0        0    27199 2023-04-19 10:53:34.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/ief.py
+-rw-rw-rw-   0        0        0    11562 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/ief_flags.py
+-rw-rw-rw-   0        0        0    12118 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/inp.py
+-rw-rw-rw-   0        0        0  1721680 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/libifcoremd.dll
+-rw-rw-rw-   0        0        0  4458832 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/libmmd.dll
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:27.719307 floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/
+-rw-rw-rw-   0        0        0       76 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/__init__.py
+-rw-rw-rw-   0        0        0    11006 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf.py
+-rw-rw-rw-   0        0        0     9863 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf_helpers.py
+-rw-rw-rw-   0        0        0    15807 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf_params.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:27.869871 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/
+-rw-rw-rw-   0        0        0       85 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/__init__.py
+-rw-rw-rw-   0        0        0      153 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/conftest.py
+-rw-rw-rw-   0        0        0     4306 2023-03-10 15:27:46.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_backup.py
+-rw-rw-rw-   0        0        0     3284 2023-03-10 14:00:10.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_dat.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:29.209645 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/
+-rw-rw-rw-   0        0        0    33666 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/All Units 4_6.DAT
+-rw-rw-rw-   0        0        0    33666 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/All Units 4_6.feb
+-rw-rw-rw-   0        0        0    32682 2022-05-23 13:45:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/BRIDGE.DAT
+-rw-rw-rw-   0        0        0     1473 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.dat
+-rw-rw-rw-   0        0        0     1473 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.feb
+-rw-rw-rw-   0        0        0     2157 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakADI.xml
+-rw-rw-rw-   0        0        0     2373 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakFAST.xml
+-rw-rw-rw-   0        0        0     2138 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakFAST_dy.xml
+-rw-rw-rw-   0        0        0     2183 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakTVD.xml
+-rw-rw-rw-   0        0        0     2248 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreach.xml
+-rw-rw-rw-   0        0        0     2403 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreachFAST.xml
+-rw-rw-rw-   0        0        0     2169 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreachFAST_dy.xml
+-rw-rw-rw-   0        0        0     2604 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1+2_QH.xml
+-rw-rw-rw-   0        0        0     1463 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_H.xml
+-rw-rw-rw-   0        0        0     1472 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q.xml
+-rw-rw-rw-   0        0        0     1771 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q_FAST.xml
+-rw-rw-rw-   0        0        0     1779 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q_FAST_dy.xml
+-rw-rw-rw-   0        0        0     1475 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_W.xml
+-rw-rw-rw-   0        0        0    22430 2021-12-14 12:06:23.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.DAT
+-rw-rw-rw-   0        0        0     1685 2021-12-14 11:50:12.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.ext
+-rw-rw-rw-   0        0        0    23132 2021-12-14 11:49:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.feb
+-rw-rw-rw-   0        0        0     1685 2021-12-14 12:06:23.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.gxy
+-rw-rw-rw-   0        0        0    14395 2021-12-10 17:29:13.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.DAT
+-rw-rw-rw-   0        0        0     3449 2021-12-10 17:29:13.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.ext
+-rw-rw-rw-   0        0        0    14395 2021-12-10 18:13:32.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.feb
+-rw-rw-rw-   0        0        0    11795 2015-01-30 20:38:06.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX18.DAT
+-rw-rw-rw-   0        0        0     7346 2015-01-30 12:55:52.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX2.DAT
+-rw-rw-rw-   0        0        0    32692 2021-10-06 15:55:52.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX3.DAT
+-rw-rw-rw-   0        0        0    56320 2021-12-10 19:43:48.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.DAT
+-rw-rw-rw-   0        0        0    11125 2021-12-10 19:42:52.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.ext
+-rw-rw-rw-   0        0        0    56276 2021-12-10 19:42:21.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.feb
+-rw-rw-rw-   0        0        0     9303 2021-12-10 17:50:14.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.DAT
+-rw-rw-rw-   0        0        0     1721 2021-12-10 17:49:24.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.ext
+-rw-rw-rw-   0        0        0     9303 2021-12-10 18:13:34.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.feb
+-rw-rw-rw-   0        0        0     2190 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2D.xml
+-rw-rw-rw-   0        0        0     2300 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2DFAST.xml
+-rw-rw-rw-   0        0        0     2067 2022-09-02 15:28:25.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2DFAST_dy.xml
+-rw-rw-rw-   0        0        0     1397 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.dat
+-rw-rw-rw-   0        0        0      538 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.ext
+-rw-rw-rw-   0        0        0      278 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.feb
+-rw-rw-rw-   0        0        0      921 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.gxy
+-rw-rw-rw-   0        0        0     6607 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.dat
+-rw-rw-rw-   0        0        0      536 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.ext
+-rw-rw-rw-   0        0        0      278 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.feb
+-rw-rw-rw-   0        0        0     2450 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.fmpx
+-rw-rw-rw-   0        0        0     1057 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.gxy
+-rw-rw-rw-   0        0        0      381 2022-09-05 15:46:08.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex3.ief
+-rw-rw-rw-   0        0        0    94378 2022-09-07 12:44:27.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex3.lf1
+-rw-rw-rw-   0        0        0    47074 2015-01-30 19:36:38.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex4.DAT
+-rw-rw-rw-   0        0        0    84885 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex4_changed.DAT
+-rw-rw-rw-   0        0        0    17968 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example1.inp
+-rw-rw-rw-   0        0        0     7422 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example2.inp
+-rw-rw-rw-   0        0        0    17690 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example3.inp
+-rw-rw-rw-   0        0        0    19479 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example4.inp
+-rw-rw-rw-   0        0        0     5633 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example5.inp
+-rw-rw-rw-   0        0        0     6428 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example6.inp
+-rw-rw-rw-   0        0        0     4913 2015-01-30 20:28:40.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/jump.dat
+-rw-rw-rw-   0        0        0    84297 2021-07-08 14:24:13.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.dat
+-rw-rw-rw-   0        0        0      538 2021-07-08 14:32:20.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.ext
+-rw-rw-rw-   0        0        0       86 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.exy
+-rw-rw-rw-   0        0        0      926 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.feb
+-rw-rw-rw-   0        0        0      926 2022-04-29 10:36:42.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.ied
+-rw-rw-rw-   0        0        0      351 2021-07-08 14:36:52.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.ief
+-rw-rw-rw-   0        0        0     5633 2022-07-08 16:08:39.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.inp
+-rw-rw-rw-   0        0        0     8600 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.mmm
+-rw-rw-rw-   0        0        0      713 2021-07-08 14:32:48.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.pxy
+-rw-rw-rw-   0        0        0        0 2021-07-08 14:36:34.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.uic
+-rw-rw-rw-   0        0        0     4824 2021-07-08 14:37:06.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzd
+-rw-rw-rw-   0        0        0     2176 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzl
+-rw-rw-rw-   0        0        0   373584 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzn
+-rw-rw-rw-   0        0        0        0 2021-07-08 14:36:37.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzu
+-rw-rw-rw-   0        0        0   311556 2021-07-08 14:37:05.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzx
+-rw-rw-rw-   0        0        0     3302 2021-07-12 12:02:06.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network_from_tabularCSV.csv
+-rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.dat
+-rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.ext
+-rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.feb
+-rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.gxy
+-rw-rw-rw-   0        0        0     3415 2023-01-25 13:31:41.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.dat
+-rw-rw-rw-   0        0        0      513 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.ext
+-rw-rw-rw-   0        0        0      278 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.feb
+-rw-rw-rw-   0        0        0     2433 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.fmpx
+-rw-rw-rw-   0        0        0      611 2022-09-09 15:42:49.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.gxy
+-rw-rw-rw-   0        0        0     4475 2023-04-12 11:21:04.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/test_output.csv
+-rw-rw-rw-   0        0        0      516 2022-05-11 10:13:09.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/unit checks.dat
+-rw-rw-rw-   0        0        0      820 2023-03-10 14:00:10.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_ied.py
+-rw-rw-rw-   0        0        0      539 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_ief.py
+-rw-rw-rw-   0        0        0     1534 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_inp.py
+-rw-rw-rw-   0        0        0     1361 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_logs_lf.py
+-rw-rw-rw-   0        0        0     5721 2023-04-19 10:53:03.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_xml2d.py
+-rw-rw-rw-   0        0        0     1141 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_zzn.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:29.331323 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/
+-rw-rw-rw-   0        0        0       22 2022-06-15 09:09:07.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/__init__.py
+-rw-rw-rw-   0        0        0     3515 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/_base.py
+-rw-rw-rw-   0        0        0    20183 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/boundaries.py
+-rw-rw-rw-   0        0        0     9212 2023-03-10 14:34:15.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/conduits.py
+-rw-rw-rw-   0        0        0     4335 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/helpers.py
+-rw-rw-rw-   0        0        0     3790 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/iic.py
+-rw-rw-rw-   0        0        0    12646 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/losses.py
+-rw-rw-rw-   0        0        0    15761 2023-03-14 17:11:07.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/sections.py
+-rw-rw-rw-   0        0        0    71393 2023-03-10 14:34:17.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/structures.py
+-rw-rw-rw-   0        0        0     6235 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/units.py
+-rw-rw-rw-   0        0        0     2029 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/units/unsupported.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:29.427064 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/
+-rw-rw-rw-   0        0        0       27 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/_base.py
+-rw-rw-rw-   0        0        0     3931 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/conduits.py
+-rw-rw-rw-   0        0        0     2056 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/general_parameters.py
+-rw-rw-rw-   0        0        0     3363 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/junctions.py
+-rw-rw-rw-   0        0        0     3228 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/losses.py
+-rw-rw-rw-   0        0        0     4751 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/outfalls.py
+-rw-rw-rw-   0        0        0     4644 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/raingauges.py
+-rw-rw-rw-   0        0        0     3323 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/subsections.py
+-rw-rw-rw-   0        0        0     5697 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/xsections.py
+-rw-rw-rw-   0        0        0     1079 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/util.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:29.494883 floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/
+-rw-rw-rw-   0        0        0       39 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/__init__.py
+-rw-rw-rw-   0        0        0    15545 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/parameters.py
+-rw-rw-rw-   0        0        0    12322 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/urban_parameters.py
+-rw-rw-rw-   0        0        0     4340 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/validation.py
+-rw-rw-rw-   0        0        0       29 2023-04-19 11:30:44.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/version.py
+-rw-rw-rw-   0        0        0    29045 2023-04-19 10:53:04.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/xml2d.py
+-rw-rw-rw-   0        0        0     1847 2023-03-10 14:34:16.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/xml2d_template.py
+-rw-rw-rw-   0        0        0    16560 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/zzn.py
+-rw-rw-rw-   0        0        0    76800 2022-06-15 09:19:31.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api/zzn_read.dll
+drwxrwxrwx   0        0        0        0 2023-04-19 11:32:27.665419 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/
+-rw-rw-rw-   0        0        0     4590 2023-04-19 11:32:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6195 2023-04-19 11:32:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:32:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-19 11:32:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-19 11:32:26.000000 floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      933 2023-03-10 11:35:45.000000 floodmodeller_api-0.4.1.post1/license.txt
+-rw-rw-rw-   0        0        0       40 2023-03-06 17:10:56.000000 floodmodeller_api-0.4.1.post1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:32:29.501863 floodmodeller_api-0.4.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2023-03-10 15:29:53.000000 floodmodeller_api-0.4.1.post1/setup.py
```

### Comparing `floodmodeller_api-0.4.1/PKG-INFO` & `floodmodeller_api-0.4.1.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floodmodeller_api
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Extends the functionality of Flood Modeller to python users
 Home-page: UNKNOWN
 Author: Jacobs
 Author-email: joe.pierce@jacobs.com
 License: GNU General Public License V3. Copyright (C) 2023 Jacobs U.K. Limited.
 Project-URL: API Documentation, https://api.floodmodeller.com/api/
 Project-URL: Flood Modeller Homepage, https://www.floodmodeller.com/
@@ -15,15 +15,18 @@
         [![PyPI Latest Release](https://img.shields.io/pypi/v/floodmodeller-api.svg)](https://pypi.org/project/floodmodeller-api/)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/People-Places-Solutions/floodmodeller-api/blob/main/LICENSE.txt)
         ![example workflow](https://github.com/People-Places-Solutions/floodmodeller-api/actions/workflows/run_tests.yml/badge.svg)
         [![Downloads](https://static.pepy.tech/personalized-badge/floodmodeller-api?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/floodmodeller-api)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         
+        
         # Flood Modeller Python API
+        [![Try in GitHub Codespaces!](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=39-try-api-link&repo=473959586&machine=basicLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+        
         This python package is designed to be used in conjunction with your installation of Flood Modeller to provide users with a set of tools to extend the capabilities of Flood Modeller and build into automated workflows.
         
         ![API Overview](https://raw.githubusercontent.com/People-Places-Solutions/floodmodeller-api/main/docs/source/getting_started/api_overview_small.png)
         
         ## Installation
         You can install the floodmodeller_api package from PyPI with the following command:
```

### Comparing `floodmodeller_api-0.4.1/README.md` & `floodmodeller_api-0.4.1.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/floodmodeller-api.svg)](https://pypi.org/project/floodmodeller-api/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/People-Places-Solutions/floodmodeller-api/blob/main/LICENSE.txt)
 ![example workflow](https://github.com/People-Places-Solutions/floodmodeller-api/actions/workflows/run_tests.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/floodmodeller-api?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/floodmodeller-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
+
 # Flood Modeller Python API
+[![Try in GitHub Codespaces!](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=39-try-api-link&repo=473959586&machine=basicLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+
 This python package is designed to be used in conjunction with your installation of Flood Modeller to provide users with a set of tools to extend the capabilities of Flood Modeller and build into automated workflows.
 
 ![API Overview](https://raw.githubusercontent.com/People-Places-Solutions/floodmodeller-api/main/docs/source/getting_started/api_overview_small.png)
 
 ## Installation
 You can install the floodmodeller_api package from PyPI with the following command:
```

### Comparing `floodmodeller_api-0.4.1/code-of-conduct.md` & `floodmodeller_api-0.4.1.post1/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/_base.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/_base.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/backup.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/backup.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/dat.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/dat.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/diff.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/diff.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/ied.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/ied.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/ief.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/ief.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,18 @@
             ief_string = ""
             event = 0  # Used as a counter for multiple eventdata files
             for idx, prop in enumerate(self._ief_properties):
                 if prop.startswith("["):
                     # writes the [] bound headers to ief string
                     ief_string += prop + "\n"
                 elif prop.lstrip().startswith(";"):
-                    if not self._ief_properties[idx + 1] == "EventData":
+                    if not self._ief_properties[idx + 1].lower() == "eventdata":
                         # Only write comment if not preceding event data
                         ief_string += prop + "\n"
-                elif prop == "EventData":
+                elif prop.lower() == "eventdata":
                     event_data = getattr(self, prop)
                     # Add multiple EventData if present
                     for event_idx, key in enumerate(event_data):
                         if event_idx == event:
                             ief_string += f";{key}\n{prop}={str(event_data[key])}\n"
                             break
                     event += 1
@@ -170,54 +170,58 @@
                 self._ief_properties.append(line)
         del blank_ief
 
     def _update_ief_properties(self):
         """Updates the list of properties included in the IEF file"""
         # Add new properties
         for prop, val in self.__dict__.copy().items():
-            if (prop not in self._ief_properties) and (not prop.startswith("_")):
+            if (
+                (prop not in self._ief_properties)
+                and (not prop.startswith("_"))
+                and prop != "file"
+            ):
                 # Check if valid flag
                 if prop.upper() not in flags:
                     print(
                         f"Warning: '{prop}' is not a valid IEF flag, it will be ommited from the IEF\n"
                     )
                     continue
 
-                elif prop.upper() == "EVENTDATA":
+                if prop.upper() == "EVENTDATA":
                     # This will be triggered in special case where eventdata has been added with different case, but case
                     # needs to be kept as 'EventData', to allow dealing wiht multiple IEDs
-                    if (
-                        not prop == "EventData"
-                    ):  # In case of EventData being added with correct case where it doesn't already
+                    if prop != "EventData":  
+                        # In case of EventData being added with correct case where it doesn't already
                         # exist, this stops it being deleted
                         # Add new values to EventData flag
-                        setattr(self, "EventData", val)
                         delattr(self, prop)
+                        setattr(self, "EventData", val)
+                        prop = "EventData"
+
+                
+                # Check ief group header
+                group = f"[{flags[prop.upper()]}]"
+                if group in self._ief_properties:
+                    # If group already exists, add property to end of group
+                    group_idx = False
+                    # defaults to inserting in last place
+                    insert_index = len(self._ief_properties)
+                    for idx, item in enumerate(self._ief_properties):
+                        if group_idx == True and item.startswith("["):
+                            insert_index = idx
+                            break
+                        if item == group:
+                            group_idx = True
 
+                    self._ief_properties.insert(insert_index, prop)
                 else:
-                    # Check ief group header
-                    group = f"[{flags[prop.upper()]}]"
-                    if group in self._ief_properties:
-                        # If group already exists, add property to end of group
-                        group_idx = False
-                        # defaults to inserting in last place
-                        insert_index = len(self._ief_properties)
-                        for idx, item in enumerate(self._ief_properties):
-                            if group_idx == True and item.startswith("["):
-                                insert_index = idx
-                                break
-                            if item == group:
-                                group_idx = True
-
-                        self._ief_properties.insert(insert_index, prop)
-                    else:
-                        # Add group header to the end of list
-                        self._ief_properties.append(group)
-                        # Add property to end of list
-                        self._ief_properties.append(prop)
+                    # Add group header to the end of list
+                    self._ief_properties.append(group)
+                    # Add property to end of list
+                    self._ief_properties.append(prop)
 
         # Remove any deleted properties
         self._ief_properties = [
             line
             for line in self._ief_properties
             if (
                 line.startswith("[")
@@ -394,16 +398,16 @@
         Raises:
             UserWarning: Raised if ief filepath not already specified
 
         Returns:
             subprocess.Popen(): If method == 'RETURN_PROCESS', the Popen() instance of the process is returned.
         """
         try:
-            self.range_function = range_function
-            self.range_settings = range_settings
+            self._range_function = range_function
+            self._range_settings = range_settings
             if self._filepath == None:
                 raise UserWarning(
                     "IEF must be saved to a specific filepath before simulate() can be called."
                 )
             if precision.upper() == "DEFAULT":
                 precision = "SINGLE"  # Defaults to single...
                 for attr in dir(self):
@@ -602,15 +606,15 @@
         """Updates progress bar based on log file"""
 
         # only if there is a log file
         if self._lf is None:
             return
 
         # tqdm progress bar
-        for i in self.range_function(100, **self.range_settings):
+        for i in self._range_function(100, **self._range_settings):
 
             # Process still running
             while process.poll() is None:
 
                 time.sleep(0.1)
 
                 # Find progress
```

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/ief_flags.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/ief_flags.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/inp.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/inp.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/libifcoremd.dll` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/libifcoremd.dll`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/libmmd.dll` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/libmmd.dll`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/logs/lf.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/logs/lf_helpers.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf_helpers.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/logs/lf_params.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/logs/lf_params.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_backup.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_backup.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_dat.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_dat.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/All Units 4_6.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/All Units 4_6.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/All Units 4_6.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/All Units 4_6.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/BRIDGE.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/BRIDGE.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Culvert_Inlet_Outlet.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakADI.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakADI.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakFAST.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakFAST.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakFAST_dy.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakFAST_dy.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DamBreakTVD.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DamBreakTVD.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreach.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreach.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreachFAST.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreachFAST.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/DefenceBreachFAST_dy.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/DefenceBreachFAST_dy.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1+2_QH.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1+2_QH.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_H.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_H.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q_FAST.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q_FAST.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_Q_FAST_dy.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_Q_FAST_dy.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Domain1_W.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Domain1_W.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX1.gxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX1.gxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX17.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX17.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX18.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX18.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX2.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX2.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX3.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX3.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/EX6.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/EX6.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Event Data Example.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Event Data Example.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2D.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2D.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2DFAST.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2DFAST.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/Linked1D2DFAST_dy.xml` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/Linked1D2DFAST_dy.xml`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/blockage.gxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/blockage.gxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.fmpx` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.fmpx`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/defaultUnits.gxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/defaultUnits.gxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex3.lf1` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex3.lf1`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex4.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex4.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/ex4_changed.DAT` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/ex4_changed.DAT`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example1.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example1.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example2.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example2.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example3.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example3.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example4.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example4.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example5.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example5.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/example6.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/example6.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/jump.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/jump.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.feb` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.feb`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.ied` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.ied`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.inp` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.inp`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.mmm` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.mmm`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.pxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.pxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzd` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzd`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzl` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzl`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzn` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzn`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network.zzx` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network.zzx`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/network_from_tabularCSV.csv` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/network_from_tabularCSV.csv`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir.gxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir.gxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.ext` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.ext`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.fmpx` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.fmpx`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/rnweir_default.gxy` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/rnweir_default.gxy`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/test_output.csv` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/test_output.csv`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_data/unit checks.dat` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_data/unit checks.dat`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_ied.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_ied.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_ief.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_ief.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_inp.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_inp.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_logs_lf.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_logs_lf.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/test/test_zzn.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/test/test_zzn.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/_base.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/_base.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/boundaries.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/boundaries.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/conduits.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/conduits.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/helpers.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/helpers.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/iic.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/iic.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/losses.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/losses.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/sections.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/sections.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,68 @@
 
     Methods:
         convert_to_muskingham: Not currently supported but planned for future release
     """
 
     _unit = "RIVER"
 
+    def _create_from_blank(
+        self,
+        name="new_section",
+        comment="",
+        spill1 ="",
+        spill2 ="",
+        lat1 ="",
+        lat2 ="",
+        lat3 ="",
+        lat4 ="",
+        dist_to_next = 0,
+        slope=0.0001,
+        density=1000.0,
+        data=None
+    ):
+
+        # Initiate new SECTION (currently hardcoding this as default)
+        self._subtype = 'SECTION'
+
+        for param, val in {
+            "name": name,
+            "comment": comment,
+            "spill1": spill1,
+            "spill2": spill2,
+            "lat1": lat1,
+            "lat2": lat2,
+            "lat3": lat3,
+            "lat4": lat4,
+            "dist_to_next": dist_to_next,
+            "slope": slope,
+            "density": density,
+            "data": data
+        }.items():
+            setattr(self, param, val)
+
+        self.data = (
+            data
+            if isinstance(data, pd.DataFrame)
+            else pd.DataFrame(
+                [],
+                columns=[
+                    "X",
+                    "Y",
+                    "Mannings n",
+                    "Panel",
+                    "RPL",
+                    "Marker",
+                    "Easting",
+                    "Northing",
+                    "Deactivation",
+                    "SP. Marker",
+                ],)
+        )
+
     def _read(self, riv_block):
         """Function to read a given RIVER block and store data as class attributes."""
 
         self._subtype = riv_block[1].split(" ")[0].strip()
         # Only supporting 'SECTION' subtype for now
         if self.subtype == "SECTION":
             # Extends label line to be correct length before splitting to pick up blank labels
```

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/structures.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/structures.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/units.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/units.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/units/unsupported.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/units/unsupported.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/_base.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/_base.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/conduits.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/conduits.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/general_parameters.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/general_parameters.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/junctions.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/junctions.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/losses.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/losses.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/outfalls.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/outfalls.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/raingauges.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/raingauges.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/subsections.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/subsections.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/urban1d/xsections.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/urban1d/xsections.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/util.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/util.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/validation/parameters.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/parameters.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/validation/urban_parameters.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/urban_parameters.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/validation/validation.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/validation/validation.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/xml2d.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/xml2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,16 @@
             )
             raise ValueError(msg)
 
     def _recursive_update_xml(self, new_dict, orig_dict, parent_key, list_idx=None):
         # TODO: Handle removing params
 
         for key, item in new_dict.items():
+            if key in self._multi_value_keys and type(item) != list:
+                raise Exception(f"Element: '{key}' must be added as list")
             if parent_key == "ROOT":
                 parent = self._xmltree.getroot()
             else:
                 parent = self._xmltree.findall(f".//{self._ns}{parent_key}")[
                     list_idx or 0
                 ]
 
@@ -238,57 +240,67 @@
                         try:
                             self._recursive_update_xml(
                                 _item, orig_dict[key][i], key, list_idx=i
                             )
                         except IndexError:
                             # New thing added, Add it all recursively
                             self._recursive_add_element(
-                                parent=parent, add_item=_item, add_key=key
+                                parent=parent,
+                                add_item=_item,
+                                add_key=key,
+                                from_list=True,
                             )
 
             else:
                 if parent_key == "ROOT":
                     item = getattr(self, key)
                 try:
                     if not item == orig_dict[key]:
                         if key == "value":
                             # Value has been updated
                             parent.text = str(item)
                         else:
                             # Attribute has been updated
                             elems = parent.findall(f"{self._ns}{key}")
-                            if len(elems) == 1:
-                                elem = elems[0]
-                                if type(item) == list:
-                                    elem.text = "\n".join(item)
-                                else:
-                                    elem.text = str(item)
-                            elif len(elems) > 1:
+                            if type(item) == list and key != "variables":
                                 # Handle multiple similar elements
                                 if len(elems) < len(item):
                                     while len(elems) < len(item):
                                         elems.append(
                                             etree.SubElement(parent, f"{self._ns}{key}")
                                         )
                                 elif len(elems) > len(item):
                                     while len(elems) > len(item):
                                         parent.remove(elems.pop())
 
                                 for i in range(len(elems)):
                                     elems[i].text = item[i]
+                                    
+                            elif len(elems) == 1:
+                                elem = elems[0]
+                                if type(item) == list:
+                                    elem.text = "\n".join(item)
+                                else:
+                                    elem.text = str(item)
 
                             else:
                                 parent.set(key, str(item))
                 except KeyError:
                     # New value/attribute added
                     self._recursive_add_element(
                         parent=parent, add_item=item, add_key=key
                     )
 
-    def _recursive_add_element(self, parent, add_item, add_key):
+    def _recursive_add_element(self, parent, add_item, add_key, from_list=False):
+        if (
+            add_key in self._multi_value_keys
+            and type(add_item) != list
+            and not from_list
+        ):
+            raise Exception(f"Element: '{add_key}' must be added as list")
         if type(add_item) == dict:
             new_element = etree.SubElement(parent, f"{self._ns}{add_key}")
             for key, item in add_item.items():
                 self._recursive_add_element(
                     parent=new_element, add_item=item, add_key=key
                 )
         elif type(add_item) == list:
@@ -296,15 +308,15 @@
             if add_key == "variables":
                 # Variables is special case where we have list but add to one element
                 new_element = etree.SubElement(parent, f"{self._ns}{add_key}")
                 new_element.text = "\n".join(add_item)
             else:
                 for item in add_item:
                     self._recursive_add_element(
-                        parent=parent, add_item=item, add_key=add_key
+                        parent=parent, add_item=item, add_key=add_key, from_list=True
                     )
         else:
             if add_key == "value":  # Value has been added
                 parent.text = str(add_item)
             else:  # Attribute or element added
                 # Check schema to see if we should use parent.set for attribute
                 # or etree.subelement() and set text
@@ -347,15 +359,15 @@
             if elem_key in self._multi_value_keys:
                 if not list_idx_key == elem_key:
                     list_idx_key = elem_key
                     list_idx = 0
                 try:
                     self._recursive_remove_data_xml(new_dict[elem_key][list_idx], elem)
                     list_idx += 1
-                except IndexError:
+                except (IndexError, KeyError):
                     parent.remove(elem)
 
             elif elem_key in new_dict:
                 self._recursive_remove_data_xml(new_dict[elem_key], elem)
 
             else:
                 parent.remove(elem)
@@ -375,17 +387,21 @@
         ]:
             if getattr(self, attr) is not None:
                 if attr == "domains":
                     self._data["domain"] = [
                         domain for _, domain in self.domains.items()
                     ]
                 else:
-                    self._data[attr] = getattr(self, attr)
+                    try:
+                        self._data[attr] = getattr(self, attr)
+                    except AttributeError:
+                        self._data[attr] = None
 
     def _write(self) -> str:
+        orig_xml_tree = deepcopy(self._xmltree)
         try:
             self._update_dict()
             self._recursive_update_xml(self._data, self._raw_data, "ROOT")
             self._recursive_remove_data_xml(self._data, self._xmltree.getroot())
             etree.indent(self._xmltree, space="    ")
             try:
                 self._validate()
@@ -394,14 +410,15 @@
                 self._validate()
 
             self._raw_data = deepcopy(self._data)  # reset raw data to equal data
 
             return f'<?xml version="1.0" standalone="yes"?>\n{etree.tostring(self._xmltree.getroot()).decode()}'
 
         except Exception as e:
+            self._xmltree = orig_xml_tree
             self._handle_exception(e, when="write")
 
     def _get_multi_value_keys(self):
         self._multi_value_keys = []
         root = self._xsd.getroot()
         for elem in root.findall(".//{http://www.w3.org/2001/XMLSchema}element"):
             if elem.attrib.get("maxOccurs") not in (None, "0", "1"):
```

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/xml2d_template.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/xml2d_template.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/zzn.py` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/zzn.py`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api/zzn_read.dll` & `floodmodeller_api-0.4.1.post1/floodmodeller_api/zzn_read.dll`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api.egg-info/PKG-INFO` & `floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floodmodeller-api
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Extends the functionality of Flood Modeller to python users
 Home-page: UNKNOWN
 Author: Jacobs
 Author-email: joe.pierce@jacobs.com
 License: GNU General Public License V3. Copyright (C) 2023 Jacobs U.K. Limited.
 Project-URL: API Documentation, https://api.floodmodeller.com/api/
 Project-URL: Flood Modeller Homepage, https://www.floodmodeller.com/
@@ -15,15 +15,18 @@
         [![PyPI Latest Release](https://img.shields.io/pypi/v/floodmodeller-api.svg)](https://pypi.org/project/floodmodeller-api/)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/People-Places-Solutions/floodmodeller-api/blob/main/LICENSE.txt)
         ![example workflow](https://github.com/People-Places-Solutions/floodmodeller-api/actions/workflows/run_tests.yml/badge.svg)
         [![Downloads](https://static.pepy.tech/personalized-badge/floodmodeller-api?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/floodmodeller-api)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         
+        
         # Flood Modeller Python API
+        [![Try in GitHub Codespaces!](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=39-try-api-link&repo=473959586&machine=basicLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+        
         This python package is designed to be used in conjunction with your installation of Flood Modeller to provide users with a set of tools to extend the capabilities of Flood Modeller and build into automated workflows.
         
         ![API Overview](https://raw.githubusercontent.com/People-Places-Solutions/floodmodeller-api/main/docs/source/getting_started/api_overview_small.png)
         
         ## Installation
         You can install the floodmodeller_api package from PyPI with the following command:
```

### Comparing `floodmodeller_api-0.4.1/floodmodeller_api.egg-info/SOURCES.txt` & `floodmodeller_api-0.4.1.post1/floodmodeller_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/license.txt` & `floodmodeller_api-0.4.1.post1/license.txt`

 * *Files identical despite different names*

### Comparing `floodmodeller_api-0.4.1/setup.py` & `floodmodeller_api-0.4.1.post1/setup.py`

 * *Files identical despite different names*

