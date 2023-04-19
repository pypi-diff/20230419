# Comparing `tmp/lavacli-1.8.tar.gz` & `tmp/lavacli-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavacli-1.8.tar", last modified: Wed Apr 12 15:50:06 2023, max compression
+gzip compressed data, was "lavacli-1.9.tar", last modified: Wed Apr 19 07:56:41 2023, max compression
```

## Comparing `lavacli-1.8.tar` & `lavacli-1.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.877318 lavacli-1.8/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-1.8/.coveragerc
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2506 2023-03-17 09:18:40.000000 lavacli-1.8/.gitlab-ci.yml
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-1.8/LICENSE
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-1.8/MANIFEST.in
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-12 15:50:06.877318 lavacli-1.8/PKG-INFO
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/doc/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-1.8/doc/Makefile
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-1.8/doc/conf.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-1.8/doc/configuration.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-1.8/doc/index.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      721 2019-04-24 15:25:09.000000 lavacli-1.8/doc/install.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-1.8/doc/usage.rst
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/lavacli/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1344 2023-04-12 15:49:32.000000 lavacli-1.8/lavacli/__about__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9098 2023-04-12 15:39:30.000000 lavacli-1.8/lavacli/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/__main__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-1.8/lavacli/colors.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/lavacli/commands/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-1.8/lavacli/commands/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-1.8/lavacli/commands/device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-1.8/lavacli/commands/events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-1.8/lavacli/commands/groups.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    33751 2023-04-12 15:39:33.000000 lavacli-1.8/lavacli/commands/lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-1.8/lavacli/commands/system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-1.8/lavacli/commands/users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-1.8/lavacli/commands/utils.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/workers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-1.8/lavacli/utils.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/lavacli.egg-info/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/PKG-INFO
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1242 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/SOURCES.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/dependency_links.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/entry_points.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/requires.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/top_level.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/zip-safe
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-03-17 09:09:30.000000 lavacli-1.8/requirements.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-04-12 15:50:06.877318 lavacli-1.8/setup.cfg
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2417 2023-03-17 09:10:17.000000 lavacli-1.8/setup.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/share/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-1.8/share/lavacli.yaml
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/tests/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-1.8/tests/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-1.8/tests/conftest.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_helpers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-1.8/tests/test_jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    78667 2023-04-12 15:39:33.000000 lavacli-1.8/tests/test_lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_lavacli.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-1.8/tests/test_users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-1.8/tests/test_workers.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.306845 lavacli-1.9/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-1.9/.coveragerc
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2506 2023-03-17 09:18:40.000000 lavacli-1.9/.gitlab-ci.yml
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-1.9/LICENSE
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-1.9/MANIFEST.in
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-19 07:56:41.306845 lavacli-1.9/PKG-INFO
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/doc/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-1.9/doc/Makefile
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-1.9/doc/conf.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-1.9/doc/configuration.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-1.9/doc/index.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      721 2019-04-24 15:25:09.000000 lavacli-1.9/doc/install.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-1.9/doc/usage.rst
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/lavacli/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1344 2023-04-19 07:56:07.000000 lavacli-1.9/lavacli/__about__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9098 2023-04-12 15:39:30.000000 lavacli-1.9/lavacli/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/__main__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-1.9/lavacli/colors.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.302845 lavacli-1.9/lavacli/commands/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-1.9/lavacli/commands/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-1.9/lavacli/commands/device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-1.9/lavacli/commands/events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-1.9/lavacli/commands/groups.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    37032 2023-04-19 07:55:03.000000 lavacli-1.9/lavacli/commands/lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-1.9/lavacli/commands/system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-1.9/lavacli/commands/users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-1.9/lavacli/commands/utils.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/workers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-1.9/lavacli/utils.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/lavacli.egg-info/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/PKG-INFO
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1242 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/SOURCES.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/dependency_links.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/entry_points.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/requires.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/top_level.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/zip-safe
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-03-17 09:09:30.000000 lavacli-1.9/requirements.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-04-19 07:56:41.306845 lavacli-1.9/setup.cfg
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2417 2023-03-17 09:10:17.000000 lavacli-1.9/setup.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.302845 lavacli-1.9/share/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-1.9/share/lavacli.yaml
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.306845 lavacli-1.9/tests/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-1.9/tests/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-1.9/tests/conftest.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_helpers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-1.9/tests/test_jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    94482 2023-04-19 07:55:03.000000 lavacli-1.9/tests/test_lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_lavacli.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-1.9/tests/test_users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-1.9/tests/test_workers.py
```

### Comparing `lavacli-1.8/.gitlab-ci.yml` & `lavacli-1.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/LICENSE` & `lavacli-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/PKG-INFO` & `lavacli-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.8
+Version: 1.9
 Summary: LAVA XML-RPC command line interface
 Home-page: https://git.lavasoftware.org/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
 Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
```

### Comparing `lavacli-1.8/doc/Makefile` & `lavacli-1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/doc/conf.py` & `lavacli-1.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/doc/configuration.rst` & `lavacli-1.9/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/doc/install.rst` & `lavacli-1.9/doc/install.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/doc/usage.rst` & `lavacli-1.9/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/__about__.py` & `lavacli-1.9/lavacli/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
 
 __author__ = "Rémi Duraffort"
 __author_email__ = "remi.duraffort@linaro.org"
 __description__ = "LAVA XML-RPC command line interface"
 __license__ = "AGPLv3+"
 __url__ = "https://git.lavasoftware.org/lava/lavacli"
-__version__ = "1.8"
+__version__ = "1.9"
```

### Comparing `lavacli-1.8/lavacli/__init__.py` & `lavacli-1.9/lavacli/__init__.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/__main__.py` & `lavacli-1.9/lavacli/__main__.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/aliases.py` & `lavacli-1.9/lavacli/commands/aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/device_types.py` & `lavacli-1.9/lavacli/commands/device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/devices.py` & `lavacli-1.9/lavacli/commands/devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/events.py` & `lavacli-1.9/lavacli/commands/events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/groups.py` & `lavacli-1.9/lavacli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/identities.py` & `lavacli-1.9/lavacli/commands/identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/jobs.py` & `lavacli-1.9/lavacli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/lab.py` & `lavacli-1.9/lavacli/commands/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,25 +54,39 @@
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         return [
             f.name for f in fields(self) if getattr(self, f.name) != data.get(f.name)
         ]
 
 
+@dataclass(frozen=True, order=True)
+class GroupDevicePermission:
+    name: str
+    group: str
+
+    def dump(self):
+        data = {k: v for k, v in asdict(self).items()}
+        return data if data else None
+
+    def __repr__(self):
+        return f"{self.name:<25}{self.group}"
+
+
 @dataclass
 class Device(Base):
     hostname: str
     device_type: str
     worker: str
     description: str = None
     tags: Set[str] = field(default_factory=set)
-    # TODO: add permissions
+    permissions: Set[GroupDevicePermission] = field(default_factory=set)
 
     def __post_init__(self):
         self.tags = set(self.tags)
+        self.permissions = set([GroupDevicePermission(**p) for p in self.permissions])
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         data = data.copy()
         data["tags"] = set(data["tags"])
         if data["description"] is None:
             data["description"] = ""
         if self.description is None:
@@ -90,14 +104,18 @@
         if "description" in data and data["description"] in ["", None]:
             del data["description"]
         if not data["tags"]:
             del data["tags"]
         else:
             data["tags"] = sorted(data["tags"])
         del data["hostname"]
+        if not data["permissions"]:
+            del data["permissions"]
+        else:
+            data["permissions"] = [p.dump() for p in sorted(data["permissions"])]
         return data if data else None
 
     def get_dict(self, base):
         with contextlib.suppress(FileNotFoundError):
             return (base / "devices" / f"{self.hostname}.jinja2").read_text(
                 encoding="utf-8"
             )
@@ -116,18 +134,19 @@
     name: str
     description: str = ""
     health_disabled: str = False
     health_denominator: str = "hours"
     health_frequency: int = 24
     aliases: Set[str] = field(default_factory=set)
     display: bool = True
-    # TODO: add permissions
+    permissions: Set[GroupDevicePermission] = field(default_factory=set)
 
     def __post_init__(self):
         self.aliases = set(self.aliases)
+        self.permissions = set([GroupDevicePermission(**p) for p in self.permissions])
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         data = data.copy()
         data["aliases"] = set(data["aliases"])
         if data["description"] is None:
             data["description"] = ""
         if self.description is None:
@@ -145,14 +164,18 @@
         if not data["aliases"]:
             del data["aliases"]
         else:
             data["aliases"] = sorted(data["aliases"])
         if "description" in data and data["description"] in ["", None]:
             del data["description"]
         del data["name"]
+        if not data["permissions"]:
+            del data["permissions"]
+        else:
+            data["permissions"] = [p.dump() for p in sorted(data["permissions"])]
         return data if data else None
 
     def get_health_check(self, base):
         with contextlib.suppress(FileNotFoundError):
             return (base / "health-checks" / f"{self.name}.yaml").read_text(
                 encoding="utf-8"
             )
@@ -534,16 +557,20 @@
                         dt.display or True,
                         # owners_only is deprecated.
                         None,
                         dt.health_frequency or 24,
                         dt.health_denominator or "hours",
                     )
             data = proxy.scheduler.device_types.show(dt.name)
+            if config["version"] >= (2023, 3):
+                data["permissions"] = set(
+                    [GroupDevicePermission(**p) for p in data.get("permissions", [])]
+                )
             diff = dt.diff(data)
-            dt_diff = [n for n in diff if n != "aliases"]
+            dt_diff = [n for n in diff if n not in ["aliases", "permissions"]]
             if dt_diff:
                 for name in dt_diff:
                     print(
                         f"    {colors.yellow}-> {name}: '{data[name]}' => '{getattr(dt, name)}'{colors.reset}"
                     )
                 if not options.dry_run:
                     proxy.scheduler.device_types.update(
@@ -564,14 +591,31 @@
                         proxy.scheduler.device_types.aliases.add(dt.name, alias)
                 missing = set(data["aliases"]).difference(dt.aliases)
                 for alias in missing:
                     print(f"      {colors.red}- {alias}{colors.reset}")
                     if not options.dry_run:
                         proxy.scheduler.device_types.aliases.delete(dt.name, alias)
 
+            if config["version"] >= (2023, 3) and "permissions" in diff:
+                print(f"    {colors.yellow}->  {'permission':<25}group{colors.reset}")
+                missing = sorted(dt.permissions.difference(set(data["permissions"])))
+                for perm in missing:
+                    print(f"      {colors.green}+ {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.device_types.perms_add(
+                            dt.name, perm.group, perm.name
+                        )
+                missing = sorted(set(data["permissions"]).difference(dt.permissions))
+                for perm in missing:
+                    print(f"      {colors.red}- {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.device_types.perms_delete(
+                            dt.name, perm.group, perm.name
+                        )
+
             try:
                 hc = str(proxy.scheduler.device_types.get_health_check(dt.name))
             except xmlrpc.client.Fault as exc:
                 if exc.faultCode != 404:
                     raise
                 hc = None
             if dt.get_health_check(base) != hc:
@@ -688,16 +732,20 @@
                         None,
                         None,
                         None,
                         None,
                         device.description,
                     )
             data = proxy.scheduler.devices.show(device.hostname)
+            if config["version"] >= (2023, 3):
+                data["permissions"] = set(
+                    [GroupDevicePermission(**p) for p in data.get("permissions", [])]
+                )
             diff = device.diff(data)
-            device_diff = [n for n in diff if n != "tags"]
+            device_diff = [n for n in diff if n not in ["tags", "permissions"]]
             if device_diff:
                 for name in device_diff:
                     print(
                         f"    {colors.yellow}-> {name}: '{data[name]}' => '{getattr(device, name)}'{colors.reset}"
                     )
                 if not options.dry_run:
                     proxy.scheduler.devices.update(
@@ -719,14 +767,35 @@
                         proxy.scheduler.devices.tags.add(device.hostname, tag)
                 missing = set(data["tags"]).difference(device.tags)
                 for tag in missing:
                     print(f"      {colors.red}- {tag}{colors.reset}")
                     if not options.dry_run:
                         proxy.scheduler.devices.tags.delete(device.hostname, tag)
 
+            if config["version"] >= (2023, 3) and "permissions" in diff:
+                print(f"    {colors.yellow}->  {'permission':<25}group{colors.reset}")
+                missing = sorted(
+                    device.permissions.difference(set(data["permissions"]))
+                )
+                for perm in missing:
+                    print(f"      {colors.green}+ {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.devices.perms_add(
+                            device.hostname, perm.group, perm.name
+                        )
+                missing = sorted(
+                    set(data["permissions"]).difference(device.permissions)
+                )
+                for perm in missing:
+                    print(f"      {colors.red}- {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.devices.perms_delete(
+                            device.hostname, perm.group, perm.name
+                        )
+
             try:
                 ddict = str(proxy.scheduler.devices.get_dictionary(device.hostname))
             except xmlrpc.client.Fault as exc:
                 if exc.faultCode != 404:
                     raise
                 ddict = None
```

### Comparing `lavacli-1.8/lavacli/commands/results.py` & `lavacli-1.9/lavacli/commands/results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/system.py` & `lavacli-1.9/lavacli/commands/system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/tags.py` & `lavacli-1.9/lavacli/commands/tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/users.py` & `lavacli-1.9/lavacli/commands/users.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/utils.py` & `lavacli-1.9/lavacli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/commands/workers.py` & `lavacli-1.9/lavacli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli/utils.py` & `lavacli-1.9/lavacli/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/lavacli.egg-info/PKG-INFO` & `lavacli-1.9/lavacli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.8
+Version: 1.9
 Summary: LAVA XML-RPC command line interface
 Home-page: https://git.lavasoftware.org/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
 Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
```

### Comparing `lavacli-1.8/lavacli.egg-info/SOURCES.txt` & `lavacli-1.9/lavacli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/setup.py` & `lavacli-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/share/lavacli.yaml` & `lavacli-1.9/share/lavacli.yaml`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/conftest.py` & `lavacli-1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_aliases.py` & `lavacli-1.9/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_device_types.py` & `lavacli-1.9/tests/test_device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_devices.py` & `lavacli-1.9/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_events.py` & `lavacli-1.9/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_helpers.py` & `lavacli-1.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_identities.py` & `lavacli-1.9/tests/test_identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_jobs.py` & `lavacli-1.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_lab.py` & `lavacli-1.9/tests/test_lab.py`

 * *Files 10% similar despite different names*

```diff
@@ -183,14 +183,17 @@
                     "display": True,
                     "health_disabled": False,
                     "health_denominator": "hours",
                     "health_frequency": 24,
                     "aliases": [],
                     "devices": ["docker-01", "docker-02"],
                     "default_template": True,
+                    "permissions": [
+                        {"name": "change_devicetype", "group": "group1"},
+                    ],
                 },
             }
             self.scheduler_device_types_show_docker_custom_template = {
                 "request": "scheduler.device_types.show",
                 "args": ("docker",),
                 "ret": {
                     "name": "docker",
@@ -198,14 +201,17 @@
                     "display": True,
                     "health_disabled": False,
                     "health_denominator": "hours",
                     "health_frequency": 24,
                     "aliases": [],
                     "devices": ["docker-01", "docker-02"],
                     "default_template": False,
+                    "permissions": [
+                        {"name": "change_devicetype", "group": "group1"},
+                    ],
                 },
             }
             self.scheduler_device_types_get_health_check_docker = {
                 "request": "scheduler.device_types.get_health_check",
                 "args": ("docker",),
                 "ret": "hc-definition",
             }
@@ -454,14 +460,17 @@
                     "health_job": True,
                     "description": "Created automatically by LAVA.",
                     "pipeline": True,
                     "has_device_dict": True,
                     "worker": "worker01",
                     "current_job": None,
                     "tags": ["docker-01", "worker"],
+                    "permissions": [
+                        {"name": "change_devicetype", "group": "group1"},
+                    ],
                 },
             }
             self.scheduler_devices_get_dictionary_docker_01 = {
                 "request": "scheduler.devices.get_dictionary",
                 "args": ("docker-01",),
                 "ret": "yaml_dict",
             }
@@ -632,14 +641,24 @@
                 "ret": None,
             }
             self.scheduler_device_types_set_template_docker = {
                 "request": "scheduler.device_types.set_template",
                 "args": ("docker", "new template definition"),
                 "ret": None,
             }
+            self.scheduler_device_types_perms_add_docker = {
+                "request": "scheduler.device_types.perms_add",
+                "args": ("docker", "group1", "view_devicetype"),
+                "ret": None,
+            }
+            self.scheduler_device_types_perms_delete_docker = {
+                "request": "scheduler.device_types.perms_delete",
+                "args": ("docker", "group1", "change_devicetype"),
+                "ret": None,
+            }
             self.scheduler_workers_add_worker03 = {
                 "request": "scheduler.workers.add",
                 "args": ("worker03", "", False),
                 "ret": None,
             }
             self.scheduler_workers_update_worker01 = {
                 "request": "scheduler.workers.update",
@@ -700,36 +719,52 @@
                 "ret": None,
             }
             self.scheduler_devices_tags_delete_docker_01 = {
                 "request": "scheduler.devices.tags.delete",
                 "args": ("docker-01", "docker-01"),
                 "ret": None,
             }
+            self.scheduler_devices_perms_add_docker_01 = {
+                "request": "scheduler.devices.perms_add",
+                "args": ("docker-01", "group1", "view_devicetype"),
+                "ret": None,
+            }
+            self.scheduler_devices_perms_delete_docker_01 = {
+                "request": "scheduler.devices.perms_delete",
+                "args": ("docker-01", "group1", "change_devicetype"),
+                "ret": None,
+            }
 
     return PostData()
 
 
 @pytest.fixture
 def config_file(tmp_path):
     return tmp_path / "lab.yaml"
 
 
 @pytest.fixture
 def config_def():
     return """device_types:
   docker:
+    permissions:
+    - name: change_devicetype
+      group: group1
   qemu:
 devices:
   docker-01:
     device_type: docker
     worker: worker01
     description: Created automatically by LAVA.
     tags:
     - docker-01
     - worker
+    permissions:
+    - name: change_devicetype
+      group: group1
   docker-02:
     device_type: docker
     worker: worker02
     description: Created automatically by LAVA.
     tags:
     - docker-02
     - docker-worker
@@ -895,14 +930,17 @@
             mock_get.scheduler_workers_list_empty,
             mock_get.scheduler_devices_list_empty,
         ],
     )
 
     expected_def = """device_types:
   docker:
+    permissions:
+    - name: change_devicetype
+      group: group1
   qemu:
 devices: {}
 groups: {}
 users: {}
 workers: {}
 """
 
@@ -1548,14 +1586,168 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_dt_perms_add(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "device-types", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_post.scheduler_device_types_perms_add_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_get.scheduler_device_types_show_qemu,
+            mock_get.scheduler_device_types_get_health_check_qemu,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["device_types"]["docker"] is None:
+        data["device_types"]["docker"] = {}
+    data["device_types"]["docker"]["permissions"].append(
+        {"name": "view_devicetype", "group": "group1"}
+    )
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[32m* docker\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[32m+ view_devicetype          group1\x1b[0m\n  \x1b[32m* qemu\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_dt_perms_delete(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "device-types", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_post.scheduler_device_types_perms_delete_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_get.scheduler_device_types_show_qemu,
+            mock_get.scheduler_device_types_get_health_check_qemu,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["device_types"]["docker"] is None:
+        data["device_types"]["docker"] = {}
+    del data["device_types"]["docker"]["permissions"]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[32m* docker\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[91m- change_devicetype        group1\x1b[0m\n  \x1b[32m* qemu\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_dt_perms_update(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "device-types", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_post.scheduler_device_types_perms_add_docker,
+            mock_post.scheduler_device_types_perms_delete_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_get.scheduler_device_types_show_qemu,
+            mock_get.scheduler_device_types_get_health_check_qemu,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["device_types"]["docker"] is None:
+        data["device_types"]["docker"] = {}
+    data["device_types"]["docker"]["permissions"] = [
+        {"name": "view_devicetype", "group": "group1"},
+    ]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[32m* docker\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[32m+ view_devicetype          group1\x1b[0m\n      \x1b[91m- change_devicetype        group1\x1b[0m\n  \x1b[32m* qemu\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_dt_perms_unsupported(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "device-types", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_2,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_get.scheduler_device_types_show_qemu,
+            mock_get.scheduler_device_types_get_health_check_qemu,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["device_types"]["docker"] is None:
+        data["device_types"]["docker"] = {}
+    data["device_types"]["docker"]["permissions"] = [
+        {"name": "view_devicetype", "group": "group1"},
+    ]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[32m* docker\x1b[0m\n  \x1b[32m* qemu\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
 def test_lab_apply_workers_no_change(
     setup, monkeypatch, capsys, config_file, config_def, mock_get
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
@@ -2061,7 +2253,205 @@
         yaml.dump(data, f)
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n    \x1b[33m-> tags\x1b[0m\n      \x1b[91m- docker-01\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
+
+
+def test_lab_apply_devices_perms_add(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_post.scheduler_devices_perms_add_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["devices"]["docker-01"] is None:
+        data["devices"]["docker-01"] = {}
+    data["devices"]["docker-01"]["permissions"].append(
+        {"name": "view_devicetype", "group": "group1"}
+    )
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[32m+ view_devicetype          group1\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_devices_perms_delete(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_post.scheduler_devices_perms_delete_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["devices"]["docker-01"] is None:
+        data["devices"]["docker-01"] = {}
+    del data["devices"]["docker-01"]["permissions"]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[91m- change_devicetype        group1\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_devices_perms_update(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_post.scheduler_devices_perms_add_docker_01,
+            mock_post.scheduler_devices_perms_delete_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["devices"]["docker-01"] is None:
+        data["devices"]["docker-01"] = {}
+    data["devices"]["docker-01"]["permissions"] = [
+        {"name": "view_devicetype", "group": "group1"},
+    ]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n    \x1b[33m->  permission               group\x1b[0m\n      \x1b[32m+ view_devicetype          group1\x1b[0m\n      \x1b[91m- change_devicetype        group1\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
+def test_lab_apply_devices_perms_unsupported(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_2,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    if data["devices"]["docker-01"] is None:
+        data["devices"]["docker-01"] = {}
+    data["devices"]["docker-01"]["permissions"] = [
+        {"name": "view_devicetype", "group": "group1"},
+    ]
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
```

### Comparing `lavacli-1.8/tests/test_lavacli.py` & `lavacli-1.9/tests/test_lavacli.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_results.py` & `lavacli-1.9/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_system.py` & `lavacli-1.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_tags.py` & `lavacli-1.9/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_users.py` & `lavacli-1.9/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.8/tests/test_workers.py` & `lavacli-1.9/tests/test_workers.py`

 * *Files identical despite different names*

