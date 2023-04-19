# Comparing `tmp/pyjls-0.5.2.tar.gz` & `tmp/pyjls-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.5.2.tar", last modified: Thu Mar 30 20:13:48 2023, max compression
+gzip compressed data, was "pyjls-0.5.3.tar", last modified: Wed Apr 19 20:43:22 2023, max compression
```

## Comparing `pyjls-0.5.2.tar` & `pyjls-0.5.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.705110 pyjls-0.5.2/
--rw-rw-rw-   0        0        0     3807 2023-03-30 20:06:01.000000 pyjls-0.5.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.5.2/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14665 2023-03-30 20:13:48.704610 pyjls-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.575593 pyjls-0.5.2/include/
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.618599 pyjls-0.5.2/include/jls/
--rw-rw-rw-   0        0        0     2721 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/backend.h
--rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/cmacro.h
--rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/crc32c.h
--rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/ec.h
--rw-rw-rw-   0        0        0    24367 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/format.h
--rw-rw-rw-   0        0        0    11557 2023-03-29 21:42:56.000000 pyjls-0.5.2/include/jls/log.h
--rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/raw.h
--rw-rw-rw-   0        0        0     9052 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/reader.h
--rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/statistics.h
--rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/threaded_writer.h
--rw-rw-rw-   0        0        0    12408 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/time.h
--rw-rw-rw-   0        0        0     2752 2023-03-29 21:44:42.000000 pyjls-0.5.2/include/jls/version.h
--rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls/writer.h
--rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.5.2/include/jls.h
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.564090 pyjls-0.5.2/include_prv/
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.644099 pyjls-0.5.2/include_prv/jls/
--rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.5.2/include_prv/jls/bit_shift.h
--rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/cdef.h
--rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.5.2/include_prv/jls/datatype.h
--rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/msg_ring_buffer.h
--rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/util.h
--rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/wr_fsr.h
--rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/wr_prv.h
--rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.5.2/include_prv/jls/wr_ts.h
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.649599 pyjls-0.5.2/pyjls/
--rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.5.2/pyjls/__init__.py
--rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/__main__.py
--rw-rw-rw-   0        0        0  1569957 2023-03-29 21:46:52.000000 pyjls-0.5.2/pyjls/binding.c
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.658600 pyjls-0.5.2/pyjls/entry_points/
--rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/entry_points/annotate.py
--rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/entry_points/info.py
--rw-rw-rw-   0        0        0     2128 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/structs.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.659601 pyjls-0.5.2/pyjls/test/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/test/__init__.py
--rw-rw-rw-   0        0        0     9517 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/test/test_binding.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.659601 pyjls-0.5.2/pyjls/v1/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.2/pyjls/v1/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-03-29 21:44:42.000000 pyjls-0.5.2/pyjls/version.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.657100 pyjls-0.5.2/pyjls.egg-info/
--rw-rw-rw-   0        0        0    14665 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1272 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-30 20:13:48.000000 pyjls-0.5.2/pyjls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 20:13:48.705110 pyjls-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     6931 2023-03-09 18:55:17.000000 pyjls-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:13:48.704110 pyjls-0.5.2/src/
--rw-rw-rw-   0        0        0     8676 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/backend_posix.c
--rw-rw-rw-   0        0        0     9038 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/backend_win.c
--rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.5.2/src/bit_shift.c
--rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/crc32c_arm_neon.c
--rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/crc32c_intel_sse4.c
--rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/crc32c_sw.c
--rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.5.2/src/datatype.c
--rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/ec.c
--rw-rw-rw-   0        0        0     1627 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/log.c
--rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.5.2/src/msg_ring_buffer.c
--rw-rw-rw-   0        0        0    17303 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/raw.c
--rw-rw-rw-   0        0        0    50573 2023-03-04 19:36:06.000000 pyjls-0.5.2/src/reader.c
--rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/statistics.c
--rw-rw-rw-   0        0        0    11268 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/threaded_writer.c
--rw-rw-rw-   0        0        0    22020 2023-03-16 12:30:55.000000 pyjls-0.5.2/src/wr_fsr.c
--rw-rw-rw-   0        0        0     9691 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/wr_ts.c
--rw-rw-rw-   0        0        0    30342 2022-03-05 19:14:45.000000 pyjls-0.5.2/src/writer.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.495623 pyjls-0.5.3/
+-rw-rw-rw-   0        0        0     3885 2023-04-19 20:33:20.000000 pyjls-0.5.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.5.3/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    14665 2023-04-19 20:43:22.495623 pyjls-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.455550 pyjls-0.5.3/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.461069 pyjls-0.5.3/include/jls/
+-rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.5.3/include/jls/backend.h
+-rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/cmacro.h
+-rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/crc32c.h
+-rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/ec.h
+-rw-rw-rw-   0        0        0    24367 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/format.h
+-rw-rw-rw-   0        0        0    11561 2023-04-19 17:02:21.000000 pyjls-0.5.3/include/jls/log.h
+-rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/raw.h
+-rw-rw-rw-   0        0        0     9052 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/reader.h
+-rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/statistics.h
+-rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/threaded_writer.h
+-rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.5.3/include/jls/time.h
+-rw-rw-rw-   0        0        0     2760 2023-04-19 20:32:45.000000 pyjls-0.5.3/include/jls/version.h
+-rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/writer.h
+-rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.452041 pyjls-0.5.3/include_prv/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.464573 pyjls-0.5.3/include_prv/jls/
+-rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.5.3/include_prv/jls/bit_shift.h
+-rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/cdef.h
+-rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.5.3/include_prv/jls/datatype.h
+-rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/msg_ring_buffer.h
+-rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/util.h
+-rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_fsr.h
+-rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_prv.h
+-rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_ts.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.467578 pyjls-0.5.3/pyjls/
+-rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.5.3/pyjls/__init__.py
+-rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/__main__.py
+-rw-rw-rw-   0        0        0  1571611 2023-04-19 20:27:59.000000 pyjls-0.5.3/pyjls/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.487104 pyjls-0.5.3/pyjls/entry_points/
+-rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/annotate.py
+-rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/info.py
+-rw-rw-rw-   0        0        0     2128 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.488104 pyjls-0.5.3/pyjls/test/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/test/__init__.py
+-rw-rw-rw-   0        0        0     9517 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/test/test_binding.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.488104 pyjls-0.5.3/pyjls/v1/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/v1/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-04-19 17:03:22.000000 pyjls-0.5.3/pyjls/version.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.485599 pyjls-0.5.3/pyjls.egg-info/
+-rw-rw-rw-   0        0        0    14665 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:43:22.496625 pyjls-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     6931 2023-03-09 18:55:17.000000 pyjls-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.495623 pyjls-0.5.3/src/
+-rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.5.3/src/backend_posix.c
+-rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.5.3/src/backend_win.c
+-rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/bit_shift.c
+-rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_arm_neon.c
+-rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_intel_sse4.c
+-rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_sw.c
+-rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/datatype.c
+-rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/ec.c
+-rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.5.3/src/log.c
+-rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/msg_ring_buffer.c
+-rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.5.3/src/raw.c
+-rw-rw-rw-   0        0        0    50573 2023-03-04 19:36:06.000000 pyjls-0.5.3/src/reader.c
+-rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/statistics.c
+-rw-rw-rw-   0        0        0    11268 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/threaded_writer.c
+-rw-rw-rw-   0        0        0    22020 2023-03-16 12:30:55.000000 pyjls-0.5.3/src/wr_fsr.c
+-rw-rw-rw-   0        0        0     9691 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/wr_ts.c
+-rw-rw-rw-   0        0        0    30342 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/writer.c
```

### Comparing `pyjls-0.5.2/CHANGELOG.md` & `pyjls-0.5.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.5.3
+
+2023 Apr 19
+
+* Fixed build warnings for fn() declarations.
+
+
 ## 0.5.2
 
 2023 Mar 30
 
 * Reduced default log level to WARNING.
```

### Comparing `pyjls-0.5.2/CREDITS.html` & `pyjls-0.5.3/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/LICENSE` & `pyjls-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/PKG-INFO` & `pyjls-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.5.2
+Version: 0.5.3
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.5.2/README.md` & `pyjls-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/backend.h` & `pyjls-0.5.3/include/jls/backend.h`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 int jls_bkt_process_lock(struct jls_bkt_s * self);      // 0 on success or error code
 int jls_bkt_process_unlock(struct jls_bkt_s * self);    // 0 on success or error code
 void jls_bkt_msg_wait(struct jls_bkt_s * self);
 void jls_bkt_msg_signal(struct jls_bkt_s * self);
 void jls_bkt_sleep_ms(uint32_t duration_ms);
 
 
-int64_t jls_now();
-struct jls_time_counter_s jls_time_counter();
+int64_t jls_now(void);
+struct jls_time_counter_s jls_time_counter(void);
 
 /** @} */
 
 JLS_CPP_GUARD_END
 
 #endif  /* JLS_PRIV_RAW_BACKEND_H__ */
```

### Comparing `pyjls-0.5.2/include/jls/cmacro.h` & `pyjls-0.5.3/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/crc32c.h` & `pyjls-0.5.3/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/ec.h` & `pyjls-0.5.3/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/format.h` & `pyjls-0.5.3/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/log.h` & `pyjls-0.5.3/include/jls/log.h`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 JLS_API void jls_log_register(jls_log_cbk handler);
 
 /**
  * @brief Finalize the logging feature.
  *
  * This is equivalent to calling jls_log_initialize(0).
  */
-JLS_API void jls_log_unregister();
+JLS_API void jls_log_unregister(void);
 
 /**
  * @def JLS_LOG_PRINTF
  * @brief The printf function including log formatting.
  *
  * @param level The level for this log message
  * @param format The formatting string
```

### Comparing `pyjls-0.5.2/include/jls/raw.h` & `pyjls-0.5.3/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/reader.h` & `pyjls-0.5.3/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/statistics.h` & `pyjls-0.5.3/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/threaded_writer.h` & `pyjls-0.5.3/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls/time.h` & `pyjls-0.5.3/include/jls/time.h`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
  *
  *      python
  *      import datetime
  *      import dateutil.parser
  *      epoch = dateutil.parser.parse('2018-01-01T00:00:00Z').timestamp()
  *      datetime.datetime.fromtimestamp((my_time >> 30) + epoch)
  */
-JLS_API int64_t jls_now();
+JLS_API int64_t jls_now(void);
 
 /**
  * @brief The platform counter structure.
  */
 struct jls_time_counter_s {
     /// The counter value.
     uint64_t value;
@@ -373,25 +373,25 @@
  * The counter must be monotonic.  If the underlying hardware is less
  * than the full 64 bits, then the platform must unwrap and extend
  * the hardware value to 64-bit.
  *
  * The JLS authors recommend this counter starts at 0 when the
  * system powers up.
  */
-JLS_API struct jls_time_counter_s jls_time_counter();
+JLS_API struct jls_time_counter_s jls_time_counter(void);
 
 /**
  * @brief Get the monotonic platform time as a 34Q30 fixed point number.
  *
  * @return The monotonic platform time based upon the jls_time_counter().
  *      The platform time has no guaranteed relationship with
  *      UTC or wall-clock calendar time.  This time has both
  *      offset and scale errors relative to UTC.
  */
-static inline int64_t jls_time_rel() {
+static inline int64_t jls_time_rel(void) {
     struct jls_time_counter_s counter = jls_time_counter();
     return JLS_COUNTER_TO_TIME(counter.value, counter.frequency);
 }
 
 JLS_CPP_GUARD_END
 
 /** @} */
```

### Comparing `pyjls-0.5.2/include/jls/version.h` & `pyjls-0.5.3/include/jls/version.h`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
 #define JLS_VERSION_MINOR 5
-#define JLS_VERSION_PATCH 2
+#define JLS_VERSION_PATCH 3
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
@@ -81,21 +81,21 @@
 #define JLS_VERSION_STR JLS_VERSION_ENCODE_STR(JLS_VERSION_MAJOR, JLS_VERSION_MINOR, JLS_VERSION_PATCH)
 
 /**
  * @brief Get the JLS version string.
  * 
  * @return The JLS version string.
  */
-JLS_API const char * jls_version_str();
+JLS_API const char * jls_version_str(void);
 
 /**
  * @brief Get the JLS version u32.
  * 
  * @return The JLS version u32 value.
  */
-JLS_API uint32_t jls_version_u32();
+JLS_API uint32_t jls_version_u32(void);
 
 JLS_CPP_GUARD_END
 
 /** @} */
 
 #endif /* JLS_VERSION_H_ */
```

### Comparing `pyjls-0.5.2/include/jls/writer.h` & `pyjls-0.5.3/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include/jls.h` & `pyjls-0.5.3/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/bit_shift.h` & `pyjls-0.5.3/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/cdef.h` & `pyjls-0.5.3/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/datatype.h` & `pyjls-0.5.3/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.5.3/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/util.h` & `pyjls-0.5.3/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/wr_fsr.h` & `pyjls-0.5.3/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/wr_prv.h` & `pyjls-0.5.3/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/include_prv/jls/wr_ts.h` & `pyjls-0.5.3/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/__init__.py` & `pyjls-0.5.3/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/__main__.py` & `pyjls-0.5.3/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/binding.c` & `pyjls-0.5.3/pyjls/binding.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
             "include",
             "include_prv",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "pyjls.binding",
         "sources": [
             "pyjls/binding.pyx",
             "src/bit_shift.c",
             "src/datatype.c",
             "src/ec.c",
@@ -43,16 +43,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -237,15 +237,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -276,15 +276,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1138,195 +1138,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1360,42 +1360,42 @@
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback;
 struct __pyx_obj_5pyjls_7binding_Reader;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2176,20 +2176,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
@@ -13535,15 +13543,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13552,29 +13560,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13585,15 +13593,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13602,29 +13610,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13635,15 +13643,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13652,29 +13660,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13685,15 +13693,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13702,29 +13710,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13735,15 +13743,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13752,29 +13760,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13785,212 +13793,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":928
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":932
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":940
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14006,15 +14014,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -14022,53 +14030,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -14076,30 +14084,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14114,15 +14122,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":946
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14138,15 +14146,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14154,53 +14162,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -14208,30 +14216,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14246,15 +14254,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":952
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14270,15 +14278,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14286,53 +14294,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -14340,30 +14348,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14378,176 +14386,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":966
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":981
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":996
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -29141,26 +29149,26 @@
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
   __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_3248624, __pyx_int_200305830, __pyx_int_134405936); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -29731,52 +29739,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -33885,28 +33908,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -35207,44 +35230,62 @@
     return -1;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `pyjls-0.5.2/pyjls/entry_points/__init__.py` & `pyjls-0.5.3/pyjls/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/entry_points/annotate.py` & `pyjls-0.5.3/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/entry_points/info.py` & `pyjls-0.5.3/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/structs.py` & `pyjls-0.5.3/pyjls/structs.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/test/__init__.py` & `pyjls-0.5.3/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/test/test_binding.py` & `pyjls-0.5.3/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/v1/__init__.py` & `pyjls-0.5.3/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyjls/version.py` & `pyjls-0.5.3/pyjls/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 __title__ = "pyjls"
 __description__ = 'Joulescope™ file format'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjls-0.5.2/pyjls.egg-info/PKG-INFO` & `pyjls-0.5.3/pyjls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.5.2
+Version: 0.5.3
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.5.2/pyjls.egg-info/SOURCES.txt` & `pyjls-0.5.3/pyjls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/pyproject.toml` & `pyjls-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/setup.py` & `pyjls-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/backend_posix.c` & `pyjls-0.5.3/src/backend_posix.c`

 * *Files 1% similar despite different names*

```diff
@@ -277,26 +277,26 @@
     ts.tv_sec = duration_ms / 1000;
     ts.tv_nsec = ((long) (duration_ms % 1000)) * 1000000;
     do {
         rv = nanosleep(&ts, &ts);
     } while (rv && errno == EINTR);
 }
 
-int64_t jls_now() {
+int64_t jls_now(void) {
     int64_t t;
     struct timespec ts;
     if (clock_gettime(CLOCK_REALTIME, &ts)) {
         JLS_LOGE("clock_gettime error");
     }
     t = ((int64_t) ts.tv_sec + JLS_TIME_EPOCH_UNIX_OFFSET_SECONDS) * JLS_TIME_SECOND;
     t += JLS_COUNTER_TO_TIME(ts.tv_nsec, 1000000000LL);
     return t;
 }
 
-struct jls_time_counter_s jls_time_counter() {
+struct jls_time_counter_s jls_time_counter(void) {
     struct jls_time_counter_s counter;
     struct timespec ts;
     if (clock_gettime(CLOCK_MONOTONIC, &ts)) {
         JLS_LOGE("clock_gettime error");
     }
     counter.value = ((int64_t) ts.tv_sec + JLS_TIME_EPOCH_UNIX_OFFSET_SECONDS) * JLS_TIME_SECOND;
     counter.value += JLS_COUNTER_TO_TIME(ts.tv_nsec, 1000000000LL);
```

### Comparing `pyjls-0.5.2/src/backend_win.c` & `pyjls-0.5.3/src/backend_win.c`

 * *Files 2% similar despite different names*

```diff
@@ -254,29 +254,29 @@
 }
 
 void jls_bkt_sleep_ms(uint32_t duration_ms) {
     Sleep(duration_ms);
 }
 
 
-int64_t jls_now() {
+int64_t jls_now(void) {
     // Contains a 64-bit value representing the number of 100-nanosecond intervals since January 1, 1601 (UTC).
     // python
     // import dateutil.parser
     // dateutil.parser.parse('2018-01-01T00:00:00Z').timestamp() - dateutil.parser.parse('1601-01-01T00:00:00Z').timestamp()
     static const int64_t offset_s = 131592384000000000LL;  // 100 ns
     static const uint64_t frequency = 10000000; // 100 ns
     FILETIME filetime;
     GetSystemTimePreciseAsFileTime(&filetime);
     uint64_t t = ((uint64_t) filetime.dwLowDateTime) | (((uint64_t) filetime.dwHighDateTime) << 32);
     t -= offset_s;
     return JLS_COUNTER_TO_TIME(t, frequency);
 }
 
-struct jls_time_counter_s jls_time_counter() {
+struct jls_time_counter_s jls_time_counter(void) {
     struct jls_time_counter_s counter;
     static int first = 1;
     static uint64_t offset = 0;     // in 34Q30 time
     static LARGE_INTEGER perf_frequency = {.QuadPart = 0};
 
     // https://docs.microsoft.com/en-us/windows/win32/sysinfo/acquiring-high-resolution-time-stamps
     LARGE_INTEGER perf_counter;
```

### Comparing `pyjls-0.5.2/src/bit_shift.c` & `pyjls-0.5.3/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/crc32c_arm_neon.c` & `pyjls-0.5.3/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/crc32c_intel_sse4.c` & `pyjls-0.5.3/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/crc32c_sw.c` & `pyjls-0.5.3/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/datatype.c` & `pyjls-0.5.3/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/ec.c` & `pyjls-0.5.3/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/log.c` & `pyjls-0.5.3/src/log.c`

 * *Files 7% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     if (NULL == handler) {
         cbk_ = cbk_default;
     } else {
         cbk_ = handler;
     }
 }
 
-JLS_API void jls_log_unregister() {
+JLS_API void jls_log_unregister(void) {
     jls_log_register(NULL);
 }
```

### Comparing `pyjls-0.5.2/src/msg_ring_buffer.c` & `pyjls-0.5.3/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/raw.c` & `pyjls-0.5.3/src/raw.c`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,14 @@
         case JLS_TAG_TRACK_UTC_SUMMARY:         return "track_utc_summary";
         case JLS_TAG_USER_DATA:                 return "user_data";
         case JLS_TAG_END:                       return "end";
         default:                                return "unknown";
     }
 }
 
-const char * jls_version_str() {
+const char * jls_version_str(void) {
     return JLS_VERSION_STR;
 }
 
-uint32_t jls_version_u32() {
+uint32_t jls_version_u32(void) {
     return JLS_VERSION_U32;
 }
```

### Comparing `pyjls-0.5.2/src/reader.c` & `pyjls-0.5.3/src/reader.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/statistics.c` & `pyjls-0.5.3/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/threaded_writer.c` & `pyjls-0.5.3/src/threaded_writer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/wr_fsr.c` & `pyjls-0.5.3/src/wr_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/wr_ts.c` & `pyjls-0.5.3/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.2/src/writer.c` & `pyjls-0.5.3/src/writer.c`

 * *Files identical despite different names*

