# Comparing `tmp/llnl-hatchet-2022.2.0.tar.gz` & `tmp/llnl-hatchet-2022.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llnl-hatchet-2022.2.0.tar", last modified: Thu Aug 18 03:46:40 2022, max compression
+gzip compressed data, was "dist/llnl-hatchet-2022.2.2.tar", last modified: Wed Apr 19 21:25:06 2023, max compression
```

## Comparing `llnl-hatchet-2022.2.0.tar` & `llnl-hatchet-2022.2.2.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.509933 llnl-hatchet-2022.2.0/
--rw-r--r--   0 root         (0) root         (0)     1092 2022-08-16 22:41:38.000000 llnl-hatchet-2022.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1167 2022-08-16 22:41:38.000000 llnl-hatchet-2022.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)      389 2022-08-18 03:46:40.509933 llnl-hatchet-2022.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4370 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.399933 llnl-hatchet-2022.2.0/hatchet/
--rw-r--r--   0 root         (0) root         (0)      312 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.439933 llnl-hatchet-2022.2.0/hatchet/cython_modules/
--rw-r--r--   0 root         (0) root         (0)   800770 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/cython_modules/graphframe_modules.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.469933 llnl-hatchet-2022.2.0/hatchet/cython_modules/libs/
--rw-r--r--   0 root         (0) root         (0)      181 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/cython_modules/libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)   763943 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/cython_modules/reader_modules.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.479933 llnl-hatchet-2022.2.0/hatchet/external/
--rw-r--r--   0 root         (0) root         (0)      285 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13163 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/external/console.py
--rw-r--r--   0 root         (0) root         (0)     2831 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/frame.py
--rw-r--r--   0 root         (0) root         (0)    14363 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/graph.py
--rw-r--r--   0 root         (0) root         (0)    60037 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/hatchet/graphframe.py
--rw-r--r--   0 root         (0) root         (0)     7033 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/node.py
--rw-r--r--   0 root         (0) root         (0)    61218 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/hatchet/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.489933 llnl-hatchet-2022.2.0/hatchet/readers/
--rw-r--r--   0 root         (0) root         (0)      181 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16234 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/hatchet/readers/caliper_native_reader.py
--rw-r--r--   0 root         (0) root         (0)    16534 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/caliper_reader.py
--rw-r--r--   0 root         (0) root         (0)     4515 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/cprofile_reader.py
--rw-r--r--   0 root         (0) root         (0)     3061 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/dataframe_reader.py
--rw-r--r--   0 root         (0) root         (0)     4154 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/gprof_dot_reader.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/hdf5_reader.py
--rw-r--r--   0 root         (0) root         (0)    16325 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/hpctoolkit_reader.py
--rw-r--r--   0 root         (0) root         (0)     5744 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/literal_reader.py
--rw-r--r--   0 root         (0) root         (0)     3565 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/pyinstrument_reader.py
--rw-r--r--   0 root         (0) root         (0)     5976 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/spotdb_reader.py
--rw-r--r--   0 root         (0) root         (0)    23415 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/tau_reader.py
--rw-r--r--   0 root         (0) root         (0)    25694 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/readers/timemory_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.499933 llnl-hatchet-2022.2.0/hatchet/tests/
--rw-r--r--   0 root         (0) root         (0)     9934 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/caliper.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/callgrind.py
--rw-r--r--   0 root         (0) root         (0)    42862 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2036 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/cprofile.py
--rw-r--r--   0 root         (0) root         (0)     7619 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/dataframe_ops.py
--rw-r--r--   0 root         (0) root         (0)      920 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/executable.py
--rw-r--r--   0 root         (0) root         (0)     2353 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/frame.py
--rw-r--r--   0 root         (0) root         (0)     2455 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/graph.py
--rw-r--r--   0 root         (0) root         (0)     4632 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/graph_literal.py
--rw-r--r--   0 root         (0) root         (0)     1211 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/graph_ops.py
--rw-r--r--   0 root         (0) root         (0)    40128 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/hatchet/tests/graphframe.py
--rw-r--r--   0 root         (0) root         (0)     7491 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/hpctoolkit.py
--rw-r--r--   0 root         (0) root         (0)     3362 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/node.py
--rw-r--r--   0 root         (0) root         (0)     2454 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/profiler.py
--rw-r--r--   0 root         (0) root         (0)     4178 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/pyinstrument.py
--rw-r--r--   0 root         (0) root         (0)    44885 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/hatchet/tests/query.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/spotdb_test.py
--rw-r--r--   0 root         (0) root         (0)     2932 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/tau.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/timemory_func.py
--rw-r--r--   0 root         (0) root         (0)     3087 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/tests/timemory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.499933 llnl-hatchet-2022.2.0/hatchet/util/
--rw-r--r--   0 root         (0) root         (0)      181 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4097 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/colormaps.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/config.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/deprecated.py
--rw-r--r--   0 root         (0) root         (0)     3512 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/dot.py
--rw-r--r--   0 root         (0) root         (0)      639 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/executable.py
--rw-r--r--   0 root         (0) root         (0)     3274 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/profiler.py
--rw-r--r--   0 root         (0) root         (0)     1522 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/util/timer.py
--rw-r--r--   0 root         (0) root         (0)      261 2022-08-18 03:37:17.000000 llnl-hatchet-2022.2.0/hatchet/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.499933 llnl-hatchet-2022.2.0/hatchet/writers/
--rw-r--r--   0 root         (0) root         (0)      181 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/writers/dataframe_writer.py
--rw-r--r--   0 root         (0) root         (0)      844 2022-08-16 22:41:39.000000 llnl-hatchet-2022.2.0/hatchet/writers/hdf5_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 03:46:40.509933 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      389 2022-08-18 03:46:40.000000 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1811 2022-08-18 03:46:40.000000 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-18 03:46:40.000000 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2022-08-18 03:46:40.000000 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-18 03:46:40.000000 llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      534 2022-08-18 03:37:17.000000 llnl-hatchet-2022.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-18 03:46:40.509933 llnl-hatchet-2022.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1880 2022-08-17 03:54:00.000000 llnl-hatchet-2022.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/
+-rw-r--r--   0 root         (0) root         (0)      261 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/version.py
+-rw-r--r--   0 root         (0) root         (0)    68856 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/writers/
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/dataframe_writer.py
+-rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      844 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/hdf5_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/util/
+-rw-r--r--   0 root         (0) root         (0)      256 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/timer.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/deprecated.py
+-rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/colormaps.py
+-rw-r--r--   0 root         (0) root         (0)      639 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/executable.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/dot.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/profiler.py
+-rw-r--r--   0 root         (0) root         (0)    14363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/tests/
+-rw-r--r--   0 root         (0) root         (0)    43179 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7619 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/dataframe_ops.py
+-rw-r--r--   0 root         (0) root         (0)    10497 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/caliper.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/timemory_func.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/cprofile.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/spotdb_test.py
+-rw-r--r--   0 root         (0) root         (0)    45936 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/query.py
+-rw-r--r--   0 root         (0) root         (0)     7547 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/hpctoolkit.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/pyinstrument.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph_literal.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/callgrind.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/timemory_test.py
+-rw-r--r--   0 root         (0) root         (0)      920 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/executable.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/frame.py
+-rw-r--r--   0 root         (0) root         (0)    40391 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graphframe.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph_ops.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/tau.py
+-rw-r--r--   0 root         (0) root         (0)      839 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/json_test.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/node.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/profiler.py
+-rw-r--r--   0 root         (0) root         (0)      345 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/libs/
+-rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   800770 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/graphframe_modules.c
+-rw-r--r--   0 root         (0) root         (0)   763943 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/reader_modules.c
+-rw-r--r--   0 root         (0) root         (0)     2831 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/frame.py
+-rw-r--r--   0 root         (0) root         (0)    61311 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/graphframe.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/readers/
+-rw-r--r--   0 root         (0) root         (0)     4154 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/gprof_dot_reader.py
+-rw-r--r--   0 root         (0) root         (0)    16534 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/caliper_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/pyinstrument_reader.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/hdf5_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/dataframe_reader.py
+-rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/literal_reader.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/cprofile_reader.py
+-rw-r--r--   0 root         (0) root         (0)    25694 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/timemory_reader.py
+-rw-r--r--   0 root         (0) root         (0)    23415 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/tau_reader.py
+-rw-r--r--   0 root         (0) root         (0)    16325 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/hpctoolkit_reader.py
+-rw-r--r--   0 root         (0) root         (0)    18371 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/caliper_native_reader.py
+-rw-r--r--   0 root         (0) root         (0)     5976 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/spotdb_reader.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/json_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/external/
+-rw-r--r--   0 root         (0) root         (0)    13290 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/external/console.py
+-rw-r--r--   0 root         (0) root         (0)      285 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/external/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1092 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      534 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1167 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4370 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1880 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `llnl-hatchet-2022.2.0/LICENSE` & `llnl-hatchet-2022.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/NOTICE` & `llnl-hatchet-2022.2.2/NOTICE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/README.md` & `llnl-hatchet-2022.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/cython_modules/graphframe_modules.c` & `llnl-hatchet-2022.2.2/hatchet/cython_modules/graphframe_modules.c`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/cython_modules/reader_modules.c` & `llnl-hatchet-2022.2.2/hatchet/cython_modules/reader_modules.c`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/external/console.py` & `llnl-hatchet-2022.2.2/hatchet/external/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,20 @@
 class ConsoleRenderer:
     def __init__(self, unicode=False, color=False):
         self.unicode = unicode
         self.color = color
         self.visited = []
 
     def render(self, roots, dataframe, **kwargs):
-        result = self.render_preamble()
+        self.render_header = kwargs["render_header"]
+
+        if self.render_header:
+            result = self.render_preamble()
+        else:
+            result = ""
 
         if roots is None:
             result += "The graph is empty.\n\n"
             return result
 
         self.metric_columns = kwargs["metric_column"]
         self.precision = kwargs["precision"]
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/frame.py` & `llnl-hatchet-2022.2.2/hatchet/frame.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/graph.py` & `llnl-hatchet-2022.2.2/hatchet/graph.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/graphframe.py` & `llnl-hatchet-2022.2.2/hatchet/graphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import traceback
 
 from collections import defaultdict
 
 import pandas as pd
 import numpy as np
 import multiprocess as mp
+import json
 
 from .node import Node
 from .graph import Graph
 from .frame import Frame
 from .query import AbstractQuery, QueryMatcher, parse_cypher_query
 from .external.console import ConsoleRenderer
 from .util.dot import trees_to_dot
@@ -297,14 +298,20 @@
         df.sort_index(inplace=True)
 
         gf = GraphFrame(graph, df, ["time"], [])
         gf.update_inclusive_columns()
         return gf
 
     @staticmethod
+    def from_json(json_spec, **kwargs):
+        from .readers.json_reader import JsonReader
+
+        return JsonReader(json_spec).read(**kwargs)
+
+    @staticmethod
     def from_hdf(filename, **kwargs):
         # import this lazily to avoid circular dependencies
         from .readers.hdf5_reader import HDF5Reader
 
         return HDF5Reader(filename).read(**kwargs)
 
     def to_hdf(self, filename, key="hatchet_graphframe", **kwargs):
@@ -886,14 +893,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     ):
         """Format this graphframe as a tree and return the resulting string."""
         color = sys.stdout.isatty()
         shell = None
         if metric_column is None:
             metric_column = self.default_metric
 
@@ -923,14 +931,15 @@
             context_column=context_column,
             rank=rank,
             thread=thread,
             depth=depth,
             highlight_name=highlight_name,
             colormap=colormap,
             invert_colormap=invert_colormap,
+            render_header=render_header,
         )
 
     def to_dot(self, metric=None, name="name", rank=0, thread=0, threshold=0.0):
         """Write the graph in the graphviz dot format:
         https://www.graphviz.org/doc/info/lang.html
         """
         if metric is None:
@@ -1080,14 +1089,45 @@
             return node_dict
 
         for root in sorted(self.graph.roots, key=lambda n: n.frame):
             graph_literal.append(add_nodes(root))
 
         return graph_literal
 
+    def to_dict(self):
+        hatchet_dict = {}
+
+        """
+        Nodes: {hatchet_nid: {node data, children:[by-id]}}
+        """
+        graphs = []
+        for root in self.graph.roots:
+            formatted_graph_dict = {}
+            for n in root.traverse():
+                formatted_graph_dict[n._hatchet_nid] = {
+                    "data": n.frame.attrs,
+                    "children": [c._hatchet_nid for c in n.children],
+                }
+            graphs.append(formatted_graph_dict)
+
+        hatchet_dict["graph"] = graphs
+
+        hatchet_dict["dataframe_indices"] = list(self.dataframe.index.names)
+        ef = self.dataframe.reset_index()
+        ef["node"] = ef["node"].apply(lambda n: n._hatchet_nid)
+        hatchet_dict["dataframe"] = ef.replace({np.nan: None}).to_dict("records")
+
+        hatchet_dict["inclusive_metrics"] = self.inc_metrics
+        hatchet_dict["exclusive_metrics"] = self.exc_metrics
+
+        return hatchet_dict
+
+    def to_json(self):
+        return json.dumps(self.to_dict())
+
     def _operator(self, other, op):
         """Generic function to apply operator to two dataframes and store
         result in self.
 
         Arguments:
             self (graphframe): self's graphframe
             other (graphframe): other's graphframe
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/node.py` & `llnl-hatchet-2022.2.2/hatchet/node.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/query.py` & `llnl-hatchet-2022.2.2/hatchet/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     ABC = ABCMeta("ABC", (object,), {"__slots__": ()})
 
 from itertools import groupby
 from numbers import Real
 import re
 import sys
+import warnings
 import pandas as pd
 from pandas import DataFrame
 from pandas.core.indexes.multi import MultiIndex
 from textx import metamodel_from_str
 from textx.exceptions import TextXError
 
 # Flake8 to ignore this import, it does not recognize that eval("np.nan") needs
@@ -174,14 +175,17 @@
                         if key == "depth":
                             node = df_row.name
                             if isinstance(
                                 single_value, str
                             ) and single_value.lower().startswith(compops):
                                 return eval("{} {}".format(node._depth, single_value))
                             if isinstance(single_value, Real):
+                                # If the value for "depth" is -1, check if the node is a leaf
+                                if single_value == -1:
+                                    return len(node.children) == 0
                                 return node._depth == single_value
                             raise InvalidQueryFilter(
                                 "Attribute {} has a numeric type. Valid filters for this attribute are a string starting with a comparison operator or a real number.".format(
                                     key
                                 )
                             )
                         if key == "node_id":
@@ -671,17 +675,19 @@
 ConditionExpr: conditions+=CompoundCond;
 CompoundCond: UnaryCond | BinaryCond;
 BinaryCond: AndCond | OrCond;
 AndCond: 'AND' subcond=UnaryCond;
 OrCond: 'OR' subcond=UnaryCond;
 UnaryCond: NotCond | SingleCond;
 NotCond: 'NOT' subcond=SingleCond;
-SingleCond: StringCond | NumberCond | NoneCond | NotNoneCond;
+SingleCond: StringCond | NumberCond | NoneCond | NotNoneCond | LeafCond | NotLeafCond;
 NoneCond: name=ID '.' prop=STRING 'IS NONE';
 NotNoneCond: name=ID '.' prop=STRING 'IS NOT NONE';
+LeafCond: name=ID 'IS LEAF';
+NotLeafCond: name=ID 'IS NOT LEAF';
 StringCond: StringEq | StringStartsWith | StringEndsWith | StringContains | StringMatch;
 StringEq: name=ID '.' prop=STRING '=' val=STRING;
 StringStartsWith: name=ID '.' prop=STRING 'STARTS WITH' val=STRING;
 StringEndsWith: name=ID '.' prop=STRING 'ENDS WITH' val=STRING;
 StringContains: name=ID '.' prop=STRING 'CONTAINS' val=STRING;
 StringMatch: name=ID '.' prop=STRING '=~' val=STRING;
 NumberCond: NumEq | NumLt | NumGt | NumLte | NumGte | NumNan | NumNotNan | NumInf | NumNotInf;
@@ -810,15 +816,15 @@
                     self.filters[i][0][0] = None
 
     def _is_unary_cond(self, obj):
         if (
             cname(obj) == "NotCond"
             or self._is_str_cond(obj)
             or self._is_num_cond(obj)
-            or cname(obj) in ["NoneCond", "NotNoneCond"]
+            or cname(obj) in ["NoneCond", "NotNoneCond", "LeafCond", "NotLeafCond"]
         ):
             return True
         return False
 
     def _is_binary_cond(self, obj):
         if cname(obj) in ["AndCond", "OrCond"]:
             return True
@@ -856,14 +862,18 @@
             return self._parse_str(obj)
         if self._is_num_cond(obj):
             return self._parse_num(obj)
         if cname(obj) == "NoneCond":
             return self._parse_none(obj)
         if cname(obj) == "NotNoneCond":
             return self._parse_not_none(obj)
+        if cname(obj) == "LeafCond":
+            return self._parse_leaf(obj)
+        if cname(obj) == "NotLeafCond":
+            return self._parse_not_leaf(obj)
         raise RuntimeError("Bad Single Condition")
 
     def _parse_none(self, obj):
         if obj.prop == "depth":
             return [
                 None,
                 obj.name,
@@ -902,14 +912,30 @@
         return [
             None,
             obj.name,
             'df_row["{}"] is not None'.format(obj.prop),
             None,
         ]
 
+    def _parse_leaf(self, obj):
+        return [
+            None,
+            obj.name,
+            "len(df_row.name.children) == 0",
+            None,
+        ]
+
+    def _parse_not_leaf(self, obj):
+        return [
+            None,
+            obj.name,
+            "len(df_row.name.children) > 0",
+            None,
+        ]
+
     def _is_str_cond(self, obj):
         if cname(obj) in [
             "StringEq",
             "StringStartsWith",
             "StringEndsWith",
             "StringContains",
             "StringMatch",
@@ -1004,21 +1030,64 @@
             return self._parse_num_inf(obj)
         if cname(obj) == "NumNotInf":
             return self._parse_num_not_inf(obj)
         raise RuntimeError("Bad Number Op Class")
 
     def _parse_num_eq(self, obj):
         if obj.prop == "depth":
+            if obj.val == -1:
+                return [
+                    None,
+                    obj.name,
+                    "len(df_row.name.children) == 0",
+                    None,
+                ]
+            elif obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'depth' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._depth, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._depth == {}".format(obj.val),
                 "isinstance(df_row.name._depth, Real)",
             ]
         if obj.prop == "node_id":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'node_id' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._hatchet_nid, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._hatchet_nid == {}".format(obj.val),
                 "isinstance(df_row.name._hatchet_nid, Real)",
             ]
         return [
@@ -1026,21 +1095,57 @@
             obj.name,
             'df_row["{}"] == {}'.format(obj.prop, obj.val),
             "isinstance(df_row['{}'], Real)".format(obj.prop),
         ]
 
     def _parse_num_lt(self, obj):
         if obj.prop == "depth":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'depth' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._depth, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._depth < {}".format(obj.val),
                 "isinstance(df_row.name._depth, Real)",
             ]
         if obj.prop == "node_id":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'node_id' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._hatchet_nid, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._hatchet_nid < {}".format(obj.val),
                 "isinstance(df_row.name._hatchet_nid, Real)",
             ]
         return [
@@ -1048,21 +1153,57 @@
             obj.name,
             'df_row["{}"] < {}'.format(obj.prop, obj.val),
             "isinstance(df_row['{}'], Real)".format(obj.prop),
         ]
 
     def _parse_num_gt(self, obj):
         if obj.prop == "depth":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'depth' property of a Node is strictly non-negative.
+                    This condition will always be true.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "True",
+                    "isinstance(df_row.name._depth, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._depth > {}".format(obj.val),
                 "isinstance(df_row.name._depth, Real)",
             ]
         if obj.prop == "node_id":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'node_id' property of a Node is strictly non-negative.
+                    This condition will always be true.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "True",
+                    "isinstance(df_row.name._hatchet_nid, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._hatchet_nid > {}".format(obj.val),
                 "isinstance(df_row.name._hatchet_nid, Real)",
             ]
         return [
@@ -1070,21 +1211,57 @@
             obj.name,
             'df_row["{}"] > {}'.format(obj.prop, obj.val),
             "isinstance(df_row['{}'], Real)".format(obj.prop),
         ]
 
     def _parse_num_lte(self, obj):
         if obj.prop == "depth":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'depth' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._depth, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._depth <= {}".format(obj.val),
                 "isinstance(df_row.name._depth, Real)",
             ]
         if obj.prop == "node_id":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'node_id' property of a Node is strictly non-negative.
+                    This condition will always be false.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "False",
+                    "isinstance(df_row.name._hatchet_nid, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._hatchet_nid <= {}".format(obj.val),
                 "isinstance(df_row.name._hatchet_nid, Real)",
             ]
         return [
@@ -1092,21 +1269,57 @@
             obj.name,
             'df_row["{}"] <= {}'.format(obj.prop, obj.val),
             "isinstance(df_row['{}'], Real)".format(obj.prop),
         ]
 
     def _parse_num_gte(self, obj):
         if obj.prop == "depth":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'depth' property of a Node is strictly non-negative.
+                    This condition will always be true.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "True",
+                    "isinstance(df_row.name._depth, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._depth >= {}".format(obj.val),
                 "isinstance(df_row.name._depth, Real)",
             ]
         if obj.prop == "node_id":
+            if obj.val < 0:
+                warnings.warn(
+                    """
+                    The 'node_id' property of a Node is strictly non-negative.
+                    This condition will always be true.
+                    The statement that triggered this warning is:
+                    {}
+                    """.format(
+                        obj
+                    ),
+                    RedundantQueryFilterWarning,
+                )
+                return [
+                    None,
+                    obj.name,
+                    "True",
+                    "isinstance(df_row.name._hatchet_nid, Real)",
+                ]
             return [
                 None,
                 obj.name,
                 "df_row.name._hatchet_nid >= {}".format(obj.val),
                 "isinstance(df_row.name._hatchet_nid, Real)",
             ]
         return [
@@ -1505,9 +1718,13 @@
     """Raised when a query does not have the correct syntax"""
 
 
 class InvalidQueryFilter(Exception):
     """Raised when a query filter does not have a valid syntax"""
 
 
+class RedundantQueryFilterWarning(Warning):
+    """Warned when a query filter does nothing or is redundant"""
+
+
 class BadNumberNaryQueryArgs(Exception):
     """Raised when a query filter does not have a valid syntax"""
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/caliper_native_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/caliper_native_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,16 @@
             if self.filename_or_caliperreader.attribute(col).is_value():
                 self.metric_cols.append(col)
 
         df_metrics = pd.DataFrame.from_dict(data=all_metrics)
         return df_metrics
 
     def create_graph(self, ctx="path"):
+        list_roots = []
+
         def _create_parent(child_node, parent_callpath):
             """We may encounter a parent node in the callpath before we see it
             as a child node. In this case, we need to create a hatchet node for
             the parent.
 
             This function recursively creates parent nodes in a callpath
             until it reaches the already existing parent in that callpath.
@@ -127,35 +129,54 @@
             if parent_node:
                 # return if arrives at the parent
                 parent_node.add_child(child_node)
                 child_node.add_parent(parent_node)
                 return
             else:
                 # else create the parent and add parent/child
-                grandparent_callpath = parent_callpath[:-1]
-                parent_name = parent_callpath[-1]
-
-                parent_node = Node(
-                    Frame({"type": "function", "name": parent_name}), None
-                )
-
-                self.callpath_to_node[parent_callpath] = parent_node
-                self.callpath_to_idx[parent_callpath] = self.global_nid
-
-                node_dict = dict(
-                    {"name": parent_name, "node": parent_node, "nid": self.global_nid},
-                )
-                self.idx_to_node[self.global_nid] = node_dict
-                self.global_nid += 1
 
-                parent_node.add_child(child_node)
-                child_node.add_parent(parent_node)
-                _create_parent(parent_node, grandparent_callpath)
+                # if root node, end recursive call to create parent nodes
+                if not parent_callpath:
+                    list_roots.append(child_node)
+
+                    node_dict = dict(
+                        {
+                            "name": child_node.frame["name"],
+                            "node": child_node,
+                            "nid": self.global_nid,
+                        }
+                    )
+
+                    self.idx_to_node[self.global_nid] = node_dict
+                    self.global_nid += 1
+                else:
+                    grandparent_callpath = parent_callpath[:-1]
+                    parent_name = parent_callpath[-1]
+
+                    parent_node = Node(
+                        Frame({"type": "function", "name": parent_name}), None
+                    )
+
+                    self.callpath_to_node[parent_callpath] = parent_node
+                    self.callpath_to_idx[parent_callpath] = self.global_nid
+
+                    node_dict = dict(
+                        {
+                            "name": parent_name,
+                            "node": parent_node,
+                            "nid": self.global_nid,
+                        },
+                    )
+                    self.idx_to_node[self.global_nid] = node_dict
+                    self.global_nid += 1
+
+                    parent_node.add_child(child_node)
+                    child_node.add_parent(parent_node)
+                    _create_parent(parent_node, grandparent_callpath)
 
-        list_roots = []
         parent_hnode = None
         records = self.filename_or_caliperreader.records
 
         for record in records:
             node_label = ""
             if ctx in record:
                 if (
@@ -237,14 +258,48 @@
                             )
 
                             self.idx_to_node[self.global_nid] = node_dict
                             self.global_nid += 1
 
         return list_roots
 
+    def _parse_metadata(self, mdata):
+        """Convert Caliper Metadata values into correct Python objects.
+
+        Args:
+            mdata (dict[str: str]): metadata to convert
+
+        Return:
+            (dict[str: str]): modified metadata
+        """
+        parsed_mdata = {}
+        for k, v in mdata.items():
+            # If the value is an int, convert it to an int.
+            try:
+                parsed_mdata[k] = int(v)
+            except ValueError:
+                # If the value is a float, convert it to a float
+                try:
+                    parsed_mdata[k] = float(v)
+                except ValueError:
+                    # If the value is a list or tuple, convert it to a list or
+                    # tuple
+                    if v.startswith("[") and v.endswith("]"):
+                        parsed_mdata[k] = [
+                            elem.strip() for elem in v.strip("][").split(",")
+                        ]
+                    elif v.startswith("(") and v.endswith(")"):
+                        parsed_mdata[k] = [
+                            elem.strip() for elem in v.strip(")(").split(",")
+                        ]
+                    # If the value is a string, just save it as-is
+                    else:
+                        parsed_mdata[k] = v
+        return parsed_mdata
+
     def read(self):
         """Read the caliper records to extract the calling context tree."""
         if isinstance(self.filename_or_caliperreader, str):
             if self.filename_ext != ".cali":
                 raise ValueError("from_caliperreader() needs a .cali file")
             else:
                 cali_file = self.filename_or_caliperreader
@@ -366,16 +421,17 @@
                 self.default_metric = "avg#inclusive#sum#time.duration"
             elif len(inc_metrics) > 0:
                 self.default_metric = inc_metrics[0]
             elif len(exc_metrics) > 0:
                 self.default_metric = exc_metrics[0]
 
         metadata = self.filename_or_caliperreader.globals
+        parsed_metadata = self._parse_metadata(metadata)
 
         return hatchet.graphframe.GraphFrame(
             graph,
             dataframe,
             exc_metrics,
             inc_metrics,
             self.default_metric,
-            metadata=metadata,
+            metadata=parsed_metadata,
         )
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/caliper_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/caliper_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/cprofile_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/cprofile_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/dataframe_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/gprof_dot_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/gprof_dot_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/hdf5_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/hdf5_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/hpctoolkit_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/hpctoolkit_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/literal_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/literal_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/pyinstrument_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/pyinstrument_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/spotdb_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/spotdb_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/tau_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/tau_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/readers/timemory_reader.py` & `llnl-hatchet-2022.2.2/hatchet/readers/timemory_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/caliper.py` & `llnl-hatchet-2022.2.2/hatchet/tests/caliper.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,14 +172,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "121489.000 main" in output
     assert "663.000 LagrangeElements" in output
     assert "21493.000 CalcTimeConstraintsForElems" in output
 
     output = ConsoleRenderer(unicode=True, color=False).render(
         gf.graph.roots,
@@ -191,14 +192,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "662712.000 EvalEOSForElems" in output
     assert "2895319.000 LagrangeNodal" in output
 
 
 def test_graphframe_to_literal(lulesh_caliper_json):
     """Sanity test a GraphFrame object with known data."""
@@ -222,27 +224,31 @@
         if col in ("time (inc)", "time"):
             assert gf.dataframe[col].dtype == np.float64
         elif col in ("nid", "rank"):
             assert gf.dataframe[col].dtype == np.int64
         elif col in ("name", "node"):
             assert gf.dataframe[col].dtype == object
 
+    assert type(gf.metadata["cali.channel"]) == str
+    assert type(gf.metadata["cali.caliper.version"]) == str
+
 
 @pytest.mark.skipif(
     not caliperreader_avail, reason="needs caliper-reader package to be loaded"
 )
 def test_graphframe_native_lulesh_from_caliperreader(lulesh_caliper_cali):
     """Sanity check the native Caliper reader by examining a known input."""
     r = caliperreader.CaliperReader()
     r.read(lulesh_caliper_cali)
 
     gf = GraphFrame.from_caliperreader(r)
 
     assert len(gf.dataframe.groupby("name")) == 19
     assert "cali.caliper.version" in gf.metadata.keys()
+    assert type(gf.metadata["cali.caliper.version"]) == str
 
     for col in gf.dataframe.columns:
         if col in ("time (inc)", "time"):
             assert gf.dataframe[col].dtype == np.float64
         elif col in ("nid", "rank"):
             assert gf.dataframe[col].dtype == np.int64
         elif col in ("name", "node"):
@@ -280,20 +286,28 @@
             assert gf.dataframe[col].dtype == np.int64
         elif col in "name":
             assert gf.dataframe[col].dtype == object
 
     for col in gf.exc_metrics + gf.inc_metrics:
         assert col in gf.dataframe.columns
 
+    assert type(gf.metadata["mpi.world.size"]) == int
+    assert type(gf.metadata["cali.caliper.version"]) == str
+    assert type(gf.metadata["cali.channel"]) == str
+
 
 def test_sw4_cuda_summary_from_caliperreader(
     sw4_caliper_cuda_activity_profile_summary_cali,
 ):
     gf = GraphFrame.from_caliperreader(sw4_caliper_cuda_activity_profile_summary_cali)
 
     assert len(gf.graph) == 393
     assert all(
         metric in gf.dataframe.columns for metric in gf.exc_metrics + gf.inc_metrics
     )
 
     for col in gf.exc_metrics + gf.inc_metrics:
         assert col in gf.dataframe.columns
+
+    assert type(gf.metadata["mpi.world.size"]) == int
+    assert type(gf.metadata["cali.caliper.version"]) == str
+    assert type(gf.metadata["cali.channel"]) == str
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/callgrind.py` & `llnl-hatchet-2022.2.2/hatchet/tests/callgrind.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/conftest.py` & `llnl-hatchet-2022.2.2/hatchet/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1085,7 +1085,18 @@
         cali_json_dir, "caliper_cuda_activity_profile_summary_v2.cali"
     )
 
     shutil.copy(cali_json_file, str(tmpdir))
     tmpfile = os.path.join(str(tmpdir), "caliper_cuda_activity_profile_summary_v2.cali")
 
     return tmpfile
+
+
+@pytest.fixture
+def json_graphframe_specification(data_dir, tmpdir):
+    json_dir = os.path.join(data_dir, "json")
+    json_file = os.path.join(json_dir, "hatchet-graph-literal.json")
+
+    shutil.copy(json_file, str(tmpdir))
+    tmpfile = os.path.join(str(tmpdir), "hatchet-graph-literal.json")
+
+    return tmpfile
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/cprofile.py` & `llnl-hatchet-2022.2.2/hatchet/tests/cprofile.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "g pstats_reader_test.py" in output
     assert "<method 'disable' ...Profiler' objects> ~" in output
 
     output = ConsoleRenderer(unicode=True, color=False).render(
         gf.graph.roots,
         gf.dataframe,
@@ -58,10 +59,11 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "f pstats_reader_test.py" in output
     assert re.match("(.|\n)*recursive(.|\n)*recursive", output)
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/dataframe_ops.py` & `llnl-hatchet-2022.2.2/hatchet/tests/dataframe_ops.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/executable.py` & `llnl-hatchet-2022.2.2/hatchet/tests/executable.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/frame.py` & `llnl-hatchet-2022.2.2/hatchet/tests/frame.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/graph.py` & `llnl-hatchet-2022.2.2/hatchet/tests/graph.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/graph_literal.py` & `llnl-hatchet-2022.2.2/hatchet/tests/graph_literal.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/graph_ops.py` & `llnl-hatchet-2022.2.2/hatchet/tests/graph_ops.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/graphframe.py` & `llnl-hatchet-2022.2.2/hatchet/tests/graphframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from hatchet import GraphFrame, QueryMatcher
 from hatchet.graphframe import InvalidFilter, EmptyFilter
 from hatchet.frame import Frame
 from hatchet.graph import Graph
 from hatchet.node import Node
 from hatchet.external.console import ConsoleRenderer
+from hatchet.version import __version__
 
 
 def test_copy(mock_graph_literal):
     self = GraphFrame.from_literal(mock_graph_literal)
     other = self.copy()
 
     assert self is not other
@@ -717,18 +718,20 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "0.000 foo" in output
     assert "10.000 waldo" in output
     assert "15.000 garply" in output
+    assert "v" + __version__ in output
 
     output = ConsoleRenderer(unicode=True, color=False).render(
         gf.graph.roots,
         gf.dataframe,
         metric_column="time (inc)",
         precision=3,
         name_column="name",
@@ -736,17 +739,19 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=False,
     )
     assert "55.000 waldo" in output
     assert "15.000 garply" in output
+    assert "v" + __version__ not in output
 
 
 def test_to_dot(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     output = gf.to_dot(metric="time")
 
     # do a simple edge check -- this isn't exhaustive
@@ -794,14 +799,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "0.000 C" in output
     assert u"nan D ▶" in output
     assert u"10.000 H ◀" in output
 
     gf5 = gf1 - gf3
 
@@ -823,14 +829,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "15.000 A" in output
     assert u"5.000 C ◀" in output
     assert u"10.000 H ◀" in output
 
 
 def test_div_decorator(small_mock1, small_mock2):
@@ -857,14 +864,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "1.000 C" in output
     assert "inf B" in output
     assert u"nan D ▶" in output
     assert u"10.000 H ◀" in output
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/hpctoolkit.py` & `llnl-hatchet-2022.2.2/hatchet/tests/hpctoolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "0.000 <program root> <unknown file>" in output
     assert (
         "0.000 198:MPIR_Init_thread /tmp/dpkg-mkdeb.gouoc49UG7/src/mvapich/src/build/../src/mpi/init/initthread.c"
         in output
     )
 
@@ -132,14 +133,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "17989.000 interp.c:0 interp.c" in output
     assert (
         "999238.000 230:psm_dofinalize /tmp/dpkg-mkdeb.gouoc49UG7/src/mvapich/src/build/../src/mpid/ch3/channels/psm/src/psm_exit.c"
         in output
     )
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/node.py` & `llnl-hatchet-2022.2.2/hatchet/tests/node.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/profiler.py` & `llnl-hatchet-2022.2.2/hatchet/tests/profiler.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/pyinstrument.py` & `llnl-hatchet-2022.2.2/hatchet/tests/pyinstrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "0.000 <module> examples.py" in output
     assert "0.025 read hatchet/readers/caliper_reader.py" in output
 
     output = ConsoleRenderer(unicode=True, color=False).render(
         gf.graph.roots,
         gf.dataframe,
@@ -105,14 +106,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "0.478 <module> examples.py" in output
     assert "0.063 from_caliper_json hatchet/graphframe.py" in output
 
 
 def test_graphframe_to_literal(hatchet_pyinstrument_json):
     """Sanity test a GraphFrame object with known data."""
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/query.py` & `llnl-hatchet-2022.2.2/hatchet/tests/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1207,7 +1207,43 @@
         roots[0].children[1].children[0].children[0].children[0].children[0],
         roots[0].children[2].children[0].children[0],
         roots[0].children[2].children[0].children[1].children[0].children[0],
         roots[1].children[0].children[0],
     ]
     assert sorted(compound_query1.apply(gf)) == sorted(matches)
     assert sorted(compound_query2.apply(gf)) == sorted(matches)
+
+
+def test_leaf_query(small_mock2):
+    gf = GraphFrame.from_literal(small_mock2)
+    roots = gf.graph.roots
+    matches = [
+        roots[0].children[0].children[0],
+        roots[0].children[0].children[1],
+        roots[0].children[1].children[0],
+        roots[0].children[1].children[1],
+    ]
+    nodes = set(gf.graph.traverse())
+    nonleaves = list(nodes - set(matches))
+    obj_query = QueryMatcher([{"depth": -1}])
+    str_query_numeric = parse_cypher_query(
+        u"""
+        MATCH (p)
+        WHERE p."depth" = -1
+        """
+    )
+    str_query_is_leaf = parse_cypher_query(
+        u"""
+        MATCH (p)
+        WHERE p IS LEAF
+        """
+    )
+    str_query_is_not_leaf = parse_cypher_query(
+        u"""
+        MATCH (p)
+        WHERE p IS NOT LEAF
+        """
+    )
+    assert sorted(obj_query.apply(gf)) == sorted(matches)
+    assert sorted(str_query_numeric.apply(gf)) == sorted(matches)
+    assert sorted(str_query_is_leaf.apply(gf)) == sorted(matches)
+    assert sorted(str_query_is_not_leaf.apply(gf)) == sorted(nonleaves)
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/spotdb_test.py` & `llnl-hatchet-2022.2.2/hatchet/tests/spotdb_test.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/tau.py` & `llnl-hatchet-2022.2.2/hatchet/tests/tau.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "449.000 .TAU application" in output
     assert "4458.000 MPI_Finalize()" in output
     assert "218.000 MPI_Bcast()" in output
 
     # check the tree for rank 1
     output = ConsoleRenderer(unicode=True, color=False).render(
@@ -59,14 +60,15 @@
         context_column="",
         rank=1,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
     assert "419.000 .TAU application" in output
     assert "4894.000 MPI_Finalize()" in output
     assert "333.000 MPI_Bcast()" in output
 
 
 def test_children(tau_profile_dir):
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/timemory_func.py` & `llnl-hatchet-2022.2.2/hatchet/tests/timemory_func.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/tests/timemory_test.py` & `llnl-hatchet-2022.2.2/hatchet/tests/timemory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
 
     print(output)
 
     output = ConsoleRenderer(unicode=True, color=False).render(
         gf.graph.roots,
         gf.dataframe,
@@ -72,14 +73,15 @@
         context_column="file",
         rank=0,
         thread=0,
         depth=10000,
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
+        render_header=True,
     )
 
     print(output)
 
 
 @pytest.mark.skipif(not timemory_avail, reason="timemory package not available")
 def test_graphframe_to_literal(timemory_json_data):
```

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/colormaps.py` & `llnl-hatchet-2022.2.2/hatchet/util/colormaps.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/deprecated.py` & `llnl-hatchet-2022.2.2/hatchet/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/dot.py` & `llnl-hatchet-2022.2.2/hatchet/util/dot.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/executable.py` & `llnl-hatchet-2022.2.2/hatchet/util/executable.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/profiler.py` & `llnl-hatchet-2022.2.2/hatchet/util/profiler.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/util/timer.py` & `llnl-hatchet-2022.2.2/hatchet/util/timer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/writers/dataframe_writer.py` & `llnl-hatchet-2022.2.2/hatchet/writers/dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/hatchet/writers/hdf5_writer.py` & `llnl-hatchet-2022.2.2/hatchet/writers/hdf5_writer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.0/llnl_hatchet.egg-info/SOURCES.txt` & `llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 hatchet/readers/caliper_native_reader.py
 hatchet/readers/caliper_reader.py
 hatchet/readers/cprofile_reader.py
 hatchet/readers/dataframe_reader.py
 hatchet/readers/gprof_dot_reader.py
 hatchet/readers/hdf5_reader.py
 hatchet/readers/hpctoolkit_reader.py
+hatchet/readers/json_reader.py
 hatchet/readers/literal_reader.py
 hatchet/readers/pyinstrument_reader.py
 hatchet/readers/spotdb_reader.py
 hatchet/readers/tau_reader.py
 hatchet/readers/timemory_reader.py
 hatchet/tests/caliper.py
 hatchet/tests/callgrind.py
@@ -36,14 +37,15 @@
 hatchet/tests/executable.py
 hatchet/tests/frame.py
 hatchet/tests/graph.py
 hatchet/tests/graph_literal.py
 hatchet/tests/graph_ops.py
 hatchet/tests/graphframe.py
 hatchet/tests/hpctoolkit.py
+hatchet/tests/json_test.py
 hatchet/tests/node.py
 hatchet/tests/profiler.py
 hatchet/tests/pyinstrument.py
 hatchet/tests/query.py
 hatchet/tests/spotdb_test.py
 hatchet/tests/tau.py
 hatchet/tests/timemory_func.py
```

### Comparing `llnl-hatchet-2022.2.0/pyproject.toml` & `llnl-hatchet-2022.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llnl-hatchet"
-version = "2022.2.0"
+version = "2022.2.2"
 description = "A Python library for analyzing hierarchical performance data."
 authors = [
     "Abhinav Bhatele <bhatele@cs.umd.edu>",
     "Stephanie Brink <brink2@llnl.gov>",
     "Todd Gamblin <tgamblin@llnl.gov>",
 ]
 license = "MIT"
```

### Comparing `llnl-hatchet-2022.2.0/setup.py` & `llnl-hatchet-2022.2.2/setup.py`

 * *Files identical despite different names*

