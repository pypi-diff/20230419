# Comparing `tmp/netin-1.0.5.4.tar.gz` & `tmp/netin-1.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.4.tar", last modified: Wed Apr 19 10:19:05 2023, max compression
+gzip compressed data, was "netin-1.0.5.5.tar", last modified: Wed Apr 19 11:44:07 2023, max compression
```

## Comparing `netin-1.0.5.4.tar` & `netin-1.0.5.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.4/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.4/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 10:19:05.788822 netin-1.0.5.4/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.4/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.780821 netin-1.0.5.4/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.784822 netin-1.0.5.4/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.4/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.4/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.4/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.784822 netin-1.0.5.4/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3100 2023-04-17 23:26:28.000000 netin-1.0.5.4/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.784822 netin-1.0.5.4/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.4/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.4/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.4/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.4/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.784822 netin-1.0.5.4/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-19 08:35:59.000000 netin-1.0.5.4/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.4/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.4/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.4/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.4/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.4/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.4/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.4/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.4/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.4/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.4/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.4/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.4/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.4/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.4/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.4/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.4/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.4/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.4/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.4/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.4/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.4/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.4/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.4/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.4/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.4/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.4/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.4/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    26582 2023-04-19 10:03:43.000000 netin-1.0.5.4/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 10:19:05.000000 netin-1.0.5.4/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1268 2023-04-19 10:19:05.000000 netin-1.0.5.4/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-19 10:19:05.000000 netin-1.0.5.4/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.4/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-19 10:19:05.000000 netin-1.0.5.4/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-19 10:19:05.000000 netin-1.0.5.4/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 10:19:05.788822 netin-1.0.5.4/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.4/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.4/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-19 10:19:05.788822 netin-1.0.5.4/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.4/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.5/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.5/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 11:44:07.288888 netin-1.0.5.5/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.5/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.284888 netin-1.0.5.5/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.284888 netin-1.0.5.5/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.5/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.5/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.5/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.5/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.5/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.5/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.5/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.5/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-19 10:53:22.000000 netin-1.0.5.5/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.5/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.5/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.5/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.5/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.5/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.5/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.5/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.5/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.5/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.5/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.5/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.5/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.5/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.5/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.5/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.5/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.5/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.5/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.5/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.5/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.5/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.5/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.5/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.5/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    26851 2023-04-19 11:35:51.000000 netin-1.0.5.5/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1268 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.5/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.5/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.5/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-19 11:44:07.288888 netin-1.0.5.5/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.5/setup.py
```

### Comparing `netin-1.0.5.4/LICENSE` & `netin-1.0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/PKG-INFO` & `netin-1.0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.4
+Version: 1.0.5.5
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.4/README.rst` & `netin-1.0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/examples/notebooks/deleteme.py` & `netin-1.0.5.5/examples/notebooks/deleteme.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,58 +40,59 @@
     :param kwargs:
     :return:
     """
 
     if type(data) not in [list, set, List, Set]:
         data = [data]
 
-        w, h = len(data) * 3.2, 3.2  # default figure size (width, height)
-        width = kwargs.pop('width_bar', 0.25)  # the width of the bars
-        figsize = kwargs.pop('figsize', (w, h))  # figure size (width, height)
-        loc = kwargs.pop('loc', 'upper right')  # position of legend
-        ncols = kwargs.pop('ncols', 1)  # number of columns in legend
-
-        fig, ax = plt.subplots(1, 1, figsize=figsize, layout='constrained')
-        multiplier = 0
-
-        x = None
-        groups = None
-        maxy = 0
-        for g in data:
-            etc = g.count_edges_types()
-            name = update_name_homophily(g)
-
-            groups = list(etc.keys()) if groups is None else groups
-            x = np.arange(len(groups)) if x is None else x
-            y = [etc[i] for i in groups]
-            maxy = max(max(y), maxy)
-
-            offset = width * multiplier
-            rects = ax.bar(x + offset, y, width, label=name)
-            ax.bar_label(rects, padding=3)
-            multiplier += 1
-
-            # Add some text for labels, title and custom x-axis tick labels, etc.
-            ax.set_ylabel('Counts')
-            ax.set_title("Counts of edge types");
-            ax.set_xticks(x + width, groups)
-            ax.legend(loc=loc, ncols=ncols)
-
-            # set limits
-            ax.set_ylim(0, maxy * 1.1)
-
-            # save plot
-            if fn is not None:
-                validate_path(fn)
-                fig.savefig(fname=fn, bbox_inches='tight', dpi=300)
-                print(f'{fn} saved.')
-
-                # Final
-                plt.show()
-                plt.close()
+    w, h = len(data) * 3.2, 3.2  # default figure size (width, height)
+    width = kwargs.pop('width_bar', 0.25)  # the width of the bars
+    figsize = kwargs.pop('figsize', (w, h))  # figure size (width, height)
+    loc = kwargs.pop('loc', 'upper right')  # position of legend
+    ncols = kwargs.pop('nc_legend', 1)  # number of columns in legend
+
+    fig, ax = plt.subplots(1, 1, figsize=figsize, layout='constrained')
+    multiplier = 0
+
+    x = None
+    groups = None
+    maxy = 0
+    for g in data:
+        etc = g.count_edges_types()
+        name = update_name_homophily(g)
+
+        groups = list(etc.keys()) if groups is None else groups
+        x = np.arange(len(groups)) if x is None else x
+        y = [etc[i] for i in groups]
+        maxy = max(max(y), maxy)
+
+        offset = width * multiplier
+        rects = ax.bar(x + offset, y, width, label=name)
+        ax.bar_label(rects, padding=3)
+        multiplier += 1
+
+        # Add some text for labels, title and custom x-axis tick labels, etc.
+        ax.set_ylabel('Counts')
+        ax.set_title("Counts of edge types");
+        ax.set_xticks(x + width, groups)
+        ax.legend(loc=loc, ncols=ncols)
+
+        # set limits
+        ax.set_ylim(0, maxy * 1.1)
+
+    # save plot
+    if fn is not None:
+        validate_path(fn)
+        fig.savefig(fname=fn, bbox_inches='tight', dpi=300)
+        print(f'{fn} saved.')
+
+    # Final
+    plt.show()
+    plt.close()
 
 def validate_path(fn):
     import os
     path = os.path.dirname(fn)
-    if not os.path.exists(path):
-        # Create a new directory because it does not exist
-        os.makedirs(path)
+    if path != '':
+        if not os.path.exists(path):
+            # Create a new directory because it does not exist
+            os.makedirs(path)
```

### Comparing `netin-1.0.5.4/netin/generators/dh.py` & `netin-1.0.5.5/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/directed.py` & `netin-1.0.5.5/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/dpa.py` & `netin-1.0.5.5/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/dpah.py` & `netin-1.0.5.5/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/graph.py` & `netin-1.0.5.5/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/h.py` & `netin-1.0.5.5/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/pa.py` & `netin-1.0.5.5/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/pah.py` & `netin-1.0.5.5/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/patc.py` & `netin-1.0.5.5/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/patch.py` & `netin-1.0.5.5/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/tc.py` & `netin-1.0.5.5/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/tests/test_directed.py` & `netin-1.0.5.5/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/tests/test_dpah.py` & `netin-1.0.5.5/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/tests/test_patch.py` & `netin-1.0.5.5/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/tests/test_undirected.py` & `netin-1.0.5.5/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/generators/undirected.py` & `netin-1.0.5.5/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/stats/distributions.py` & `netin-1.0.5.5/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/stats/ranking.py` & `netin-1.0.5.5/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/utils/constants.py` & `netin-1.0.5.5/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/utils/validator.py` & `netin-1.0.5.5/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/netin/viz/handlers.py` & `netin-1.0.5.5/netin/viz/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     -------
 
     """
     maj_patch = mpatches.Patch(color=COLOR_MAJORITY, label='majority')
     min_patch = mpatches.Patch(color=COLOR_MINORITY, label='minority')
     bbox = kwargs.pop('bbox', (1.04, 1))
     loc = kwargs.pop('loc', "upper left")
-    fig.legend(handles=[maj_patch, min_patch], bbox_to_anchor=bbox, loc=loc, **kwargs)
+    fig.legend(handles=[maj_patch, min_patch], bbox_to_anchor=bbox, loc=loc)
 
 
 def plot_graph(data: Union[Graph, Set[Graph], List[Graph]], share_pos: bool = False, fn : str = None, **kwargs):
     """
     Plots one or multiple (netin.Graph) graphs as matplotlib figures.
 
     Parameters
@@ -591,28 +591,29 @@
 
     def get_me_label(f_m, ys, beta=None) -> (str, float, str):
         from netin.stats import ranking
         # value
         me = ranking.get_ranking_inequity(f_m, ys)
         # label
         ineq = ranking.get_ranking_inequity_class(me, beta)
-        # position
+        # position right
         right = False
         bottom = np.any(np.array(ys[:5]) > 0.8)
         y = 0 + (gap * 2) if bottom else 1 - (gap * 2)
         x = 0 + (gap * 2)
 
         if f_m <= 0.2 and bottom:
+            # right - top
             right = True
             bottom = False
             y = 0 + (gap * 2) if bottom else 1 - (gap * 2)
-            x = 0 + (gap * 2)
+            x = 1 - (gap * 2)
 
             if np.any(np.array(ys[5:]) > 0.8):
-                # above minority
+                # left - above fraction of minority
                 right = False
                 bottom = True
                 y = f_m + (gap * 2)
                 x = 0 + (gap * 2)
 
         va = 'bottom' if bottom else 'top'
         ha = 'right' if right else 'left'
@@ -735,25 +736,33 @@
 
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
         class_label: str
         iter_groups = df.groupby(hue) if hue is not None else [(None, df)]
         for class_label, group in iter_groups:
             group_nonzero = group.query(f"{_col_name}>0")
+
+            if group_nonzero[_col_name].nunique() == 1:
+                # not enough data to fit the powerlaw
+                continue
+
             discrete = group_nonzero[_col_name].dtype == np.int64
             fit = fit_power_law(group_nonzero.loc[:, _col_name].values, discrete=discrete, verbose=verbose)
 
             color = _get_class_label_color(class_label)
 
             efnc = fit.plot_ccdf if kind == "ccdf" else fit.plot_cdf if kind == 'cdf' else fit.plot_pdf
             fnc = fit.power_law.plot_ccdf if kind == "ccdf" else fit.power_law.plot_cdf if kind == 'cdf' \
                 else fit.power_law.plot_pdf
 
-            ax = efnc(label=r"Empirical", ax=ax, color=color, **kwargs)
-            ax = fnc(label=f'Powerlaw $\gamma={fit.alpha:.2f}$', linestyle='--', ax=ax, color=color, **kwargs)
+            try:
+                ax = efnc(label=r"Empirical", ax=ax, color=color, **kwargs)
+                ax = fnc(label=f'Powerlaw $\gamma={fit.alpha:.2f}$', linestyle='--', ax=ax, color=color, **kwargs)
+            except Exception as ex:
+                logging.warning("%s saved" % fn)
 
             # legend inside: empirical vs powerlaw
             handles, labels = ax.get_legend_handles_labels()
             loc = loc if loc is not None else 4 if kind == 'cdf' else 1
             leg = ax.legend(handles, labels, loc=loc, fontsize=fontsize)
             leg.draw_frame(False)
 
@@ -772,12 +781,11 @@
 
     # suptitle
     if suptitle is not None:
         fig.suptitle(suptitle)
 
     # legend (min, maj)
     if hue and bbox:
-        kwargs['bbox'] = bbox
-        _add_class_legend(fig, **kwargs)
+        _add_class_legend(fig, bbox=bbox, **kwargs)
 
     # save plot
     _save_plot(fig, fn, wspace=wspace, hspace=hspace, **kwargs)
```

### Comparing `netin-1.0.5.4/netin.egg-info/PKG-INFO` & `netin-1.0.5.5/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.4
+Version: 1.0.5.5
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.4/netin.egg-info/SOURCES.txt` & `netin-1.0.5.5/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.4/setup.py` & `netin-1.0.5.5/setup.py`

 * *Files identical despite different names*

