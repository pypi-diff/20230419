# Comparing `tmp/orthoseg-0.4.2.tar.gz` & `tmp/orthoseg-0.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthoseg-0.4.2.tar", last modified: Wed Apr 19 08:55:56 2023, max compression
+gzip compressed data, was "orthoseg-0.4.2a1.tar", last modified: Tue Apr 18 08:54:13 2023, max compression
```

## Comparing `orthoseg-0.4.2.tar` & `orthoseg-0.4.2a1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.395499 orthoseg-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 08:55:45.000000 orthoseg-0.4.2/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 08:55:45.000000 orthoseg-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-19 08:55:56.395499 orthoseg-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 08:55:45.000000 orthoseg-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.383499 orthoseg-0.4.2/orthoseg/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.387499 orthoseg-0.4.2/orthoseg/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/helpers/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/helpers/email_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/helpers/vectorfile_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.387499 orthoseg-0.4.2/orthoseg/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37195 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/lib/postprocess_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/lib/predicter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32689 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/lib/prepare_traindatasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25052 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/lib/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/load_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/load_sampleprojects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.387499 orthoseg-0.4.2/orthoseg/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/model/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32221 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/model/model_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    18289 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/project_defaults.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/scriptrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/scriptrunner_defaults.ini
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.391499 orthoseg-0.4.2/orthoseg/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/git_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/log_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/ows_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/progress_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/util/vector_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 08:55:45.000000 orthoseg-0.4.2/orthoseg/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.383499 orthoseg-0.4.2/orthoseg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 08:55:56.000000 orthoseg-0.4.2/orthoseg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 08:55:56.395499 orthoseg-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-19 08:55:45.000000 orthoseg-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:56.395499 orthoseg-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_end2end.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_load_sampleprojects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_ows_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_postprocess_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_prepare_traindata.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_vector_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_vectorfile_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-19 08:55:45.000000 orthoseg-0.4.2/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/
+-rw-rw-rw-   0        0        0    35823 2022-11-01 21:06:33.000000 orthoseg-0.4.2a1/LICENSE.MD
+-rw-rw-rw-   0        0        0      111 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1232 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2022-11-10 10:57:18.000000 orthoseg-0.4.2a1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.455407 orthoseg-0.4.2a1/orthoseg/
+-rw-rw-rw-   0        0        0      498 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/orthoseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.502271 orthoseg-0.4.2a1/orthoseg/helpers/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/helpers/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-04-11 12:35:06.000000 orthoseg-0.4.2a1/orthoseg/helpers/config_helper.py
+-rw-rw-rw-   0        0        0     2302 2022-11-22 17:31:16.000000 orthoseg-0.4.2a1/orthoseg/helpers/email_helper.py
+-rw-rw-rw-   0        0        0     2817 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/helpers/vectorfile_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.533311 orthoseg-0.4.2a1/orthoseg/lib/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/lib/__init__.py
+-rw-rw-rw-   0        0        0    38210 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/lib/postprocess_predictions.py
+-rw-rw-rw-   0        0        0    27801 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/lib/predicter.py
+-rw-rw-rw-   0        0        0    33489 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/lib/prepare_traindatasets.py
+-rw-rw-rw-   0        0        0    25661 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/orthoseg/lib/trainer.py
+-rw-rw-rw-   0        0        0     6799 2023-04-12 12:57:54.000000 orthoseg-0.4.2a1/orthoseg/load_images.py
+-rw-rw-rw-   0        0        0     4185 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/orthoseg/load_sampleprojects.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.549165 orthoseg-0.4.2a1/orthoseg/model/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/model/__init__.py
+-rw-rw-rw-   0        0        0    18952 2022-12-09 22:17:37.000000 orthoseg-0.4.2a1/orthoseg/model/model_factory.py
+-rw-rw-rw-   0        0        0    33034 2022-09-23 11:12:51.000000 orthoseg-0.4.2a1/orthoseg/model/model_helper.py
+-rw-rw-rw-   0        0        0     6180 2022-12-08 00:31:41.000000 orthoseg-0.4.2a1/orthoseg/postprocess.py
+-rw-rw-rw-   0        0        0    12305 2022-12-06 16:37:31.000000 orthoseg-0.4.2a1/orthoseg/predict.py
+-rw-rw-rw-   0        0        0    18730 2022-12-10 13:45:38.000000 orthoseg-0.4.2a1/orthoseg/project_defaults.ini
+-rw-rw-rw-   0        0        0     6083 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/scriptrunner.py
+-rw-rw-rw-   0        0        0     2718 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/scriptrunner_defaults.ini
+-rw-rw-rw-   0        0        0    24067 2022-12-02 09:52:36.000000 orthoseg-0.4.2a1/orthoseg/train.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.595847 orthoseg-0.4.2a1/orthoseg/util/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/util/__init__.py
+-rw-rw-rw-   0        0        0     5126 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/config_util.py
+-rw-rw-rw-   0        0        0     4711 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/general_util.py
+-rw-rw-rw-   0        0        0     4675 2023-02-23 21:56:59.000000 orthoseg-0.4.2a1/orthoseg/util/git_downloader.py
+-rw-rw-rw-   0        0        0     6359 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/log_util.py
+-rw-rw-rw-   0        0        0    40677 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/util/ows_util.py
+-rw-rw-rw-   0        0        0     3434 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/util/progress_util.py
+-rw-rw-rw-   0        0        0    15608 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/util/vector_util.py
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:53:48.000000 orthoseg-0.4.2a1/orthoseg/version.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.486645 orthoseg-0.4.2a1/orthoseg.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      303 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/tests/__init__.py
+-rw-rw-rw-   0        0        0     7212 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/tests/test_end2end.py
+-rw-rw-rw-   0        0        0     3598 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_helper.py
+-rw-rw-rw-   0        0        0     2203 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/tests/test_load_sampleprojects.py
+-rw-rw-rw-   0        0        0     2767 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_model_factory.py
+-rw-rw-rw-   0        0        0     5572 2022-11-14 14:38:51.000000 orthoseg-0.4.2a1/tests/test_ows_util.py
+-rw-rw-rw-   0        0        0     2361 2022-11-22 14:10:08.000000 orthoseg-0.4.2a1/tests/test_postprocess_predictions.py
+-rw-rw-rw-   0        0        0    11276 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_prepare_traindata.py
+-rw-rw-rw-   0        0        0      679 2022-09-20 18:54:20.000000 orthoseg-0.4.2a1/tests/test_train.py
+-rw-rw-rw-   0        0        0    16067 2023-01-20 22:38:51.000000 orthoseg-0.4.2a1/tests/test_vector_util.py
+-rw-rw-rw-   0        0        0     3505 2022-12-08 00:31:41.000000 orthoseg-0.4.2a1/tests/test_vectorfile_helper.py
+-rw-rw-rw-   0        0        0      382 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_version.py
```

### Comparing `orthoseg-0.4.2/LICENSE.MD` & `orthoseg-0.4.2a1/LICENSE.MD`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `orthoseg-0.4.2/PKG-INFO` & `orthoseg-0.4.2a1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: orthoseg
-Version: 0.4.2
-Summary: Package to make it easier to segment orthophotos.
-Home-page: https://github.com/orthoseg/orthoseg
-Author: Pieter Roggemans
-Author-email: pieter.roggemans@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.MD
-
-# Orthophoto segmentation
-
-[![Actions Status](https://github.com/orthoseg/orthoseg/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/orthoseg/orthoseg/actions?query=workflow%3ATests) 
-[![PyPI version](https://img.shields.io/pypi/v/orthoseg.svg)](https://pypi.org/project/orthoseg)
-
-This project provides a procedure and (python) scripts to make it (relatively) easy to 
-1. create a training dataset for a topic of your choice
-2. train a neural network to segment orthophotos
-3. run the segmentation on a larger area + vectorize the result
-4. apply some basic postprocessing like dissolve,...
-
-Only open source software is needed, eg. QGIS and tensorflow.
-
-Installation and usage instructions can be found in the [orthoseg wiki](https://github.com/orthoseg/orthoseg/wiki)
+# Orthophoto segmentation
+
+[![Actions Status](https://github.com/orthoseg/orthoseg/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/orthoseg/orthoseg/actions?query=workflow%3ATests) 
+[![PyPI version](https://img.shields.io/pypi/v/orthoseg.svg)](https://pypi.org/project/orthoseg)
+
+This project provides a procedure and (python) scripts to make it (relatively) easy to 
+1. create a training dataset for a topic of your choice
+2. train a neural network to segment orthophotos
+3. run the segmentation on a larger area + vectorize the result
+4. apply some basic postprocessing like dissolve,...
+
+Only open source software is needed, eg. QGIS and tensorflow.
+
+Installation and usage instructions can be found in the [orthoseg wiki](https://github.com/orthoseg/orthoseg/wiki)
```

### Comparing `orthoseg-0.4.2/orthoseg/helpers/config_helper.py` & `orthoseg-0.4.2a1/orthoseg/helpers/config_helper.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-# -*- coding: utf-8 -*-
-"""
-Module with specific helper functions to manage the configuration of orthoseg.
-"""
-
-import configparser
-import json
-import logging
-from pathlib import Path
-import pprint
-
-from orthoseg.util import config_util
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# Define the chars that cannot be used in codes that are use in filenames.
-# Remark: '_' cannot be used because '_' is used as devider to parse filenames, and if
-# it is used in codes as well the parsing becomes a lot more difficult.
-illegal_chars_in_codes = ["_", ",", ".", "?", ":"]
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def read_orthoseg_config(config_path: Path):
-
-    # Determine list of config files that should be loaded
-    config_paths = config_util.get_config_files(config_path)  # type: ignore
-    # Load them
-    global config
-    config = config_util.read_config_ext(config_paths)
-
-    # Now do orthoseg-specific checks, inits,... on config
-    global config_filepaths_used
-    config_filepaths_used = config_paths
-
-    # Now set global variables to each section as shortcuts
-    global general
-    general = config["general"]
-    global model
-    model = config["model"]
-    global download
-    download = config["download"]
-    global train
-    train = config["train"]
-    global predict
-    predict = config["predict"]
-    global postprocess
-    postprocess = config["postprocess"]
-    global dirs
-    dirs = config["dirs"]
-    global files
-    files = config["files"]
-    global logging
-    logging = config["logging"]
-    global email
-    email = config["email"]
-
-    # Some checks to make sure the config is loaded properly
-    segment_subject = general.get("segment_subject")
-    if segment_subject is None or segment_subject == "MUST_OVERRIDE":
-        raise Exception(
-            "Projectconfig parameter general.segment_subject needs to be overruled to"
-            "a proper name in a specific project config file, \nwith config_filepaths "
-            f"{config_paths}"
-        )
-    elif any(
-        illegal_character in segment_subject
-        for illegal_character in illegal_chars_in_codes
-    ):
-        raise Exception(
-            f"Projectconfig parameter general.segment_subject ({segment_subject}) "
-            f"should not contain any of the following chars: {illegal_chars_in_codes}"
-        )
-
-    # If the projects_dir parameter is a relative path, resolve it towards the location
-    # of the project config file.
-    projects_dir = dirs.getpath("projects_dir")
-    if not projects_dir.is_absolute():
-        projects_dir_absolute = (config_paths[-1].parent / projects_dir).resolve()
-        logger.info(
-            f"dirs.projects_dir was relative: is resolved to {projects_dir_absolute}"
-        )
-        dirs["projects_dir"] = projects_dir_absolute.as_posix()
-
-    # Read the layer config
-    layer_config_filepath = files.getpath("image_layers_config_filepath")
-    global layer_config_filepath_used
-    layer_config_filepath_used = layer_config_filepath
-
-    global image_layers
-    image_layers = read_layer_config(layer_config_filepath=layer_config_filepath)
-
-
-def read_layer_config(layer_config_filepath: Path) -> dict:
-    # Init
-    if not layer_config_filepath.exists():
-        raise Exception(f"Layer config file not found: {layer_config_filepath}")
-
-    # Read config file...
-    layer_config = configparser.ConfigParser(
-        interpolation=configparser.ExtendedInterpolation(),
-        converters={
-            "list": lambda x: [i.strip() for i in x.split(",")],
-            "listint": lambda x: [int(i.strip()) for i in x.split(",")],
-            "dict": lambda x: None if x is None else json.loads(x),
-            "path": lambda x: Path(x),
-        },
-    )
-    layer_config.read(layer_config_filepath)
-
-    # Prepare data
-    image_layers = {}
-    for image_layer in layer_config.sections():
-        # First check if the image_layer code doesn't contain 'illegal' characters
-        if any(illegal_char in image_layer for illegal_char in illegal_chars_in_codes):
-            raise Exception(
-                f"Section name [{image_layer}] in layer config should not contain any"
-                f"of these chars: {illegal_chars_in_codes}, in {layer_config_filepath}"
-            )
-
-        # Init layer with all parameters in the section as dict
-        image_layers[image_layer] = dict(layer_config[image_layer])
-
-        # If the layer source(s) are specified in a json parameter, parse it
-        if "layersources" in image_layers[image_layer]:
-            image_layers[image_layer]["layersources"] = layer_config[
-                image_layer
-            ].getdict("layersources")
-
-            # Give default values to some optional properties of a server
-            for layersource in image_layers[image_layer]["layersources"]:
-                if "random_sleep" not in layersource:
-                    layersource["random_sleep"] = 0
-                if "wms_ignore_capabilities_url" not in layersource:
-                    layersource["wms_ignore_capabilities_url"] = False
-                if "wms_username" not in layersource:
-                    layersource["wms_username"] = None
-                if "wms_password" not in layersource:
-                    layersource["wms_password"] = None
-
-        else:
-            # If not, the layersource should be specified in seperate parameters
-            layersource = {}
-            layersource["wms_server_url"] = layer_config[image_layer].get(
-                "wms_server_url"
-            )
-            layersource["wms_version"] = layer_config[image_layer].get(
-                "wms_version", fallback="1.3.0"
-            )
-            layersource["wms_username"] = layer_config[image_layer].get(
-                "wms_username", fallback=None
-            )
-            layersource["wms_password"] = layer_config[image_layer].get(
-                "wms_password", fallback=None
-            )
-            # The layer names and layer styles are lists
-            layersource["layernames"] = layer_config[image_layer].getlist(
-                "wms_layernames"
-            )
-            layersource["layerstyles"] = layer_config[image_layer].getlist(
-                "wms_layerstyles"
-            )
-            # Some more properties
-            layersource["bands"] = layer_config[image_layer].getlist(
-                "bands", fallback=None
-            )
-            layersource["random_sleep"] = layer_config[image_layer].getint(
-                "random_sleep", fallback=0
-            )
-            layersource["wms_ignore_capabilities_url"] = layer_config[
-                image_layer
-            ].getboolean("wms_ignore_capabilities_url", fallback=False)
-            image_layers[image_layer]["layersources"] = [layersource]
-
-        # Read nb_concurrent calls param
-        image_layers[image_layer]["nb_concurrent_calls"] = layer_config[
-            image_layer
-        ].getint("nb_concurrent_calls", fallback=6)
-
-        # Check if a region of interest is specified as file or bbox
-        roi_filepath = layer_config[image_layer].getpath("roi_filepath", fallback=None)
-        image_layers[image_layer]["roi_filepath"] = roi_filepath
-        bbox_tuple = None
-        if layer_config.has_option(image_layer, "bbox"):
-            bbox_list = layer_config[image_layer].getlist("bbox")
-            bbox_tuple = (
-                float(bbox_list[0]),
-                float(bbox_list[1]),
-                float(bbox_list[2]),
-                float(bbox_list[3]),
-            )
-            image_layers[image_layer]["bbox"] = bbox_tuple
-        image_layers[image_layer]["bbox"] = bbox_tuple
-
-        # Check if the grid xmin and xmax are specified
-        grid_xmin = 0
-        if layer_config.has_option(image_layer, "grid_xmin"):
-            grid_xmin = layer_config[image_layer].getfloat("grid_xmin")
-        image_layers[image_layer]["grid_xmin"] = grid_xmin
-        grid_ymin = 0
-        if layer_config.has_option(image_layer, "grid_ymin"):
-            grid_ymin = layer_config[image_layer].getfloat("grid_ymin")
-        image_layers[image_layer]["grid_ymin"] = grid_ymin
-
-        # Check if a image_pixels_ignore_border is specified
-        image_pixels_ignore_border = layer_config[image_layer].getint(
-            "image_pixels_ignore_border", fallback=0
-        )
-        image_layers[image_layer][
-            "image_pixels_ignore_border"
-        ] = image_pixels_ignore_border
-    return image_layers
-
-
-def pformat_config():
-    message = f"Config files used: {pprint.pformat(config_filepaths_used)} \n"
-    message += f"Layer config file used: {layer_config_filepath_used} \n"
-    message += "Config info listing:\n"
-    message += pprint.pformat(config_util.as_dict(config))
-    message += "Layer config info listing:\n"
-    message += pprint.pformat(image_layers)
-    return message
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module with specific helper functions to manage the configuration of orthoseg.
+"""
+
+import configparser
+import json
+import logging
+from pathlib import Path
+import pprint
+
+from orthoseg.util import config_util
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# Define the chars that cannot be used in codes that are use in filenames.
+# Remark: '_' cannot be used because '_' is used as devider to parse filenames, and if
+# it is used in codes as well the parsing becomes a lot more difficult.
+illegal_chars_in_codes = ["_", ",", ".", "?", ":"]
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def read_orthoseg_config(config_path: Path):
+
+    # Determine list of config files that should be loaded
+    config_paths = config_util.get_config_files(config_path)  # type: ignore
+    # Load them
+    global config
+    config = config_util.read_config_ext(config_paths)
+
+    # Now do orthoseg-specific checks, inits,... on config
+    global config_filepaths_used
+    config_filepaths_used = config_paths
+
+    # Now set global variables to each section as shortcuts
+    global general
+    general = config["general"]
+    global model
+    model = config["model"]
+    global download
+    download = config["download"]
+    global train
+    train = config["train"]
+    global predict
+    predict = config["predict"]
+    global postprocess
+    postprocess = config["postprocess"]
+    global dirs
+    dirs = config["dirs"]
+    global files
+    files = config["files"]
+    global logging
+    logging = config["logging"]
+    global email
+    email = config["email"]
+
+    # Some checks to make sure the config is loaded properly
+    segment_subject = general.get("segment_subject")
+    if segment_subject is None or segment_subject == "MUST_OVERRIDE":
+        raise Exception(
+            "Projectconfig parameter general.segment_subject needs to be overruled to"
+            "a proper name in a specific project config file, \nwith config_filepaths "
+            f"{config_paths}"
+        )
+    elif any(
+        illegal_character in segment_subject
+        for illegal_character in illegal_chars_in_codes
+    ):
+        raise Exception(
+            f"Projectconfig parameter general.segment_subject ({segment_subject}) "
+            f"should not contain any of the following chars: {illegal_chars_in_codes}"
+        )
+
+    # If the projects_dir parameter is a relative path, resolve it towards the location
+    # of the project config file.
+    projects_dir = dirs.getpath("projects_dir")
+    if not projects_dir.is_absolute():
+        projects_dir_absolute = (config_paths[-1].parent / projects_dir).resolve()
+        logger.info(
+            f"dirs.projects_dir was relative: is resolved to {projects_dir_absolute}"
+        )
+        dirs["projects_dir"] = projects_dir_absolute.as_posix()
+
+    # Read the layer config
+    layer_config_filepath = files.getpath("image_layers_config_filepath")
+    global layer_config_filepath_used
+    layer_config_filepath_used = layer_config_filepath
+
+    global image_layers
+    image_layers = read_layer_config(layer_config_filepath=layer_config_filepath)
+
+
+def read_layer_config(layer_config_filepath: Path) -> dict:
+    # Init
+    if not layer_config_filepath.exists():
+        raise Exception(f"Layer config file not found: {layer_config_filepath}")
+
+    # Read config file...
+    layer_config = configparser.ConfigParser(
+        interpolation=configparser.ExtendedInterpolation(),
+        converters={
+            "list": lambda x: [i.strip() for i in x.split(",")],
+            "listint": lambda x: [int(i.strip()) for i in x.split(",")],
+            "dict": lambda x: None if x is None else json.loads(x),
+            "path": lambda x: Path(x),
+        },
+    )
+    layer_config.read(layer_config_filepath)
+
+    # Prepare data
+    image_layers = {}
+    for image_layer in layer_config.sections():
+        # First check if the image_layer code doesn't contain 'illegal' characters
+        if any(illegal_char in image_layer for illegal_char in illegal_chars_in_codes):
+            raise Exception(
+                f"Section name [{image_layer}] in layer config should not contain any"
+                f"of these chars: {illegal_chars_in_codes}, in {layer_config_filepath}"
+            )
+
+        # Init layer with all parameters in the section as dict
+        image_layers[image_layer] = dict(layer_config[image_layer])
+
+        # If the layer source(s) are specified in a json parameter, parse it
+        if "layersources" in image_layers[image_layer]:
+            image_layers[image_layer]["layersources"] = layer_config[
+                image_layer
+            ].getdict("layersources")
+
+            # Give default values to some optional properties of a server
+            for layersource in image_layers[image_layer]["layersources"]:
+                if "random_sleep" not in layersource:
+                    layersource["random_sleep"] = 0
+                if "wms_ignore_capabilities_url" not in layersource:
+                    layersource["wms_ignore_capabilities_url"] = False
+                if "wms_username" not in layersource:
+                    layersource["wms_username"] = None
+                if "wms_password" not in layersource:
+                    layersource["wms_password"] = None
+
+        else:
+            # If not, the layersource should be specified in seperate parameters
+            layersource = {}
+            layersource["wms_server_url"] = layer_config[image_layer].get(
+                "wms_server_url"
+            )
+            layersource["wms_version"] = layer_config[image_layer].get(
+                "wms_version", fallback="1.3.0"
+            )
+            layersource["wms_username"] = layer_config[image_layer].get(
+                "wms_username", fallback=None
+            )
+            layersource["wms_password"] = layer_config[image_layer].get(
+                "wms_password", fallback=None
+            )
+            # The layer names and layer styles are lists
+            layersource["layernames"] = layer_config[image_layer].getlist(
+                "wms_layernames"
+            )
+            layersource["layerstyles"] = layer_config[image_layer].getlist(
+                "wms_layerstyles"
+            )
+            # Some more properties
+            layersource["bands"] = layer_config[image_layer].getlist(
+                "bands", fallback=None
+            )
+            layersource["random_sleep"] = layer_config[image_layer].getint(
+                "random_sleep", fallback=0
+            )
+            layersource["wms_ignore_capabilities_url"] = layer_config[
+                image_layer
+            ].getboolean("wms_ignore_capabilities_url", fallback=False)
+            image_layers[image_layer]["layersources"] = [layersource]
+
+        # Read nb_concurrent calls param
+        image_layers[image_layer]["nb_concurrent_calls"] = layer_config[
+            image_layer
+        ].getint("nb_concurrent_calls", fallback=6)
+
+        # Check if a region of interest is specified as file or bbox
+        roi_filepath = layer_config[image_layer].getpath("roi_filepath", fallback=None)
+        image_layers[image_layer]["roi_filepath"] = roi_filepath
+        bbox_tuple = None
+        if layer_config.has_option(image_layer, "bbox"):
+            bbox_list = layer_config[image_layer].getlist("bbox")
+            bbox_tuple = (
+                float(bbox_list[0]),
+                float(bbox_list[1]),
+                float(bbox_list[2]),
+                float(bbox_list[3]),
+            )
+            image_layers[image_layer]["bbox"] = bbox_tuple
+        image_layers[image_layer]["bbox"] = bbox_tuple
+
+        # Check if the grid xmin and xmax are specified
+        grid_xmin = 0
+        if layer_config.has_option(image_layer, "grid_xmin"):
+            grid_xmin = layer_config[image_layer].getfloat("grid_xmin")
+        image_layers[image_layer]["grid_xmin"] = grid_xmin
+        grid_ymin = 0
+        if layer_config.has_option(image_layer, "grid_ymin"):
+            grid_ymin = layer_config[image_layer].getfloat("grid_ymin")
+        image_layers[image_layer]["grid_ymin"] = grid_ymin
+
+        # Check if a image_pixels_ignore_border is specified
+        image_pixels_ignore_border = layer_config[image_layer].getint(
+            "image_pixels_ignore_border", fallback=0
+        )
+        image_layers[image_layer][
+            "image_pixels_ignore_border"
+        ] = image_pixels_ignore_border
+    return image_layers
+
+
+def pformat_config():
+    message = f"Config files used: {pprint.pformat(config_filepaths_used)} \n"
+    message += f"Layer config file used: {layer_config_filepath_used} \n"
+    message += "Config info listing:\n"
+    message += pprint.pformat(config_util.as_dict(config))
+    message += "Layer config info listing:\n"
+    message += pprint.pformat(image_layers)
+    return message
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    raise Exception("Not implemented")
```

### Comparing `orthoseg-0.4.2/orthoseg/helpers/vectorfile_helper.py` & `orthoseg-0.4.2a1/orthoseg/helpers/vectorfile_helper.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# -*- coding: utf-8 -*-
-"""
-Modile with generic Utility functions for vectorfile manipulations.
-"""
-
-import logging
-from pathlib import Path
-
-import geofileops as gfo
-
-from orthoseg.util import vector_util
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def reclassify_neighbours(
-    input_path: Path,
-    reclassify_column: str,
-    query: str,
-    output_path: Path,
-    class_background: str = "background",
-    force: bool = False,
-):
-    """
-    For features that comply to the query, if they have a neighbour (touch/overlap),
-    change their classname to that of the neighbour with the longest intersection and
-    dissolve to merge them.
-
-    The query should follow the syntax of pandas.query queries and can us the following
-    fields:
-        - area (float): the area of the geometry.
-        - perimeter (float): the perimeter of the geometry.
-
-    Args:
-        gdf (gpd.GeoDataFrame): input
-        reclassify_column (str): column to reclassify.
-        query (str): th query to find the features to reclassify.
-        class_background (str, optional): the classname to treat as background.
-            Defaults to "background".
-        force (bool, optional): True to force calculation even if output file exists.
-            Defaults to False.
-
-    Raises:
-        ValueError: raised if incompatible parameters are passed.
-    """
-    if output_path.exists():
-        if not force:
-            logger.info(
-                f"reclassify_neighbours: return as output_path exists: {output_path}"
-            )
-            return
-        gfo.remove(output_path)
-
-    logger.info(f"reclassify_neighbours on {input_path} to {output_path}")
-    input_gdf = gfo.read_file(input_path, columns=[reclassify_column])
-    output_gdf = vector_util.reclassify_neighbours(
-        input_gdf,
-        reclassify_column=reclassify_column,
-        query=query,
-        border_bounds=None,
-        class_background=class_background,
-    )
-    gfo.to_file(output_gdf, output_path)
-
-    # Add/recalculate columns with area and nbcoords
-    gfo.add_column(
-        path=output_path,
-        name="area",
-        type=gfo.DataType.REAL,
-        expression="ST_Area(geom)",
-        force_update=True,
-    )
-    gfo.add_column(
-        path=output_path,
-        name="nbcoords",
-        type=gfo.DataType.INTEGER,
-        expression="ST_NPoints(geom)",
-        force_update=True,
-    )
+# -*- coding: utf-8 -*-
+"""
+Modile with generic Utility functions for vectorfile manipulations.
+"""
+
+import logging
+from pathlib import Path
+
+import geofileops as gfo
+
+from orthoseg.util import vector_util
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def reclassify_neighbours(
+    input_path: Path,
+    reclassify_column: str,
+    query: str,
+    output_path: Path,
+    class_background: str = "background",
+    force: bool = False,
+):
+    """
+    For features that comply to the query, if they have a neighbour (touch/overlap),
+    change their classname to that of the neighbour with the longest intersection and
+    dissolve to merge them.
+
+    The query should follow the syntax of pandas.query queries and can us the following
+    fields:
+        - area (float): the area of the geometry.
+        - perimeter (float): the perimeter of the geometry.
+
+    Args:
+        gdf (gpd.GeoDataFrame): input
+        reclassify_column (str): column to reclassify.
+        query (str): th query to find the features to reclassify.
+        class_background (str, optional): the classname to treat as background.
+            Defaults to "background".
+        force (bool, optional): True to force calculation even if output file exists.
+            Defaults to False.
+
+    Raises:
+        ValueError: raised if incompatible parameters are passed.
+    """
+    if output_path.exists():
+        if not force:
+            logger.info(
+                f"reclassify_neighbours: return as output_path exists: {output_path}"
+            )
+            return
+        gfo.remove(output_path)
+
+    logger.info(f"reclassify_neighbours on {input_path} to {output_path}")
+    input_gdf = gfo.read_file(input_path, columns=[reclassify_column])
+    output_gdf = vector_util.reclassify_neighbours(
+        input_gdf,
+        reclassify_column=reclassify_column,
+        query=query,
+        border_bounds=None,
+        class_background=class_background,
+    )
+    gfo.to_file(output_gdf, output_path)
+
+    # Add/recalculate columns with area and nbcoords
+    gfo.add_column(
+        path=output_path,
+        name="area",
+        type=gfo.DataType.REAL,
+        expression="ST_Area(geom)",
+        force_update=True,
+    )
+    gfo.add_column(
+        path=output_path,
+        name="nbcoords",
+        type=gfo.DataType.INTEGER,
+        expression="ST_NPoints(geom)",
+        force_update=True,
+    )
```

### Comparing `orthoseg-0.4.2/orthoseg/lib/predicter.py` & `orthoseg-0.4.2a1/orthoseg/lib/predicter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,621 +1,621 @@
-# -*- coding: utf-8 -*-
-"""
-Module with high-level operations to segment images.
-"""
-
-from concurrent import futures
-import csv
-import datetime
-import json
-import logging
-import multiprocessing
-from pathlib import Path
-import shutil
-import tempfile
-import time
-import traceback
-from typing import List, Optional
-
-import geofileops as gfo
-import numpy as np
-import pandas as pd
-import rasterio as rio
-import rasterio.crs as rio_crs
-import rasterio.plot as rio_plot
-import tensorflow as tf
-import keras.models
-
-import orthoseg.lib.postprocess_predictions as postp
-from orthoseg.util.progress_util import ProgressLogger
-from orthoseg.util import general_util
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def predict_dir(
-    model: keras.models.Model,
-    input_image_dir: Path,
-    output_image_dir: Path,
-    output_vector_path: Optional[Path],
-    classes: list,
-    min_probability: float = 0.5,
-    postprocess: dict = {},
-    border_pixels_to_ignore: int = 0,
-    projection_if_missing: Optional[str] = None,
-    input_mask_dir: Optional[Path] = None,
-    batch_size: int = 16,
-    evaluate_mode: bool = False,
-    cancel_filepath: Optional[Path] = None,
-    nb_parallel_postprocess: int = 1,
-    max_prediction_errors: int = 100,
-    force: bool = False,
-):
-    """
-    Create a prediction for all the images in the directories specified
-    using the model specified.
-
-    If evaluate_mode is False, the output folder(s) will contain:
-        * the "raw" prediction for every image (if there are white pixels)
-        * a geojson with the vectorized prediction, with a column "onborder"
-          for each feature that is 1 if the feature is on the border of the
-          tile, taking the border_pixels_to_ignore in account if applicable.
-          This columns can be used to speed up union operations afterwards,
-          because only features on the border of tiles need to be unioned.
-
-    If evaluate_mode is True, the results will all be put in the root of the
-    output folder, and the following files will be outputted:
-        * the original image
-        * the mask that was provided, if available
-        * the "raw" prediction
-        * a "cleaned" version of the prediction
-    The files will in this case be prefixed with a number so they are ordered
-    in a way that is interesting for evaluation. If a mask was available, this
-    prefix will be the % overlap of the mask and the prediction. If no mask is
-    available, the prefix is the % white pixels in the prediction.
-
-    Args
-        input_image_dir (Pathlike): dir where the input images are located
-        output_base_dir (Pathlike): dir where the output will be put
-        output_vector_path (Pathlike): the path to write the vector output to
-        classes (list): a list of the different class names. Mandatory
-            if more than background + 1 class.
-        postprocess (dict, optional): specifies which postprocessing should be applied
-            to the prediction. Default is {}, so no postprocessing.
-        border_pixels_to_ignore: because the segmentation at the borders of the
-            input images images is not as good, you can specify that x
-            pixels need to be ignored
-        input_mask_dir: optional dir where the mask images are located
-        projection_if_missing: Normally the projection should be in the raster file. If
-            it is not, you can explicitly specify one.
-        batch_size: batch size to use while predicting. This must be choosen
-            depending on the neural network architecture and available
-            memory on you GPU.
-        evaluate_mode: True to run in evaluate mode
-        cancel_filepath: If the file in this path exists, processing stops asap
-        nb_parallel_postprocess (int, optional): The number of parallel
-            processes used to vectorize,... the predictions. If -1, all
-            available CPU's are used. Defaults to 1.
-        max_prediction_errors (int, optional): the maximum number of errors that is
-            tolerated before stopping prediction. If -1, no limit. Defaults to 100.
-        force: False to skip images that already have a prediction, true to
-            ignore existing predictions and overwrite them
-    """
-
-    # Init
-    if not input_image_dir.exists():
-        logger.warning(f"input_image_dir doesn't exist, so return: {input_image_dir}")
-        return
-    if output_vector_path is not None and output_vector_path.exists():
-        logger.warning(f"output file exists already, so return: {output_vector_path}")
-        return
-    tmp_dir = Path(tempfile.gettempdir()) / Path(__file__).stem
-
-    logger.info(f"Start predict for input_image_dir: {input_image_dir}")
-
-    # Eager and not eager prediction seems +- the same performance-wise
-    # model.run_eagerly = False
-
-    # If we are using evaluate mode, change the output dir...
-    if evaluate_mode:
-        output_image_dir = Path(str(output_image_dir) + "_eval")
-
-    # Create the output dir's if they don't exist yet...
-    for dir in [output_image_dir, tmp_dir]:
-        if not dir.exists():
-            dir.mkdir()
-
-    # Write prediction config used, so it can be used for postprocessing
-    prediction_config_path = output_image_dir / "prediction_config.json"
-    with open(prediction_config_path, "w") as pred_conf_file:
-        pred_conf = {}
-        pred_conf["border_pixels_to_ignore"] = border_pixels_to_ignore
-        pred_conf["classes"] = classes
-        json.dump(pred_conf, pred_conf_file)
-
-    # Get list of all image files to process and to skip
-    image_filepaths: List[Path] = []
-    input_ext = [".png", ".tif", ".jpg"]
-    for input_ext_cur in input_ext:
-        image_filepaths.extend(input_image_dir.rglob("*" + input_ext_cur))
-    image_filepaths = sorted(image_filepaths)
-    nb_images = len(image_filepaths)
-    logger.info(
-        f"Found {nb_images} {input_ext} images to predict on in {input_image_dir}"
-    )
-
-    # If force is false, get list of all existing predictions
-    # Getting the list once is way faster than checking file per file later on!
-    images_done_log_filepath = output_image_dir / "images_done.txt"
-    image_done_filenames = set()
-    if force is False:
-        # First read the listing files if they exists
-        if images_done_log_filepath.exists():
-            with images_done_log_filepath.open() as f:
-                for filename in f:
-                    image_done_filenames.add(filename.rstrip())
-        if len(image_done_filenames) > 0:
-            logger.info(
-                f"{len(image_done_filenames)} images in were processed before, "
-                f"they will be skipped"
-            )
-
-    # Clear error file
-    images_error_log_filepath = output_image_dir / "images_error.csv"
-    images_error_log_filepath.unlink(missing_ok=True)
-
-    # Write output to tmp files, so we know if the process completed correctly or not
-    pred_tmp_output_path = None
-    if output_vector_path is not None:
-        pred_tmp_output_path = output_image_dir / f"{output_vector_path.stem}_tmp.gpkg"
-        pred_tmp_output_lock_path = Path(f"{str(pred_tmp_output_path)}.lock")
-        # if lock file exists, remove it:
-        if pred_tmp_output_lock_path.exists():
-            pred_tmp_output_lock_path.unlink()
-
-    # Loop through all files to process them
-    nb_parallel_read = batch_size * 6
-    if nb_parallel_postprocess == -1:
-        nb_parallel_postprocess = multiprocessing.cpu_count()
-    predict_images = []
-    nb_to_process = nb_images
-    nb_processed = 0
-    nb_errors = 0
-    read_sleep_logged = False
-    progress = None
-    postp_future_to_input_path = {}
-    read_future_to_input_path = {}
-    image_id = -1
-    last_image_reached = False
-
-    # We don't want the postprocess workers to block the entire system,
-    # so make them a bit nicer
-    def init_postprocess_worker():
-        general_util.setprocessnice(15)
-
-    with futures.ThreadPoolExecutor(
-        nb_parallel_read
-    ) as read_pool, futures.ProcessPoolExecutor(
-        nb_parallel_postprocess, initializer=init_postprocess_worker()
-    ) as postprocess_pool:
-
-        # Start looping.
-        # If ready to stop, the code below will break
-        perf_time_start = datetime.datetime.now()
-        while True:
-
-            # If we are ready, stop!
-            if (
-                last_image_reached is True
-                and len(read_future_to_input_path) == 0
-                and len(postp_future_to_input_path) == 0
-            ):
-                break
-
-            # If the cancel file exists, stop processing...
-            if cancel_filepath is not None and cancel_filepath.exists():
-                print()
-                logger.info(f"Cancel file found, so stop: {cancel_filepath}")
-                break
-
-            # Get the next filepath to be processed
-            image_filepath = None
-            if image_id < (len(image_filepaths) - 1):
-                image_id += 1
-                image_filepath = image_filepaths[image_id]
-
-                # Check if the image has been processed already
-                if force is False and image_filepath.name in image_done_filenames:
-                    logger.debug(
-                        "Predict for image has already been done before and force is "
-                        f"False, so skip: {image_filepath.name}"
-                    )
-                    nb_to_process -= 1
-                    continue
-
-                nb_processed += 1
-
-                # Schedule file to be read
-                read_future = read_pool.submit(
-                    read_image,  # Function
-                    image_filepath,  # Arg 1
-                    projection_if_missing,
-                )  # Arg 2)
-                read_future_to_input_path[read_future] = image_filepath
-            else:
-                last_image_reached = True
-
-            # Prepare batch_size images that have been read for prediction
-            while (
-                len(read_future_to_input_path) > 0 and len(predict_images) < batch_size
-            ):
-
-                # If the read pool is not full, first schedule extra reads
-                if (
-                    last_image_reached is False
-                    and len(read_future_to_input_path) < nb_parallel_read
-                ):
-                    break
-
-                # Prepare the images that have been read for predicting
-                futures_done = [
-                    future
-                    for future in read_future_to_input_path
-                    if future.done() is True
-                ]
-                for future in futures_done:
-
-                    # Prediction can only handle batch_size images
-                    if len(predict_images) >= batch_size:
-                        break
-
-                    try:
-                        # Get the result from the read
-                        read_result = future.result()
-                        image_filepath_read = read_result["image_filepath"]
-
-                        # Prepare the filepath for the output
-                        output_suffix = ".tif"
-                        if evaluate_mode:
-                            # In evaluate mode, put everyting in output base dir for
-                            # easier comparison
-                            output_image_pred_dir = output_image_dir
-
-                            # Prepare complete filepath for image prediction
-                            output_image_pred_path = (
-                                output_image_dir / image_filepath_read.stem
-                            )
-                        else:
-                            # If saving predictions to images for real, keep hierarchic
-                            # structure if present
-                            tmp_output_filepath = Path(
-                                str(image_filepath_read).replace(
-                                    str(input_image_dir), str(output_image_dir)
-                                )
-                            )
-                            output_image_pred_dir = tmp_output_filepath.parent
-                            output_image_pred_path = (
-                                output_image_pred_dir
-                                / f"{image_filepath_read.stem}_pred{output_suffix}"
-                            )
-
-                        predict_images.append(
-                            {
-                                "input_image_filepath": image_filepath_read,
-                                "output_pred_filepath": output_image_pred_path,
-                                "output_image_pred_dir": output_image_pred_dir,
-                                "image_crs": read_result["image_crs"],
-                                "image_transform": read_result["image_transform"],
-                                "image_data": read_result["image_data"],
-                            }
-                        )
-
-                    finally:
-                        # Remove from queue...
-                        del read_future_to_input_path[future]
-
-                # If not at last image + not enough images yet for predict + read
-                # queue is full, sleep
-                if (
-                    last_image_reached is False
-                    and len(predict_images) < batch_size
-                    and len(read_future_to_input_path) >= nb_parallel_read
-                ):
-                    if read_sleep_logged is False:
-                        logger.info("Wait for images to be read")
-                        read_sleep_logged = True
-                    time.sleep(0.01)
-
-            # If batch_size images are ready for prediction or we are at
-            # the last images: predict
-            if len(predict_images) == batch_size or (
-                last_image_reached is True and len(predict_images) > 0
-            ):
-                read_sleep_logged = False
-                perf_time_now = datetime.datetime.now()
-                perfinfo = f"waiting for read took {perf_time_now-perf_time_start}"
-                perf_time_start = perf_time_now
-
-                # Predict!
-                logger.debug(f"Start prediction for {len(predict_images)} images")
-                perf_time_start = datetime.datetime.now()
-                curr_batch_image_list = [
-                    curr_batch_image_info["image_data"]
-                    for curr_batch_image_info in predict_images
-                ]
-                curr_batch_image_arr = np.stack(curr_batch_image_list)
-                curr_batch_image_pred_arr = model.predict_on_batch(curr_batch_image_arr)
-
-                perf_time_now = datetime.datetime.now()
-                perfinfo += f", predict took {perf_time_now-perf_time_start}"
-                perf_time_start = perf_time_now
-
-                # In tf > 2.1 a tf.tensor object is returned, but we want an ndarray
-                if type(curr_batch_image_pred_arr) is tf.Tensor:
-                    curr_batch_image_pred_arr = np.array(
-                        curr_batch_image_pred_arr.numpy()  # type: ignore
-                    )
-                else:
-                    curr_batch_image_pred_arr = np.array(curr_batch_image_pred_arr)
-
-                # Save predictions
-                # Remark: trying to parallelize this doesn't seem to help at all!
-                logger.debug("Start post-processing")
-                for batch_image_id, image_info in enumerate(predict_images):
-                    try:
-                        # If not in evaluate mode... save to vector in background
-                        if (
-                            evaluate_mode is False
-                            and output_vector_path is not None
-                            and pred_tmp_output_path is not None
-                        ):
-                            # Prepare prediction array...
-                            #   - convert to uint8 to reduce pickle size/time
-                            image_pred_arr_uint8 = (
-                                (curr_batch_image_pred_arr[batch_image_id, :, :, :])
-                                * 255
-                            ).astype(np.uint8)
-                            future = postprocess_pool.submit(
-                                postp.polygonize_pred_multiclass_to_file,
-                                image_pred_arr_uint8,
-                                image_info["image_crs"],
-                                image_info["image_transform"],
-                                classes,
-                                pred_tmp_output_path,
-                                min_probability,
-                                postprocess,
-                                border_pixels_to_ignore,
-                            )
-                            postp_future_to_input_path[future] = image_info[
-                                "input_image_filepath"
-                            ]
-
-                        else:
-                            # Saving the predictions as images at the moment only used
-                            # for evaluate mode...
-                            # TODO: would ideally be moved to the background
-                            # processing as well to simplify code here...
-                            postp.clean_and_save_prediction(
-                                image_image_filepath=image_info["input_image_filepath"],
-                                image_crs=image_info["image_crs"],
-                                image_transform=image_info["image_transform"],
-                                image_pred_arr=curr_batch_image_pred_arr[
-                                    batch_image_id
-                                ],
-                                output_dir=image_info["output_image_pred_dir"],
-                                input_image_dir=input_image_dir,
-                                input_mask_dir=input_mask_dir,
-                                border_pixels_to_ignore=border_pixels_to_ignore,
-                                min_probability=min_probability,
-                                evaluate_mode=evaluate_mode,
-                                classes=classes,
-                                force=force,
-                            )
-
-                            # Write filepath to file with files that are done
-                            with images_done_log_filepath.open(
-                                "a+"
-                            ) as image_donelog_file:
-                                image_donelog_file.write(
-                                    f"{image_info['input_image_filepath'].name}\n"
-                                )
-                    except Exception as ex:
-                        nb_errors += 1
-                        image_path = image_info["input_image_filepath"]
-                        _handle_error(image_path, ex, images_error_log_filepath)
-
-                perf_time_now = datetime.datetime.now()
-                perfinfo += (
-                    f", scheduling postprocessings took {perf_time_now-perf_time_start}"
-                )
-                perf_time_start = perf_time_now
-
-                # Poll for completed postprocessings
-                postp_sleep_logged = False
-                while len(postp_future_to_input_path) > 0:
-
-                    # If not at last file, get results from all futures that are
-                    # done, if at last file, wait till all are done
-                    if last_image_reached is False:
-                        futures_done = [
-                            future
-                            for future in postp_future_to_input_path
-                            if future.done() is True
-                        ]
-                    else:
-                        logger.info("Wait for last batch")
-                        futures_done = futures.wait(postp_future_to_input_path).done
-                    for future in futures_done:
-                        # Get the result from the polygonization
-                        try:
-                            # Get the result (= exception when something went wrong)
-                            result = future.result()
-                            logger.debug(
-                                f"result for {postp_future_to_input_path[future].name}:"
-                                f" {result}"
-                            )
-
-                            # Write filepath to file with files that are done
-                            with images_done_log_filepath.open(
-                                "a+"
-                            ) as image_donelog_file:
-                                image_donelog_file.write(
-                                    postp_future_to_input_path[future].name + "\n"
-                                )
-                        except Exception as ex:
-                            nb_errors += 1
-                            image_path = postp_future_to_input_path[future]
-                            _handle_error(image_path, ex, images_error_log_filepath)
-
-                        finally:
-                            # Remove from queue...
-                            del postp_future_to_input_path[future]
-
-                    # Wait till number below thresshold to evade huge waiting
-                    # list (and memory issues)
-                    if len(postp_future_to_input_path) > nb_parallel_postprocess * 2:
-                        if postp_sleep_logged is False:
-                            logger.info(
-                                "Postprocessing takes longer than prediction, so wait"
-                            )
-                            postp_sleep_logged = True
-                        time.sleep(0.01)
-                    else:
-                        # No need to wait (anymore)...
-                        if postp_sleep_logged is True:
-                            logger.info(
-                                "Waited enough for postprocessing to catch up..."
-                            )
-
-                        perf_time_now = datetime.datetime.now()
-                        perfinfo += (
-                            f", after postproces: took {perf_time_now-perf_time_start}"
-                        )
-                        perf_time_start = perf_time_now
-                        break
-
-                # Reset variable for next batch
-                predict_images = []
-
-                # Log the progress and prediction speed
-                if len(perfinfo) > 0:
-                    logger.debug(perfinfo)
-                if progress is not None:
-                    progress.step(nb_steps=batch_size)
-                # Init progress only when some imags were already processed, as the
-                # first are very slow.
-                if progress is None and nb_processed > 0:
-                    progress = ProgressLogger(
-                        message=f"predict to {output_image_dir.parent.name}/{output_image_dir.name}",  # noqa: E501
-                        nb_steps_total=nb_to_process,
-                        nb_steps_done=batch_size,
-                    )
-
-                # If max number errors reached, stop processings
-                if max_prediction_errors >= 0 and nb_errors >= max_prediction_errors:
-                    break
-
-        # If errors occured, raise error
-        if images_error_log_filepath.exists():
-            errors = pd.read_csv(
-                images_error_log_filepath,
-                usecols=["filename", "error"]
-                # ).to_string(justify="left", index=False)
-            ).to_html(justify="left", index=False)
-            raise Exception(f"Error(s) occured while predicting:\n{errors}")
-
-        # If alle images were processed, rename to real output file + cleanup
-        if (
-            last_image_reached is True
-            and output_vector_path is not None
-            and pred_tmp_output_path is not None
-            and pred_tmp_output_path.exists()
-        ):
-            output_vector_path.parent.mkdir(parents=True, exist_ok=True)
-            gfo.move(pred_tmp_output_path, output_vector_path)
-            gfo.rename_layer(output_vector_path, output_vector_path.stem)
-            shutil.rmtree(output_image_dir)
-
-
-def _handle_error(image_path: Path, ex: Exception, log_path: Path):
-    # Print exception + trace
-    exception_trace = traceback.format_exc()
-    exception_trace_print = exception_trace.replace("\n", "\n\t")
-    logger.error(f"Error postprocessing pred for {image_path}: {exception_trace_print}")
-
-    # Write error to error log file
-    first_error = False
-    if not log_path.exists():
-        first_error = True
-    with log_path.open("a+") as log_file:
-        if first_error:
-            log_file.write("filename,error,traceback\n")
-        writer = csv.writer(log_file)
-        exception_trace_csv = exception_trace.replace("\n", "\\n")
-        fields = [image_path.name, ex, exception_trace_csv]
-        writer.writerow(fields)
-
-
-def read_image(
-    image_filepath: Path, projection_if_missing: Optional[str] = None
-) -> dict:
-
-    # Read input file
-    # Because sometimes a read seems to fail, retry up to 3 times...
-    retry_count = 0
-    while True:
-        try:
-            with rio.open(str(image_filepath)) as image_ds:
-                # Read geo info
-                image_crs = image_ds.profile["crs"]
-                image_transform = image_ds.transform
-
-                # Read pixels + change from (channels, width, height) to
-                # (width, height, channels) + normalize to between 0 and 1
-                image_data = image_ds.read()
-                image_data = rio_plot.reshape_as_image(image_data)
-                image_data = image_data / 255.0
-
-            # Read worked, so jump out of the loop...
-            break
-        except Exception as ex:
-            retry_count += 1
-            logger.warning(f"Read failed, retry nb {retry_count} for {image_filepath}")
-            if retry_count >= 3:
-                message = f"Read failed {retry_count} times for {image_filepath}: {ex}"
-                logger.error(message)
-                raise Exception(message)
-
-    # The read was successfull, now check if there was a projection in the
-    # file and/or if one was provided
-    if image_crs is None:
-        if projection_if_missing is not None:
-            image_crs = rio_crs.CRS.from_string(projection_if_missing)
-        else:
-            message = (
-                f"Image has no proj and projection_if_missing is None: {image_filepath}"
-            )
-            logger.error(message)
-            raise Exception(message)
-
-    # Now return the result
-    result = {
-        "image_data": image_data,
-        "image_crs": image_crs,
-        "image_transform": image_transform,
-        "image_filepath": image_filepath,
-    }
-    return result
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module with high-level operations to segment images.
+"""
+
+from concurrent import futures
+import csv
+import datetime
+import json
+import logging
+import multiprocessing
+from pathlib import Path
+import shutil
+import tempfile
+import time
+import traceback
+from typing import List, Optional
+
+import geofileops as gfo
+import numpy as np
+import pandas as pd
+import rasterio as rio
+import rasterio.crs as rio_crs
+import rasterio.plot as rio_plot
+import tensorflow as tf
+import keras.models
+
+import orthoseg.lib.postprocess_predictions as postp
+from orthoseg.util.progress_util import ProgressLogger
+from orthoseg.util import general_util
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def predict_dir(
+    model: keras.models.Model,
+    input_image_dir: Path,
+    output_image_dir: Path,
+    output_vector_path: Optional[Path],
+    classes: list,
+    min_probability: float = 0.5,
+    postprocess: dict = {},
+    border_pixels_to_ignore: int = 0,
+    projection_if_missing: Optional[str] = None,
+    input_mask_dir: Optional[Path] = None,
+    batch_size: int = 16,
+    evaluate_mode: bool = False,
+    cancel_filepath: Optional[Path] = None,
+    nb_parallel_postprocess: int = 1,
+    max_prediction_errors: int = 100,
+    force: bool = False,
+):
+    """
+    Create a prediction for all the images in the directories specified
+    using the model specified.
+
+    If evaluate_mode is False, the output folder(s) will contain:
+        * the "raw" prediction for every image (if there are white pixels)
+        * a geojson with the vectorized prediction, with a column "onborder"
+          for each feature that is 1 if the feature is on the border of the
+          tile, taking the border_pixels_to_ignore in account if applicable.
+          This columns can be used to speed up union operations afterwards,
+          because only features on the border of tiles need to be unioned.
+
+    If evaluate_mode is True, the results will all be put in the root of the
+    output folder, and the following files will be outputted:
+        * the original image
+        * the mask that was provided, if available
+        * the "raw" prediction
+        * a "cleaned" version of the prediction
+    The files will in this case be prefixed with a number so they are ordered
+    in a way that is interesting for evaluation. If a mask was available, this
+    prefix will be the % overlap of the mask and the prediction. If no mask is
+    available, the prefix is the % white pixels in the prediction.
+
+    Args
+        input_image_dir (Pathlike): dir where the input images are located
+        output_base_dir (Pathlike): dir where the output will be put
+        output_vector_path (Pathlike): the path to write the vector output to
+        classes (list): a list of the different class names. Mandatory
+            if more than background + 1 class.
+        postprocess (dict, optional): specifies which postprocessing should be applied
+            to the prediction. Default is {}, so no postprocessing.
+        border_pixels_to_ignore: because the segmentation at the borders of the
+            input images images is not as good, you can specify that x
+            pixels need to be ignored
+        input_mask_dir: optional dir where the mask images are located
+        projection_if_missing: Normally the projection should be in the raster file. If
+            it is not, you can explicitly specify one.
+        batch_size: batch size to use while predicting. This must be choosen
+            depending on the neural network architecture and available
+            memory on you GPU.
+        evaluate_mode: True to run in evaluate mode
+        cancel_filepath: If the file in this path exists, processing stops asap
+        nb_parallel_postprocess (int, optional): The number of parallel
+            processes used to vectorize,... the predictions. If -1, all
+            available CPU's are used. Defaults to 1.
+        max_prediction_errors (int, optional): the maximum number of errors that is
+            tolerated before stopping prediction. If -1, no limit. Defaults to 100.
+        force: False to skip images that already have a prediction, true to
+            ignore existing predictions and overwrite them
+    """
+
+    # Init
+    if not input_image_dir.exists():
+        logger.warning(f"input_image_dir doesn't exist, so return: {input_image_dir}")
+        return
+    if output_vector_path is not None and output_vector_path.exists():
+        logger.warning(f"output file exists already, so return: {output_vector_path}")
+        return
+    tmp_dir = Path(tempfile.gettempdir()) / Path(__file__).stem
+
+    logger.info(f"Start predict for input_image_dir: {input_image_dir}")
+
+    # Eager and not eager prediction seems +- the same performance-wise
+    # model.run_eagerly = False
+
+    # If we are using evaluate mode, change the output dir...
+    if evaluate_mode:
+        output_image_dir = Path(str(output_image_dir) + "_eval")
+
+    # Create the output dir's if they don't exist yet...
+    for dir in [output_image_dir, tmp_dir]:
+        if not dir.exists():
+            dir.mkdir()
+
+    # Write prediction config used, so it can be used for postprocessing
+    prediction_config_path = output_image_dir / "prediction_config.json"
+    with open(prediction_config_path, "w") as pred_conf_file:
+        pred_conf = {}
+        pred_conf["border_pixels_to_ignore"] = border_pixels_to_ignore
+        pred_conf["classes"] = classes
+        json.dump(pred_conf, pred_conf_file)
+
+    # Get list of all image files to process and to skip
+    image_filepaths: List[Path] = []
+    input_ext = [".png", ".tif", ".jpg"]
+    for input_ext_cur in input_ext:
+        image_filepaths.extend(input_image_dir.rglob("*" + input_ext_cur))
+    image_filepaths = sorted(image_filepaths)
+    nb_images = len(image_filepaths)
+    logger.info(
+        f"Found {nb_images} {input_ext} images to predict on in {input_image_dir}"
+    )
+
+    # If force is false, get list of all existing predictions
+    # Getting the list once is way faster than checking file per file later on!
+    images_done_log_filepath = output_image_dir / "images_done.txt"
+    image_done_filenames = set()
+    if force is False:
+        # First read the listing files if they exists
+        if images_done_log_filepath.exists():
+            with images_done_log_filepath.open() as f:
+                for filename in f:
+                    image_done_filenames.add(filename.rstrip())
+        if len(image_done_filenames) > 0:
+            logger.info(
+                f"{len(image_done_filenames)} images in were processed before, "
+                f"they will be skipped"
+            )
+
+    # Clear error file
+    images_error_log_filepath = output_image_dir / "images_error.csv"
+    images_error_log_filepath.unlink(missing_ok=True)
+
+    # Write output to tmp files, so we know if the process completed correctly or not
+    pred_tmp_output_path = None
+    if output_vector_path is not None:
+        pred_tmp_output_path = output_image_dir / f"{output_vector_path.stem}_tmp.gpkg"
+        pred_tmp_output_lock_path = Path(f"{str(pred_tmp_output_path)}.lock")
+        # if lock file exists, remove it:
+        if pred_tmp_output_lock_path.exists():
+            pred_tmp_output_lock_path.unlink()
+
+    # Loop through all files to process them
+    nb_parallel_read = batch_size * 6
+    if nb_parallel_postprocess == -1:
+        nb_parallel_postprocess = multiprocessing.cpu_count()
+    predict_images = []
+    nb_to_process = nb_images
+    nb_processed = 0
+    nb_errors = 0
+    read_sleep_logged = False
+    progress = None
+    postp_future_to_input_path = {}
+    read_future_to_input_path = {}
+    image_id = -1
+    last_image_reached = False
+
+    # We don't want the postprocess workers to block the entire system,
+    # so make them a bit nicer
+    def init_postprocess_worker():
+        general_util.setprocessnice(15)
+
+    with futures.ThreadPoolExecutor(
+        nb_parallel_read
+    ) as read_pool, futures.ProcessPoolExecutor(
+        nb_parallel_postprocess, initializer=init_postprocess_worker()
+    ) as postprocess_pool:
+
+        # Start looping.
+        # If ready to stop, the code below will break
+        perf_time_start = datetime.datetime.now()
+        while True:
+
+            # If we are ready, stop!
+            if (
+                last_image_reached is True
+                and len(read_future_to_input_path) == 0
+                and len(postp_future_to_input_path) == 0
+            ):
+                break
+
+            # If the cancel file exists, stop processing...
+            if cancel_filepath is not None and cancel_filepath.exists():
+                print()
+                logger.info(f"Cancel file found, so stop: {cancel_filepath}")
+                break
+
+            # Get the next filepath to be processed
+            image_filepath = None
+            if image_id < (len(image_filepaths) - 1):
+                image_id += 1
+                image_filepath = image_filepaths[image_id]
+
+                # Check if the image has been processed already
+                if force is False and image_filepath.name in image_done_filenames:
+                    logger.debug(
+                        "Predict for image has already been done before and force is "
+                        f"False, so skip: {image_filepath.name}"
+                    )
+                    nb_to_process -= 1
+                    continue
+
+                nb_processed += 1
+
+                # Schedule file to be read
+                read_future = read_pool.submit(
+                    read_image,  # Function
+                    image_filepath,  # Arg 1
+                    projection_if_missing,
+                )  # Arg 2)
+                read_future_to_input_path[read_future] = image_filepath
+            else:
+                last_image_reached = True
+
+            # Prepare batch_size images that have been read for prediction
+            while (
+                len(read_future_to_input_path) > 0 and len(predict_images) < batch_size
+            ):
+
+                # If the read pool is not full, first schedule extra reads
+                if (
+                    last_image_reached is False
+                    and len(read_future_to_input_path) < nb_parallel_read
+                ):
+                    break
+
+                # Prepare the images that have been read for predicting
+                futures_done = [
+                    future
+                    for future in read_future_to_input_path
+                    if future.done() is True
+                ]
+                for future in futures_done:
+
+                    # Prediction can only handle batch_size images
+                    if len(predict_images) >= batch_size:
+                        break
+
+                    try:
+                        # Get the result from the read
+                        read_result = future.result()
+                        image_filepath_read = read_result["image_filepath"]
+
+                        # Prepare the filepath for the output
+                        output_suffix = ".tif"
+                        if evaluate_mode:
+                            # In evaluate mode, put everyting in output base dir for
+                            # easier comparison
+                            output_image_pred_dir = output_image_dir
+
+                            # Prepare complete filepath for image prediction
+                            output_image_pred_path = (
+                                output_image_dir / image_filepath_read.stem
+                            )
+                        else:
+                            # If saving predictions to images for real, keep hierarchic
+                            # structure if present
+                            tmp_output_filepath = Path(
+                                str(image_filepath_read).replace(
+                                    str(input_image_dir), str(output_image_dir)
+                                )
+                            )
+                            output_image_pred_dir = tmp_output_filepath.parent
+                            output_image_pred_path = (
+                                output_image_pred_dir
+                                / f"{image_filepath_read.stem}_pred{output_suffix}"
+                            )
+
+                        predict_images.append(
+                            {
+                                "input_image_filepath": image_filepath_read,
+                                "output_pred_filepath": output_image_pred_path,
+                                "output_image_pred_dir": output_image_pred_dir,
+                                "image_crs": read_result["image_crs"],
+                                "image_transform": read_result["image_transform"],
+                                "image_data": read_result["image_data"],
+                            }
+                        )
+
+                    finally:
+                        # Remove from queue...
+                        del read_future_to_input_path[future]
+
+                # If not at last image + not enough images yet for predict + read
+                # queue is full, sleep
+                if (
+                    last_image_reached is False
+                    and len(predict_images) < batch_size
+                    and len(read_future_to_input_path) >= nb_parallel_read
+                ):
+                    if read_sleep_logged is False:
+                        logger.info("Wait for images to be read")
+                        read_sleep_logged = True
+                    time.sleep(0.01)
+
+            # If batch_size images are ready for prediction or we are at
+            # the last images: predict
+            if len(predict_images) == batch_size or (
+                last_image_reached is True and len(predict_images) > 0
+            ):
+                read_sleep_logged = False
+                perf_time_now = datetime.datetime.now()
+                perfinfo = f"waiting for read took {perf_time_now-perf_time_start}"
+                perf_time_start = perf_time_now
+
+                # Predict!
+                logger.debug(f"Start prediction for {len(predict_images)} images")
+                perf_time_start = datetime.datetime.now()
+                curr_batch_image_list = [
+                    curr_batch_image_info["image_data"]
+                    for curr_batch_image_info in predict_images
+                ]
+                curr_batch_image_arr = np.stack(curr_batch_image_list)
+                curr_batch_image_pred_arr = model.predict_on_batch(curr_batch_image_arr)
+
+                perf_time_now = datetime.datetime.now()
+                perfinfo += f", predict took {perf_time_now-perf_time_start}"
+                perf_time_start = perf_time_now
+
+                # In tf > 2.1 a tf.tensor object is returned, but we want an ndarray
+                if type(curr_batch_image_pred_arr) is tf.Tensor:
+                    curr_batch_image_pred_arr = np.array(
+                        curr_batch_image_pred_arr.numpy()  # type: ignore
+                    )
+                else:
+                    curr_batch_image_pred_arr = np.array(curr_batch_image_pred_arr)
+
+                # Save predictions
+                # Remark: trying to parallelize this doesn't seem to help at all!
+                logger.debug("Start post-processing")
+                for batch_image_id, image_info in enumerate(predict_images):
+                    try:
+                        # If not in evaluate mode... save to vector in background
+                        if (
+                            evaluate_mode is False
+                            and output_vector_path is not None
+                            and pred_tmp_output_path is not None
+                        ):
+                            # Prepare prediction array...
+                            #   - convert to uint8 to reduce pickle size/time
+                            image_pred_arr_uint8 = (
+                                (curr_batch_image_pred_arr[batch_image_id, :, :, :])
+                                * 255
+                            ).astype(np.uint8)
+                            future = postprocess_pool.submit(
+                                postp.polygonize_pred_multiclass_to_file,
+                                image_pred_arr_uint8,
+                                image_info["image_crs"],
+                                image_info["image_transform"],
+                                classes,
+                                pred_tmp_output_path,
+                                min_probability,
+                                postprocess,
+                                border_pixels_to_ignore,
+                            )
+                            postp_future_to_input_path[future] = image_info[
+                                "input_image_filepath"
+                            ]
+
+                        else:
+                            # Saving the predictions as images at the moment only used
+                            # for evaluate mode...
+                            # TODO: would ideally be moved to the background
+                            # processing as well to simplify code here...
+                            postp.clean_and_save_prediction(
+                                image_image_filepath=image_info["input_image_filepath"],
+                                image_crs=image_info["image_crs"],
+                                image_transform=image_info["image_transform"],
+                                image_pred_arr=curr_batch_image_pred_arr[
+                                    batch_image_id
+                                ],
+                                output_dir=image_info["output_image_pred_dir"],
+                                input_image_dir=input_image_dir,
+                                input_mask_dir=input_mask_dir,
+                                border_pixels_to_ignore=border_pixels_to_ignore,
+                                min_probability=min_probability,
+                                evaluate_mode=evaluate_mode,
+                                classes=classes,
+                                force=force,
+                            )
+
+                            # Write filepath to file with files that are done
+                            with images_done_log_filepath.open(
+                                "a+"
+                            ) as image_donelog_file:
+                                image_donelog_file.write(
+                                    f"{image_info['input_image_filepath'].name}\n"
+                                )
+                    except Exception as ex:
+                        nb_errors += 1
+                        image_path = image_info["input_image_filepath"]
+                        _handle_error(image_path, ex, images_error_log_filepath)
+
+                perf_time_now = datetime.datetime.now()
+                perfinfo += (
+                    f", scheduling postprocessings took {perf_time_now-perf_time_start}"
+                )
+                perf_time_start = perf_time_now
+
+                # Poll for completed postprocessings
+                postp_sleep_logged = False
+                while len(postp_future_to_input_path) > 0:
+
+                    # If not at last file, get results from all futures that are
+                    # done, if at last file, wait till all are done
+                    if last_image_reached is False:
+                        futures_done = [
+                            future
+                            for future in postp_future_to_input_path
+                            if future.done() is True
+                        ]
+                    else:
+                        logger.info("Wait for last batch")
+                        futures_done = futures.wait(postp_future_to_input_path).done
+                    for future in futures_done:
+                        # Get the result from the polygonization
+                        try:
+                            # Get the result (= exception when something went wrong)
+                            result = future.result()
+                            logger.debug(
+                                f"result for {postp_future_to_input_path[future].name}:"
+                                f" {result}"
+                            )
+
+                            # Write filepath to file with files that are done
+                            with images_done_log_filepath.open(
+                                "a+"
+                            ) as image_donelog_file:
+                                image_donelog_file.write(
+                                    postp_future_to_input_path[future].name + "\n"
+                                )
+                        except Exception as ex:
+                            nb_errors += 1
+                            image_path = postp_future_to_input_path[future]
+                            _handle_error(image_path, ex, images_error_log_filepath)
+
+                        finally:
+                            # Remove from queue...
+                            del postp_future_to_input_path[future]
+
+                    # Wait till number below thresshold to evade huge waiting
+                    # list (and memory issues)
+                    if len(postp_future_to_input_path) > nb_parallel_postprocess * 2:
+                        if postp_sleep_logged is False:
+                            logger.info(
+                                "Postprocessing takes longer than prediction, so wait"
+                            )
+                            postp_sleep_logged = True
+                        time.sleep(0.01)
+                    else:
+                        # No need to wait (anymore)...
+                        if postp_sleep_logged is True:
+                            logger.info(
+                                "Waited enough for postprocessing to catch up..."
+                            )
+
+                        perf_time_now = datetime.datetime.now()
+                        perfinfo += (
+                            f", after postproces: took {perf_time_now-perf_time_start}"
+                        )
+                        perf_time_start = perf_time_now
+                        break
+
+                # Reset variable for next batch
+                predict_images = []
+
+                # Log the progress and prediction speed
+                if len(perfinfo) > 0:
+                    logger.debug(perfinfo)
+                if progress is not None:
+                    progress.step(nb_steps=batch_size)
+                # Init progress only when some imags were already processed, as the
+                # first are very slow.
+                if progress is None and nb_processed > 0:
+                    progress = ProgressLogger(
+                        message=f"predict to {output_image_dir.parent.name}/{output_image_dir.name}",  # noqa: E501
+                        nb_steps_total=nb_to_process,
+                        nb_steps_done=batch_size,
+                    )
+
+                # If max number errors reached, stop processings
+                if max_prediction_errors >= 0 and nb_errors >= max_prediction_errors:
+                    break
+
+        # If errors occured, raise error
+        if images_error_log_filepath.exists():
+            errors = pd.read_csv(
+                images_error_log_filepath,
+                usecols=["filename", "error"]
+                # ).to_string(justify="left", index=False)
+            ).to_html(justify="left", index=False)
+            raise Exception(f"Error(s) occured while predicting:\n{errors}")
+
+        # If alle images were processed, rename to real output file + cleanup
+        if (
+            last_image_reached is True
+            and output_vector_path is not None
+            and pred_tmp_output_path is not None
+            and pred_tmp_output_path.exists()
+        ):
+            output_vector_path.parent.mkdir(parents=True, exist_ok=True)
+            gfo.move(pred_tmp_output_path, output_vector_path)
+            gfo.rename_layer(output_vector_path, output_vector_path.stem)
+            shutil.rmtree(output_image_dir)
+
+
+def _handle_error(image_path: Path, ex: Exception, log_path: Path):
+    # Print exception + trace
+    exception_trace = traceback.format_exc()
+    exception_trace_print = exception_trace.replace("\n", "\n\t")
+    logger.error(f"Error postprocessing pred for {image_path}: {exception_trace_print}")
+
+    # Write error to error log file
+    first_error = False
+    if not log_path.exists():
+        first_error = True
+    with log_path.open("a+") as log_file:
+        if first_error:
+            log_file.write("filename,error,traceback\n")
+        writer = csv.writer(log_file)
+        exception_trace_csv = exception_trace.replace("\n", "\\n")
+        fields = [image_path.name, ex, exception_trace_csv]
+        writer.writerow(fields)
+
+
+def read_image(
+    image_filepath: Path, projection_if_missing: Optional[str] = None
+) -> dict:
+
+    # Read input file
+    # Because sometimes a read seems to fail, retry up to 3 times...
+    retry_count = 0
+    while True:
+        try:
+            with rio.open(str(image_filepath)) as image_ds:
+                # Read geo info
+                image_crs = image_ds.profile["crs"]
+                image_transform = image_ds.transform
+
+                # Read pixels + change from (channels, width, height) to
+                # (width, height, channels) + normalize to between 0 and 1
+                image_data = image_ds.read()
+                image_data = rio_plot.reshape_as_image(image_data)
+                image_data = image_data / 255.0
+
+            # Read worked, so jump out of the loop...
+            break
+        except Exception as ex:
+            retry_count += 1
+            logger.warning(f"Read failed, retry nb {retry_count} for {image_filepath}")
+            if retry_count >= 3:
+                message = f"Read failed {retry_count} times for {image_filepath}: {ex}"
+                logger.error(message)
+                raise Exception(message)
+
+    # The read was successfull, now check if there was a projection in the
+    # file and/or if one was provided
+    if image_crs is None:
+        if projection_if_missing is not None:
+            image_crs = rio_crs.CRS.from_string(projection_if_missing)
+        else:
+            message = (
+                f"Image has no proj and projection_if_missing is None: {image_filepath}"
+            )
+            logger.error(message)
+            raise Exception(message)
+
+    # Now return the result
+    result = {
+        "image_data": image_data,
+        "image_crs": image_crs,
+        "image_transform": image_transform,
+        "image_filepath": image_filepath,
+    }
+    return result
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    raise Exception("Not implemented")
```

### Comparing `orthoseg-0.4.2/orthoseg/lib/prepare_traindatasets.py` & `orthoseg-0.4.2a1/orthoseg/lib/prepare_traindatasets.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,800 +1,800 @@
-# -*- coding: utf-8 -*-
-"""
-Module to prepare the training datasets.
-"""
-
-from __future__ import print_function
-import logging
-import shutil
-import math
-from pathlib import Path
-import pprint
-from typing import List, Optional, Tuple, Union
-import warnings
-import urllib3
-
-import geofileops as gfo
-import pandas as pd
-import geopandas as gpd
-import numpy as np
-import owslib
-import owslib.wms
-import owslib.util
-from PIL import Image
-import pygeos
-import rasterio as rio
-import rasterio.features as rio_features
-import rasterio.profiles as rio_profiles
-import shapely.geometry as sh_geom
-
-from orthoseg.util.progress_util import ProgressLogger
-from orthoseg.util import ows_util
-from orthoseg.util import vector_util
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-class LabelInfo:
-    def __init__(
-        self,
-        locations_path: Path,
-        polygons_path: Path,
-        image_layer: str,
-        locations_gdf: Optional[gpd.GeoDataFrame] = None,
-        polygons_gdf: Optional[gpd.GeoDataFrame] = None,
-    ):
-        self.locations_path = locations_path
-        self.polygons_path = polygons_path
-        self.image_layer = image_layer
-        self.locations_gdf = locations_gdf
-        self.polygons_gdf = polygons_gdf
-
-    def __repr__(self):
-        repr = (
-            f"LabelInfo with image_layer: {self.image_layer}, locations_path: "
-            f"{self.locations_path}, polygons_path: {self.polygons_path}"
-        )
-        return repr
-
-
-class ValidationError(ValueError):
-    def __init__(self, message, errors):
-        # Call the base class constructor with the parameters it needs
-        super().__init__(message)
-
-        # Now for your custom code...
-        self.errors = errors
-
-    def __repr__(self):
-        repr = super().__repr__()
-        if self.errors is not None and len(self.errors) > 0:
-            repr += f"\n  -> Errors: {pprint.pformat(self.errors, indent=4, width=100)}"
-        return repr
-
-    def __str__(self):
-        repr = super().__str__()
-        if self.errors is not None and len(self.errors) > 0:
-            repr += f"\n  -> Errors: {pprint.pformat(self.errors, indent=4, width=100)}"
-        return repr
-
-    def to_html(self):
-        repr = super().__str__()
-        if self.errors is not None and len(self.errors) > 0:
-            errors_df = pd.DataFrame(self.errors, columns=["error"])
-            repr += f"{errors_df.to_html()}"
-        return repr
-
-
-def prepare_traindatasets(
-    label_infos: List[LabelInfo],
-    classes: dict,
-    image_layers: dict,
-    training_dir: Path,
-    labelname_column: str = "classname",
-    image_pixel_x_size: float = 0.25,
-    image_pixel_y_size: float = 0.25,
-    image_pixel_width: int = 512,
-    image_pixel_height: int = 512,
-    ssl_verify: Union[bool, str] = True,
-    force: bool = False,
-) -> Tuple[Path, int]:
-    """
-    This function prepares training data for the vector labels provided.
-
-    It will:
-        * get orthophoto's from a WMS server
-        * create the corresponding label mask for each orthophoto
-
-    Returns a tuple with (output_dir, dataversion):
-        output_dir: the dir where the traindataset was created/found
-        dataversion: a version number for the dataset created/found
-
-    Args
-        label_infos (List[LabelInfo]): paths to the files with label polygons
-            and locations to generate images for
-        classes (dict): dict with the classes to detect as keys. The values
-            are the following:
-                - labelnames: list of labels to use for this class
-                - weight:
-                - burn_value:
-        image_layers (dict):
-        training_dir (Path):
-        labelname_column (str): the column where the label names are stored in
-            the polygon files. If the column name specified is not found, column
-            "label_name" is used if it exists for backwards compatibility.
-        ssl_verify (bool or str, optional): True to use the default
-            certificate bundle as installed on your system. False disables
-            certificate validation (NOT recommended!). If a path to a
-            certificate bundle file (.pem) is passed, this will be used.
-            In corporate networks using a proxy server this is often needed
-            to evade CERTIFICATE_VERIFY_FAILED errors. Defaults to True.
-    """
-    # Init stuff
-    # Interprete ssl_verify
-    auth = None
-    if ssl_verify is not None:
-        # If it is a string, make sure it isn't actually a bool
-        if isinstance(ssl_verify, str):
-            if ssl_verify.lower() == "true":
-                ssl_verify = True
-            elif ssl_verify.lower() == "false":
-                ssl_verify = False
-
-        auth = owslib.util.Authentication(verify=ssl_verify)  # type: ignore
-        if isinstance(ssl_verify, bool) and ssl_verify is False:
-            urllib3.disable_warnings()
-            logger.warn("SSL VERIFICATION IS TURNED OFF!!!")
-
-    # Check if the first class is named "background"
-    if len(classes) == 0:
-        raise Exception("No classes specified")
-    elif list(classes)[0].lower() != "background":
-        classes_str = pprint.pformat(classes, sort_dicts=False, width=50)
-        raise Exception(
-            f"By convention, the first class must be called background!\n{classes_str}"
-        )
-
-    # Check if the latest version of training data is already ok
-    # Determine the current data version based on existing output data dir(s),
-    # If dir ends on _TMP_* ignore it, as it (probably) ended with an error.
-    output_dirs = training_dir.glob("[0-9]*/")
-    output_dirs = [
-        output_dir for output_dir in output_dirs if "_TMP_" not in output_dir.name
-    ]
-
-    reuse_traindata = False
-    if len(output_dirs) == 0:
-        dataversion_new = 1
-    else:
-        # Get the output dir with the highest version (=first if sorted desc)
-        output_dir_mostrecent = sorted(output_dirs, reverse=True)[0]
-        dataversion_mostrecent = int(output_dir_mostrecent.name)
-
-        # If none of the input files changed since previous run, reuse dataset
-        for label_file in label_infos:
-            reuse_traindata = True
-            labellocations_output_mostrecent_path = (
-                output_dir_mostrecent / label_file.locations_path.name
-            )
-            labeldata_output_mostrecent_path = (
-                output_dir_mostrecent / label_file.polygons_path.name
-            )
-            if not (
-                labellocations_output_mostrecent_path.exists()
-                and labeldata_output_mostrecent_path.exists()
-                and gfo.cmp(
-                    label_file.locations_path, labellocations_output_mostrecent_path
-                )
-                and gfo.cmp(label_file.polygons_path, labeldata_output_mostrecent_path)
-            ):
-                reuse_traindata = False
-                break
-        if reuse_traindata:
-            dataversion_new = dataversion_mostrecent
-            logger.info(
-                "Input label file(s) didn't change since last prepare_traindatasets, "
-                f"so reuse version {dataversion_new}"
-            )
-        else:
-            dataversion_new = dataversion_mostrecent + 1
-            logger.info(
-                "Input label file(s) changed since last prepare_traindatasets, "
-                f"so create new training data version {dataversion_new}"
-            )
-
-    # Determine the output dir
-    training_dataversion_dir = training_dir / f"{dataversion_new:02d}"
-
-    # If the train data is already ok, just return
-    if reuse_traindata is True:
-        return (training_dataversion_dir, dataversion_new)
-
-    # The input labels have changed: create new train version
-    # -------------------------------------------------------
-    # read, validate and prepare data
-    labeldata = prepare_labeldata(
-        label_infos=label_infos,
-        classes=classes,
-        labelname_column=labelname_column,
-        image_pixel_x_size=image_pixel_x_size,
-        image_pixel_y_size=image_pixel_y_size,
-        image_pixel_width=image_pixel_width,
-        image_pixel_height=image_pixel_height,
-    )
-
-    # Reading label data was succesfull, so prepare temp dir to put training dataset in.
-    # A temp dir, so it can be removed/ignored if an error occurs later on.
-    output_tmp_dir = create_tmp_dir(
-        training_dir, f"{dataversion_new:02d}", remove_existing=True
-    )
-
-    # Copy the label input files to dest dir + to a backup dir.
-    for label_file in label_infos:
-        gfo.copy(label_file.locations_path, output_tmp_dir)
-        gfo.copy(label_file.polygons_path, output_tmp_dir)
-        backup_dir = label_file.locations_path.parent / f"backup_v{dataversion_new:02d}"
-        shutil.rmtree(backup_dir, ignore_errors=True)
-        backup_dir.mkdir(parents=True, exist_ok=True)
-        gfo.copy(label_file.locations_path, backup_dir)
-        gfo.copy(label_file.polygons_path, backup_dir)
-
-    # Now create the images/masks for the new train version for the different traindata
-    # types.
-    traindata_types = ["train", "validation", "test"]
-    nb_todo = 0
-    for labellocations_gdf, _ in labeldata:
-        labellocations_curr_gdf = labellocations_gdf[
-            labellocations_gdf["traindata_type"].isin(traindata_types)
-        ]
-        nb_todo += len(labellocations_curr_gdf)
-    progress = ProgressLogger(message="prepare training images", nb_steps_total=nb_todo)
-    logger.info(f"Get images for {nb_todo} labels")
-
-    for traindata_type in traindata_types:
-        # Create output dirs...
-        output_imagedatatype_dir = output_tmp_dir / traindata_type
-        output_imagedata_image_dir = output_imagedatatype_dir / "image"
-        output_imagedata_mask_dir = output_imagedatatype_dir / "mask"
-        for dir in [
-            output_imagedatatype_dir,
-            output_imagedata_mask_dir,
-            output_imagedata_image_dir,
-        ]:
-            if dir and not dir.exists():
-                dir.mkdir(parents=True, exist_ok=True)
-
-        for labellocations_gdf, labels_to_burn_gdf in labeldata:
-            try:
-                # Get the label locations for this traindata type
-                labellocations_curr_gdf = labellocations_gdf[
-                    labellocations_gdf["traindata_type"] == traindata_type
-                ]
-
-                # Loop trough all locations labels to get an image for each of them
-                created_images_gdf = gpd.GeoDataFrame()
-                created_images_gdf["geometry"] = None
-                wms_imagelayer_layersources = {}
-                for i, label_tuple in enumerate(labellocations_curr_gdf.itertuples()):
-
-                    img_bbox = label_tuple.geometry
-                    image_layer = getattr(label_tuple, "image_layer")
-
-                    # If the wms to be used hasn't been initialised yet
-                    if image_layer not in wms_imagelayer_layersources:
-                        wms_imagelayer_layersources[image_layer] = []
-                        for layersource in image_layers[image_layer]["layersources"]:
-                            wms_service = owslib.wms.WebMapService(
-                                url=layersource["wms_server_url"],
-                                version=layersource["wms_version"],
-                                auth=auth,
-                            )
-                            if layersource["wms_ignore_capabilities_url"]:
-                                # If the wms url in capabilities should be ignored,
-                                # overwrite with original url
-                                nb = len(
-                                    wms_service.getOperationByName("GetMap").methods
-                                )
-                                for method_id in range(nb):
-                                    wms_service.getOperationByName("GetMap").methods[
-                                        method_id
-                                    ]["url"] = layersource["wms_server_url"]
-                            wms_imagelayer_layersources[image_layer].append(
-                                ows_util.LayerSource(
-                                    wms_service=wms_service,
-                                    layernames=layersource["layernames"],
-                                    layerstyles=layersource["layerstyles"],
-                                    bands=layersource["bands"],
-                                    random_sleep=layersource["random_sleep"],
-                                )
-                            )
-
-                    # Now really get the image
-                    logger.debug(f"Get image for coordinates {img_bbox.bounds}")
-                    assert labellocations_gdf.crs is not None
-                    image_filepath = ows_util.getmap_to_file(
-                        layersources=wms_imagelayer_layersources[image_layer],
-                        output_dir=output_imagedata_image_dir,
-                        crs=labellocations_gdf.crs,
-                        bbox=img_bbox.bounds,  # type: ignore
-                        size=(image_pixel_width, image_pixel_height),
-                        image_format=ows_util.FORMAT_PNG,
-                        # image_format_save=ows_util.FORMAT_TIFF,
-                        image_pixels_ignore_border=image_layers[image_layer][
-                            "image_pixels_ignore_border"
-                        ],
-                        transparent=False,
-                        layername_in_filename=True,
-                    )
-
-                    # Create a mask corresponding with the image file
-                    # image_filepath can be None if file exists, so check if not None...
-                    if image_filepath is not None:
-                        # Mask should not be in a lossy format!
-                        mask_filepath = Path(
-                            str(image_filepath)
-                            .replace(
-                                str(output_imagedata_image_dir),
-                                str(output_imagedata_mask_dir),
-                            )
-                            .replace(".jpg", ".png")
-                        )
-                        nb_classes = len(classes)
-
-                        # Only keep the labels that are meant for this image layer
-                        labels_for_layer_gdf = (
-                            labels_to_burn_gdf.loc[
-                                labels_to_burn_gdf["image_layer"] == image_layer
-                            ]
-                        ).copy()
-                        # assert to evade pyLance warning
-                        if len(labels_for_layer_gdf) == 0:
-                            logger.info(
-                                f"No polygons to burn for image_layer {image_layer}!"
-                            )
-                        assert isinstance(labels_for_layer_gdf, gpd.GeoDataFrame)
-                        _create_mask(
-                            input_image_filepath=image_filepath,
-                            output_mask_filepath=mask_filepath,
-                            labels_to_burn_gdf=labels_for_layer_gdf,
-                            nb_classes=nb_classes,
-                            force=force,
-                        )
-
-                    # Log the progress and prediction speed
-                    progress.step()
-
-            except Exception as ex:
-                raise ex
-
-    # If everything went fine, rename output_tmp_dir to the final output_dir
-    output_tmp_dir.rename(training_dataversion_dir)
-
-    return (training_dataversion_dir, dataversion_new)
-
-
-def prepare_labeldata(
-    label_infos: List[LabelInfo],
-    classes: dict,
-    labelname_column: str,
-    image_pixel_x_size: float,
-    image_pixel_y_size: float,
-    image_pixel_width: int,
-    image_pixel_height: int,
-) -> List[Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]]:
-    """
-    Prepare and validate the data in the labelinfos so it is ready to be uses to fetch
-    train images and burn masks.
-
-    Args:
-        label_infos (List[LabelInfo]): the label files/data.
-        classes (dict): dict with classes and their corresponding
-            label class names + weights.
-        labelname_column (str): the column name in the label polygon files where the
-            label classname can be found. Defaults to "classname".
-
-    Raises:
-        ValidationError: if the data is somehow not valid. All issues are listed in the
-            errors property.
-
-    Returns:
-        List[Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]]: returns a list of tuples with
-            geodataframes with labellocations and labelpolygons to burn.
-    """
-    labeldata_result = []
-    errors_found = []
-    labellocations_found = False
-    for label_info in label_infos:
-        # Read label locations if needed
-        if label_info.locations_gdf is not None:
-            labellocations_gdf = label_info.locations_gdf
-        else:
-            logger.debug(f"Read label locations from {label_info.locations_path}")
-            labellocations_gdf = gfo.read_file(label_info.locations_path)
-            if labellocations_gdf is not None and len(labellocations_gdf) > 0:
-                labellocations_gdf.loc[:, "path"] = str(label_info.locations_path)
-                labellocations_gdf.loc[:, "image_layer"] = label_info.image_layer
-                # Remark: geopandas 0.7.0 drops fid column internally!
-                labellocations_gdf.loc[
-                    :, "row_nb_orig"
-                ] = labellocations_gdf.index  # type: ignore
-            else:
-                logger.warn(f"No label locations found in {label_info.locations_path}")
-                continue
-
-        if len(labellocations_gdf) > 0:
-            labellocations_found = True
-
-        # Read label polygons if needed
-        if label_info.polygons_gdf is not None:
-            labelpolygons_gdf = label_info.polygons_gdf
-        else:
-            logger.debug(f"Read label data from {label_info.polygons_path}")
-            labelpolygons_gdf = gfo.read_file(label_info.polygons_path)
-            if labelpolygons_gdf is not None and len(labelpolygons_gdf) > 0:
-                labelpolygons_gdf.loc[:, "path"] = str(label_info.polygons_path)
-                labelpolygons_gdf.loc[:, "image_layer"] = label_info.image_layer
-            else:
-                logger.warn(f"No label polygons found in {label_info.polygons_path}")
-
-        assert labellocations_gdf is not None
-        assert labelpolygons_gdf is not None
-
-        if labellocations_gdf is None or len(labellocations_gdf) == 0:
-            errors_found.append("No label locations found in labellocations_gdf")
-            continue
-
-        # Validate + process the location data
-        # ------------------------------------
-        if "traindata_type" not in labellocations_gdf.columns:
-            errors_found.append(
-                "Mandatory column traindata_type not found in "
-                f"{label_info.locations_path}"
-            )
-
-        # Check + correct the geom of the location to make sure it matches the size of
-        # the training images/masks to be generated...
-        image_crs_width = math.fabs(
-            image_pixel_width * image_pixel_x_size
-        )  # tile width in units of crs => 500 m
-        image_crs_height = math.fabs(
-            image_pixel_height * image_pixel_y_size
-        )  # tile height in units of crs => 500 m
-        locations_none = []
-        for location in labellocations_gdf.itertuples():
-            if location.geometry is None or location.geometry.is_empty:
-                logger.warning(
-                    f"No or empty geometry found in file {Path(location.path).name} "
-                    f"for index {location.Index}, it will be ignored"
-                )
-                locations_none.append(location.Index)
-                continue
-
-            # Check if the traindata_type is valid
-            if location.traindata_type not in ["train", "validation", "test", "todo"]:
-                errors_found.append(
-                    f"Invalid traindata_type in {Path(location.path).name}: "
-                    f"{location.geometry.wkt}"
-                )
-
-            # Check if the geometry is valid
-            is_valid_reason = pygeos.is_valid_reason(
-                labellocations_gdf.geometry.array.data[location.Index]
-            )
-            if is_valid_reason != "Valid Geometry":
-                errors_found.append(
-                    f"Invalid geometry in {Path(location.path).name}: "
-                    f"{is_valid_reason}"
-                )
-                continue
-
-            geom_bounds = location.geometry.bounds
-            xmin = geom_bounds[0] - (geom_bounds[0] % image_pixel_x_size)
-            ymin = geom_bounds[1] - (geom_bounds[1] % image_pixel_y_size)
-            xmax = xmin + image_crs_width
-            ymax = ymin + image_crs_height
-            location_geom_aligned = sh_geom.box(xmin, ymin, xmax, ymax)
-
-            # Check if the realigned geom overlaps good enough with the original
-            intersection = location_geom_aligned.intersection(
-                labellocations_gdf.at[location.Index, "geometry"]
-            )
-            area_1row_1col = (
-                image_pixel_x_size * image_crs_width
-                + image_pixel_y_size * image_crs_height
-            )
-            if intersection.area < (location_geom_aligned.area - area_1row_1col):
-                # Original geom was digitized too small
-                errors_found.append(
-                    f"Location geometry too small in {Path(location.path).name}: "
-                    f"{location.geometry.wkt}"
-                )
-            elif location_geom_aligned.area > 1.1 * sh_geom.box(*geom_bounds).area:
-                logger.warn(
-                    "Location geometry larger than expected in file "
-                    f"{Path(location.path).name}: {location.geometry.wkt}"
-                )
-            labellocations_gdf.at[location.Index, "geometry"] = location_geom_aligned
-
-        # Remove locations with None or point/line geoms
-        labellocations_gdf = labellocations_gdf[
-            ~labellocations_gdf.index.isin(locations_none)
-        ]  # type: ignore
-
-        # Check if labellocations has a proper crs
-        if labellocations_gdf.crs is None:
-            errors_found.append(
-                "No crs in labellocations, labellocation_gdf.crs: "
-                f"{labellocations_gdf.crs}"
-            )
-
-        # Validate + process the polygons data
-        # ------------------------------------
-        if labelpolygons_gdf is None:
-            errors_found.append("No labelpolygons in the training data!")
-            continue
-
-        # Create list with only the input polygons that need to be burned in the mask
-        labels_to_burn_gdf = None
-        if labelname_column not in labelpolygons_gdf.columns:
-            # For backwards compatibility, also support old default column name
-            labelname_column = "label_name"
-        if labelname_column in labelpolygons_gdf.columns:
-            # If there is a column labelname_column, use the burn values specified in
-            # the configuration
-            labels_to_burn_gdf = labelpolygons_gdf
-            labels_to_burn_gdf.loc[:, "burn_value"] = None  # type: ignore
-            for classname in classes:
-                labels_to_burn_gdf.loc[
-                    (
-                        labels_to_burn_gdf[labelname_column].isin(
-                            classes[classname]["labelnames"]
-                        )
-                    ),
-                    "burn_value",
-                ] = classes[classname]["burn_value"]
-
-            # Check if there are invalid class names
-            invalid_gdf = labels_to_burn_gdf.loc[
-                labels_to_burn_gdf["burn_value"].isnull()
-            ]
-            for _, invalid_row in invalid_gdf.iterrows():
-                errors_found.append(
-                    f"Invalid classname in {Path(invalid_row['path']).name}: "
-                    f"{invalid_row[labelname_column]}"
-                )
-
-            # Filter away rows that are going to burn 0, as this is useless...
-            labels_to_burn_gdf = labels_to_burn_gdf.loc[
-                labels_to_burn_gdf["burn_value"] != 0
-            ].copy()
-
-        elif len(classes) == 2:
-            # There is no column with label names, but there are only 2 classes
-            # (background + subject), so no problem...
-            logger.info(
-                f"Column ({labelname_column}) not found, so use all polygons in "
-                f"{label_info.polygons_path.name}"
-            )
-            labels_to_burn_gdf = labelpolygons_gdf
-            labels_to_burn_gdf.loc[:, "burn_value"] = 1  # type: ignore
-
-        else:
-            # There is no column with label names, but more than two classes, so stop.
-            errors_found.append(
-                f"Column {labelname_column} is mandatory in labeldata if multiple "
-                f"classes specified: {classes}"
-            )
-
-        # Check if we ended up with label data to burn.
-        if labels_to_burn_gdf is None:
-            errors_found.append(
-                "Not any labelpolygon retained to burn in the training data!"
-            )
-            continue
-
-        # Filter away None and empty geometries... they cannot be burned
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", "GeoSeries.notna", UserWarning)
-            labels_to_burn_gdf = labels_to_burn_gdf[
-                ~labels_to_burn_gdf.geometry.is_empty
-                & labels_to_burn_gdf.geometry.notna()
-            ].copy()
-
-        # Make sure all label polygons are valid
-        labels_to_burn_gdf.loc[  # type: ignore
-            :, "is_valid_reason"
-        ] = vector_util.is_valid_reason(labels_to_burn_gdf.geometry)
-        invalid_gdf = labels_to_burn_gdf.query("is_valid_reason != 'Valid Geometry'")
-        for invalid in invalid_gdf.itertuples():
-            errors_found.append(
-                f"Invalid geometry in {Path(invalid.path).name}: "
-                f"{invalid.is_valid_reason}"
-            )
-
-        assert isinstance(labels_to_burn_gdf, gpd.GeoDataFrame)
-        labeldata_result.append((labellocations_gdf, labels_to_burn_gdf))
-
-    # If errors found, raise
-    if len(errors_found) > 0:
-        raise ValidationError(
-            f"Errors found in label data: {len(errors_found)}", errors_found
-        )
-    if not labellocations_found:
-        errors_found.append("No labellocations found in the training data")
-        raise ValidationError("No labellocations found", errors_found)
-
-    return labeldata_result
-
-
-def create_tmp_dir(
-    parent_dir: Path, dir_name: str, remove_existing: bool = False
-) -> Path:
-    """
-    Helper function to create a 'TMP' dir based on a directory name:
-        parent_dir / <dir_name>_TMP_<sequence>
-
-    Use: if you want to write data to a directory in a "transactional way",
-    it is the safest to write to a temp dir first, and then rename it to the
-    final name. This way, if a hard crash occurs while writing the data, it
-    is clear that the directory wasn't ready. Additionally, in case of a hard
-    crash, file locks can remain which makes it impossible to remove a
-    directory for a while.
-
-    Args:
-        parent_dir (Path): The dir to create the temp dir in.
-        dir_name (str): The name of the dir to base the temp dir on.
-        remove_existing (bool, optional): If True, existing TMP directories
-            will be removed if possible. Defaults to False.
-
-    Raises:
-        Exception: [description]
-
-    Returns:
-        Path: [description]
-    """
-    # The final dir should not exists yet!
-    final_dir = parent_dir / dir_name
-    if final_dir.exists():
-        raise Exception(
-            f"It is not supported to create a TMP dir for an existing dir: {final_dir}"
-        )
-
-    # Try to delete all existing TMP dir's
-    if remove_existing is True:
-        existing_tmp_dirs = parent_dir.glob(f"{dir_name}_TMP_*")
-        for existing_tmp_dir in existing_tmp_dirs:
-            try:
-                shutil.rmtree(existing_tmp_dir)
-            except Exception:
-                tmp_dir = None
-
-    # Create the TMP dir
-    tmp_dir = None
-    for i in range(100):
-        tmp_dir = parent_dir / f"{dir_name}_TMP_{i:02d}"
-
-        if tmp_dir.exists():
-            # If it (still) exists try next sequence
-            tmp_dir = None
-            continue
-        else:
-            # If it doesn't exist, try to create it
-            try:
-                tmp_dir.mkdir(parents=True)
-                break
-            except Exception:
-                # If it fails to create, try next sequence
-                tmp_dir = None
-                continue
-
-    # If no output tmp dir could be found/created... stop...
-    if tmp_dir is None:
-        raise Exception(
-            f"Error creating/replacing TMP dir for {dir_name} in {parent_dir}"
-        )
-
-    return tmp_dir
-
-
-def _create_mask(
-    input_image_filepath: Path,
-    output_mask_filepath: Path,
-    labels_to_burn_gdf: gpd.GeoDataFrame,
-    nb_classes: int = 1,
-    output_imagecopy_filepath: Optional[Path] = None,
-    minimum_pct_labeled: float = 0.0,
-    force: bool = False,
-) -> Optional[bool]:
-
-    # If file exists already and force is False... stop.
-    if force is False and output_mask_filepath.exists():
-        logger.debug(
-            f"Output file exist, and force is False, return: {output_mask_filepath}"
-        )
-        return
-
-    # Create a mask corresponding with the image file
-    # First read the properties of the input image to copy them for the output
-    logger.debug(f"Create mask to {output_mask_filepath}")
-    with rio.open(input_image_filepath) as image_ds:
-        image_input_profile = image_ds.profile
-        image_transform_affine = image_ds.transform
-
-    # Prepare the file profile for the mask depending on output type
-    output_ext_lower = output_mask_filepath.suffix.lower()
-    if output_ext_lower == ".tif":
-        image_output_profile = rio_profiles.DefaultGTiffProfile(
-            count=1, transform=image_transform_affine, crs=image_input_profile["crs"]
-        )
-    if output_ext_lower == ".png":
-        image_output_profile = rio_profiles.Profile(driver="PNG", count=1)
-    else:
-        raise Exception(
-            f"Unsupported mask suffix (should be lossless format!): {output_ext_lower}"
-        )
-    image_output_profile.update(
-        width=image_input_profile["width"],
-        height=image_input_profile["height"],
-        dtype=rio.uint8,
-    )
-
-    # Burn the vectors in a mask
-    burn_shapes = [
-        (geom, value)
-        for geom, value in zip(
-            labels_to_burn_gdf.geometry, labels_to_burn_gdf.burn_value
-        )
-        if geom is not None and geom.is_empty is False
-    ]
-    if len(burn_shapes) > 0:
-        try:
-            mask_arr = rio_features.rasterize(
-                shapes=burn_shapes,
-                transform=image_transform_affine,
-                dtype=rio.uint8,
-                fill=0,
-                out_shape=(
-                    image_output_profile["width"],  # type: ignore
-                    image_output_profile["height"],  # type: ignore
-                ),
-            )
-
-        except Exception as ex:
-            raise Exception(f"Error creating mask for {image_transform_affine}") from ex
-    else:
-        mask_arr = np.zeros(
-            shape=(
-                image_output_profile["width"],  # type: ignore
-                image_output_profile["height"],  # type: ignore
-            ),
-            dtype=rio.uint8,
-        )
-
-    # Check if the mask meets the requirements to be written...
-    if minimum_pct_labeled > 0:
-        nb_pixels = np.size(mask_arr, 0) * np.size(mask_arr, 1)
-        nb_pixels_data = nb_pixels - np.sum(
-            mask_arr == 0
-        )  # np.count_nonnan(image == NoData_value)
-        logger.debug(
-            f"nb_pixels: {nb_pixels}, nb_pixels_data: {nb_pixels_data}, "
-            f"pct data: {nb_pixels_data / nb_pixels}"
-        )
-
-        if nb_pixels_data / nb_pixels < minimum_pct_labeled:
-            return False
-
-    # Write the labeled mask as .png (so without transform/crs info)
-    im = Image.fromarray(mask_arr)
-    im.save(output_mask_filepath)
-
-    return True
+# -*- coding: utf-8 -*-
+"""
+Module to prepare the training datasets.
+"""
+
+from __future__ import print_function
+import logging
+import shutil
+import math
+from pathlib import Path
+import pprint
+from typing import List, Optional, Tuple, Union
+import warnings
+import urllib3
+
+import geofileops as gfo
+import pandas as pd
+import geopandas as gpd
+import numpy as np
+import owslib
+import owslib.wms
+import owslib.util
+from PIL import Image
+import pygeos
+import rasterio as rio
+import rasterio.features as rio_features
+import rasterio.profiles as rio_profiles
+import shapely.geometry as sh_geom
+
+from orthoseg.util.progress_util import ProgressLogger
+from orthoseg.util import ows_util
+from orthoseg.util import vector_util
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+class LabelInfo:
+    def __init__(
+        self,
+        locations_path: Path,
+        polygons_path: Path,
+        image_layer: str,
+        locations_gdf: Optional[gpd.GeoDataFrame] = None,
+        polygons_gdf: Optional[gpd.GeoDataFrame] = None,
+    ):
+        self.locations_path = locations_path
+        self.polygons_path = polygons_path
+        self.image_layer = image_layer
+        self.locations_gdf = locations_gdf
+        self.polygons_gdf = polygons_gdf
+
+    def __repr__(self):
+        repr = (
+            f"LabelInfo with image_layer: {self.image_layer}, locations_path: "
+            f"{self.locations_path}, polygons_path: {self.polygons_path}"
+        )
+        return repr
+
+
+class ValidationError(ValueError):
+    def __init__(self, message, errors):
+        # Call the base class constructor with the parameters it needs
+        super().__init__(message)
+
+        # Now for your custom code...
+        self.errors = errors
+
+    def __repr__(self):
+        repr = super().__repr__()
+        if self.errors is not None and len(self.errors) > 0:
+            repr += f"\n  -> Errors: {pprint.pformat(self.errors, indent=4, width=100)}"
+        return repr
+
+    def __str__(self):
+        repr = super().__str__()
+        if self.errors is not None and len(self.errors) > 0:
+            repr += f"\n  -> Errors: {pprint.pformat(self.errors, indent=4, width=100)}"
+        return repr
+
+    def to_html(self):
+        repr = super().__str__()
+        if self.errors is not None and len(self.errors) > 0:
+            errors_df = pd.DataFrame(self.errors, columns=["error"])
+            repr += f"{errors_df.to_html()}"
+        return repr
+
+
+def prepare_traindatasets(
+    label_infos: List[LabelInfo],
+    classes: dict,
+    image_layers: dict,
+    training_dir: Path,
+    labelname_column: str = "classname",
+    image_pixel_x_size: float = 0.25,
+    image_pixel_y_size: float = 0.25,
+    image_pixel_width: int = 512,
+    image_pixel_height: int = 512,
+    ssl_verify: Union[bool, str] = True,
+    force: bool = False,
+) -> Tuple[Path, int]:
+    """
+    This function prepares training data for the vector labels provided.
+
+    It will:
+        * get orthophoto's from a WMS server
+        * create the corresponding label mask for each orthophoto
+
+    Returns a tuple with (output_dir, dataversion):
+        output_dir: the dir where the traindataset was created/found
+        dataversion: a version number for the dataset created/found
+
+    Args
+        label_infos (List[LabelInfo]): paths to the files with label polygons
+            and locations to generate images for
+        classes (dict): dict with the classes to detect as keys. The values
+            are the following:
+                - labelnames: list of labels to use for this class
+                - weight:
+                - burn_value:
+        image_layers (dict):
+        training_dir (Path):
+        labelname_column (str): the column where the label names are stored in
+            the polygon files. If the column name specified is not found, column
+            "label_name" is used if it exists for backwards compatibility.
+        ssl_verify (bool or str, optional): True to use the default
+            certificate bundle as installed on your system. False disables
+            certificate validation (NOT recommended!). If a path to a
+            certificate bundle file (.pem) is passed, this will be used.
+            In corporate networks using a proxy server this is often needed
+            to evade CERTIFICATE_VERIFY_FAILED errors. Defaults to True.
+    """
+    # Init stuff
+    # Interprete ssl_verify
+    auth = None
+    if ssl_verify is not None:
+        # If it is a string, make sure it isn't actually a bool
+        if isinstance(ssl_verify, str):
+            if ssl_verify.lower() == "true":
+                ssl_verify = True
+            elif ssl_verify.lower() == "false":
+                ssl_verify = False
+
+        auth = owslib.util.Authentication(verify=ssl_verify)  # type: ignore
+        if isinstance(ssl_verify, bool) and ssl_verify is False:
+            urllib3.disable_warnings()
+            logger.warn("SSL VERIFICATION IS TURNED OFF!!!")
+
+    # Check if the first class is named "background"
+    if len(classes) == 0:
+        raise Exception("No classes specified")
+    elif list(classes)[0].lower() != "background":
+        classes_str = pprint.pformat(classes, sort_dicts=False, width=50)
+        raise Exception(
+            f"By convention, the first class must be called background!\n{classes_str}"
+        )
+
+    # Check if the latest version of training data is already ok
+    # Determine the current data version based on existing output data dir(s),
+    # If dir ends on _TMP_* ignore it, as it (probably) ended with an error.
+    output_dirs = training_dir.glob("[0-9]*/")
+    output_dirs = [
+        output_dir for output_dir in output_dirs if "_TMP_" not in output_dir.name
+    ]
+
+    reuse_traindata = False
+    if len(output_dirs) == 0:
+        dataversion_new = 1
+    else:
+        # Get the output dir with the highest version (=first if sorted desc)
+        output_dir_mostrecent = sorted(output_dirs, reverse=True)[0]
+        dataversion_mostrecent = int(output_dir_mostrecent.name)
+
+        # If none of the input files changed since previous run, reuse dataset
+        for label_file in label_infos:
+            reuse_traindata = True
+            labellocations_output_mostrecent_path = (
+                output_dir_mostrecent / label_file.locations_path.name
+            )
+            labeldata_output_mostrecent_path = (
+                output_dir_mostrecent / label_file.polygons_path.name
+            )
+            if not (
+                labellocations_output_mostrecent_path.exists()
+                and labeldata_output_mostrecent_path.exists()
+                and gfo.cmp(
+                    label_file.locations_path, labellocations_output_mostrecent_path
+                )
+                and gfo.cmp(label_file.polygons_path, labeldata_output_mostrecent_path)
+            ):
+                reuse_traindata = False
+                break
+        if reuse_traindata:
+            dataversion_new = dataversion_mostrecent
+            logger.info(
+                "Input label file(s) didn't change since last prepare_traindatasets, "
+                f"so reuse version {dataversion_new}"
+            )
+        else:
+            dataversion_new = dataversion_mostrecent + 1
+            logger.info(
+                "Input label file(s) changed since last prepare_traindatasets, "
+                f"so create new training data version {dataversion_new}"
+            )
+
+    # Determine the output dir
+    training_dataversion_dir = training_dir / f"{dataversion_new:02d}"
+
+    # If the train data is already ok, just return
+    if reuse_traindata is True:
+        return (training_dataversion_dir, dataversion_new)
+
+    # The input labels have changed: create new train version
+    # -------------------------------------------------------
+    # read, validate and prepare data
+    labeldata = prepare_labeldata(
+        label_infos=label_infos,
+        classes=classes,
+        labelname_column=labelname_column,
+        image_pixel_x_size=image_pixel_x_size,
+        image_pixel_y_size=image_pixel_y_size,
+        image_pixel_width=image_pixel_width,
+        image_pixel_height=image_pixel_height,
+    )
+
+    # Reading label data was succesfull, so prepare temp dir to put training dataset in.
+    # A temp dir, so it can be removed/ignored if an error occurs later on.
+    output_tmp_dir = create_tmp_dir(
+        training_dir, f"{dataversion_new:02d}", remove_existing=True
+    )
+
+    # Copy the label input files to dest dir + to a backup dir.
+    for label_file in label_infos:
+        gfo.copy(label_file.locations_path, output_tmp_dir)
+        gfo.copy(label_file.polygons_path, output_tmp_dir)
+        backup_dir = label_file.locations_path.parent / f"backup_v{dataversion_new:02d}"
+        shutil.rmtree(backup_dir, ignore_errors=True)
+        backup_dir.mkdir(parents=True, exist_ok=True)
+        gfo.copy(label_file.locations_path, backup_dir)
+        gfo.copy(label_file.polygons_path, backup_dir)
+
+    # Now create the images/masks for the new train version for the different traindata
+    # types.
+    traindata_types = ["train", "validation", "test"]
+    nb_todo = 0
+    for labellocations_gdf, _ in labeldata:
+        labellocations_curr_gdf = labellocations_gdf[
+            labellocations_gdf["traindata_type"].isin(traindata_types)
+        ]
+        nb_todo += len(labellocations_curr_gdf)
+    progress = ProgressLogger(message="prepare training images", nb_steps_total=nb_todo)
+    logger.info(f"Get images for {nb_todo} labels")
+
+    for traindata_type in traindata_types:
+        # Create output dirs...
+        output_imagedatatype_dir = output_tmp_dir / traindata_type
+        output_imagedata_image_dir = output_imagedatatype_dir / "image"
+        output_imagedata_mask_dir = output_imagedatatype_dir / "mask"
+        for dir in [
+            output_imagedatatype_dir,
+            output_imagedata_mask_dir,
+            output_imagedata_image_dir,
+        ]:
+            if dir and not dir.exists():
+                dir.mkdir(parents=True, exist_ok=True)
+
+        for labellocations_gdf, labels_to_burn_gdf in labeldata:
+            try:
+                # Get the label locations for this traindata type
+                labellocations_curr_gdf = labellocations_gdf[
+                    labellocations_gdf["traindata_type"] == traindata_type
+                ]
+
+                # Loop trough all locations labels to get an image for each of them
+                created_images_gdf = gpd.GeoDataFrame()
+                created_images_gdf["geometry"] = None
+                wms_imagelayer_layersources = {}
+                for i, label_tuple in enumerate(labellocations_curr_gdf.itertuples()):
+
+                    img_bbox = label_tuple.geometry
+                    image_layer = getattr(label_tuple, "image_layer")
+
+                    # If the wms to be used hasn't been initialised yet
+                    if image_layer not in wms_imagelayer_layersources:
+                        wms_imagelayer_layersources[image_layer] = []
+                        for layersource in image_layers[image_layer]["layersources"]:
+                            wms_service = owslib.wms.WebMapService(
+                                url=layersource["wms_server_url"],
+                                version=layersource["wms_version"],
+                                auth=auth,
+                            )
+                            if layersource["wms_ignore_capabilities_url"]:
+                                # If the wms url in capabilities should be ignored,
+                                # overwrite with original url
+                                nb = len(
+                                    wms_service.getOperationByName("GetMap").methods
+                                )
+                                for method_id in range(nb):
+                                    wms_service.getOperationByName("GetMap").methods[
+                                        method_id
+                                    ]["url"] = layersource["wms_server_url"]
+                            wms_imagelayer_layersources[image_layer].append(
+                                ows_util.LayerSource(
+                                    wms_service=wms_service,
+                                    layernames=layersource["layernames"],
+                                    layerstyles=layersource["layerstyles"],
+                                    bands=layersource["bands"],
+                                    random_sleep=layersource["random_sleep"],
+                                )
+                            )
+
+                    # Now really get the image
+                    logger.debug(f"Get image for coordinates {img_bbox.bounds}")
+                    assert labellocations_gdf.crs is not None
+                    image_filepath = ows_util.getmap_to_file(
+                        layersources=wms_imagelayer_layersources[image_layer],
+                        output_dir=output_imagedata_image_dir,
+                        crs=labellocations_gdf.crs,
+                        bbox=img_bbox.bounds,  # type: ignore
+                        size=(image_pixel_width, image_pixel_height),
+                        image_format=ows_util.FORMAT_PNG,
+                        # image_format_save=ows_util.FORMAT_TIFF,
+                        image_pixels_ignore_border=image_layers[image_layer][
+                            "image_pixels_ignore_border"
+                        ],
+                        transparent=False,
+                        layername_in_filename=True,
+                    )
+
+                    # Create a mask corresponding with the image file
+                    # image_filepath can be None if file exists, so check if not None...
+                    if image_filepath is not None:
+                        # Mask should not be in a lossy format!
+                        mask_filepath = Path(
+                            str(image_filepath)
+                            .replace(
+                                str(output_imagedata_image_dir),
+                                str(output_imagedata_mask_dir),
+                            )
+                            .replace(".jpg", ".png")
+                        )
+                        nb_classes = len(classes)
+
+                        # Only keep the labels that are meant for this image layer
+                        labels_for_layer_gdf = (
+                            labels_to_burn_gdf.loc[
+                                labels_to_burn_gdf["image_layer"] == image_layer
+                            ]
+                        ).copy()
+                        # assert to evade pyLance warning
+                        if len(labels_for_layer_gdf) == 0:
+                            logger.info(
+                                f"No polygons to burn for image_layer {image_layer}!"
+                            )
+                        assert isinstance(labels_for_layer_gdf, gpd.GeoDataFrame)
+                        _create_mask(
+                            input_image_filepath=image_filepath,
+                            output_mask_filepath=mask_filepath,
+                            labels_to_burn_gdf=labels_for_layer_gdf,
+                            nb_classes=nb_classes,
+                            force=force,
+                        )
+
+                    # Log the progress and prediction speed
+                    progress.step()
+
+            except Exception as ex:
+                raise ex
+
+    # If everything went fine, rename output_tmp_dir to the final output_dir
+    output_tmp_dir.rename(training_dataversion_dir)
+
+    return (training_dataversion_dir, dataversion_new)
+
+
+def prepare_labeldata(
+    label_infos: List[LabelInfo],
+    classes: dict,
+    labelname_column: str,
+    image_pixel_x_size: float,
+    image_pixel_y_size: float,
+    image_pixel_width: int,
+    image_pixel_height: int,
+) -> List[Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]]:
+    """
+    Prepare and validate the data in the labelinfos so it is ready to be uses to fetch
+    train images and burn masks.
+
+    Args:
+        label_infos (List[LabelInfo]): the label files/data.
+        classes (dict): dict with classes and their corresponding
+            label class names + weights.
+        labelname_column (str): the column name in the label polygon files where the
+            label classname can be found. Defaults to "classname".
+
+    Raises:
+        ValidationError: if the data is somehow not valid. All issues are listed in the
+            errors property.
+
+    Returns:
+        List[Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]]: returns a list of tuples with
+            geodataframes with labellocations and labelpolygons to burn.
+    """
+    labeldata_result = []
+    errors_found = []
+    labellocations_found = False
+    for label_info in label_infos:
+        # Read label locations if needed
+        if label_info.locations_gdf is not None:
+            labellocations_gdf = label_info.locations_gdf
+        else:
+            logger.debug(f"Read label locations from {label_info.locations_path}")
+            labellocations_gdf = gfo.read_file(label_info.locations_path)
+            if labellocations_gdf is not None and len(labellocations_gdf) > 0:
+                labellocations_gdf.loc[:, "path"] = str(label_info.locations_path)
+                labellocations_gdf.loc[:, "image_layer"] = label_info.image_layer
+                # Remark: geopandas 0.7.0 drops fid column internally!
+                labellocations_gdf.loc[
+                    :, "row_nb_orig"
+                ] = labellocations_gdf.index  # type: ignore
+            else:
+                logger.warn(f"No label locations found in {label_info.locations_path}")
+                continue
+
+        if len(labellocations_gdf) > 0:
+            labellocations_found = True
+
+        # Read label polygons if needed
+        if label_info.polygons_gdf is not None:
+            labelpolygons_gdf = label_info.polygons_gdf
+        else:
+            logger.debug(f"Read label data from {label_info.polygons_path}")
+            labelpolygons_gdf = gfo.read_file(label_info.polygons_path)
+            if labelpolygons_gdf is not None and len(labelpolygons_gdf) > 0:
+                labelpolygons_gdf.loc[:, "path"] = str(label_info.polygons_path)
+                labelpolygons_gdf.loc[:, "image_layer"] = label_info.image_layer
+            else:
+                logger.warn(f"No label polygons found in {label_info.polygons_path}")
+
+        assert labellocations_gdf is not None
+        assert labelpolygons_gdf is not None
+
+        if labellocations_gdf is None or len(labellocations_gdf) == 0:
+            errors_found.append("No label locations found in labellocations_gdf")
+            continue
+
+        # Validate + process the location data
+        # ------------------------------------
+        if "traindata_type" not in labellocations_gdf.columns:
+            errors_found.append(
+                "Mandatory column traindata_type not found in "
+                f"{label_info.locations_path}"
+            )
+
+        # Check + correct the geom of the location to make sure it matches the size of
+        # the training images/masks to be generated...
+        image_crs_width = math.fabs(
+            image_pixel_width * image_pixel_x_size
+        )  # tile width in units of crs => 500 m
+        image_crs_height = math.fabs(
+            image_pixel_height * image_pixel_y_size
+        )  # tile height in units of crs => 500 m
+        locations_none = []
+        for location in labellocations_gdf.itertuples():
+            if location.geometry is None or location.geometry.is_empty:
+                logger.warning(
+                    f"No or empty geometry found in file {Path(location.path).name} "
+                    f"for index {location.Index}, it will be ignored"
+                )
+                locations_none.append(location.Index)
+                continue
+
+            # Check if the traindata_type is valid
+            if location.traindata_type not in ["train", "validation", "test", "todo"]:
+                errors_found.append(
+                    f"Invalid traindata_type in {Path(location.path).name}: "
+                    f"{location.geometry.wkt}"
+                )
+
+            # Check if the geometry is valid
+            is_valid_reason = pygeos.is_valid_reason(
+                labellocations_gdf.geometry.array.data[location.Index]
+            )
+            if is_valid_reason != "Valid Geometry":
+                errors_found.append(
+                    f"Invalid geometry in {Path(location.path).name}: "
+                    f"{is_valid_reason}"
+                )
+                continue
+
+            geom_bounds = location.geometry.bounds
+            xmin = geom_bounds[0] - (geom_bounds[0] % image_pixel_x_size)
+            ymin = geom_bounds[1] - (geom_bounds[1] % image_pixel_y_size)
+            xmax = xmin + image_crs_width
+            ymax = ymin + image_crs_height
+            location_geom_aligned = sh_geom.box(xmin, ymin, xmax, ymax)
+
+            # Check if the realigned geom overlaps good enough with the original
+            intersection = location_geom_aligned.intersection(
+                labellocations_gdf.at[location.Index, "geometry"]
+            )
+            area_1row_1col = (
+                image_pixel_x_size * image_crs_width
+                + image_pixel_y_size * image_crs_height
+            )
+            if intersection.area < (location_geom_aligned.area - area_1row_1col):
+                # Original geom was digitized too small
+                errors_found.append(
+                    f"Location geometry too small in {Path(location.path).name}: "
+                    f"{location.geometry.wkt}"
+                )
+            elif location_geom_aligned.area > 1.1 * sh_geom.box(*geom_bounds).area:
+                logger.warn(
+                    "Location geometry larger than expected in file "
+                    f"{Path(location.path).name}: {location.geometry.wkt}"
+                )
+            labellocations_gdf.at[location.Index, "geometry"] = location_geom_aligned
+
+        # Remove locations with None or point/line geoms
+        labellocations_gdf = labellocations_gdf[
+            ~labellocations_gdf.index.isin(locations_none)
+        ]  # type: ignore
+
+        # Check if labellocations has a proper crs
+        if labellocations_gdf.crs is None:
+            errors_found.append(
+                "No crs in labellocations, labellocation_gdf.crs: "
+                f"{labellocations_gdf.crs}"
+            )
+
+        # Validate + process the polygons data
+        # ------------------------------------
+        if labelpolygons_gdf is None:
+            errors_found.append("No labelpolygons in the training data!")
+            continue
+
+        # Create list with only the input polygons that need to be burned in the mask
+        labels_to_burn_gdf = None
+        if labelname_column not in labelpolygons_gdf.columns:
+            # For backwards compatibility, also support old default column name
+            labelname_column = "label_name"
+        if labelname_column in labelpolygons_gdf.columns:
+            # If there is a column labelname_column, use the burn values specified in
+            # the configuration
+            labels_to_burn_gdf = labelpolygons_gdf
+            labels_to_burn_gdf.loc[:, "burn_value"] = None  # type: ignore
+            for classname in classes:
+                labels_to_burn_gdf.loc[
+                    (
+                        labels_to_burn_gdf[labelname_column].isin(
+                            classes[classname]["labelnames"]
+                        )
+                    ),
+                    "burn_value",
+                ] = classes[classname]["burn_value"]
+
+            # Check if there are invalid class names
+            invalid_gdf = labels_to_burn_gdf.loc[
+                labels_to_burn_gdf["burn_value"].isnull()
+            ]
+            for _, invalid_row in invalid_gdf.iterrows():
+                errors_found.append(
+                    f"Invalid classname in {Path(invalid_row['path']).name}: "
+                    f"{invalid_row[labelname_column]}"
+                )
+
+            # Filter away rows that are going to burn 0, as this is useless...
+            labels_to_burn_gdf = labels_to_burn_gdf.loc[
+                labels_to_burn_gdf["burn_value"] != 0
+            ].copy()
+
+        elif len(classes) == 2:
+            # There is no column with label names, but there are only 2 classes
+            # (background + subject), so no problem...
+            logger.info(
+                f"Column ({labelname_column}) not found, so use all polygons in "
+                f"{label_info.polygons_path.name}"
+            )
+            labels_to_burn_gdf = labelpolygons_gdf
+            labels_to_burn_gdf.loc[:, "burn_value"] = 1  # type: ignore
+
+        else:
+            # There is no column with label names, but more than two classes, so stop.
+            errors_found.append(
+                f"Column {labelname_column} is mandatory in labeldata if multiple "
+                f"classes specified: {classes}"
+            )
+
+        # Check if we ended up with label data to burn.
+        if labels_to_burn_gdf is None:
+            errors_found.append(
+                "Not any labelpolygon retained to burn in the training data!"
+            )
+            continue
+
+        # Filter away None and empty geometries... they cannot be burned
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", "GeoSeries.notna", UserWarning)
+            labels_to_burn_gdf = labels_to_burn_gdf[
+                ~labels_to_burn_gdf.geometry.is_empty
+                & labels_to_burn_gdf.geometry.notna()
+            ].copy()
+
+        # Make sure all label polygons are valid
+        labels_to_burn_gdf.loc[  # type: ignore
+            :, "is_valid_reason"
+        ] = vector_util.is_valid_reason(labels_to_burn_gdf.geometry)
+        invalid_gdf = labels_to_burn_gdf.query("is_valid_reason != 'Valid Geometry'")
+        for invalid in invalid_gdf.itertuples():
+            errors_found.append(
+                f"Invalid geometry in {Path(invalid.path).name}: "
+                f"{invalid.is_valid_reason}"
+            )
+
+        assert isinstance(labels_to_burn_gdf, gpd.GeoDataFrame)
+        labeldata_result.append((labellocations_gdf, labels_to_burn_gdf))
+
+    # If errors found, raise
+    if len(errors_found) > 0:
+        raise ValidationError(
+            f"Errors found in label data: {len(errors_found)}", errors_found
+        )
+    if not labellocations_found:
+        errors_found.append("No labellocations found in the training data")
+        raise ValidationError("No labellocations found", errors_found)
+
+    return labeldata_result
+
+
+def create_tmp_dir(
+    parent_dir: Path, dir_name: str, remove_existing: bool = False
+) -> Path:
+    """
+    Helper function to create a 'TMP' dir based on a directory name:
+        parent_dir / <dir_name>_TMP_<sequence>
+
+    Use: if you want to write data to a directory in a "transactional way",
+    it is the safest to write to a temp dir first, and then rename it to the
+    final name. This way, if a hard crash occurs while writing the data, it
+    is clear that the directory wasn't ready. Additionally, in case of a hard
+    crash, file locks can remain which makes it impossible to remove a
+    directory for a while.
+
+    Args:
+        parent_dir (Path): The dir to create the temp dir in.
+        dir_name (str): The name of the dir to base the temp dir on.
+        remove_existing (bool, optional): If True, existing TMP directories
+            will be removed if possible. Defaults to False.
+
+    Raises:
+        Exception: [description]
+
+    Returns:
+        Path: [description]
+    """
+    # The final dir should not exists yet!
+    final_dir = parent_dir / dir_name
+    if final_dir.exists():
+        raise Exception(
+            f"It is not supported to create a TMP dir for an existing dir: {final_dir}"
+        )
+
+    # Try to delete all existing TMP dir's
+    if remove_existing is True:
+        existing_tmp_dirs = parent_dir.glob(f"{dir_name}_TMP_*")
+        for existing_tmp_dir in existing_tmp_dirs:
+            try:
+                shutil.rmtree(existing_tmp_dir)
+            except Exception:
+                tmp_dir = None
+
+    # Create the TMP dir
+    tmp_dir = None
+    for i in range(100):
+        tmp_dir = parent_dir / f"{dir_name}_TMP_{i:02d}"
+
+        if tmp_dir.exists():
+            # If it (still) exists try next sequence
+            tmp_dir = None
+            continue
+        else:
+            # If it doesn't exist, try to create it
+            try:
+                tmp_dir.mkdir(parents=True)
+                break
+            except Exception:
+                # If it fails to create, try next sequence
+                tmp_dir = None
+                continue
+
+    # If no output tmp dir could be found/created... stop...
+    if tmp_dir is None:
+        raise Exception(
+            f"Error creating/replacing TMP dir for {dir_name} in {parent_dir}"
+        )
+
+    return tmp_dir
+
+
+def _create_mask(
+    input_image_filepath: Path,
+    output_mask_filepath: Path,
+    labels_to_burn_gdf: gpd.GeoDataFrame,
+    nb_classes: int = 1,
+    output_imagecopy_filepath: Optional[Path] = None,
+    minimum_pct_labeled: float = 0.0,
+    force: bool = False,
+) -> Optional[bool]:
+
+    # If file exists already and force is False... stop.
+    if force is False and output_mask_filepath.exists():
+        logger.debug(
+            f"Output file exist, and force is False, return: {output_mask_filepath}"
+        )
+        return
+
+    # Create a mask corresponding with the image file
+    # First read the properties of the input image to copy them for the output
+    logger.debug(f"Create mask to {output_mask_filepath}")
+    with rio.open(input_image_filepath) as image_ds:
+        image_input_profile = image_ds.profile
+        image_transform_affine = image_ds.transform
+
+    # Prepare the file profile for the mask depending on output type
+    output_ext_lower = output_mask_filepath.suffix.lower()
+    if output_ext_lower == ".tif":
+        image_output_profile = rio_profiles.DefaultGTiffProfile(
+            count=1, transform=image_transform_affine, crs=image_input_profile["crs"]
+        )
+    if output_ext_lower == ".png":
+        image_output_profile = rio_profiles.Profile(driver="PNG", count=1)
+    else:
+        raise Exception(
+            f"Unsupported mask suffix (should be lossless format!): {output_ext_lower}"
+        )
+    image_output_profile.update(
+        width=image_input_profile["width"],
+        height=image_input_profile["height"],
+        dtype=rio.uint8,
+    )
+
+    # Burn the vectors in a mask
+    burn_shapes = [
+        (geom, value)
+        for geom, value in zip(
+            labels_to_burn_gdf.geometry, labels_to_burn_gdf.burn_value
+        )
+        if geom is not None and geom.is_empty is False
+    ]
+    if len(burn_shapes) > 0:
+        try:
+            mask_arr = rio_features.rasterize(
+                shapes=burn_shapes,
+                transform=image_transform_affine,
+                dtype=rio.uint8,
+                fill=0,
+                out_shape=(
+                    image_output_profile["width"],  # type: ignore
+                    image_output_profile["height"],  # type: ignore
+                ),
+            )
+
+        except Exception as ex:
+            raise Exception(f"Error creating mask for {image_transform_affine}") from ex
+    else:
+        mask_arr = np.zeros(
+            shape=(
+                image_output_profile["width"],  # type: ignore
+                image_output_profile["height"],  # type: ignore
+            ),
+            dtype=rio.uint8,
+        )
+
+    # Check if the mask meets the requirements to be written...
+    if minimum_pct_labeled > 0:
+        nb_pixels = np.size(mask_arr, 0) * np.size(mask_arr, 1)
+        nb_pixels_data = nb_pixels - np.sum(
+            mask_arr == 0
+        )  # np.count_nonnan(image == NoData_value)
+        logger.debug(
+            f"nb_pixels: {nb_pixels}, nb_pixels_data: {nb_pixels_data}, "
+            f"pct data: {nb_pixels_data / nb_pixels}"
+        )
+
+        if nb_pixels_data / nb_pixels < minimum_pct_labeled:
+            return False
+
+    # Write the labeled mask as .png (so without transform/crs info)
+    im = Image.fromarray(mask_arr)
+    im.save(output_mask_filepath)
+
+    return True
```

### Comparing `orthoseg-0.4.2/orthoseg/lib/trainer.py` & `orthoseg-0.4.2a1/orthoseg/lib/trainer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,609 +1,609 @@
-# -*- coding: utf-8 -*-
-"""
-Module with high-level operations to segment images.
-"""
-
-import logging
-import math
-import os
-from pathlib import Path
-from typing import Tuple, Optional
-
-import numpy as np
-import tensorflow as tf
-from tensorflow import keras as kr
-
-# import keras as kr
-
-import pandas as pd
-from PIL import Image
-
-import orthoseg.model.model_factory as mf
-import orthoseg.model.model_helper as mh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def train(
-    traindata_dir: Path,
-    validationdata_dir: Path,
-    model_save_dir: Path,
-    segment_subject: str,
-    traindata_id: int,
-    hyperparams: mh.HyperParams,
-    model_preload_filepath: Optional[Path] = None,
-    image_width: int = 512,
-    image_height: int = 512,
-    image_subdir: str = "image",
-    mask_subdir: str = "mask",
-    save_augmented_subdir: Optional[str] = None,
-):
-    """
-    Create a new or load an existing neural network and train it using
-    data from the train and validation directories specified.
-
-    The best models will be saved to model_save_dir. The filenames of the
-    models will be constructed like this:
-    {model_save_base_filename}_{combined_acc}_{train_acc}_{validation_acc}_{epoch}
-        * combined_acc: average of train_acc and validation_acc
-        * train_acc: the jaccard coëficient of train dataset for the model
-        * validation_acc: the jaccard coëficient of validation dataset
-    In the scripts, if the "best model" is mentioned, this is the one with the
-    highest "combined_acc".
-
-    Args
-        traindata_dir: dir where the train data is located
-        validationdata_dir: dir where the validation data is located
-        model_save_dir: dir where (intermediate) best models will be saved
-        segment_subject (str): segment subject
-        traindata_id (int): train data version
-        hyperparams (mh.HyperParams): the hyper parameters to use for the model
-        image_width: width the input images will be rescaled to for training
-        image_height: height the input images will be rescaled to for training
-        image_subdir: subdir where the images can be found in traindata_dir and
-            validationdata_dir
-        mask_subdir: subdir where the corresponding masks can be found in traindata_dir
-            and validationdata_dir
-        model_preload_filepath: filepath to the model to continue training on,
-            or None if you want to start from scratch
-    """
-    # These are the augmentations that will be applied to the input training
-    # images/masks.
-    # Remark: fill_mode + cval are defined as they are so missing pixels after
-    #    eg. rotation are filled with 0, and so the mask will take care that they are
-    #    +- ignored.
-
-    # Create the train generator
-    train_gen = create_train_generator(
-        input_data_dir=traindata_dir,
-        image_subdir=image_subdir,
-        mask_subdir=mask_subdir,
-        image_augment_dict=hyperparams.train.image_augmentations,
-        mask_augment_dict=hyperparams.train.mask_augmentations,
-        batch_size=hyperparams.train.batch_size,
-        target_size=(image_width, image_height),
-        nb_classes=len(hyperparams.architecture.classes),
-        save_to_subdir=save_augmented_subdir,
-        seed=2,
-    )
-
-    # Create validation generator
-    validation_augmentations = dict(
-        rescale=hyperparams.train.image_augmentations["rescale"]
-    )
-    validation_mask_augmentations = dict(
-        rescale=hyperparams.train.mask_augmentations["rescale"]
-    )
-    validation_gen = create_train_generator(
-        input_data_dir=validationdata_dir,
-        image_subdir=image_subdir,
-        mask_subdir=mask_subdir,
-        image_augment_dict=validation_augmentations,
-        mask_augment_dict=validation_mask_augmentations,
-        batch_size=hyperparams.train.batch_size,
-        target_size=(image_width, image_height),
-        nb_classes=len(hyperparams.architecture.classes),
-        save_to_subdir=save_augmented_subdir,
-        shuffle=False,
-        seed=3,
-    )
-
-    # Get the max epoch number from the log file if it exists...
-    start_epoch = 0
-    model_save_base_filename = mh.format_model_basefilename(
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        architecture_id=hyperparams.architecture.architecture_id,
-        trainparams_id=hyperparams.train.trainparams_id,
-    )
-    csv_log_filepath = model_save_dir / (model_save_base_filename + "_log.csv")
-    if csv_log_filepath.exists() and os.path.getsize(csv_log_filepath) > 0:
-        if not model_preload_filepath:
-            message = (
-                "log file exists but preload model file not specified: "
-                f"{csv_log_filepath}"
-            )
-            logger.critical(message)
-            raise Exception(message)
-
-        train_log_df = pd.read_csv(
-            csv_log_filepath, sep=";", usecols=["epoch", "lr"]
-        )
-        assert isinstance(train_log_df, pd.DataFrame)
-        logger.debug(f"train_log csv contents:\n{train_log_df}")
-        start_epoch = train_log_df["epoch"].max()
-        hyperparams.train.optimizer_params["learning_rate"] = float(
-            pd.to_numeric(train_log_df["lr"], downcast="float").min()
-        )
-    logger.info(
-        f"start_epoch: {start_epoch}, learning_rate: "
-        f"{hyperparams.train.optimizer_params['learning_rate']}"
-    )
-
-    # If no existing model provided, create it from scratch
-    if not model_preload_filepath:
-        # If the encode should be frozen for some epochs...
-        if hyperparams.train.nb_epoch_with_freeze > 0:
-            freeze = True
-        else:
-            freeze = False
-
-        # Get the model we want to use
-        model = mf.get_model(
-            architecture=hyperparams.architecture.architecture,
-            nb_channels=hyperparams.architecture.nb_channels,
-            nb_classes=len(hyperparams.architecture.classes),
-            activation=hyperparams.architecture.activation_function,
-            freeze=freeze,
-        )
-
-        # Save the model architecture to json
-        model_json_filepath = model_save_dir / f"{model_save_base_filename}_model.json"
-        if not model_save_dir.exists():
-            model_save_dir.mkdir(parents=True)
-        if not model_json_filepath.exists():
-            with model_json_filepath.open("w") as dst:
-                dst.write(str(model.to_json()))
-    else:
-        # If a preload model is provided, load that if it exists...
-        if not model_preload_filepath.exists():
-            message = (
-                f"Error: preload model file doesn't exist: {model_preload_filepath}"
-            )
-            logger.critical(message)
-            raise Exception(message)
-
-        # Load the existing model
-        # Remark: compiling during load crashes, so compile 'manually'
-        logger.info(f"Load model from {model_preload_filepath}")
-        model = mf.load_model(model_preload_filepath, compile=False)
-
-    # Now prepare the model for training
-    nb_gpu = len(tf.config.experimental.list_physical_devices("GPU"))
-
-    # TODO: because of bug in tensorflow 1.14, multi GPU doesn't work (this way),
-    # so always use standard model
-    if nb_gpu <= 1:
-        model_for_train = mf.compile_model(
-            model=model,
-            optimizer=hyperparams.train.optimizer,
-            optimizer_params=hyperparams.train.optimizer_params,
-            loss=hyperparams.train.loss_function,
-            class_weights=hyperparams.train.class_weights,
-        )
-        logger.info(f"Train using single GPU or CPU, with nb_gpu: {nb_gpu}")
-    else:
-        # If multiple GPU's available, should create a multi-GPU model
-        model_for_train = model
-        logger.info(f"Train using all GPU's, with nb_gpu: {nb_gpu}")
-        logger.warn("MULTI GPU TRAINING NOT TESTED BUT WILL BE TRIED ANYWAY")
-        strategy = tf.distribute.MirroredStrategy()
-        with strategy.scope():
-            model_for_train = mf.compile_model(
-                model=model,
-                optimizer=hyperparams.train.optimizer,
-                optimizer_params=hyperparams.train.optimizer_params,
-                loss=hyperparams.train.loss_function,
-                class_weights=hyperparams.train.class_weights,
-            )
-
-    # Define some callbacks for the training
-    train_callbacks = []
-    # Reduce the learning rate if the loss doesn't improve anymore
-    reduce_lr = kr.callbacks.ReduceLROnPlateau(
-        monitor="loss", factor=0.2, patience=20, min_lr=1e-20, verbose=True
-    )
-    train_callbacks.append(reduce_lr)
-
-    # Custom callback that saves the best models using both train and
-    # validation metric
-    # Remark: the save of the model should be done on the standard model, not
-    #         on the parallel_model, otherwise issues to use it afterwards
-    if nb_gpu > 1:
-        model_template_for_save = model
-    else:
-        model_template_for_save = None
-    model_checkpoint_saver = mh.ModelCheckpointExt(
-        model_save_dir=model_save_dir,
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        architecture_id=hyperparams.architecture.architecture_id,
-        trainparams_id=hyperparams.train.trainparams_id,
-        monitor_metric=hyperparams.train.monitor_metric,
-        monitor_metric_mode=hyperparams.train.monitor_metric_mode,
-        save_format=hyperparams.train.save_format,
-        save_best_only=hyperparams.train.save_best_only,
-        save_min_accuracy=hyperparams.train.save_min_accuracy,
-        model_template_for_save=model_template_for_save,
-    )
-    train_callbacks.append(model_checkpoint_saver)
-
-    # Callbacks for logging
-    if hyperparams.train.log_tensorboard is True:
-        tensorboard_log_dir = model_save_dir / (
-            model_save_base_filename + "_tensorboard_log"
-        )
-        tensorboard_logger = kr.callbacks.TensorBoard(log_dir=str(tensorboard_log_dir))
-        train_callbacks.append(tensorboard_logger)
-    if hyperparams.train.log_csv is True:
-        csv_logger = kr.callbacks.CSVLogger(
-            str(csv_log_filepath), append=True, separator=";"
-        )
-        train_callbacks.append(csv_logger)
-
-    # Stop if no more improvement
-    early_stopping = kr.callbacks.EarlyStopping(
-        monitor=hyperparams.train.earlystop_monitor_metric,
-        patience=hyperparams.train.earlystop_patience,
-        mode=hyperparams.train.earlystop_monitor_metric_mode,
-        restore_best_weights=False,
-    )
-    train_callbacks.append(early_stopping)
-
-    # Prepare the parameters to pass to fit...
-    # Supported filetypes to train/validate on
-    input_ext = [".tif", ".jpg", ".png"]
-
-    # Calculate the size of the input datasets
-    # train_dataset_size = len(glob.glob(f"{traindata_dir}/{image_subdir}/*.*"))
-    train_dataset_size = 0
-    for input_ext_cur in input_ext:
-        traindata_image_dir = traindata_dir / image_subdir
-        train_dataset_size += len(list(traindata_image_dir.rglob("*" + input_ext_cur)))
-    validation_dataset_size = 0
-    for input_ext_cur in input_ext:
-        validationdata_image_dir = validationdata_dir / image_subdir
-        validation_dataset_size += len(
-            list(validationdata_image_dir.rglob("*" + input_ext_cur))
-        )
-
-    # Calculate the number of steps within an epoch
-    # Remark: number of steps per epoch should be at least 1, even if nb samples
-    # < batch size...
-    train_steps_per_epoch = math.ceil(train_dataset_size / hyperparams.train.batch_size)
-    validation_steps_per_epoch = math.ceil(
-        validation_dataset_size / hyperparams.train.batch_size
-    )
-
-    # Start training
-    logger.info(
-        f"Start training with batch_size: {hyperparams.train.batch_size}, "
-        f"train_dataset_size: {train_dataset_size}, train_steps_per_epoch: "
-        f"{train_steps_per_epoch}, validation_dataset_size: {validation_dataset_size}, "
-        f"validation_steps_per_epoch: {validation_steps_per_epoch}"
-    )
-
-    logger.info(f"{hyperparams.toJSON()}")
-    hyperparams_filepath = (
-        model_save_dir / f"{model_save_base_filename}_hyperparams.json"
-    )
-    hyperparams_filepath.write_text(hyperparams.toJSON())
-
-    try:
-        # If the encoder should be frozen for the first epochs, do so
-        if hyperparams.train.nb_epoch_with_freeze > 0:
-            logger.info(
-                f"First train for {hyperparams.train.nb_epoch_with_freeze} epochs with "
-                "frozen layers"
-            )
-            model_for_train.fit(
-                train_gen,
-                steps_per_epoch=train_steps_per_epoch,
-                epochs=hyperparams.train.nb_epoch_with_freeze,
-                validation_data=validation_gen,
-                # Number of items in validation/batch_size
-                validation_steps=validation_steps_per_epoch,
-                callbacks=train_callbacks,
-                initial_epoch=start_epoch,
-                verbose=2,  # type: ignore
-            )
-            mf.set_trainable(model=model_for_train, recompile=False)
-            model_for_train = mf.compile_model(
-                model=model_for_train,
-                optimizer=hyperparams.train.optimizer,
-                optimizer_params=hyperparams.train.optimizer_params,
-                loss=hyperparams.train.loss_function,
-                class_weights=hyperparams.train.class_weights,
-            )
-
-        # Train!
-        model_for_train.fit(
-            train_gen,
-            steps_per_epoch=train_steps_per_epoch,
-            epochs=hyperparams.train.nb_epoch,
-            validation_data=validation_gen,
-            # Number of items in validation/batch_size
-            validation_steps=validation_steps_per_epoch,
-            callbacks=train_callbacks,
-            initial_epoch=start_epoch,
-            verbose=2,  # type: ignore
-        )
-
-        # Write some reporting
-        train_report_path = model_save_dir / (model_save_base_filename + "_report.pdf")
-        train_log_df = pd.read_csv(csv_log_filepath, sep=";")
-        assert isinstance(train_log_df, pd.DataFrame)
-        columns_to_keep = []
-        for column in train_log_df.columns:
-            if column.endswith("accuracy") or column.endswith("f1-score"):
-                columns_to_keep.append(column)
-
-        train_log_vis_df = train_log_df[columns_to_keep]
-        train_log_vis_df.plot().get_figure().savefig(str(train_report_path))
-
-    finally:
-        # Release the memory from the GPU...
-        # from keras import backend as K
-        # K.clear_session()
-        kr.backend.clear_session()
-
-
-def create_train_generator(
-    input_data_dir: Path,
-    image_subdir: str,
-    mask_subdir: str,
-    image_augment_dict: dict,
-    mask_augment_dict: dict,
-    batch_size: int = 32,
-    image_color_mode: str = "rgb",
-    mask_color_mode: str = "grayscale",
-    save_to_subdir: Optional[str] = None,
-    image_save_prefix: str = "image",
-    mask_save_prefix: str = "mask",
-    nb_classes: int = 1,
-    target_size: Tuple[int, int] = (256, 256),
-    shuffle: bool = True,
-    seed: int = 1,
-):
-    """
-    Creates a generator to generate and augment train images. The augmentations
-    specified in aug_dict will be applied. For the augmentations that can be
-    specified in aug_dict look at the documentation of
-    keras.preprocessing.image.ImageDataGenerator
-
-    For more info about the other parameters, check keras flow_from_directory.
-
-    Remarks: * use the same seed for image_datagen and mask_datagen to ensure
-               the transformation for image and mask is the same
-             * set save_to_dir = "your path" to check results of the generator
-    """
-    # Init
-    # Do some checks on the augmentations specified, as it is easy to
-    # introduce illogical values
-    if (
-        image_augment_dict is not None
-        and mask_augment_dict is None
-        or image_augment_dict is not None
-        and mask_augment_dict is None
-    ):
-        logger.warn(
-            "Only augmentations specified for either image or mask: "
-            f"image_augment_dict: {image_augment_dict}, mask_augment_dict: "
-            f"{mask_augment_dict}"
-        )
-
-    # Checks that involve comparing augmentations between the image and the mask
-    if image_augment_dict is not None and mask_augment_dict is not None:
-        # If an augmentation is specified for image, it should be specified
-        # for the mask as well and the other way around to evade issues
-        for augmentation in image_augment_dict:
-            if augmentation not in mask_augment_dict:
-                raise Exception(
-                    f"{augmentation} in image_augment_dict but not in mask_augment_dict"
-                )
-        for augmentation in mask_augment_dict:
-            if augmentation not in image_augment_dict:
-                raise Exception(
-                    f"{augmentation} in mask_augment_dict but not in image_augment_dict"
-                )
-
-        # Check if the brightness range has valid values
-        image_brightness_range = image_augment_dict.get("brightness_range")
-        mask_brightness_range = mask_augment_dict.get("brightness_range")
-        if image_brightness_range is None and mask_brightness_range is not None:
-            # If brightness_range None for image, it should be None for the mask as well
-            raise Exception(
-                "augmentation brightness_range is None (null) in image_augment_dict "
-                f"but isn't in mask_augment_dict: {mask_brightness_range}"
-            )
-        elif image_brightness_range is not None and mask_brightness_range is None:
-            # If brightness_range None for mask, it should be None for the image as well
-            raise Exception(
-                "augmentation brightness_range is None (null) in mask_augment_dict but "
-                f"isn't in image_augment_dict: {image_brightness_range}"
-            )
-        elif image_brightness_range is not None and mask_brightness_range is not None:
-            # The brightness_range values should be >= 0
-            if image_brightness_range[0] < 0 or image_brightness_range[1] < 0:
-                raise Exception(
-                    "augmentation brightness_range values should be > 0: value 1.0 = "
-                    "don't do anything, 0 = black"
-                )
-            # brightness_range is applied to the image, it should be [1,1] for the mask
-            if mask_brightness_range[0] != 1.0 or mask_brightness_range[1] != 1.0:
-                raise Exception(
-                    "augmentation brightness_range is specified on the image: then the "
-                    f"mask should get range [1, 1], not {mask_brightness_range}"
-                )
-
-    # Some checks specific for the mask
-    if mask_augment_dict is not None:
-        # Check cval value
-        if "cval" in mask_augment_dict and mask_augment_dict["cval"] != 0:
-            logger.warn(
-                "cval typically should be 0 for the mask, even if it is different for "
-                "the image, as the cval of the mask refers to these locations being of "
-                f"class 'background'. It is: {mask_augment_dict['cval']}"
-            )
-
-        # If there are more than two classes, the mask will have integers as values
-        # to code the different masks in, and one hot-encoding will be applied to
-        # it, so it should not be rescaled!!!
-        if (
-            nb_classes > 2
-            and "rescale" in mask_augment_dict
-            and mask_augment_dict["rescale"] != 1
-        ):
-            raise Exception(
-                f"With nb_classes > 2 ({nb_classes}), the mask should have a rescale "
-                f"value of 1, not {mask_augment_dict['rescale']}"
-            )
-
-    # Now create the generators
-    # Create the image generators with the augment info
-
-    # TODO: brightness_range is buggy on 2021-08-11, with keras preprocessing
-    # version 1.1, so is implemented here in a hacky way!
-    image_augment_dict_temp = {
-        key: value
-        for (key, value) in image_augment_dict.items()
-        if key != "brightness_range"
-    }
-    mask_augment_dict_temp = {
-        key: value
-        for (key, value) in mask_augment_dict.items()
-        if key != "brightness_range"
-    }
-    image_datagen = kr.preprocessing.image.ImageDataGenerator(**image_augment_dict_temp)
-    mask_datagen = kr.preprocessing.image.ImageDataGenerator(**mask_augment_dict_temp)
-
-    # Format save_to_dir
-    # Remark: flow_from_directory doesn't support Path, so supply str immediately as
-    # well, otherwise, if str(Path) is used later on, it becomes 'None' instead of None!
-    save_to_dir = None
-    if save_to_subdir is not None:
-        save_to_dir = input_data_dir / save_to_subdir
-        if not save_to_dir.exists():
-            save_to_dir.mkdir(parents=True)
-
-    image_generator = image_datagen.flow_from_directory(
-        directory=str(input_data_dir),
-        classes=[image_subdir],
-        class_mode=None,
-        color_mode=image_color_mode,
-        target_size=target_size,
-        batch_size=batch_size,
-        save_to_dir=None,
-        save_prefix=image_save_prefix,
-        shuffle=shuffle,
-        seed=seed,
-    )
-
-    mask_generator = mask_datagen.flow_from_directory(
-        directory=str(input_data_dir),
-        classes=[mask_subdir],
-        class_mode=None,
-        color_mode=mask_color_mode,
-        target_size=target_size,
-        batch_size=batch_size,
-        save_to_dir=None,
-        save_prefix=mask_save_prefix,
-        shuffle=shuffle,
-        seed=seed,
-    )
-
-    train_generator = zip(image_generator, mask_generator)
-
-    for batch_id, (image, mask) in enumerate(train_generator):
-        # Cast to arrays to evade type errors
-        image = np.array(image)
-        mask = np.array(mask)
-
-        # TODO: brightness_range is buggy on 2021-08-11, with keras preprocessing
-        # version 1.1, so is implemented here in a hacky way!
-        if (
-            "brightness_range" in image_augment_dict
-            and image_augment_dict["brightness_range"] is not None
-            and (
-                image_augment_dict["brightness_range"][0] != 1
-                or image_augment_dict["brightness_range"][1] != 1
-            )
-        ):
-
-            # Random brightness shift to apply to all images in batch
-            brightness_shift = np.random.uniform(
-                image_augment_dict["brightness_range"][0],
-                image_augment_dict["brightness_range"][1],
-            )
-            image = image * brightness_shift
-
-        # One-hot encode mask if multiple classes
-        if nb_classes > 1:
-            mask = kr.utils.to_categorical(mask, nb_classes)
-
-        # Because the default save_to_dir option doesn't support saving the
-        # augmented masks in seperate files per class, implement this here.
-        if save_to_dir is not None:
-            # Save mask for every class seperately
-            # Get the number of images in this batch + the nb classes
-            mask_shape = mask.shape
-            nb_images = mask_shape[0]
-            nb_classes = mask_shape[3]
-
-            # Loop through images in this batch
-            for image_id in range(nb_images):
-                # Slice the next image from the array
-                image_to_save = image[image_id, :, :, :]
-
-                # Reverse the rescale if there is one
-                if (
-                    image_augment_dict is not None
-                    and "rescale" in image_augment_dict
-                    and image_augment_dict["rescale"] != 1
-                ):
-                    image_to_save = image_to_save / image_augment_dict["rescale"]
-
-                # Now convert to uint8 image and save!
-                # , image_color_mode
-                colormode = None
-                if image_color_mode.upper() == "RGB":
-                    colormode = "RGB"
-                im = Image.fromarray(image_to_save.astype(np.uint8), mode=colormode)
-                image_dir = save_to_dir / f"{batch_id:0>4}"
-                image_dir.mkdir(parents=True, exist_ok=True)
-                image_path = image_dir / f"{image_id}_image.jpg"
-                im.save(image_path)
-
-                # Loop through the masks for each class
-                for channel_id in range(nb_classes):
-                    mask_to_save = mask[image_id, :, :, channel_id]
-                    mask_dir = save_to_dir / f"{batch_id:0>4}"
-                    mask_path = mask_dir / f"{image_id}_mask_{channel_id}.png"
-                    im = Image.fromarray((mask_to_save * 255).astype(np.uint8))
-                    im.save(mask_path)
-
-        yield (image, mask)
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module with high-level operations to segment images.
+"""
+
+import logging
+import math
+import os
+from pathlib import Path
+from typing import Tuple, Optional
+
+import numpy as np
+import tensorflow as tf
+from tensorflow import keras as kr
+
+# import keras as kr
+
+import pandas as pd
+from PIL import Image
+
+import orthoseg.model.model_factory as mf
+import orthoseg.model.model_helper as mh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def train(
+    traindata_dir: Path,
+    validationdata_dir: Path,
+    model_save_dir: Path,
+    segment_subject: str,
+    traindata_id: int,
+    hyperparams: mh.HyperParams,
+    model_preload_filepath: Optional[Path] = None,
+    image_width: int = 512,
+    image_height: int = 512,
+    image_subdir: str = "image",
+    mask_subdir: str = "mask",
+    save_augmented_subdir: Optional[str] = None,
+):
+    """
+    Create a new or load an existing neural network and train it using
+    data from the train and validation directories specified.
+
+    The best models will be saved to model_save_dir. The filenames of the
+    models will be constructed like this:
+    {model_save_base_filename}_{combined_acc}_{train_acc}_{validation_acc}_{epoch}
+        * combined_acc: average of train_acc and validation_acc
+        * train_acc: the jaccard coëficient of train dataset for the model
+        * validation_acc: the jaccard coëficient of validation dataset
+    In the scripts, if the "best model" is mentioned, this is the one with the
+    highest "combined_acc".
+
+    Args
+        traindata_dir: dir where the train data is located
+        validationdata_dir: dir where the validation data is located
+        model_save_dir: dir where (intermediate) best models will be saved
+        segment_subject (str): segment subject
+        traindata_id (int): train data version
+        hyperparams (mh.HyperParams): the hyper parameters to use for the model
+        image_width: width the input images will be rescaled to for training
+        image_height: height the input images will be rescaled to for training
+        image_subdir: subdir where the images can be found in traindata_dir and
+            validationdata_dir
+        mask_subdir: subdir where the corresponding masks can be found in traindata_dir
+            and validationdata_dir
+        model_preload_filepath: filepath to the model to continue training on,
+            or None if you want to start from scratch
+    """
+    # These are the augmentations that will be applied to the input training
+    # images/masks.
+    # Remark: fill_mode + cval are defined as they are so missing pixels after
+    #    eg. rotation are filled with 0, and so the mask will take care that they are
+    #    +- ignored.
+
+    # Create the train generator
+    train_gen = create_train_generator(
+        input_data_dir=traindata_dir,
+        image_subdir=image_subdir,
+        mask_subdir=mask_subdir,
+        image_augment_dict=hyperparams.train.image_augmentations,
+        mask_augment_dict=hyperparams.train.mask_augmentations,
+        batch_size=hyperparams.train.batch_size,
+        target_size=(image_width, image_height),
+        nb_classes=len(hyperparams.architecture.classes),
+        save_to_subdir=save_augmented_subdir,
+        seed=2,
+    )
+
+    # Create validation generator
+    validation_augmentations = dict(
+        rescale=hyperparams.train.image_augmentations["rescale"]
+    )
+    validation_mask_augmentations = dict(
+        rescale=hyperparams.train.mask_augmentations["rescale"]
+    )
+    validation_gen = create_train_generator(
+        input_data_dir=validationdata_dir,
+        image_subdir=image_subdir,
+        mask_subdir=mask_subdir,
+        image_augment_dict=validation_augmentations,
+        mask_augment_dict=validation_mask_augmentations,
+        batch_size=hyperparams.train.batch_size,
+        target_size=(image_width, image_height),
+        nb_classes=len(hyperparams.architecture.classes),
+        save_to_subdir=save_augmented_subdir,
+        shuffle=False,
+        seed=3,
+    )
+
+    # Get the max epoch number from the log file if it exists...
+    start_epoch = 0
+    model_save_base_filename = mh.format_model_basefilename(
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        architecture_id=hyperparams.architecture.architecture_id,
+        trainparams_id=hyperparams.train.trainparams_id,
+    )
+    csv_log_filepath = model_save_dir / (model_save_base_filename + "_log.csv")
+    if csv_log_filepath.exists() and os.path.getsize(csv_log_filepath) > 0:
+        if not model_preload_filepath:
+            message = (
+                "log file exists but preload model file not specified: "
+                f"{csv_log_filepath}"
+            )
+            logger.critical(message)
+            raise Exception(message)
+
+        train_log_df = pd.read_csv(
+            csv_log_filepath, sep=";", usecols=["epoch", "lr"]
+        )
+        assert isinstance(train_log_df, pd.DataFrame)
+        logger.debug(f"train_log csv contents:\n{train_log_df}")
+        start_epoch = train_log_df["epoch"].max()
+        hyperparams.train.optimizer_params["learning_rate"] = float(
+            pd.to_numeric(train_log_df["lr"], downcast="float").min()
+        )
+    logger.info(
+        f"start_epoch: {start_epoch}, learning_rate: "
+        f"{hyperparams.train.optimizer_params['learning_rate']}"
+    )
+
+    # If no existing model provided, create it from scratch
+    if not model_preload_filepath:
+        # If the encode should be frozen for some epochs...
+        if hyperparams.train.nb_epoch_with_freeze > 0:
+            freeze = True
+        else:
+            freeze = False
+
+        # Get the model we want to use
+        model = mf.get_model(
+            architecture=hyperparams.architecture.architecture,
+            nb_channels=hyperparams.architecture.nb_channels,
+            nb_classes=len(hyperparams.architecture.classes),
+            activation=hyperparams.architecture.activation_function,
+            freeze=freeze,
+        )
+
+        # Save the model architecture to json
+        model_json_filepath = model_save_dir / f"{model_save_base_filename}_model.json"
+        if not model_save_dir.exists():
+            model_save_dir.mkdir(parents=True)
+        if not model_json_filepath.exists():
+            with model_json_filepath.open("w") as dst:
+                dst.write(str(model.to_json()))
+    else:
+        # If a preload model is provided, load that if it exists...
+        if not model_preload_filepath.exists():
+            message = (
+                f"Error: preload model file doesn't exist: {model_preload_filepath}"
+            )
+            logger.critical(message)
+            raise Exception(message)
+
+        # Load the existing model
+        # Remark: compiling during load crashes, so compile 'manually'
+        logger.info(f"Load model from {model_preload_filepath}")
+        model = mf.load_model(model_preload_filepath, compile=False)
+
+    # Now prepare the model for training
+    nb_gpu = len(tf.config.experimental.list_physical_devices("GPU"))
+
+    # TODO: because of bug in tensorflow 1.14, multi GPU doesn't work (this way),
+    # so always use standard model
+    if nb_gpu <= 1:
+        model_for_train = mf.compile_model(
+            model=model,
+            optimizer=hyperparams.train.optimizer,
+            optimizer_params=hyperparams.train.optimizer_params,
+            loss=hyperparams.train.loss_function,
+            class_weights=hyperparams.train.class_weights,
+        )
+        logger.info(f"Train using single GPU or CPU, with nb_gpu: {nb_gpu}")
+    else:
+        # If multiple GPU's available, should create a multi-GPU model
+        model_for_train = model
+        logger.info(f"Train using all GPU's, with nb_gpu: {nb_gpu}")
+        logger.warn("MULTI GPU TRAINING NOT TESTED BUT WILL BE TRIED ANYWAY")
+        strategy = tf.distribute.MirroredStrategy()
+        with strategy.scope():
+            model_for_train = mf.compile_model(
+                model=model,
+                optimizer=hyperparams.train.optimizer,
+                optimizer_params=hyperparams.train.optimizer_params,
+                loss=hyperparams.train.loss_function,
+                class_weights=hyperparams.train.class_weights,
+            )
+
+    # Define some callbacks for the training
+    train_callbacks = []
+    # Reduce the learning rate if the loss doesn't improve anymore
+    reduce_lr = kr.callbacks.ReduceLROnPlateau(
+        monitor="loss", factor=0.2, patience=20, min_lr=1e-20, verbose=True
+    )
+    train_callbacks.append(reduce_lr)
+
+    # Custom callback that saves the best models using both train and
+    # validation metric
+    # Remark: the save of the model should be done on the standard model, not
+    #         on the parallel_model, otherwise issues to use it afterwards
+    if nb_gpu > 1:
+        model_template_for_save = model
+    else:
+        model_template_for_save = None
+    model_checkpoint_saver = mh.ModelCheckpointExt(
+        model_save_dir=model_save_dir,
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        architecture_id=hyperparams.architecture.architecture_id,
+        trainparams_id=hyperparams.train.trainparams_id,
+        monitor_metric=hyperparams.train.monitor_metric,
+        monitor_metric_mode=hyperparams.train.monitor_metric_mode,
+        save_format=hyperparams.train.save_format,
+        save_best_only=hyperparams.train.save_best_only,
+        save_min_accuracy=hyperparams.train.save_min_accuracy,
+        model_template_for_save=model_template_for_save,
+    )
+    train_callbacks.append(model_checkpoint_saver)
+
+    # Callbacks for logging
+    if hyperparams.train.log_tensorboard is True:
+        tensorboard_log_dir = model_save_dir / (
+            model_save_base_filename + "_tensorboard_log"
+        )
+        tensorboard_logger = kr.callbacks.TensorBoard(log_dir=str(tensorboard_log_dir))
+        train_callbacks.append(tensorboard_logger)
+    if hyperparams.train.log_csv is True:
+        csv_logger = kr.callbacks.CSVLogger(
+            str(csv_log_filepath), append=True, separator=";"
+        )
+        train_callbacks.append(csv_logger)
+
+    # Stop if no more improvement
+    early_stopping = kr.callbacks.EarlyStopping(
+        monitor=hyperparams.train.earlystop_monitor_metric,
+        patience=hyperparams.train.earlystop_patience,
+        mode=hyperparams.train.earlystop_monitor_metric_mode,
+        restore_best_weights=False,
+    )
+    train_callbacks.append(early_stopping)
+
+    # Prepare the parameters to pass to fit...
+    # Supported filetypes to train/validate on
+    input_ext = [".tif", ".jpg", ".png"]
+
+    # Calculate the size of the input datasets
+    # train_dataset_size = len(glob.glob(f"{traindata_dir}/{image_subdir}/*.*"))
+    train_dataset_size = 0
+    for input_ext_cur in input_ext:
+        traindata_image_dir = traindata_dir / image_subdir
+        train_dataset_size += len(list(traindata_image_dir.rglob("*" + input_ext_cur)))
+    validation_dataset_size = 0
+    for input_ext_cur in input_ext:
+        validationdata_image_dir = validationdata_dir / image_subdir
+        validation_dataset_size += len(
+            list(validationdata_image_dir.rglob("*" + input_ext_cur))
+        )
+
+    # Calculate the number of steps within an epoch
+    # Remark: number of steps per epoch should be at least 1, even if nb samples
+    # < batch size...
+    train_steps_per_epoch = math.ceil(train_dataset_size / hyperparams.train.batch_size)
+    validation_steps_per_epoch = math.ceil(
+        validation_dataset_size / hyperparams.train.batch_size
+    )
+
+    # Start training
+    logger.info(
+        f"Start training with batch_size: {hyperparams.train.batch_size}, "
+        f"train_dataset_size: {train_dataset_size}, train_steps_per_epoch: "
+        f"{train_steps_per_epoch}, validation_dataset_size: {validation_dataset_size}, "
+        f"validation_steps_per_epoch: {validation_steps_per_epoch}"
+    )
+
+    logger.info(f"{hyperparams.toJSON()}")
+    hyperparams_filepath = (
+        model_save_dir / f"{model_save_base_filename}_hyperparams.json"
+    )
+    hyperparams_filepath.write_text(hyperparams.toJSON())
+
+    try:
+        # If the encoder should be frozen for the first epochs, do so
+        if hyperparams.train.nb_epoch_with_freeze > 0:
+            logger.info(
+                f"First train for {hyperparams.train.nb_epoch_with_freeze} epochs with "
+                "frozen layers"
+            )
+            model_for_train.fit(
+                train_gen,
+                steps_per_epoch=train_steps_per_epoch,
+                epochs=hyperparams.train.nb_epoch_with_freeze,
+                validation_data=validation_gen,
+                # Number of items in validation/batch_size
+                validation_steps=validation_steps_per_epoch,
+                callbacks=train_callbacks,
+                initial_epoch=start_epoch,
+                verbose=2,  # type: ignore
+            )
+            mf.set_trainable(model=model_for_train, recompile=False)
+            model_for_train = mf.compile_model(
+                model=model_for_train,
+                optimizer=hyperparams.train.optimizer,
+                optimizer_params=hyperparams.train.optimizer_params,
+                loss=hyperparams.train.loss_function,
+                class_weights=hyperparams.train.class_weights,
+            )
+
+        # Train!
+        model_for_train.fit(
+            train_gen,
+            steps_per_epoch=train_steps_per_epoch,
+            epochs=hyperparams.train.nb_epoch,
+            validation_data=validation_gen,
+            # Number of items in validation/batch_size
+            validation_steps=validation_steps_per_epoch,
+            callbacks=train_callbacks,
+            initial_epoch=start_epoch,
+            verbose=2,  # type: ignore
+        )
+
+        # Write some reporting
+        train_report_path = model_save_dir / (model_save_base_filename + "_report.pdf")
+        train_log_df = pd.read_csv(csv_log_filepath, sep=";")
+        assert isinstance(train_log_df, pd.DataFrame)
+        columns_to_keep = []
+        for column in train_log_df.columns:
+            if column.endswith("accuracy") or column.endswith("f1-score"):
+                columns_to_keep.append(column)
+
+        train_log_vis_df = train_log_df[columns_to_keep]
+        train_log_vis_df.plot().get_figure().savefig(str(train_report_path))
+
+    finally:
+        # Release the memory from the GPU...
+        # from keras import backend as K
+        # K.clear_session()
+        kr.backend.clear_session()
+
+
+def create_train_generator(
+    input_data_dir: Path,
+    image_subdir: str,
+    mask_subdir: str,
+    image_augment_dict: dict,
+    mask_augment_dict: dict,
+    batch_size: int = 32,
+    image_color_mode: str = "rgb",
+    mask_color_mode: str = "grayscale",
+    save_to_subdir: Optional[str] = None,
+    image_save_prefix: str = "image",
+    mask_save_prefix: str = "mask",
+    nb_classes: int = 1,
+    target_size: Tuple[int, int] = (256, 256),
+    shuffle: bool = True,
+    seed: int = 1,
+):
+    """
+    Creates a generator to generate and augment train images. The augmentations
+    specified in aug_dict will be applied. For the augmentations that can be
+    specified in aug_dict look at the documentation of
+    keras.preprocessing.image.ImageDataGenerator
+
+    For more info about the other parameters, check keras flow_from_directory.
+
+    Remarks: * use the same seed for image_datagen and mask_datagen to ensure
+               the transformation for image and mask is the same
+             * set save_to_dir = "your path" to check results of the generator
+    """
+    # Init
+    # Do some checks on the augmentations specified, as it is easy to
+    # introduce illogical values
+    if (
+        image_augment_dict is not None
+        and mask_augment_dict is None
+        or image_augment_dict is not None
+        and mask_augment_dict is None
+    ):
+        logger.warn(
+            "Only augmentations specified for either image or mask: "
+            f"image_augment_dict: {image_augment_dict}, mask_augment_dict: "
+            f"{mask_augment_dict}"
+        )
+
+    # Checks that involve comparing augmentations between the image and the mask
+    if image_augment_dict is not None and mask_augment_dict is not None:
+        # If an augmentation is specified for image, it should be specified
+        # for the mask as well and the other way around to evade issues
+        for augmentation in image_augment_dict:
+            if augmentation not in mask_augment_dict:
+                raise Exception(
+                    f"{augmentation} in image_augment_dict but not in mask_augment_dict"
+                )
+        for augmentation in mask_augment_dict:
+            if augmentation not in image_augment_dict:
+                raise Exception(
+                    f"{augmentation} in mask_augment_dict but not in image_augment_dict"
+                )
+
+        # Check if the brightness range has valid values
+        image_brightness_range = image_augment_dict.get("brightness_range")
+        mask_brightness_range = mask_augment_dict.get("brightness_range")
+        if image_brightness_range is None and mask_brightness_range is not None:
+            # If brightness_range None for image, it should be None for the mask as well
+            raise Exception(
+                "augmentation brightness_range is None (null) in image_augment_dict "
+                f"but isn't in mask_augment_dict: {mask_brightness_range}"
+            )
+        elif image_brightness_range is not None and mask_brightness_range is None:
+            # If brightness_range None for mask, it should be None for the image as well
+            raise Exception(
+                "augmentation brightness_range is None (null) in mask_augment_dict but "
+                f"isn't in image_augment_dict: {image_brightness_range}"
+            )
+        elif image_brightness_range is not None and mask_brightness_range is not None:
+            # The brightness_range values should be >= 0
+            if image_brightness_range[0] < 0 or image_brightness_range[1] < 0:
+                raise Exception(
+                    "augmentation brightness_range values should be > 0: value 1.0 = "
+                    "don't do anything, 0 = black"
+                )
+            # brightness_range is applied to the image, it should be [1,1] for the mask
+            if mask_brightness_range[0] != 1.0 or mask_brightness_range[1] != 1.0:
+                raise Exception(
+                    "augmentation brightness_range is specified on the image: then the "
+                    f"mask should get range [1, 1], not {mask_brightness_range}"
+                )
+
+    # Some checks specific for the mask
+    if mask_augment_dict is not None:
+        # Check cval value
+        if "cval" in mask_augment_dict and mask_augment_dict["cval"] != 0:
+            logger.warn(
+                "cval typically should be 0 for the mask, even if it is different for "
+                "the image, as the cval of the mask refers to these locations being of "
+                f"class 'background'. It is: {mask_augment_dict['cval']}"
+            )
+
+        # If there are more than two classes, the mask will have integers as values
+        # to code the different masks in, and one hot-encoding will be applied to
+        # it, so it should not be rescaled!!!
+        if (
+            nb_classes > 2
+            and "rescale" in mask_augment_dict
+            and mask_augment_dict["rescale"] != 1
+        ):
+            raise Exception(
+                f"With nb_classes > 2 ({nb_classes}), the mask should have a rescale "
+                f"value of 1, not {mask_augment_dict['rescale']}"
+            )
+
+    # Now create the generators
+    # Create the image generators with the augment info
+
+    # TODO: brightness_range is buggy on 2021-08-11, with keras preprocessing
+    # version 1.1, so is implemented here in a hacky way!
+    image_augment_dict_temp = {
+        key: value
+        for (key, value) in image_augment_dict.items()
+        if key != "brightness_range"
+    }
+    mask_augment_dict_temp = {
+        key: value
+        for (key, value) in mask_augment_dict.items()
+        if key != "brightness_range"
+    }
+    image_datagen = kr.preprocessing.image.ImageDataGenerator(**image_augment_dict_temp)
+    mask_datagen = kr.preprocessing.image.ImageDataGenerator(**mask_augment_dict_temp)
+
+    # Format save_to_dir
+    # Remark: flow_from_directory doesn't support Path, so supply str immediately as
+    # well, otherwise, if str(Path) is used later on, it becomes 'None' instead of None!
+    save_to_dir = None
+    if save_to_subdir is not None:
+        save_to_dir = input_data_dir / save_to_subdir
+        if not save_to_dir.exists():
+            save_to_dir.mkdir(parents=True)
+
+    image_generator = image_datagen.flow_from_directory(
+        directory=str(input_data_dir),
+        classes=[image_subdir],
+        class_mode=None,
+        color_mode=image_color_mode,
+        target_size=target_size,
+        batch_size=batch_size,
+        save_to_dir=None,
+        save_prefix=image_save_prefix,
+        shuffle=shuffle,
+        seed=seed,
+    )
+
+    mask_generator = mask_datagen.flow_from_directory(
+        directory=str(input_data_dir),
+        classes=[mask_subdir],
+        class_mode=None,
+        color_mode=mask_color_mode,
+        target_size=target_size,
+        batch_size=batch_size,
+        save_to_dir=None,
+        save_prefix=mask_save_prefix,
+        shuffle=shuffle,
+        seed=seed,
+    )
+
+    train_generator = zip(image_generator, mask_generator)
+
+    for batch_id, (image, mask) in enumerate(train_generator):
+        # Cast to arrays to evade type errors
+        image = np.array(image)
+        mask = np.array(mask)
+
+        # TODO: brightness_range is buggy on 2021-08-11, with keras preprocessing
+        # version 1.1, so is implemented here in a hacky way!
+        if (
+            "brightness_range" in image_augment_dict
+            and image_augment_dict["brightness_range"] is not None
+            and (
+                image_augment_dict["brightness_range"][0] != 1
+                or image_augment_dict["brightness_range"][1] != 1
+            )
+        ):
+
+            # Random brightness shift to apply to all images in batch
+            brightness_shift = np.random.uniform(
+                image_augment_dict["brightness_range"][0],
+                image_augment_dict["brightness_range"][1],
+            )
+            image = image * brightness_shift
+
+        # One-hot encode mask if multiple classes
+        if nb_classes > 1:
+            mask = kr.utils.to_categorical(mask, nb_classes)
+
+        # Because the default save_to_dir option doesn't support saving the
+        # augmented masks in seperate files per class, implement this here.
+        if save_to_dir is not None:
+            # Save mask for every class seperately
+            # Get the number of images in this batch + the nb classes
+            mask_shape = mask.shape
+            nb_images = mask_shape[0]
+            nb_classes = mask_shape[3]
+
+            # Loop through images in this batch
+            for image_id in range(nb_images):
+                # Slice the next image from the array
+                image_to_save = image[image_id, :, :, :]
+
+                # Reverse the rescale if there is one
+                if (
+                    image_augment_dict is not None
+                    and "rescale" in image_augment_dict
+                    and image_augment_dict["rescale"] != 1
+                ):
+                    image_to_save = image_to_save / image_augment_dict["rescale"]
+
+                # Now convert to uint8 image and save!
+                # , image_color_mode
+                colormode = None
+                if image_color_mode.upper() == "RGB":
+                    colormode = "RGB"
+                im = Image.fromarray(image_to_save.astype(np.uint8), mode=colormode)
+                image_dir = save_to_dir / f"{batch_id:0>4}"
+                image_dir.mkdir(parents=True, exist_ok=True)
+                image_path = image_dir / f"{image_id}_image.jpg"
+                im.save(image_path)
+
+                # Loop through the masks for each class
+                for channel_id in range(nb_classes):
+                    mask_to_save = mask[image_id, :, :, channel_id]
+                    mask_dir = save_to_dir / f"{batch_id:0>4}"
+                    mask_path = mask_dir / f"{image_id}_mask_{channel_id}.png"
+                    im = Image.fromarray((mask_to_save * 255).astype(np.uint8))
+                    im.save(mask_path)
+
+        yield (image, mask)
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    raise Exception("Not implemented")
```

### Comparing `orthoseg-0.4.2/orthoseg/load_images.py` & `orthoseg-0.4.2a1/orthoseg/load_images.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-# -*- coding: utf-8 -*-
-"""
-Script to load images from a WMS server.
-"""
-
-import argparse
-import logging
-from pathlib import Path
-import shlex
-import sys
-import traceback
-
-import pyproj
-
-# orthoseg is higher in dir hierarchy, so add root to sys.path
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import config_helper as conf
-from orthoseg.helpers import email_helper
-from orthoseg.util import log_util
-from orthoseg.util import ows_util
-
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def load_images_argstr(argstr):
-    args = shlex.split(argstr)
-    load_images_args(args)
-
-
-def load_images_args(args):
-
-    # Interprete arguments
-    parser = argparse.ArgumentParser(add_help=False)
-
-    # Required arguments
-    required = parser.add_argument_group("Required arguments")
-    required.add_argument(
-        "-c", "--config", type=str, required=True, help="The config file to use"
-    )
-
-    # Optional arguments
-    optional = parser.add_argument_group("Optional arguments")
-    # Add back help
-    optional.add_argument(
-        "-h",
-        "--help",
-        action="help",
-        default=argparse.SUPPRESS,
-        help="Show this help message and exit",
-    )
-
-    # Interprete arguments
-    args = parser.parse_args(args)
-
-    # Run!
-    load_images(config_path=Path(args.config))
-
-
-def load_images(config_path: Path, load_testsample_images: bool = False):
-    """
-    Load and cache images for a segmentation project.
-
-    Args:
-        config_path (Path): Path to the projects config file.
-        load_testsample_images (bool, optional): True to only load testsample
-            images. Defaults to False.
-    """
-
-    # Init
-    # Load the config and save in a bunch of global variables zo it
-    # is accessible everywhere
-    conf.read_orthoseg_config(config_path)
-
-    # Init logging
-    log_util.clean_log_dir(
-        log_dir=conf.dirs.getpath("log_dir"),
-        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
-    )
-    global logger
-    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
-
-    # Log + send email
-    message = f"Start load_images for config {config_path.stem}"
-    logger.info(message)
-    logger.debug(f"Config used: \n{conf.pformat_config()}")
-    email_helper.sendmail(message)
-
-    try:
-        # Use different setting depending if testsample or all images
-        if load_testsample_images:
-            output_image_dir = conf.dirs.getpath("predictsample_image_input_dir")
-
-            # Use the same image size as for the training, that is the most
-            # convenient to check the quality
-            image_pixel_width = conf.train.getint("image_pixel_width")
-            image_pixel_height = conf.train.getint("image_pixel_height")
-            image_pixel_x_size = conf.train.getfloat("image_pixel_x_size")
-            image_pixel_y_size = conf.train.getfloat("image_pixel_y_size")
-            image_pixels_overlap = 0
-            image_format = ows_util.FORMAT_JPEG
-
-            # To create the testsample, fetch only on every ... images
-            nb_images_to_skip = 50
-
-        else:
-            output_image_dir = conf.dirs.getpath("predict_image_input_dir")
-
-            # Get the image size for the predict
-            image_pixel_width = conf.predict.getint("image_pixel_width")
-            image_pixel_height = conf.predict.getint("image_pixel_height")
-            image_pixel_x_size = conf.predict.getfloat("image_pixel_x_size")
-            image_pixel_y_size = conf.predict.getfloat("image_pixel_y_size")
-            image_pixels_overlap = conf.predict.getint("image_pixels_overlap")
-            image_format = ows_util.FORMAT_JPEG
-
-            # For the real prediction dataset, no skipping obviously...
-            nb_images_to_skip = 0
-
-        # Get ssl_verify setting
-        ssl_verify = conf.general["ssl_verify"]
-        # Get the download cron schedule
-        download_cron_schedule = conf.download["cron_schedule"]
-
-        # Get the layer info
-        predict_layer = conf.predict["image_layer"]
-        layersources = conf.image_layers[predict_layer]["layersources"]
-        nb_concurrent_calls = conf.image_layers[predict_layer]["nb_concurrent_calls"]
-        crs = pyproj.CRS.from_user_input(conf.image_layers[predict_layer]["projection"])
-        bbox = conf.image_layers[predict_layer]["bbox"]
-        grid_xmin = conf.image_layers[predict_layer]["grid_xmin"]
-        grid_ymin = conf.image_layers[predict_layer]["grid_ymin"]
-        image_pixels_ignore_border = conf.image_layers[predict_layer][
-            "image_pixels_ignore_border"
-        ]
-        roi_filepath = conf.image_layers[predict_layer]["roi_filepath"]
-
-        # Now we are ready to get the images...
-        ows_util.get_images_for_grid(
-            layersources=layersources,
-            output_image_dir=output_image_dir,
-            crs=crs,
-            image_gen_bounds=bbox,
-            image_gen_roi_filepath=roi_filepath,
-            grid_xmin=grid_xmin,
-            grid_ymin=grid_ymin,
-            image_crs_pixel_x_size=image_pixel_x_size,
-            image_crs_pixel_y_size=image_pixel_y_size,
-            image_pixel_width=image_pixel_width,
-            image_pixel_height=image_pixel_height,
-            image_pixels_ignore_border=image_pixels_ignore_border,
-            nb_concurrent_calls=nb_concurrent_calls,
-            cron_schedule=download_cron_schedule,
-            image_format=image_format,
-            pixels_overlap=image_pixels_overlap,
-            nb_images_to_skip=nb_images_to_skip,
-            ssl_verify=ssl_verify,
-        )
-
-        # Log and send mail
-        message = f"Completed load_images for config {config_path.stem}"
-        logger.info(message)
-        email_helper.sendmail(message)
-    except Exception as ex:
-        message = f"ERROR while running load_images for task {config_path.stem}"
-        logger.exception(message)
-        email_helper.sendmail(
-            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
-        )
-        raise Exception(message) from ex
-
-
-def main():
-    try:
-        load_images_args(sys.argv[1:])
-    except Exception as ex:
-        logger.exception(f"Error: {ex}")
-        raise
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""
+Script to load images from a WMS server.
+"""
+
+import argparse
+import logging
+from pathlib import Path
+import shlex
+import sys
+import traceback
+
+import pyproj
+
+# orthoseg is higher in dir hierarchy, so add root to sys.path
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import config_helper as conf
+from orthoseg.helpers import email_helper
+from orthoseg.util import log_util
+from orthoseg.util import ows_util
+
+# -------------------------------------------------------------
+# First define/init general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def load_images_argstr(argstr):
+    args = shlex.split(argstr)
+    load_images_args(args)
+
+
+def load_images_args(args):
+
+    # Interprete arguments
+    parser = argparse.ArgumentParser(add_help=False)
+
+    # Required arguments
+    required = parser.add_argument_group("Required arguments")
+    required.add_argument(
+        "-c", "--config", type=str, required=True, help="The config file to use"
+    )
+
+    # Optional arguments
+    optional = parser.add_argument_group("Optional arguments")
+    # Add back help
+    optional.add_argument(
+        "-h",
+        "--help",
+        action="help",
+        default=argparse.SUPPRESS,
+        help="Show this help message and exit",
+    )
+
+    # Interprete arguments
+    args = parser.parse_args(args)
+
+    # Run!
+    load_images(config_path=Path(args.config))
+
+
+def load_images(config_path: Path, load_testsample_images: bool = False):
+    """
+    Load and cache images for a segmentation project.
+
+    Args:
+        config_path (Path): Path to the projects config file.
+        load_testsample_images (bool, optional): True to only load testsample
+            images. Defaults to False.
+    """
+
+    # Init
+    # Load the config and save in a bunch of global variables zo it
+    # is accessible everywhere
+    conf.read_orthoseg_config(config_path)
+
+    # Init logging
+    log_util.clean_log_dir(
+        log_dir=conf.dirs.getpath("log_dir"),
+        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
+    )
+    global logger
+    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
+
+    # Log + send email
+    message = f"Start load_images for config {config_path.stem}"
+    logger.info(message)
+    logger.debug(f"Config used: \n{conf.pformat_config()}")
+    email_helper.sendmail(message)
+
+    try:
+        # Use different setting depending if testsample or all images
+        if load_testsample_images:
+            output_image_dir = conf.dirs.getpath("predictsample_image_input_dir")
+
+            # Use the same image size as for the training, that is the most
+            # convenient to check the quality
+            image_pixel_width = conf.train.getint("image_pixel_width")
+            image_pixel_height = conf.train.getint("image_pixel_height")
+            image_pixel_x_size = conf.train.getfloat("image_pixel_x_size")
+            image_pixel_y_size = conf.train.getfloat("image_pixel_y_size")
+            image_pixels_overlap = 0
+            image_format = ows_util.FORMAT_JPEG
+
+            # To create the testsample, fetch only on every ... images
+            nb_images_to_skip = 50
+
+        else:
+            output_image_dir = conf.dirs.getpath("predict_image_input_dir")
+
+            # Get the image size for the predict
+            image_pixel_width = conf.predict.getint("image_pixel_width")
+            image_pixel_height = conf.predict.getint("image_pixel_height")
+            image_pixel_x_size = conf.predict.getfloat("image_pixel_x_size")
+            image_pixel_y_size = conf.predict.getfloat("image_pixel_y_size")
+            image_pixels_overlap = conf.predict.getint("image_pixels_overlap")
+            image_format = ows_util.FORMAT_JPEG
+
+            # For the real prediction dataset, no skipping obviously...
+            nb_images_to_skip = 0
+
+        # Get ssl_verify setting
+        ssl_verify = conf.general["ssl_verify"]
+        # Get the download cron schedule
+        download_cron_schedule = conf.download["cron_schedule"]
+
+        # Get the layer info
+        predict_layer = conf.predict["image_layer"]
+        layersources = conf.image_layers[predict_layer]["layersources"]
+        nb_concurrent_calls = conf.image_layers[predict_layer]["nb_concurrent_calls"]
+        crs = pyproj.CRS.from_user_input(conf.image_layers[predict_layer]["projection"])
+        bbox = conf.image_layers[predict_layer]["bbox"]
+        grid_xmin = conf.image_layers[predict_layer]["grid_xmin"]
+        grid_ymin = conf.image_layers[predict_layer]["grid_ymin"]
+        image_pixels_ignore_border = conf.image_layers[predict_layer][
+            "image_pixels_ignore_border"
+        ]
+        roi_filepath = conf.image_layers[predict_layer]["roi_filepath"]
+
+        # Now we are ready to get the images...
+        ows_util.get_images_for_grid(
+            layersources=layersources,
+            output_image_dir=output_image_dir,
+            crs=crs,
+            image_gen_bounds=bbox,
+            image_gen_roi_filepath=roi_filepath,
+            grid_xmin=grid_xmin,
+            grid_ymin=grid_ymin,
+            image_crs_pixel_x_size=image_pixel_x_size,
+            image_crs_pixel_y_size=image_pixel_y_size,
+            image_pixel_width=image_pixel_width,
+            image_pixel_height=image_pixel_height,
+            image_pixels_ignore_border=image_pixels_ignore_border,
+            nb_concurrent_calls=nb_concurrent_calls,
+            cron_schedule=download_cron_schedule,
+            image_format=image_format,
+            pixels_overlap=image_pixels_overlap,
+            nb_images_to_skip=nb_images_to_skip,
+            ssl_verify=ssl_verify,
+        )
+
+        # Log and send mail
+        message = f"Completed load_images for config {config_path.stem}"
+        logger.info(message)
+        email_helper.sendmail(message)
+    except Exception as ex:
+        message = f"ERROR while running load_images for task {config_path.stem}"
+        logger.exception(message)
+        email_helper.sendmail(
+            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
+        )
+        raise Exception(message) from ex
+
+
+def main():
+    try:
+        load_images_args(sys.argv[1:])
+    except Exception as ex:
+        logger.exception(f"Error: {ex}")
+        raise
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    main()
```

### Comparing `orthoseg-0.4.2/orthoseg/load_sampleprojects.py` & `orthoseg-0.4.2a1/orthoseg/load_sampleprojects.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# -*- coding: utf-8 -*-
-"""
-Download the sample project.
-"""
-
-import argparse
-import logging
-from pathlib import Path
-import shlex
-import sys
-from typing import Optional
-
-import gdown
-
-# orthoseg is higher in dir hierarchy, add root to sys.path
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.util import git_downloader
-
-
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def parse_load_sampleprojects_argstr(argstr):
-    args = shlex.split(argstr)
-    parse_load_sampleprojects_args(args)
-
-
-def parse_load_sampleprojects_args(args) -> dict:
-
-    # Define supported arguments
-    parser = argparse.ArgumentParser(add_help=False)
-
-    help = (
-        "The directory to create the sample_projects dir in. "
-        "Eg. ~/orthoseg will create orthoseg/sample_projects in your home directory."
-    )
-    parser.add_argument("dest_dir", help=help)
-
-    help = (
-        "True to use the default certificate bundle as installed on your system. "
-        "False disables certificate validation (NOT recommended!). In corporate "
-        "networks using a proxy server it is often needed to specify a customized "
-        "certificate bundle (.pem file) to avoid CERTIFICATE_VERIFY_FAILED errors. "
-        "It is recommended to specify the path to a custum certificate bundle file "
-        "using the REQUESTS_CA_BUNDLE environment variable, but it can also passed "
-        "using this switch. Parameter defaults to True."
-    )
-    parser.add_argument("--ssl_verify", default=True, help=help)
-
-    # Interprete arguments
-    args = parser.parse_args(args)
-    dest_dir = Path(args.dest_dir).expanduser() / "orthoseg"
-    ssl_verify = args.ssl_verify
-
-    # Return arguments
-    return {"dest_dir": dest_dir, "ssl_verify": ssl_verify}
-
-
-def load_sampleprojects(dest_dir: Path, ssl_verify: Optional[bool] = None):
-    dest_dir_full = dest_dir / "sample_projects"
-    if dest_dir_full.exists():
-        raise Exception(f"Destination directory already exists: {dest_dir_full}")
-
-    # Download
-    print(f"Start download of sample projects to {str(dest_dir_full)}")
-    git_downloader.download(
-        repo_url="https://github.com/orthoseg/orthoseg/tree/master/sample_projects",
-        output_dir=dest_dir,
-        ssl_verify=ssl_verify,
-    )
-    print("Download finished")
-    print("Start download of footballfields pretrained neural net")
-    verify = True if ssl_verify is None else ssl_verify
-    footballfields_model_dir = dest_dir_full / "footballfields/models"
-    footballfields_model_dir.mkdir(parents=True, exist_ok=True)
-    model_hdf5_path = footballfields_model_dir / "footballfields_01_0.92512_242.hdf5"
-    if model_hdf5_path.exists() is False:
-        gdown.download(
-            id="1XmAenCW6K_RVwqC6xbkapJ5ws-f7-QgH",
-            output=str(model_hdf5_path),
-            verify=verify,
-        )
-    model_hyperparams_path = (
-        footballfields_model_dir / "footballfields_01_hyperparams.json"
-    )
-    if model_hyperparams_path.exists() is False:
-        gdown.download(
-            id="1umxcd4RkB81sem9PdIpLoWeiIW8ga1u7",
-            output=str(model_hyperparams_path),
-            verify=verify
-        )
-    model_modeljson_path = footballfields_model_dir / "footballfields_01_model.json"
-    if model_modeljson_path.exists() is False:
-        gdown.download(
-            id="16qe8thBTrO3dFfLMU1T22gWcfHVXt8zQ",
-            output=str(model_modeljson_path),
-            verify=verify
-        )
-    print("Download finished")
-
-
-def main():
-    try:
-        parsed_args = parse_load_sampleprojects_args(sys.argv[1:])
-        load_sampleprojects(**parsed_args)
-    except Exception as ex:
-        logger.exception(f"Error: {ex}")
-        raise
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""
+Download the sample project.
+"""
+
+import argparse
+import logging
+from pathlib import Path
+import shlex
+import sys
+from typing import Optional
+
+import gdown
+
+# orthoseg is higher in dir hierarchy, add root to sys.path
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.util import git_downloader
+
+
+# -------------------------------------------------------------
+# First define/init general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def parse_load_sampleprojects_argstr(argstr):
+    args = shlex.split(argstr)
+    parse_load_sampleprojects_args(args)
+
+
+def parse_load_sampleprojects_args(args) -> dict:
+
+    # Define supported arguments
+    parser = argparse.ArgumentParser(add_help=False)
+
+    help = (
+        "The directory to create the sample_projects dir in. "
+        "Eg. ~/orthoseg will create orthoseg/sample_projects in your home directory."
+    )
+    parser.add_argument("dest_dir", help=help)
+
+    help = (
+        "True to use the default certificate bundle as installed on your system. "
+        "False disables certificate validation (NOT recommended!). In corporate "
+        "networks using a proxy server it is often needed to specify a customized "
+        "certificate bundle (.pem file) to avoid CERTIFICATE_VERIFY_FAILED errors. "
+        "It is recommended to specify the path to a custum certificate bundle file "
+        "using the REQUESTS_CA_BUNDLE environment variable, but it can also passed "
+        "using this switch. Parameter defaults to True."
+    )
+    parser.add_argument("--ssl_verify", default=True, help=help)
+
+    # Interprete arguments
+    args = parser.parse_args(args)
+    dest_dir = Path(args.dest_dir).expanduser() / "orthoseg"
+    ssl_verify = args.ssl_verify
+
+    # Return arguments
+    return {"dest_dir": dest_dir, "ssl_verify": ssl_verify}
+
+
+def load_sampleprojects(dest_dir: Path, ssl_verify: Optional[bool] = None):
+    dest_dir_full = dest_dir / "sample_projects"
+    if dest_dir_full.exists():
+        raise Exception(f"Destination directory already exists: {dest_dir_full}")
+
+    # Download
+    print(f"Start download of sample projects to {str(dest_dir_full)}")
+    git_downloader.download(
+        repo_url="https://github.com/orthoseg/orthoseg/tree/master/sample_projects",
+        output_dir=dest_dir,
+        ssl_verify=ssl_verify,
+    )
+    print("Download finished")
+    print("Start download of footballfields pretrained neural net")
+    verify = True if ssl_verify is None else ssl_verify
+    footballfields_model_dir = dest_dir_full / "footballfields/models"
+    footballfields_model_dir.mkdir(parents=True, exist_ok=True)
+    model_hdf5_path = footballfields_model_dir / "footballfields_01_0.92512_242.hdf5"
+    if model_hdf5_path.exists() is False:
+        gdown.download(
+            id="1XmAenCW6K_RVwqC6xbkapJ5ws-f7-QgH",
+            output=str(model_hdf5_path),
+            verify=verify,
+        )
+    model_hyperparams_path = (
+        footballfields_model_dir / "footballfields_01_hyperparams.json"
+    )
+    if model_hyperparams_path.exists() is False:
+        gdown.download(
+            id="1umxcd4RkB81sem9PdIpLoWeiIW8ga1u7",
+            output=str(model_hyperparams_path),
+            verify=verify
+        )
+    model_modeljson_path = footballfields_model_dir / "footballfields_01_model.json"
+    if model_modeljson_path.exists() is False:
+        gdown.download(
+            id="16qe8thBTrO3dFfLMU1T22gWcfHVXt8zQ",
+            output=str(model_modeljson_path),
+            verify=verify
+        )
+    print("Download finished")
+
+
+def main():
+    try:
+        parsed_args = parse_load_sampleprojects_args(sys.argv[1:])
+        load_sampleprojects(**parsed_args)
+    except Exception as ex:
+        logger.exception(f"Error: {ex}")
+        raise
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `orthoseg-0.4.2/orthoseg/model/model_factory.py` & `orthoseg-0.4.2a1/orthoseg/model/model_factory.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,510 +1,510 @@
-# -*- coding: utf-8 -*-
-"""
-Module with helper functions to create models.
-
-Offers a common interface, regardless of the underlying model implementation
-and contains extra metrics, callbacks,...
-
-Many models are supported by using this segmentation model zoo:
-https://github.com/qubvel/segmentation_models
-"""
-
-import json
-import logging
-from pathlib import Path
-from typing import Any, List, Optional
-
-import numpy as np
-import tensorflow as tf
-import keras.models
-import segmentation_models as sm
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.INFO)
-
-# Force using the keras implementation in tensorflow, because the default
-# use of this implementation seems broken with tensorflow 2.5
-sm.set_framework("tf.keras")
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-"""
-preprocessing_fn = get_preprocessing('resnet34')
-x = preprocessing_fn(x)
-"""
-
-
-def get_model(
-    architecture: str,
-    input_width: Optional[int] = None,
-    input_height: Optional[int] = None,
-    nb_channels: int = 3,
-    nb_classes: int = 1,
-    activation: str = "softmax",
-    init_weights_with: str = "imagenet",
-    freeze: bool = False,
-) -> keras.models.Model:
-    """
-    Get a model.
-
-    Args:
-        architecture (str): Architecture of the network to create
-        input_width (int, optional): Width of the input images. Defaults to None.
-        input_height (int, optional): Height of the input images. Defaults to None.
-        nb_channels (int, optional): Nb of channels/bands of the input images.
-            Defaults to 3.
-        nb_classes (int, optional): Nb of classes to be segmented to. Defaults to 1.
-        activation (Activation, optional): Activation function of last layer.
-            Defaults to 'softmax'.
-        init_weights_with (str, optional): Weights to init the network with.
-            Defaults to 'imagenet'.
-        freeze (bool, optional): Freeze the final layer weights during
-            training. It is usefull to use this option for the first few
-            epochs get a more robust network. Defaults to False.
-
-    Raises:
-        Exception: [description]
-        Exception: [description]
-
-    Returns:
-        [type]: [description]
-    """
-    # Check architecture
-    segment_architecture_parts = architecture.split("+")
-    if len(segment_architecture_parts) < 2:
-        raise Exception(f"Unsupported architecture: {architecture}")
-    encoder = segment_architecture_parts[0]
-    decoder = segment_architecture_parts[1]
-
-    if decoder.lower() == "unet":
-        # Architecture implemented using the segmentation_models library
-        from segmentation_models import Unet
-
-        model = Unet(
-            backbone_name=encoder.lower(),
-            input_shape=(input_width, input_height, nb_channels),
-            classes=nb_classes,
-            activation=activation,
-            encoder_weights=init_weights_with,
-            encoder_freeze=freeze,
-        )
-        return model
-
-    elif decoder.lower() == "pspnet":
-        # Architecture implemented using the segmentation_models library
-        from segmentation_models import PSPNet
-
-        model = PSPNet(
-            backbone_name=encoder.lower(),
-            input_shape=(input_width, input_height, nb_channels),
-            classes=nb_classes,
-            activation=activation,
-            encoder_weights=init_weights_with,
-            encoder_freeze=freeze,
-        )
-        return model
-
-    elif decoder.lower() == "linknet":
-        # Architecture implemented using the segmentation_models library
-        from segmentation_models import Linknet
-
-        # First check if input size is compatible with linknet
-        if input_width is not None and input_height is not None:
-            check_image_size(decoder, input_width, input_height)
-
-        model = Linknet(
-            backbone_name=encoder.lower(),
-            input_shape=(input_width, input_height, nb_channels),
-            classes=nb_classes,
-            activation=activation,
-            encoder_weights=init_weights_with,
-            encoder_freeze=freeze,
-        )
-        return model
-
-    else:
-        raise ValueError(f"Unknown decoder architecture: {decoder}")
-
-
-def compile_model(
-    model: keras.models.Model,
-    optimizer: str,
-    optimizer_params: dict,
-    loss: str,
-    metrics: Optional[List[str]] = None,
-    sample_weight_mode: Optional[str] = None,
-    class_weights: Optional[list] = None,
-) -> keras.models.Model:
-    """
-    Compile the model for training.
-
-    Args:
-        model (keras.models.Model): the keras model to compile.
-        optimizer (str): the optimizer to use.
-        optimizer_params (dict): parameters to use for optimizer.
-        loss (str): the loss function to use. One of:
-            * categorical_crossentropy
-            * weighted_categorical_crossentropy: class_weights should be specified!
-
-        metrics (List[Metric], optional): metrics to use. Defaults to None. One of:
-            *
-        sample_weight_mode (str, optional): sample weight mode to use. Defaults to None.
-        class_weights (list, optional): class weigths to use. Defaults to None.
-    """
-    # Get number classes of model
-    nb_classes = model.output[-1].shape[-1]
-
-    # If no metrics specified, use default ones
-    metric_funcs: List[Any] = []
-    if metrics is None:
-        if loss in ["categorical_crossentropy", "weighted_categorical_crossentropy"]:
-            metric_funcs.append("categorical_accuracy")
-        elif loss == "sparse_categorical_crossentropy":
-            # metrics.append('sparse_categorical_accuracy')
-            logger.warning("loss == sparse_categorical_crossentropy not implementedd")
-        elif loss == "binary_crossentropy":
-            metric_funcs.append("binary_accuracy")
-
-        onehot_mean_iou = tf.keras.metrics.OneHotMeanIoU(
-            num_classes=nb_classes, name="one_hot_mean_iou"
-        )
-        metric_funcs.append(onehot_mean_iou)
-    else:
-        raise Exception("Specifying metrics not yet implemented")
-
-    # Check loss function
-    if loss == "bcedice":
-        loss_func = dice_coef_loss_bce
-    elif loss == "dice_loss":
-        loss_func = sm.losses.DiceLoss()
-    elif loss == "jaccard_loss":
-        loss_func = sm.losses.JaccardLoss()
-    elif loss == "weighted_categorical_crossentropy":
-        if class_weights is None:
-            raise Exception(f"With loss == {loss}, class_weights cannot be None!")
-        loss_func = weighted_categorical_crossentropy(class_weights)
-    else:
-        loss_func = loss
-
-    # Create optimizer
-    if optimizer == "adam":
-        optimizer_func = tf.keras.optimizers.Adam(**optimizer_params)
-    else:
-        raise Exception(
-            f"Error creating optimizer: {optimizer}, with params {optimizer_params}"
-        )
-
-    logger.info(
-        f"Compile model, optimizer: {optimizer}, loss: {loss}, "
-        f"class_weights: {class_weights}"
-    )
-    model.compile(
-        optimizer=optimizer_func,
-        loss=loss_func,
-        metrics=metric_funcs,
-        sample_weight_mode=sample_weight_mode,
-    )
-
-    return model
-
-
-def load_model(model_to_use_filepath: Path, compile: bool = True) -> keras.models.Model:
-    """
-    Load an existing model from a file.
-
-    If loading the architecture + model from the file doesn't work, tries
-    different things to load a model anyway:
-    1) looks for a ..._model.json file to load the architecture from,
-       the weights are then loaded from the original file
-    2) looks for a ..._hyperparams.json file to create the architecture from,
-       the weights are then loaded from the original file
-
-    Args:
-        model_to_use_filepath (Path): The file to load the model from.
-        compile (bool, optional): True to get a compiled version back that is
-            ready to train. Defaults to True.
-
-    Raises:
-        Exception: [description]
-
-    Returns:
-        tf.keras.models.Model: The loaded model.
-    """
-    errors = []
-    model = None
-    model_basestem = f"{'_'.join(model_to_use_filepath.stem.split('_')[0:2])}"
-
-    # If it is a file with the complete model, try loading it entirely...
-    if not model_to_use_filepath.stem.endswith("_weights"):
-        # Load the hyperparams file
-        hyperparams_json_filepath = (
-            model_to_use_filepath.parent / f"{model_basestem}_hyperparams.json"
-        )
-        nb_classes = 1
-        if hyperparams_json_filepath.exists():
-            with hyperparams_json_filepath.open("r") as src:
-                hyperparams = json.load(src)
-                nb_classes = len(hyperparams["architecture"]["classes"])
-
-        iou_score = sm.metrics.IOUScore()
-        f1_score = sm.metrics.FScore()
-        onehot_mean_iou = tf.keras.metrics.OneHotMeanIoU(
-            num_classes=nb_classes, name="one_hot_mean_iou"
-        )
-
-        try:
-            model = tf.keras.models.load_model(
-                str(model_to_use_filepath),
-                custom_objects={
-                    "jaccard_coef": jaccard_coef,
-                    "jaccard_coef_flat": jaccard_coef_flat,
-                    "jaccard_coef_round": jaccard_coef_round,
-                    "dice_coef": dice_coef,
-                    "iou_score": iou_score,
-                    "f1_score": f1_score,
-                    "one_hot_mean_iou": onehot_mean_iou,
-                    "weighted_categorical_crossentropy": weighted_categorical_crossentropy,  # noqa: E501
-                },
-                compile=compile,
-            )
-        except Exception as ex:
-            errors.append(
-                f"Error loading model+weights from {model_to_use_filepath}: {ex}"
-            )
-
-    # If no model returned yet, try loading loading architecture and weights seperately
-    if model is None:
-        # Load the architecture from a model.json file
-        # Check if there is a specific model.json file for these weights
-        model_json_filepath = model_to_use_filepath.parent / (
-            model_to_use_filepath.stem.replace("_weights", "") + ".json"
-        )
-        if not model_json_filepath.exists():
-            # If not, check if there is a model.json file for the training session
-            model_json_filepath = (
-                model_to_use_filepath.parent / f"{model_basestem}_model.json"
-            )
-        if model_json_filepath.exists():
-            with model_json_filepath.open("r") as src:
-                model_json = src.read()
-            try:
-                model = tf.keras.models.model_from_json(model_json)
-            except Exception as ex:
-                errors.append(
-                    f"Error loading model architecture from {model_json_filepath}: {ex}"
-                )
-        else:
-            errors.append(
-                f"No model.json file found to load model from: {model_json_filepath}"
-            )
-
-        # If loading model.json not successfull, create model based on hyperparams.json
-        if model is None:
-            # Load the hyperparams file if available
-            hyperparams_json_filepath = (
-                model_to_use_filepath.parent / f"{model_basestem}_hyperparams.json"
-            )
-            if hyperparams_json_filepath.exists():
-                with hyperparams_json_filepath.open("r") as src:
-                    hyperparams = json.load(src)
-                # Create the model we want to use
-                try:
-                    model = get_model(
-                        architecture=hyperparams["architecture"]["architecture"],
-                        nb_channels=hyperparams["architecture"]["nb_channels"],
-                        nb_classes=hyperparams["architecture"]["nb_classes"],
-                        activation=hyperparams["architecture"]["activation_function"],
-                    )
-                except Exception as ex:
-                    errors.append(
-                        "Error in get_model() with params from: "
-                        f"{hyperparams_json_filepath}: {ex}"
-                    )
-            else:
-                errors.append(
-                    f"No file found to load model from: {hyperparams_json_filepath}"
-                )
-
-        # Now load the weights
-        if model is not None:
-            try:
-                model.load_weights(str(model_to_use_filepath))
-            except Exception as ex:
-                errors.append(
-                    f"Error trying model.load_weights on: {model_to_use_filepath}: {ex}"
-                )
-
-    # Check if a model got loaded...
-    if model is not None:
-        # Eager seems to be 50% slower, tested on tensorflow 2.5
-        model.run_eagerly = False
-    else:
-        # If we still have not model... time to give up.
-        errors_str = ""
-        if len(errors) > 0:
-            errors_str = (
-                " The following errors occured while trying: \n    -> "
-                + "\n    -> ".join(errors)
-            )
-        raise Exception(f"Error loading model for {model_to_use_filepath}.{errors_str}")
-
-    return model  # type: ignore
-
-
-def set_trainable(model, recompile: bool = True):
-    sm.utils.set_trainable(
-        model=model, recompile=recompile
-    )  # doesn't seem to work, so save and load model
-
-
-def check_image_size(decoder: str, input_width: int, input_height: int):
-    if decoder.lower() == "linknet":
-        if (input_width and (input_width % 16) != 0) or (
-            input_height and (input_height % 16) != 0
-        ):
-            message = (
-                f"for decoder linknet, input_width ({input_width} and input_height "
-                f"({input_height}) should be divisable by 16!"
-            )
-            logger.error(message)
-            raise ValueError(message)
-    else:
-        logger.info(f"check_image_size is not implemented for this model: {decoder}")
-
-
-# ------------------------------------------
-# Loss functions
-# ------------------------------------------
-
-
-def weighted_categorical_crossentropy(weights):
-    """weighted_categorical_crossentropy
-
-    Args:
-        * weights<ktensor|nparray|list>: crossentropy weights
-    Returns:
-        * weighted categorical crossentropy function
-    """
-    if isinstance(weights, list) or isinstance(weights, np.ndarray):
-        weights = tf.keras.backend.variable(weights)
-
-    def loss(target, output, from_logits=False):
-        if not from_logits:
-            output /= tf.reduce_sum(output, len(output.get_shape()) - 1, True)
-            _epsilon = tf.convert_to_tensor(
-                tf.keras.backend.epsilon(), dtype=output.dtype.base_dtype
-            )
-            output = tf.clip_by_value(output, _epsilon, 1.0 - _epsilon)  # type: ignore
-            weighted_losses = target * tf.math.log(output) * weights
-            retval = -tf.reduce_sum(
-                weighted_losses, len(output.get_shape()) - 1  # type: ignore
-            )
-            return retval
-        else:
-            raise ValueError("WeightedCategoricalCrossentropy: not valid with logits")
-
-    return loss
-
-
-def dice_coef_loss(y_true, y_pred):
-    return 1 - dice_coef(y_true, y_pred)
-
-
-def bootstrapped_crossentropy(y_true, y_pred, bootstrap_type="hard", alpha=0.95):
-    target_tensor = y_true
-    prediction_tensor = y_pred
-    _epsilon = tf.convert_to_tensor(
-        tf.keras.backend.epsilon(), prediction_tensor.dtype.base_dtype
-    )
-    prediction_tensor = tf.clip_by_value(
-        prediction_tensor, _epsilon, 1 - _epsilon  # type: ignore
-    )
-    prediction_tensor = tf.keras.backend.log(
-        prediction_tensor / (1 - prediction_tensor)  # type: ignore
-    )
-
-    if bootstrap_type == "soft":
-        bootstrap_target_tensor = alpha * target_tensor + (1.0 - alpha) * tf.sigmoid(
-            prediction_tensor
-        )
-    else:
-        bootstrap_target_tensor = alpha * target_tensor + (1.0 - alpha) * tf.cast(
-            tf.sigmoid(prediction_tensor) > 0.5, tf.float32
-        )  # type: ignore
-    return tf.keras.backend.mean(
-        tf.nn.sigmoid_cross_entropy_with_logits(
-            labels=bootstrap_target_tensor, logits=prediction_tensor
-        )
-    )
-
-
-def dice_coef_loss_bce(y_true, y_pred):
-    dice = 0.5
-    bce = 0.5
-    bootstrapping = "hard"
-    alpha = 1.0
-    return (
-        bootstrapped_crossentropy(y_true, y_pred, bootstrapping, alpha) * bce
-        + dice_coef_loss(y_true, y_pred) * dice
-    )
-
-
-# ------------------------------------------
-# Metrics functions
-# ------------------------------------------
-
-SMOOTH_LOSS = 1e-12
-
-
-def jaccard_coef(y_true, y_pred):
-    intersection = tf.keras.backend.sum(y_true * y_pred, axis=[0, -1, -2])
-    sum_ = tf.keras.backend.sum(y_true + y_pred, axis=[0, -1, -2])
-
-    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
-
-    return tf.keras.backend.mean(jac)
-
-
-def jaccard_coef_round(y_true, y_pred):
-    y_pred_pos = tf.keras.backend.round(tf.keras.backend.clip(y_pred, 0, 1))
-
-    intersection = tf.keras.backend.sum(y_true * y_pred_pos, axis=[0, -1, -2])
-    sum_ = tf.keras.backend.sum(y_true + y_pred_pos, axis=[0, -1, -2])
-    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
-    return tf.keras.backend.mean(jac)
-
-
-def jaccard_coef_flat(y_true, y_pred):
-    y_true_f = tf.keras.backend.flatten(y_true)
-    y_pred_f = tf.keras.backend.flatten(y_pred)
-    intersection = tf.keras.backend.sum(y_true_f * y_pred_f)
-    return (intersection + SMOOTH_LOSS) / (
-        tf.keras.backend.sum(y_true_f)
-        + tf.keras.backend.sum(y_pred_f)
-        - intersection
-        + SMOOTH_LOSS
-    )
-
-
-def dice_coef(y_true, y_pred, smooth=1.0):
-    y_true_f = tf.keras.backend.flatten(y_true)
-    y_pred_f = tf.keras.backend.flatten(y_pred)
-    intersection = tf.keras.backend.sum(y_true_f * y_pred_f)
-    return (2.0 * intersection + smooth) / (
-        tf.keras.backend.sum(y_true_f) + tf.keras.backend.sum(y_pred_f) + smooth
-    )
-
-
-def pct_wrong(y_true, y_pred):
-    y_pred_pos = tf.keras.backend.round(tf.keras.backend.clip(y_pred, 0, 1))
-
-    intersection = tf.keras.backend.sum(y_true * y_pred_pos, axis=[0, -1, -2])
-    sum_ = tf.keras.backend.sum(y_true + y_pred_pos, axis=[0, -1, -2])
-    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
-    return tf.keras.backend.mean(jac)
+# -*- coding: utf-8 -*-
+"""
+Module with helper functions to create models.
+
+Offers a common interface, regardless of the underlying model implementation
+and contains extra metrics, callbacks,...
+
+Many models are supported by using this segmentation model zoo:
+https://github.com/qubvel/segmentation_models
+"""
+
+import json
+import logging
+from pathlib import Path
+from typing import Any, List, Optional
+
+import numpy as np
+import tensorflow as tf
+import keras.models
+import segmentation_models as sm
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.INFO)
+
+# Force using the keras implementation in tensorflow, because the default
+# use of this implementation seems broken with tensorflow 2.5
+sm.set_framework("tf.keras")
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+"""
+preprocessing_fn = get_preprocessing('resnet34')
+x = preprocessing_fn(x)
+"""
+
+
+def get_model(
+    architecture: str,
+    input_width: Optional[int] = None,
+    input_height: Optional[int] = None,
+    nb_channels: int = 3,
+    nb_classes: int = 1,
+    activation: str = "softmax",
+    init_weights_with: str = "imagenet",
+    freeze: bool = False,
+) -> keras.models.Model:
+    """
+    Get a model.
+
+    Args:
+        architecture (str): Architecture of the network to create
+        input_width (int, optional): Width of the input images. Defaults to None.
+        input_height (int, optional): Height of the input images. Defaults to None.
+        nb_channels (int, optional): Nb of channels/bands of the input images.
+            Defaults to 3.
+        nb_classes (int, optional): Nb of classes to be segmented to. Defaults to 1.
+        activation (Activation, optional): Activation function of last layer.
+            Defaults to 'softmax'.
+        init_weights_with (str, optional): Weights to init the network with.
+            Defaults to 'imagenet'.
+        freeze (bool, optional): Freeze the final layer weights during
+            training. It is usefull to use this option for the first few
+            epochs get a more robust network. Defaults to False.
+
+    Raises:
+        Exception: [description]
+        Exception: [description]
+
+    Returns:
+        [type]: [description]
+    """
+    # Check architecture
+    segment_architecture_parts = architecture.split("+")
+    if len(segment_architecture_parts) < 2:
+        raise Exception(f"Unsupported architecture: {architecture}")
+    encoder = segment_architecture_parts[0]
+    decoder = segment_architecture_parts[1]
+
+    if decoder.lower() == "unet":
+        # Architecture implemented using the segmentation_models library
+        from segmentation_models import Unet
+
+        model = Unet(
+            backbone_name=encoder.lower(),
+            input_shape=(input_width, input_height, nb_channels),
+            classes=nb_classes,
+            activation=activation,
+            encoder_weights=init_weights_with,
+            encoder_freeze=freeze,
+        )
+        return model
+
+    elif decoder.lower() == "pspnet":
+        # Architecture implemented using the segmentation_models library
+        from segmentation_models import PSPNet
+
+        model = PSPNet(
+            backbone_name=encoder.lower(),
+            input_shape=(input_width, input_height, nb_channels),
+            classes=nb_classes,
+            activation=activation,
+            encoder_weights=init_weights_with,
+            encoder_freeze=freeze,
+        )
+        return model
+
+    elif decoder.lower() == "linknet":
+        # Architecture implemented using the segmentation_models library
+        from segmentation_models import Linknet
+
+        # First check if input size is compatible with linknet
+        if input_width is not None and input_height is not None:
+            check_image_size(decoder, input_width, input_height)
+
+        model = Linknet(
+            backbone_name=encoder.lower(),
+            input_shape=(input_width, input_height, nb_channels),
+            classes=nb_classes,
+            activation=activation,
+            encoder_weights=init_weights_with,
+            encoder_freeze=freeze,
+        )
+        return model
+
+    else:
+        raise ValueError(f"Unknown decoder architecture: {decoder}")
+
+
+def compile_model(
+    model: keras.models.Model,
+    optimizer: str,
+    optimizer_params: dict,
+    loss: str,
+    metrics: Optional[List[str]] = None,
+    sample_weight_mode: Optional[str] = None,
+    class_weights: Optional[list] = None,
+) -> keras.models.Model:
+    """
+    Compile the model for training.
+
+    Args:
+        model (keras.models.Model): the keras model to compile.
+        optimizer (str): the optimizer to use.
+        optimizer_params (dict): parameters to use for optimizer.
+        loss (str): the loss function to use. One of:
+            * categorical_crossentropy
+            * weighted_categorical_crossentropy: class_weights should be specified!
+
+        metrics (List[Metric], optional): metrics to use. Defaults to None. One of:
+            *
+        sample_weight_mode (str, optional): sample weight mode to use. Defaults to None.
+        class_weights (list, optional): class weigths to use. Defaults to None.
+    """
+    # Get number classes of model
+    nb_classes = model.output[-1].shape[-1]
+
+    # If no metrics specified, use default ones
+    metric_funcs: List[Any] = []
+    if metrics is None:
+        if loss in ["categorical_crossentropy", "weighted_categorical_crossentropy"]:
+            metric_funcs.append("categorical_accuracy")
+        elif loss == "sparse_categorical_crossentropy":
+            # metrics.append('sparse_categorical_accuracy')
+            logger.warning("loss == sparse_categorical_crossentropy not implementedd")
+        elif loss == "binary_crossentropy":
+            metric_funcs.append("binary_accuracy")
+
+        onehot_mean_iou = tf.keras.metrics.OneHotMeanIoU(
+            num_classes=nb_classes, name="one_hot_mean_iou"
+        )
+        metric_funcs.append(onehot_mean_iou)
+    else:
+        raise Exception("Specifying metrics not yet implemented")
+
+    # Check loss function
+    if loss == "bcedice":
+        loss_func = dice_coef_loss_bce
+    elif loss == "dice_loss":
+        loss_func = sm.losses.DiceLoss()
+    elif loss == "jaccard_loss":
+        loss_func = sm.losses.JaccardLoss()
+    elif loss == "weighted_categorical_crossentropy":
+        if class_weights is None:
+            raise Exception(f"With loss == {loss}, class_weights cannot be None!")
+        loss_func = weighted_categorical_crossentropy(class_weights)
+    else:
+        loss_func = loss
+
+    # Create optimizer
+    if optimizer == "adam":
+        optimizer_func = tf.keras.optimizers.Adam(**optimizer_params)
+    else:
+        raise Exception(
+            f"Error creating optimizer: {optimizer}, with params {optimizer_params}"
+        )
+
+    logger.info(
+        f"Compile model, optimizer: {optimizer}, loss: {loss}, "
+        f"class_weights: {class_weights}"
+    )
+    model.compile(
+        optimizer=optimizer_func,
+        loss=loss_func,
+        metrics=metric_funcs,
+        sample_weight_mode=sample_weight_mode,
+    )
+
+    return model
+
+
+def load_model(model_to_use_filepath: Path, compile: bool = True) -> keras.models.Model:
+    """
+    Load an existing model from a file.
+
+    If loading the architecture + model from the file doesn't work, tries
+    different things to load a model anyway:
+    1) looks for a ..._model.json file to load the architecture from,
+       the weights are then loaded from the original file
+    2) looks for a ..._hyperparams.json file to create the architecture from,
+       the weights are then loaded from the original file
+
+    Args:
+        model_to_use_filepath (Path): The file to load the model from.
+        compile (bool, optional): True to get a compiled version back that is
+            ready to train. Defaults to True.
+
+    Raises:
+        Exception: [description]
+
+    Returns:
+        tf.keras.models.Model: The loaded model.
+    """
+    errors = []
+    model = None
+    model_basestem = f"{'_'.join(model_to_use_filepath.stem.split('_')[0:2])}"
+
+    # If it is a file with the complete model, try loading it entirely...
+    if not model_to_use_filepath.stem.endswith("_weights"):
+        # Load the hyperparams file
+        hyperparams_json_filepath = (
+            model_to_use_filepath.parent / f"{model_basestem}_hyperparams.json"
+        )
+        nb_classes = 1
+        if hyperparams_json_filepath.exists():
+            with hyperparams_json_filepath.open("r") as src:
+                hyperparams = json.load(src)
+                nb_classes = len(hyperparams["architecture"]["classes"])
+
+        iou_score = sm.metrics.IOUScore()
+        f1_score = sm.metrics.FScore()
+        onehot_mean_iou = tf.keras.metrics.OneHotMeanIoU(
+            num_classes=nb_classes, name="one_hot_mean_iou"
+        )
+
+        try:
+            model = tf.keras.models.load_model(
+                str(model_to_use_filepath),
+                custom_objects={
+                    "jaccard_coef": jaccard_coef,
+                    "jaccard_coef_flat": jaccard_coef_flat,
+                    "jaccard_coef_round": jaccard_coef_round,
+                    "dice_coef": dice_coef,
+                    "iou_score": iou_score,
+                    "f1_score": f1_score,
+                    "one_hot_mean_iou": onehot_mean_iou,
+                    "weighted_categorical_crossentropy": weighted_categorical_crossentropy,  # noqa: E501
+                },
+                compile=compile,
+            )
+        except Exception as ex:
+            errors.append(
+                f"Error loading model+weights from {model_to_use_filepath}: {ex}"
+            )
+
+    # If no model returned yet, try loading loading architecture and weights seperately
+    if model is None:
+        # Load the architecture from a model.json file
+        # Check if there is a specific model.json file for these weights
+        model_json_filepath = model_to_use_filepath.parent / (
+            model_to_use_filepath.stem.replace("_weights", "") + ".json"
+        )
+        if not model_json_filepath.exists():
+            # If not, check if there is a model.json file for the training session
+            model_json_filepath = (
+                model_to_use_filepath.parent / f"{model_basestem}_model.json"
+            )
+        if model_json_filepath.exists():
+            with model_json_filepath.open("r") as src:
+                model_json = src.read()
+            try:
+                model = tf.keras.models.model_from_json(model_json)
+            except Exception as ex:
+                errors.append(
+                    f"Error loading model architecture from {model_json_filepath}: {ex}"
+                )
+        else:
+            errors.append(
+                f"No model.json file found to load model from: {model_json_filepath}"
+            )
+
+        # If loading model.json not successfull, create model based on hyperparams.json
+        if model is None:
+            # Load the hyperparams file if available
+            hyperparams_json_filepath = (
+                model_to_use_filepath.parent / f"{model_basestem}_hyperparams.json"
+            )
+            if hyperparams_json_filepath.exists():
+                with hyperparams_json_filepath.open("r") as src:
+                    hyperparams = json.load(src)
+                # Create the model we want to use
+                try:
+                    model = get_model(
+                        architecture=hyperparams["architecture"]["architecture"],
+                        nb_channels=hyperparams["architecture"]["nb_channels"],
+                        nb_classes=hyperparams["architecture"]["nb_classes"],
+                        activation=hyperparams["architecture"]["activation_function"],
+                    )
+                except Exception as ex:
+                    errors.append(
+                        "Error in get_model() with params from: "
+                        f"{hyperparams_json_filepath}: {ex}"
+                    )
+            else:
+                errors.append(
+                    f"No file found to load model from: {hyperparams_json_filepath}"
+                )
+
+        # Now load the weights
+        if model is not None:
+            try:
+                model.load_weights(str(model_to_use_filepath))
+            except Exception as ex:
+                errors.append(
+                    f"Error trying model.load_weights on: {model_to_use_filepath}: {ex}"
+                )
+
+    # Check if a model got loaded...
+    if model is not None:
+        # Eager seems to be 50% slower, tested on tensorflow 2.5
+        model.run_eagerly = False
+    else:
+        # If we still have not model... time to give up.
+        errors_str = ""
+        if len(errors) > 0:
+            errors_str = (
+                " The following errors occured while trying: \n    -> "
+                + "\n    -> ".join(errors)
+            )
+        raise Exception(f"Error loading model for {model_to_use_filepath}.{errors_str}")
+
+    return model  # type: ignore
+
+
+def set_trainable(model, recompile: bool = True):
+    sm.utils.set_trainable(
+        model=model, recompile=recompile
+    )  # doesn't seem to work, so save and load model
+
+
+def check_image_size(decoder: str, input_width: int, input_height: int):
+    if decoder.lower() == "linknet":
+        if (input_width and (input_width % 16) != 0) or (
+            input_height and (input_height % 16) != 0
+        ):
+            message = (
+                f"for decoder linknet, input_width ({input_width} and input_height "
+                f"({input_height}) should be divisable by 16!"
+            )
+            logger.error(message)
+            raise ValueError(message)
+    else:
+        logger.info(f"check_image_size is not implemented for this model: {decoder}")
+
+
+# ------------------------------------------
+# Loss functions
+# ------------------------------------------
+
+
+def weighted_categorical_crossentropy(weights):
+    """weighted_categorical_crossentropy
+
+    Args:
+        * weights<ktensor|nparray|list>: crossentropy weights
+    Returns:
+        * weighted categorical crossentropy function
+    """
+    if isinstance(weights, list) or isinstance(weights, np.ndarray):
+        weights = tf.keras.backend.variable(weights)
+
+    def loss(target, output, from_logits=False):
+        if not from_logits:
+            output /= tf.reduce_sum(output, len(output.get_shape()) - 1, True)
+            _epsilon = tf.convert_to_tensor(
+                tf.keras.backend.epsilon(), dtype=output.dtype.base_dtype
+            )
+            output = tf.clip_by_value(output, _epsilon, 1.0 - _epsilon)  # type: ignore
+            weighted_losses = target * tf.math.log(output) * weights
+            retval = -tf.reduce_sum(
+                weighted_losses, len(output.get_shape()) - 1  # type: ignore
+            )
+            return retval
+        else:
+            raise ValueError("WeightedCategoricalCrossentropy: not valid with logits")
+
+    return loss
+
+
+def dice_coef_loss(y_true, y_pred):
+    return 1 - dice_coef(y_true, y_pred)
+
+
+def bootstrapped_crossentropy(y_true, y_pred, bootstrap_type="hard", alpha=0.95):
+    target_tensor = y_true
+    prediction_tensor = y_pred
+    _epsilon = tf.convert_to_tensor(
+        tf.keras.backend.epsilon(), prediction_tensor.dtype.base_dtype
+    )
+    prediction_tensor = tf.clip_by_value(
+        prediction_tensor, _epsilon, 1 - _epsilon  # type: ignore
+    )
+    prediction_tensor = tf.keras.backend.log(
+        prediction_tensor / (1 - prediction_tensor)  # type: ignore
+    )
+
+    if bootstrap_type == "soft":
+        bootstrap_target_tensor = alpha * target_tensor + (1.0 - alpha) * tf.sigmoid(
+            prediction_tensor
+        )
+    else:
+        bootstrap_target_tensor = alpha * target_tensor + (1.0 - alpha) * tf.cast(
+            tf.sigmoid(prediction_tensor) > 0.5, tf.float32
+        )  # type: ignore
+    return tf.keras.backend.mean(
+        tf.nn.sigmoid_cross_entropy_with_logits(
+            labels=bootstrap_target_tensor, logits=prediction_tensor
+        )
+    )
+
+
+def dice_coef_loss_bce(y_true, y_pred):
+    dice = 0.5
+    bce = 0.5
+    bootstrapping = "hard"
+    alpha = 1.0
+    return (
+        bootstrapped_crossentropy(y_true, y_pred, bootstrapping, alpha) * bce
+        + dice_coef_loss(y_true, y_pred) * dice
+    )
+
+
+# ------------------------------------------
+# Metrics functions
+# ------------------------------------------
+
+SMOOTH_LOSS = 1e-12
+
+
+def jaccard_coef(y_true, y_pred):
+    intersection = tf.keras.backend.sum(y_true * y_pred, axis=[0, -1, -2])
+    sum_ = tf.keras.backend.sum(y_true + y_pred, axis=[0, -1, -2])
+
+    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
+
+    return tf.keras.backend.mean(jac)
+
+
+def jaccard_coef_round(y_true, y_pred):
+    y_pred_pos = tf.keras.backend.round(tf.keras.backend.clip(y_pred, 0, 1))
+
+    intersection = tf.keras.backend.sum(y_true * y_pred_pos, axis=[0, -1, -2])
+    sum_ = tf.keras.backend.sum(y_true + y_pred_pos, axis=[0, -1, -2])
+    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
+    return tf.keras.backend.mean(jac)
+
+
+def jaccard_coef_flat(y_true, y_pred):
+    y_true_f = tf.keras.backend.flatten(y_true)
+    y_pred_f = tf.keras.backend.flatten(y_pred)
+    intersection = tf.keras.backend.sum(y_true_f * y_pred_f)
+    return (intersection + SMOOTH_LOSS) / (
+        tf.keras.backend.sum(y_true_f)
+        + tf.keras.backend.sum(y_pred_f)
+        - intersection
+        + SMOOTH_LOSS
+    )
+
+
+def dice_coef(y_true, y_pred, smooth=1.0):
+    y_true_f = tf.keras.backend.flatten(y_true)
+    y_pred_f = tf.keras.backend.flatten(y_pred)
+    intersection = tf.keras.backend.sum(y_true_f * y_pred_f)
+    return (2.0 * intersection + smooth) / (
+        tf.keras.backend.sum(y_true_f) + tf.keras.backend.sum(y_pred_f) + smooth
+    )
+
+
+def pct_wrong(y_true, y_pred):
+    y_pred_pos = tf.keras.backend.round(tf.keras.backend.clip(y_pred, 0, 1))
+
+    intersection = tf.keras.backend.sum(y_true * y_pred_pos, axis=[0, -1, -2])
+    sum_ = tf.keras.backend.sum(y_true + y_pred_pos, axis=[0, -1, -2])
+    jac = (intersection + SMOOTH_LOSS) / (sum_ - intersection + SMOOTH_LOSS)
+    return tf.keras.backend.mean(jac)
```

### Comparing `orthoseg-0.4.2/orthoseg/model/model_helper.py` & `orthoseg-0.4.2a1/orthoseg/model/model_helper.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,813 +1,813 @@
-# -*- coding: utf-8 -*-
-"""
-Module with helper functions regarding (keras) models.
-"""
-
-import json
-import logging
-from pathlib import Path
-import shutil
-from typing import List, Optional
-
-import pandas as pd
-from keras import callbacks
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.INFO)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-class ArchitectureParams:
-    def __init__(
-        self,
-        architecture: str,
-        classes: Optional[list] = None,
-        nb_channels: int = 3,
-        activation_function: str = "softmax",
-        architecture_id: int = 0,
-    ):
-        """
-        Class containing the hyper parameters needed to create the model.
-
-        Args:
-            architecture (str): the model architecture to use.
-            classes (list, optional): list of classes that will be detected by
-                the model. Default to None, and then 2 generic classes are
-                supposed.
-            nb_channels (int, optional): Number of channels of the images.
-                Defaults to 3.
-            activation_function (str, optional): activation function to use.
-                Defaults to softmax.
-            architecture_id (int, optional): id of the architecture.
-                Defaults to 0.
-        """
-        self.architecture = architecture
-        if classes is not None:
-            self.classes = classes
-        else:
-            self.classes = ["background", "segmentsubject"]
-        self.nb_channels = nb_channels
-        self.activation_function = activation_function
-        self.architecture_id = architecture_id
-
-    def toJSON(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
-
-
-class TrainParams:
-    def __init__(
-        self,
-        image_augmentations: dict,
-        mask_augmentations: dict,
-        trainparams_id: int = 0,
-        class_weights: Optional[list] = None,
-        batch_size: int = 4,
-        optimizer: str = "adam",
-        optimizer_params: Optional[dict] = None,
-        loss_function: Optional[str] = None,
-        monitor_metric: Optional[str] = None,
-        monitor_metric_mode: str = "auto",
-        save_format: str = "h5",
-        save_best_only: bool = True,
-        save_min_accuracy: float = 0.95,
-        nb_epoch: int = 1000,
-        nb_epoch_with_freeze: int = 100,
-        earlystop_patience: int = 100,
-        earlystop_monitor_metric: Optional[str] = None,
-        earlystop_monitor_metric_mode: str = "auto",
-        log_tensorboard: bool = False,
-        log_csv: bool = True,
-    ):
-        """
-        Class containing the hyper parameters needed to perform a training.
-
-        Args:
-            image_augmentations (dict): The augmentations to use on the input image
-                during training.
-            mask_augmentations (dict): The augmentations to use on the input mask
-                during training.
-            architecture_id (int, optional): id of the architecture. Defaults to 0.
-            trainparams_id (int, optional): id of the hyperparams. Defaults to 0.
-            class_weights (list, optional): [description]. Defaults to None.
-            batch_size (int, optional): batch size to use while training. This must be
-                choosen depending on the neural network architecture
-                and available memory on you GPU. Defaults to 4.
-            optimizer (str, optional): Optimizer to use for training.
-                Defaults to 'adam'.
-            optimizer_params (dict, optional): Optimizer params to use.
-                Defaults to { 'learning_rate': 0.0001 }.
-            loss_function (str, optional): [description]. Defaults to None.
-            monitor_metric (str, optional): Metric to monitor. If not specified
-                the loss function will drive the metric. Defaults to None.
-            monitor_metric_mode (str, optional): Mode of the metric to monitor.
-                Defaults to 'auto'.
-            save_format (str, optional): [description]. Defaults to 'h5'.
-            save_best_only (bool, optional): [description]. Defaults to True.
-            save_min_accuracy (float, optional): minimum accuracy to save a model.
-                Defaults to 0.95.
-            nb_epoch (int, optional): maximum number of epochs to train.
-                Defaults to 1000.
-            nb_epoch_with_freeze (int, optional): number epochs to train with
-                    part of the layers frozen. Defaults to 20.
-            earlystop_patience (int, optional): [description]. Defaults to 100.
-            earlystop_monitor_metric (str, optional): [description]. Defaults to None.
-            earlystop_monitor_metric_mode (str, optional): Mode to monitor the
-                metric: 'max' if the metric should be as high as possible,
-                'min' if it should be low. Defaults to 'auto'.
-            log_tensorboard (bool, optional): True to activate tensorboard
-                logging. Defaults to False.
-            log_csv (bool, optional): True to activate logging to a csv.
-                Defaults to True
-
-        Raises:
-            Exception: [description]
-        """
-        self.trainparams_id = trainparams_id
-        self.image_augmentations = image_augmentations
-        self.mask_augmentations = mask_augmentations
-        self.class_weights = class_weights
-        self.batch_size = batch_size
-
-        self.optimizer = optimizer
-        if optimizer_params is None:
-            # Best set to 0.0001 to start (1e-3 is not ok)
-            self.optimizer_params = {"learning_rate": 0.0001}
-        else:
-            self.optimizer_params = optimizer_params
-
-        if self.class_weights is not None:
-            self.loss_function = "weighted_categorical_crossentropy"
-        else:
-            self.loss_function = "categorical_crossentropy"
-
-        # Properties to choose the best model
-        if monitor_metric is not None:
-            self.monitor_metric = monitor_metric
-        elif self.loss_function in (
-            "weighted_categorical_crossentropy",
-            "categorical_crossentropy",
-        ):
-            self.monitor_metric = "categorical_accuracy"
-        self.monitor_metric_mode = monitor_metric_mode
-
-        self.save_format = save_format
-        self.save_best_only = save_best_only
-        self.save_min_accuracy = save_min_accuracy
-        self.nb_epoch = nb_epoch
-        self.nb_epoch_with_freeze = nb_epoch_with_freeze
-
-        # Properties to stop the training
-        self.earlystop_patience = earlystop_patience
-        if earlystop_monitor_metric is not None:
-            self.earlystop_monitor_metric = earlystop_monitor_metric
-        else:
-            self.earlystop_monitor_metric = self.monitor_metric
-        self.earlystop_monitor_metric_mode = earlystop_monitor_metric_mode
-
-        # Properties regarding logging
-        self.log_tensorboard = log_tensorboard
-        self.log_csv = log_csv
-
-    def toJSON(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
-
-
-class HyperParams:
-    def __init__(
-        self,
-        architecture: Optional[ArchitectureParams] = None,
-        train: Optional[TrainParams] = None,
-        path: Optional[Path] = None,
-    ):
-        """
-        Class to store the hyper parameters to use for the machine learning algorythm.
-
-        Args:
-            architecture (ArchitectureParams): the fixed parameters that define the
-                architecture of the neural network. When training a network, it is
-                possible to reuse the weights of another network if these parameters
-                are the same.
-            train (TrainParams): these are the parameters that can be changed with each
-                training.
-        """
-        self.fileversion = 1.1
-        if architecture is not None:
-            self.architecture = architecture
-        if train is not None:
-            self.train = train
-        if path is not None:
-            with open(path, "r") as jsonfile:
-                jsonstr = jsonfile.read()
-                data = json.loads(jsonstr)
-
-                # Read file version if it is present
-                if "fileversion" in data:
-                    self.fileversion = data["fileversion"]
-
-                # Now parse the real data. For backwards compatibility, remove
-                # 'nb_classes' parameter if it exists
-                if "nb_classes" in data["architecture"]:
-                    del data["architecture"]["nb_classes"]
-
-                self.architecture = ArchitectureParams(**data["architecture"])
-                self.train = TrainParams(**data["train"])
-
-    def toJSON(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
-
-
-def format_model_basefilename(
-    segment_subject: str,
-    traindata_id: int,
-    architecture_id: int = 0,
-    trainparams_id: int = 0,
-) -> str:
-    """
-    Format the parameters into a model_filename.
-
-    Args
-        segment_subject: the segment subject
-        traindata_id: the id of the data used to train the model
-        architecture_id: the id of the model architecture used
-        trainparams_id: the id of the hyper parameters used to train the model
-    """
-    # Format file name
-    filename = f"{segment_subject}_{traindata_id:02d}"
-
-    # If an architecture id and/or hyperparams id is specified, add those as well
-    if architecture_id > 0 or trainparams_id > 0:
-        filename = f"{filename}.{architecture_id}.{trainparams_id}"
-    return filename
-
-
-def format_model_filename(
-    segment_subject: str,
-    traindata_id: int,
-    architecture_id: int,
-    trainparams_id: int,
-    monitor_metric_accuracy: float,
-    epoch: int,
-    save_format: str,
-) -> str:
-    """
-    Format the parameters into a model_filename.
-
-    Args
-        segment_subject: the segment subject
-        traindata_id: the version of the data used to train the model
-        architecture_id: the id of the model architecture used
-        trainparams_id: the version of the hyper parameters used to train
-        monitor_metric_accuracy: the monitor metric accuracy
-        epoch: the epoch during training that reached these model weights
-        save_format (str): the format to save in:
-            * keras format: 'h5'
-            * tensorflow savedmodel: 'tf'
-    """
-    # Format file name
-    filename = format_model_basefilename(
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        architecture_id=architecture_id,
-        trainparams_id=trainparams_id,
-    )
-    filename += f"_{monitor_metric_accuracy:.5f}_{epoch}"
-
-    # Add suffix
-    if save_format == "tf":
-        filename += "_tf"
-    else:
-        filename += ".hdf5"
-
-    return filename
-
-
-def parse_model_filename(filepath: Path) -> Optional[dict]:
-    """
-    Parse a model_filename to a dict containing the properties of the model:
-        * segment_subject: the segment subject
-        * traindata_id: the version of the data used to train the model
-        * monitor_metric_accuracy: the monitored metric accuracy
-        * trainparams_id: the version of the hyper parameters used to train
-        * epoch: the epoch during training that reached these model weights
-        * save_format (str): the format to save in:
-            * keras format: 'h5'
-            * tensorflow savedmodel: 'tf'
-
-    Args
-        filepath: the filepath to the model file
-    """
-
-    # Prepare filepath to extract info
-    if filepath.is_dir():
-        # If it is a dir, it should end on _tf
-        if not filepath.name.endswith("_tf"):
-            logger.warning(
-                f"Not a valid path for a model, dir needs to end on _tf: {filepath}"
-            )
-            return None
-        save_format = "tf"
-        filename = filepath.name
-    else:
-        filename = filepath.stem
-        if filepath.suffix in (".h5", ".hdf5"):
-            save_format = "h5"
-        else:
-            logger.warning(f"Model file should have .h5 of .hdf5 as suffix: {filepath}")
-            return None
-
-    # Now extract the fields...
-    param_values = filename.split("_")
-    if len(param_values) < 3:
-        logger.warning(
-            f"Model file name nok, split('_') must result in >= 2 fields: {filepath}"
-        )
-
-    segment_subject = param_values[0]
-
-    model_info = param_values[1]
-    model_info_values = model_info.split(".")
-    traindata_id = int(model_info_values[0])
-    architecture_id = 0
-    trainparams_id = 0
-    if len(model_info_values) > 1:
-        architecture_id = int(model_info_values[1])
-        if len(model_info_values) > 2:
-            trainparams_id = int(model_info_values[2])
-
-    monitor_metric_accuracy = float(param_values[2])
-    epoch = int(param_values[3])
-
-    basefilename = format_model_basefilename(
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        architecture_id=architecture_id,
-        trainparams_id=trainparams_id,
-    )
-
-    return {
-        "filepath": filepath,
-        "filename": filename,
-        "basefilename": basefilename,
-        "segment_subject": segment_subject,
-        "traindata_id": traindata_id,
-        "architecture_id": architecture_id,
-        "trainparams_id": trainparams_id,
-        "monitor_metric_accuracy": monitor_metric_accuracy,
-        "epoch": epoch,
-        "save_format": save_format,
-    }
-
-
-def get_models(
-    model_dir: Path,
-    segment_subject: Optional[str] = None,
-    traindata_id: Optional[int] = None,
-    architecture_id: Optional[int] = None,
-    trainparams_id: Optional[int] = None,
-) -> List[dict]:
-    """
-    Return the list of models in the model_dir passed. It is returned as a
-    dataframe with the columns as returned in parse_model_filename()
-
-    Args
-        model_dir (Path): dir containing the models
-        segment_subject (str, optional): only models with this the segment subject
-        traindata_id (int, optional): only models with this traindata version
-        architecture_id (int, optional): only models with this this architecture_id
-        trainparams_id (int, optional): only models with this hyperparams version
-    """
-
-    # List models
-    model_paths = []
-    model_paths.extend(model_dir.glob("*.hdf5"))
-    model_paths.extend(model_dir.glob("*.h5"))
-    model_paths.extend(model_dir.glob("*_tf"))
-
-    # Loop through all models and extract necessary info...
-    model_info_list = []
-    for model_path in model_paths:
-        model_info = parse_model_filename(model_path)
-        if model_info is not None:
-            model_info_list.append(model_info)
-
-    # Filter, if filters provided
-    if len(model_info_list) > 0:
-        if segment_subject is not None:
-            model_info_list = [
-                model_info
-                for model_info in model_info_list
-                if model_info["segment_subject"] == segment_subject
-            ]
-        if traindata_id is not None:
-            model_info_list = [
-                model_info
-                for model_info in model_info_list
-                if model_info["traindata_id"] == traindata_id
-            ]
-        if trainparams_id is not None:
-            model_info_list = [
-                model_info
-                for model_info in model_info_list
-                if model_info["trainparams_id"] == trainparams_id
-            ]
-        if architecture_id is not None:
-            model_info_list = [
-                model_info
-                for model_info in model_info_list
-                if model_info["architecture_id"] == architecture_id
-            ]
-
-    return model_info_list
-
-
-def get_best_model(
-    model_dir: Path,
-    segment_subject: Optional[str] = None,
-    traindata_id: Optional[int] = None,
-    architecture_id: Optional[int] = None,
-    trainparams_id: Optional[int] = None,
-) -> Optional[dict]:
-    """
-    Get the properties of the model with the highest combined accuracy for the highest
-    traindata version in the dir.
-
-    Remark: regardless of the monitor function used when training, the accuracies
-    are always better if higher!
-
-    Args
-        model_dir: dir containing the models
-        segment_subject (str, optional): only models with this the segment subject
-        traindata_id (int, optional): only models with this train data id
-        architecture_id (int, optional): only models with this the architecture_id
-        trainparams_id (int, optional): only models with this hyperparams id
-
-    Returns
-        A dictionary with the info of the best model, or None if no model was found
-    """
-    # Get list of existing models for this train dataset
-    model_info_list = get_models(
-        model_dir=model_dir,
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        architecture_id=architecture_id,
-        trainparams_id=trainparams_id,
-    )
-
-    # If nothing found, return None
-    if len(model_info_list) == 0:
-        return None
-
-    # If no traindata_id provided, find highest traindata id
-    max_traindata_id = -1
-    for model_info in model_info_list:
-        if model_info["traindata_id"] > max_traindata_id:
-            max_traindata_id = model_info["traindata_id"]
-
-    # Get the list of newest model
-    newest_model_info_list = [
-        model_info
-        for model_info in model_info_list
-        if model_info["traindata_id"] == max_traindata_id
-    ]
-
-    # If only one result, return it
-    if len(newest_model_info_list) == 1:
-        return newest_model_info_list[0]
-    else:
-        max_monitor_metric_accuracy = -1
-        max_monitor_metric_accuracy_idx = -1
-        for model_info_idx, model_info in enumerate(model_info_list):
-            if model_info["monitor_metric_accuracy"] > max_monitor_metric_accuracy:
-                max_monitor_metric_accuracy = model_info["monitor_metric_accuracy"]
-                max_monitor_metric_accuracy_idx = model_info_idx
-
-        return model_info_list[max_monitor_metric_accuracy_idx]
-
-
-class ModelCheckpointExt(callbacks.Callback):
-    def __init__(
-        self,
-        model_save_dir: Path,
-        segment_subject: str,
-        traindata_id: int,
-        architecture_id: int,
-        trainparams_id: int,
-        monitor_metric: str,
-        monitor_metric_mode: str,
-        save_format: str = "h5",
-        save_best_only: bool = False,
-        save_min_accuracy: float = 0.90,
-        save_min_accuracy_ignored_epoch: int = 100,
-        save_weights_only: bool = False,
-        model_template_for_save=None,
-        verbose: bool = True,
-        only_report: bool = False,
-    ):
-        """
-        Constructor
-
-        Args:
-            model_save_dir (Path): [description]
-            segment_subject (str): segment subject
-            traindata_id (int): train data id
-            architecture_id (int): model architecture id
-            trainparams_id (int): id of the hyper parameters used
-            monitor_metric (str): The metric to monitor for accuracy
-            monitor_metric_mode (str): use 'min' if the accuracy metrics
-                should be  as low as possible, 'max' if a higher values is
-                better.
-            save_format (str, optional): The format to save in:
-                'h5' (keras format) or 'tf' (tensorflow savedmodel).
-                Defaults to 'tf'
-            save_best_only (bool, optional): only keep the best model.
-                Defaults to True.
-            save_min_accuracy (float, optional): minimum accuracy to be
-                reached to save model. Defaults to 0.9.
-            save_min_accuracy_ignored_epoch (int, optional): at this epoch the
-                save_min_accuracy is ignored, to make sure there is a model
-                saved, even if the minimum accuracy is never reached.
-            save_weights_only: optional: only save weights
-            model_template_for_save: optional, if using multi-GPU training,
-                pass the original model here to use this as template for saving
-            verbose (bool, optional): [description]. Defaults to True.
-            only_report (bool, optional): [description]. Defaults to False.
-        """
-        monitor_metric_mode_values = ["min", "max"]
-        if monitor_metric_mode not in monitor_metric_mode_values:
-            raise Exception(
-                f"Invalid value for mode: {monitor_metric_mode}, should be one of "
-                f"{monitor_metric_mode_values}"
-            )
-        save_format_values = ("h5", "tf")
-        if save_format not in save_format_values:
-            raise Exception(
-                f"Invalid value for save_format: {save_format}, should be one of "
-                f"{save_format_values}"
-            )
-
-        self.model_save_dir = model_save_dir
-        self.segment_subject = segment_subject
-        self.traindata_id = traindata_id
-        self.architecture_id = architecture_id
-        self.trainparams_id = trainparams_id
-        self.monitor_metric = monitor_metric
-        self.monitor_metric_mode = monitor_metric_mode
-        self.save_format = save_format
-        self.save_best_only = save_best_only
-        self.save_min_accuracy = save_min_accuracy
-        self.save_min_accuracy_ignored_epoch = save_min_accuracy_ignored_epoch
-        self.save_weights_only = save_weights_only
-        self.model_template_for_save = model_template_for_save
-        self.verbose = verbose
-        self.only_report = only_report
-
-    def on_epoch_end(self, epoch, logs={}):
-        logger.debug(f"Start in callback on_epoch_begin, logs contains: {logs}")
-
-        # First determine the values of the monitor metric for train and validation
-        # If the monitor_metric doesn't contain placeholder, it is easy
-        if "{" not in self.monitor_metric:
-            new_model_monitor_value = logs.get(self.monitor_metric)
-        else:
-            # There are placeholders, so we need some more logic
-            monitor_metric_formatted = self.monitor_metric.format(**logs)
-            new_model_monitor_value = eval(monitor_metric_formatted, {}, {})
-
-        # Now we can save and clean models
-        save_and_clean_models(
-            model_save_dir=self.model_save_dir,
-            segment_subject=self.segment_subject,
-            traindata_id=self.traindata_id,
-            architecture_id=self.architecture_id,
-            trainparams_id=self.trainparams_id,
-            monitor_metric_mode=self.monitor_metric_mode,
-            new_model=self.model,
-            new_model_monitor_value=new_model_monitor_value,
-            new_model_epoch=epoch,
-            save_format=self.save_format,
-            save_best_only=self.save_best_only,
-            save_min_accuracy=self.save_min_accuracy,
-            save_min_accuracy_ignored_epoch=self.save_min_accuracy_ignored_epoch,
-            save_weights_only=self.save_weights_only,
-            model_template_for_save=self.model_template_for_save,
-            verbose=self.verbose,
-            only_report=self.only_report,
-        )
-
-
-def save_and_clean_models(
-    model_save_dir: Path,
-    segment_subject: str,
-    traindata_id: int,
-    architecture_id: int,
-    trainparams_id: int,
-    monitor_metric_mode: str,
-    new_model=None,
-    new_model_monitor_value: Optional[float] = None,
-    new_model_epoch: Optional[int] = None,
-    save_format: str = "h5",
-    save_best_only: bool = False,
-    save_min_accuracy: float = 0.9,
-    save_min_accuracy_ignored_epoch: int = 100,
-    save_weights_only: bool = False,
-    model_template_for_save=None,
-    verbose: bool = True,
-    debug: bool = False,
-    only_report: bool = False,
-):
-    """
-    Save the new model if it is good enough... and cleanup existing models
-    if they are worse than the new or other existing models.
-
-    Args
-        model_save_dir (Path): dir containing the models
-        segment_subject (str): segment subject
-        traindata_id (int): train data id
-        architecture_id (int): model architecture id
-        trainparams_id (int): id of the train params
-        model_monitor_metric_mode (MetricMode): use 'min' if the monitored
-            metrics should be as low as possible, 'max' if a higher values
-            is better.
-        new_model (optional): the keras model object that will be saved
-        new_model_monitor_value (float, optional): the monitored metric value
-        new_model_epoch (int, optional): the epoch in the training
-        save_format (SaveFormat, optional): The format to save in:
-            * h5: keras format (= default)
-            * tf: tensorflow savedmodel
-        save_best_only (bool, optional): only keep the best model
-        save_min_accuracy (float, optional): minimum accuracy to save the
-            model. Defaults to 0.9.
-        save_min_accuracy_ignored_epoch (int, optional): at this epoch the
-            save_min_accuracy is ignored, to make sure there is a model saved,
-            even if the minimum accuracy is never reached.
-        save_weights_only (bool, optional): only save weights
-        model_template_for_save (optional): if using multi-GPU training, pass
-            the original model here to use this as template for saving
-        verbose (bool, optional): report the best model after save and cleanup
-        debug (bool, optional): write debug logging
-        only_report (bool, optional): only report which models would be cleaned up
-    """
-    # TODO: add option to specify minimum accuracy/iou score before saving to speed up,
-    # because saving takes quite some time!
-    # Check validaty of input
-    monitor_metric_mode_values = ["min", "max"]
-    if monitor_metric_mode not in monitor_metric_mode_values:
-        raise Exception(
-            f"Invalid value for mode: {monitor_metric_mode}, should be one of "
-            f"{monitor_metric_mode_values}"
-        )
-    save_format_values = ("h5", "tf")
-    if save_format not in save_format_values:
-        raise Exception(
-            f"Invalid value for save_format: {save_format}, should be one of "
-            f"{save_format_values}"
-        )
-
-    # Get a list of all existing models
-    model_info_list = get_models(
-        model_dir=model_save_dir,
-        segment_subject=segment_subject,
-        traindata_id=traindata_id,
-        trainparams_id=trainparams_id,
-    )
-
-    # If there is a new model passed as param, add it to the list
-    new_model_path = None
-    new_model_monitor_accuracy = None
-    if new_model is not None:
-
-        if new_model_monitor_value is None or new_model_epoch is None:
-            raise Exception(
-                "If new_model is not None, new_model_monitor_... parameters cannot be "
-                f"None either???, new_model_monitor_value: {new_model_monitor_value}, "
-                f"new_model_epoch: {new_model_epoch}"
-            )
-
-        # Build save filepath
-        # Remark: accuracy values should always be as high as possible, so
-        # recalculate values if monitor_metric_mode is 'min'
-        if monitor_metric_mode == "max":
-            new_model_monitor_accuracy = new_model_monitor_value
-        else:
-            new_model_monitor_accuracy = 1 - new_model_monitor_value
-
-        new_model_filename = format_model_filename(
-            segment_subject=segment_subject,
-            traindata_id=traindata_id,
-            architecture_id=architecture_id,
-            trainparams_id=trainparams_id,
-            monitor_metric_accuracy=new_model_monitor_accuracy,
-            epoch=new_model_epoch,
-            save_format=save_format,
-        )
-        new_model_path = Path(model_save_dir) / new_model_filename
-
-        # Append model to the retrieved models...
-        model_info_list.append(
-            {
-                "filepath": str(new_model_path),
-                "filename": new_model_filename,
-                "segment_subject": segment_subject,
-                "traindata_id": traindata_id,
-                "architecture_id": architecture_id,
-                "trainparams_id": trainparams_id,
-                "monitor_metric_accuracy": new_model_monitor_accuracy,
-                "epoch": new_model_epoch,
-                "save_format": save_format,
-            }
-        )
-
-    # Loop through all existing models
-    # Remark: the list is sorted descending before iterating it, this way new
-    # modelss are saved bevore deleting the previous best one(s)
-    model_info_df = pd.DataFrame(model_info_list)
-    model_info_sorted_df = model_info_df.sort_values(
-        by="monitor_metric_accuracy", ascending=False
-    )
-    for model_info in model_info_sorted_df.itertuples(index=False):
-
-        # If only the best needs to be kept, check only on monitor_metric_accuracy...
-        keep_model = True
-        better_ones_df = None
-        if save_best_only:
-            better_ones_df = model_info_df[
-                (model_info_df.filepath != model_info.filepath)
-                & (
-                    model_info_df.monitor_metric_accuracy
-                    >= model_info.monitor_metric_accuracy
-                )
-            ]
-            if len(better_ones_df) > 0:
-                keep_model = False
-
-        # If model is (relatively) ok, keep it
-        if keep_model is True:
-            logger.debug(f"KEEP {model_info.filename}")
-
-            # If it is the new model that needs to be kept, keep it or save to disk
-            if (
-                new_model_path is not None
-                and new_model is not None
-                and new_model_epoch is not None
-                and only_report is not True
-                and model_info.filepath == str(new_model_path)
-                and not new_model_path.exists()
-            ):
-                if (
-                    new_model_epoch > save_min_accuracy_ignored_epoch
-                    or model_info.monitor_metric_accuracy > save_min_accuracy
-                ):
-                    logger.debug("Save model start")
-                    if save_weights_only:
-                        if model_template_for_save is not None:
-                            model_template_for_save.save_weights(str(new_model_path))
-                        else:
-                            new_model.save_weights(str(new_model_path))
-                    else:
-                        if model_template_for_save is not None:
-                            model_template_for_save.save(str(new_model_path))
-                        else:
-                            new_model.save(str(new_model_path))
-                    logger.debug("Save model ready")
-                else:
-                    print(
-                        "New model is best, but accuracy < save_min_accuracy: "
-                        f"{new_model_monitor_accuracy} < {save_min_accuracy}"
-                    )
-        else:
-            # Bad model... can be removed (or not saved)
-            if only_report is True:
-                logger.debug(f"DELETE {model_info.filename}")
-            elif Path(model_info.filepath).exists() is True:
-                logger.debug(f"DELETE {model_info.filename}")
-                if Path(model_info.filepath).is_dir() is True:
-                    shutil.rmtree(model_info.filepath)
-                else:
-                    Path(model_info.filepath).unlink()
-
-            if debug is True and better_ones_df is not None:
-                print(f"Better one(s) found for{model_info.filename}:")
-                for better_one in better_ones_df.itertuples(index=False):
-                    print(f"  {better_one.filename}")
-
-    if verbose is True or debug is True:
-        best_model = get_best_model(
-            model_dir=model_save_dir,
-            segment_subject=segment_subject,
-            traindata_id=traindata_id,
-            architecture_id=architecture_id,
-            trainparams_id=trainparams_id,
-        )
-        if best_model is not None:
-            logger.info(
-                f"Current best model for {segment_subject}_{traindata_id}: "
-                f"monitor_metric_accuracy: {best_model['monitor_metric_accuracy']}, "
-                f"epoch: {best_model['epoch']}"
-            )
+# -*- coding: utf-8 -*-
+"""
+Module with helper functions regarding (keras) models.
+"""
+
+import json
+import logging
+from pathlib import Path
+import shutil
+from typing import List, Optional
+
+import pandas as pd
+from keras import callbacks
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.INFO)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+class ArchitectureParams:
+    def __init__(
+        self,
+        architecture: str,
+        classes: Optional[list] = None,
+        nb_channels: int = 3,
+        activation_function: str = "softmax",
+        architecture_id: int = 0,
+    ):
+        """
+        Class containing the hyper parameters needed to create the model.
+
+        Args:
+            architecture (str): the model architecture to use.
+            classes (list, optional): list of classes that will be detected by
+                the model. Default to None, and then 2 generic classes are
+                supposed.
+            nb_channels (int, optional): Number of channels of the images.
+                Defaults to 3.
+            activation_function (str, optional): activation function to use.
+                Defaults to softmax.
+            architecture_id (int, optional): id of the architecture.
+                Defaults to 0.
+        """
+        self.architecture = architecture
+        if classes is not None:
+            self.classes = classes
+        else:
+            self.classes = ["background", "segmentsubject"]
+        self.nb_channels = nb_channels
+        self.activation_function = activation_function
+        self.architecture_id = architecture_id
+
+    def toJSON(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+
+class TrainParams:
+    def __init__(
+        self,
+        image_augmentations: dict,
+        mask_augmentations: dict,
+        trainparams_id: int = 0,
+        class_weights: Optional[list] = None,
+        batch_size: int = 4,
+        optimizer: str = "adam",
+        optimizer_params: Optional[dict] = None,
+        loss_function: Optional[str] = None,
+        monitor_metric: Optional[str] = None,
+        monitor_metric_mode: str = "auto",
+        save_format: str = "h5",
+        save_best_only: bool = True,
+        save_min_accuracy: float = 0.95,
+        nb_epoch: int = 1000,
+        nb_epoch_with_freeze: int = 100,
+        earlystop_patience: int = 100,
+        earlystop_monitor_metric: Optional[str] = None,
+        earlystop_monitor_metric_mode: str = "auto",
+        log_tensorboard: bool = False,
+        log_csv: bool = True,
+    ):
+        """
+        Class containing the hyper parameters needed to perform a training.
+
+        Args:
+            image_augmentations (dict): The augmentations to use on the input image
+                during training.
+            mask_augmentations (dict): The augmentations to use on the input mask
+                during training.
+            architecture_id (int, optional): id of the architecture. Defaults to 0.
+            trainparams_id (int, optional): id of the hyperparams. Defaults to 0.
+            class_weights (list, optional): [description]. Defaults to None.
+            batch_size (int, optional): batch size to use while training. This must be
+                choosen depending on the neural network architecture
+                and available memory on you GPU. Defaults to 4.
+            optimizer (str, optional): Optimizer to use for training.
+                Defaults to 'adam'.
+            optimizer_params (dict, optional): Optimizer params to use.
+                Defaults to { 'learning_rate': 0.0001 }.
+            loss_function (str, optional): [description]. Defaults to None.
+            monitor_metric (str, optional): Metric to monitor. If not specified
+                the loss function will drive the metric. Defaults to None.
+            monitor_metric_mode (str, optional): Mode of the metric to monitor.
+                Defaults to 'auto'.
+            save_format (str, optional): [description]. Defaults to 'h5'.
+            save_best_only (bool, optional): [description]. Defaults to True.
+            save_min_accuracy (float, optional): minimum accuracy to save a model.
+                Defaults to 0.95.
+            nb_epoch (int, optional): maximum number of epochs to train.
+                Defaults to 1000.
+            nb_epoch_with_freeze (int, optional): number epochs to train with
+                    part of the layers frozen. Defaults to 20.
+            earlystop_patience (int, optional): [description]. Defaults to 100.
+            earlystop_monitor_metric (str, optional): [description]. Defaults to None.
+            earlystop_monitor_metric_mode (str, optional): Mode to monitor the
+                metric: 'max' if the metric should be as high as possible,
+                'min' if it should be low. Defaults to 'auto'.
+            log_tensorboard (bool, optional): True to activate tensorboard
+                logging. Defaults to False.
+            log_csv (bool, optional): True to activate logging to a csv.
+                Defaults to True
+
+        Raises:
+            Exception: [description]
+        """
+        self.trainparams_id = trainparams_id
+        self.image_augmentations = image_augmentations
+        self.mask_augmentations = mask_augmentations
+        self.class_weights = class_weights
+        self.batch_size = batch_size
+
+        self.optimizer = optimizer
+        if optimizer_params is None:
+            # Best set to 0.0001 to start (1e-3 is not ok)
+            self.optimizer_params = {"learning_rate": 0.0001}
+        else:
+            self.optimizer_params = optimizer_params
+
+        if self.class_weights is not None:
+            self.loss_function = "weighted_categorical_crossentropy"
+        else:
+            self.loss_function = "categorical_crossentropy"
+
+        # Properties to choose the best model
+        if monitor_metric is not None:
+            self.monitor_metric = monitor_metric
+        elif self.loss_function in (
+            "weighted_categorical_crossentropy",
+            "categorical_crossentropy",
+        ):
+            self.monitor_metric = "categorical_accuracy"
+        self.monitor_metric_mode = monitor_metric_mode
+
+        self.save_format = save_format
+        self.save_best_only = save_best_only
+        self.save_min_accuracy = save_min_accuracy
+        self.nb_epoch = nb_epoch
+        self.nb_epoch_with_freeze = nb_epoch_with_freeze
+
+        # Properties to stop the training
+        self.earlystop_patience = earlystop_patience
+        if earlystop_monitor_metric is not None:
+            self.earlystop_monitor_metric = earlystop_monitor_metric
+        else:
+            self.earlystop_monitor_metric = self.monitor_metric
+        self.earlystop_monitor_metric_mode = earlystop_monitor_metric_mode
+
+        # Properties regarding logging
+        self.log_tensorboard = log_tensorboard
+        self.log_csv = log_csv
+
+    def toJSON(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+
+class HyperParams:
+    def __init__(
+        self,
+        architecture: Optional[ArchitectureParams] = None,
+        train: Optional[TrainParams] = None,
+        path: Optional[Path] = None,
+    ):
+        """
+        Class to store the hyper parameters to use for the machine learning algorythm.
+
+        Args:
+            architecture (ArchitectureParams): the fixed parameters that define the
+                architecture of the neural network. When training a network, it is
+                possible to reuse the weights of another network if these parameters
+                are the same.
+            train (TrainParams): these are the parameters that can be changed with each
+                training.
+        """
+        self.fileversion = 1.1
+        if architecture is not None:
+            self.architecture = architecture
+        if train is not None:
+            self.train = train
+        if path is not None:
+            with open(path, "r") as jsonfile:
+                jsonstr = jsonfile.read()
+                data = json.loads(jsonstr)
+
+                # Read file version if it is present
+                if "fileversion" in data:
+                    self.fileversion = data["fileversion"]
+
+                # Now parse the real data. For backwards compatibility, remove
+                # 'nb_classes' parameter if it exists
+                if "nb_classes" in data["architecture"]:
+                    del data["architecture"]["nb_classes"]
+
+                self.architecture = ArchitectureParams(**data["architecture"])
+                self.train = TrainParams(**data["train"])
+
+    def toJSON(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+
+def format_model_basefilename(
+    segment_subject: str,
+    traindata_id: int,
+    architecture_id: int = 0,
+    trainparams_id: int = 0,
+) -> str:
+    """
+    Format the parameters into a model_filename.
+
+    Args
+        segment_subject: the segment subject
+        traindata_id: the id of the data used to train the model
+        architecture_id: the id of the model architecture used
+        trainparams_id: the id of the hyper parameters used to train the model
+    """
+    # Format file name
+    filename = f"{segment_subject}_{traindata_id:02d}"
+
+    # If an architecture id and/or hyperparams id is specified, add those as well
+    if architecture_id > 0 or trainparams_id > 0:
+        filename = f"{filename}.{architecture_id}.{trainparams_id}"
+    return filename
+
+
+def format_model_filename(
+    segment_subject: str,
+    traindata_id: int,
+    architecture_id: int,
+    trainparams_id: int,
+    monitor_metric_accuracy: float,
+    epoch: int,
+    save_format: str,
+) -> str:
+    """
+    Format the parameters into a model_filename.
+
+    Args
+        segment_subject: the segment subject
+        traindata_id: the version of the data used to train the model
+        architecture_id: the id of the model architecture used
+        trainparams_id: the version of the hyper parameters used to train
+        monitor_metric_accuracy: the monitor metric accuracy
+        epoch: the epoch during training that reached these model weights
+        save_format (str): the format to save in:
+            * keras format: 'h5'
+            * tensorflow savedmodel: 'tf'
+    """
+    # Format file name
+    filename = format_model_basefilename(
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        architecture_id=architecture_id,
+        trainparams_id=trainparams_id,
+    )
+    filename += f"_{monitor_metric_accuracy:.5f}_{epoch}"
+
+    # Add suffix
+    if save_format == "tf":
+        filename += "_tf"
+    else:
+        filename += ".hdf5"
+
+    return filename
+
+
+def parse_model_filename(filepath: Path) -> Optional[dict]:
+    """
+    Parse a model_filename to a dict containing the properties of the model:
+        * segment_subject: the segment subject
+        * traindata_id: the version of the data used to train the model
+        * monitor_metric_accuracy: the monitored metric accuracy
+        * trainparams_id: the version of the hyper parameters used to train
+        * epoch: the epoch during training that reached these model weights
+        * save_format (str): the format to save in:
+            * keras format: 'h5'
+            * tensorflow savedmodel: 'tf'
+
+    Args
+        filepath: the filepath to the model file
+    """
+
+    # Prepare filepath to extract info
+    if filepath.is_dir():
+        # If it is a dir, it should end on _tf
+        if not filepath.name.endswith("_tf"):
+            logger.warning(
+                f"Not a valid path for a model, dir needs to end on _tf: {filepath}"
+            )
+            return None
+        save_format = "tf"
+        filename = filepath.name
+    else:
+        filename = filepath.stem
+        if filepath.suffix in (".h5", ".hdf5"):
+            save_format = "h5"
+        else:
+            logger.warning(f"Model file should have .h5 of .hdf5 as suffix: {filepath}")
+            return None
+
+    # Now extract the fields...
+    param_values = filename.split("_")
+    if len(param_values) < 3:
+        logger.warning(
+            f"Model file name nok, split('_') must result in >= 2 fields: {filepath}"
+        )
+
+    segment_subject = param_values[0]
+
+    model_info = param_values[1]
+    model_info_values = model_info.split(".")
+    traindata_id = int(model_info_values[0])
+    architecture_id = 0
+    trainparams_id = 0
+    if len(model_info_values) > 1:
+        architecture_id = int(model_info_values[1])
+        if len(model_info_values) > 2:
+            trainparams_id = int(model_info_values[2])
+
+    monitor_metric_accuracy = float(param_values[2])
+    epoch = int(param_values[3])
+
+    basefilename = format_model_basefilename(
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        architecture_id=architecture_id,
+        trainparams_id=trainparams_id,
+    )
+
+    return {
+        "filepath": filepath,
+        "filename": filename,
+        "basefilename": basefilename,
+        "segment_subject": segment_subject,
+        "traindata_id": traindata_id,
+        "architecture_id": architecture_id,
+        "trainparams_id": trainparams_id,
+        "monitor_metric_accuracy": monitor_metric_accuracy,
+        "epoch": epoch,
+        "save_format": save_format,
+    }
+
+
+def get_models(
+    model_dir: Path,
+    segment_subject: Optional[str] = None,
+    traindata_id: Optional[int] = None,
+    architecture_id: Optional[int] = None,
+    trainparams_id: Optional[int] = None,
+) -> List[dict]:
+    """
+    Return the list of models in the model_dir passed. It is returned as a
+    dataframe with the columns as returned in parse_model_filename()
+
+    Args
+        model_dir (Path): dir containing the models
+        segment_subject (str, optional): only models with this the segment subject
+        traindata_id (int, optional): only models with this traindata version
+        architecture_id (int, optional): only models with this this architecture_id
+        trainparams_id (int, optional): only models with this hyperparams version
+    """
+
+    # List models
+    model_paths = []
+    model_paths.extend(model_dir.glob("*.hdf5"))
+    model_paths.extend(model_dir.glob("*.h5"))
+    model_paths.extend(model_dir.glob("*_tf"))
+
+    # Loop through all models and extract necessary info...
+    model_info_list = []
+    for model_path in model_paths:
+        model_info = parse_model_filename(model_path)
+        if model_info is not None:
+            model_info_list.append(model_info)
+
+    # Filter, if filters provided
+    if len(model_info_list) > 0:
+        if segment_subject is not None:
+            model_info_list = [
+                model_info
+                for model_info in model_info_list
+                if model_info["segment_subject"] == segment_subject
+            ]
+        if traindata_id is not None:
+            model_info_list = [
+                model_info
+                for model_info in model_info_list
+                if model_info["traindata_id"] == traindata_id
+            ]
+        if trainparams_id is not None:
+            model_info_list = [
+                model_info
+                for model_info in model_info_list
+                if model_info["trainparams_id"] == trainparams_id
+            ]
+        if architecture_id is not None:
+            model_info_list = [
+                model_info
+                for model_info in model_info_list
+                if model_info["architecture_id"] == architecture_id
+            ]
+
+    return model_info_list
+
+
+def get_best_model(
+    model_dir: Path,
+    segment_subject: Optional[str] = None,
+    traindata_id: Optional[int] = None,
+    architecture_id: Optional[int] = None,
+    trainparams_id: Optional[int] = None,
+) -> Optional[dict]:
+    """
+    Get the properties of the model with the highest combined accuracy for the highest
+    traindata version in the dir.
+
+    Remark: regardless of the monitor function used when training, the accuracies
+    are always better if higher!
+
+    Args
+        model_dir: dir containing the models
+        segment_subject (str, optional): only models with this the segment subject
+        traindata_id (int, optional): only models with this train data id
+        architecture_id (int, optional): only models with this the architecture_id
+        trainparams_id (int, optional): only models with this hyperparams id
+
+    Returns
+        A dictionary with the info of the best model, or None if no model was found
+    """
+    # Get list of existing models for this train dataset
+    model_info_list = get_models(
+        model_dir=model_dir,
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        architecture_id=architecture_id,
+        trainparams_id=trainparams_id,
+    )
+
+    # If nothing found, return None
+    if len(model_info_list) == 0:
+        return None
+
+    # If no traindata_id provided, find highest traindata id
+    max_traindata_id = -1
+    for model_info in model_info_list:
+        if model_info["traindata_id"] > max_traindata_id:
+            max_traindata_id = model_info["traindata_id"]
+
+    # Get the list of newest model
+    newest_model_info_list = [
+        model_info
+        for model_info in model_info_list
+        if model_info["traindata_id"] == max_traindata_id
+    ]
+
+    # If only one result, return it
+    if len(newest_model_info_list) == 1:
+        return newest_model_info_list[0]
+    else:
+        max_monitor_metric_accuracy = -1
+        max_monitor_metric_accuracy_idx = -1
+        for model_info_idx, model_info in enumerate(model_info_list):
+            if model_info["monitor_metric_accuracy"] > max_monitor_metric_accuracy:
+                max_monitor_metric_accuracy = model_info["monitor_metric_accuracy"]
+                max_monitor_metric_accuracy_idx = model_info_idx
+
+        return model_info_list[max_monitor_metric_accuracy_idx]
+
+
+class ModelCheckpointExt(callbacks.Callback):
+    def __init__(
+        self,
+        model_save_dir: Path,
+        segment_subject: str,
+        traindata_id: int,
+        architecture_id: int,
+        trainparams_id: int,
+        monitor_metric: str,
+        monitor_metric_mode: str,
+        save_format: str = "h5",
+        save_best_only: bool = False,
+        save_min_accuracy: float = 0.90,
+        save_min_accuracy_ignored_epoch: int = 100,
+        save_weights_only: bool = False,
+        model_template_for_save=None,
+        verbose: bool = True,
+        only_report: bool = False,
+    ):
+        """
+        Constructor
+
+        Args:
+            model_save_dir (Path): [description]
+            segment_subject (str): segment subject
+            traindata_id (int): train data id
+            architecture_id (int): model architecture id
+            trainparams_id (int): id of the hyper parameters used
+            monitor_metric (str): The metric to monitor for accuracy
+            monitor_metric_mode (str): use 'min' if the accuracy metrics
+                should be  as low as possible, 'max' if a higher values is
+                better.
+            save_format (str, optional): The format to save in:
+                'h5' (keras format) or 'tf' (tensorflow savedmodel).
+                Defaults to 'tf'
+            save_best_only (bool, optional): only keep the best model.
+                Defaults to True.
+            save_min_accuracy (float, optional): minimum accuracy to be
+                reached to save model. Defaults to 0.9.
+            save_min_accuracy_ignored_epoch (int, optional): at this epoch the
+                save_min_accuracy is ignored, to make sure there is a model
+                saved, even if the minimum accuracy is never reached.
+            save_weights_only: optional: only save weights
+            model_template_for_save: optional, if using multi-GPU training,
+                pass the original model here to use this as template for saving
+            verbose (bool, optional): [description]. Defaults to True.
+            only_report (bool, optional): [description]. Defaults to False.
+        """
+        monitor_metric_mode_values = ["min", "max"]
+        if monitor_metric_mode not in monitor_metric_mode_values:
+            raise Exception(
+                f"Invalid value for mode: {monitor_metric_mode}, should be one of "
+                f"{monitor_metric_mode_values}"
+            )
+        save_format_values = ("h5", "tf")
+        if save_format not in save_format_values:
+            raise Exception(
+                f"Invalid value for save_format: {save_format}, should be one of "
+                f"{save_format_values}"
+            )
+
+        self.model_save_dir = model_save_dir
+        self.segment_subject = segment_subject
+        self.traindata_id = traindata_id
+        self.architecture_id = architecture_id
+        self.trainparams_id = trainparams_id
+        self.monitor_metric = monitor_metric
+        self.monitor_metric_mode = monitor_metric_mode
+        self.save_format = save_format
+        self.save_best_only = save_best_only
+        self.save_min_accuracy = save_min_accuracy
+        self.save_min_accuracy_ignored_epoch = save_min_accuracy_ignored_epoch
+        self.save_weights_only = save_weights_only
+        self.model_template_for_save = model_template_for_save
+        self.verbose = verbose
+        self.only_report = only_report
+
+    def on_epoch_end(self, epoch, logs={}):
+        logger.debug(f"Start in callback on_epoch_begin, logs contains: {logs}")
+
+        # First determine the values of the monitor metric for train and validation
+        # If the monitor_metric doesn't contain placeholder, it is easy
+        if "{" not in self.monitor_metric:
+            new_model_monitor_value = logs.get(self.monitor_metric)
+        else:
+            # There are placeholders, so we need some more logic
+            monitor_metric_formatted = self.monitor_metric.format(**logs)
+            new_model_monitor_value = eval(monitor_metric_formatted, {}, {})
+
+        # Now we can save and clean models
+        save_and_clean_models(
+            model_save_dir=self.model_save_dir,
+            segment_subject=self.segment_subject,
+            traindata_id=self.traindata_id,
+            architecture_id=self.architecture_id,
+            trainparams_id=self.trainparams_id,
+            monitor_metric_mode=self.monitor_metric_mode,
+            new_model=self.model,
+            new_model_monitor_value=new_model_monitor_value,
+            new_model_epoch=epoch,
+            save_format=self.save_format,
+            save_best_only=self.save_best_only,
+            save_min_accuracy=self.save_min_accuracy,
+            save_min_accuracy_ignored_epoch=self.save_min_accuracy_ignored_epoch,
+            save_weights_only=self.save_weights_only,
+            model_template_for_save=self.model_template_for_save,
+            verbose=self.verbose,
+            only_report=self.only_report,
+        )
+
+
+def save_and_clean_models(
+    model_save_dir: Path,
+    segment_subject: str,
+    traindata_id: int,
+    architecture_id: int,
+    trainparams_id: int,
+    monitor_metric_mode: str,
+    new_model=None,
+    new_model_monitor_value: Optional[float] = None,
+    new_model_epoch: Optional[int] = None,
+    save_format: str = "h5",
+    save_best_only: bool = False,
+    save_min_accuracy: float = 0.9,
+    save_min_accuracy_ignored_epoch: int = 100,
+    save_weights_only: bool = False,
+    model_template_for_save=None,
+    verbose: bool = True,
+    debug: bool = False,
+    only_report: bool = False,
+):
+    """
+    Save the new model if it is good enough... and cleanup existing models
+    if they are worse than the new or other existing models.
+
+    Args
+        model_save_dir (Path): dir containing the models
+        segment_subject (str): segment subject
+        traindata_id (int): train data id
+        architecture_id (int): model architecture id
+        trainparams_id (int): id of the train params
+        model_monitor_metric_mode (MetricMode): use 'min' if the monitored
+            metrics should be as low as possible, 'max' if a higher values
+            is better.
+        new_model (optional): the keras model object that will be saved
+        new_model_monitor_value (float, optional): the monitored metric value
+        new_model_epoch (int, optional): the epoch in the training
+        save_format (SaveFormat, optional): The format to save in:
+            * h5: keras format (= default)
+            * tf: tensorflow savedmodel
+        save_best_only (bool, optional): only keep the best model
+        save_min_accuracy (float, optional): minimum accuracy to save the
+            model. Defaults to 0.9.
+        save_min_accuracy_ignored_epoch (int, optional): at this epoch the
+            save_min_accuracy is ignored, to make sure there is a model saved,
+            even if the minimum accuracy is never reached.
+        save_weights_only (bool, optional): only save weights
+        model_template_for_save (optional): if using multi-GPU training, pass
+            the original model here to use this as template for saving
+        verbose (bool, optional): report the best model after save and cleanup
+        debug (bool, optional): write debug logging
+        only_report (bool, optional): only report which models would be cleaned up
+    """
+    # TODO: add option to specify minimum accuracy/iou score before saving to speed up,
+    # because saving takes quite some time!
+    # Check validaty of input
+    monitor_metric_mode_values = ["min", "max"]
+    if monitor_metric_mode not in monitor_metric_mode_values:
+        raise Exception(
+            f"Invalid value for mode: {monitor_metric_mode}, should be one of "
+            f"{monitor_metric_mode_values}"
+        )
+    save_format_values = ("h5", "tf")
+    if save_format not in save_format_values:
+        raise Exception(
+            f"Invalid value for save_format: {save_format}, should be one of "
+            f"{save_format_values}"
+        )
+
+    # Get a list of all existing models
+    model_info_list = get_models(
+        model_dir=model_save_dir,
+        segment_subject=segment_subject,
+        traindata_id=traindata_id,
+        trainparams_id=trainparams_id,
+    )
+
+    # If there is a new model passed as param, add it to the list
+    new_model_path = None
+    new_model_monitor_accuracy = None
+    if new_model is not None:
+
+        if new_model_monitor_value is None or new_model_epoch is None:
+            raise Exception(
+                "If new_model is not None, new_model_monitor_... parameters cannot be "
+                f"None either???, new_model_monitor_value: {new_model_monitor_value}, "
+                f"new_model_epoch: {new_model_epoch}"
+            )
+
+        # Build save filepath
+        # Remark: accuracy values should always be as high as possible, so
+        # recalculate values if monitor_metric_mode is 'min'
+        if monitor_metric_mode == "max":
+            new_model_monitor_accuracy = new_model_monitor_value
+        else:
+            new_model_monitor_accuracy = 1 - new_model_monitor_value
+
+        new_model_filename = format_model_filename(
+            segment_subject=segment_subject,
+            traindata_id=traindata_id,
+            architecture_id=architecture_id,
+            trainparams_id=trainparams_id,
+            monitor_metric_accuracy=new_model_monitor_accuracy,
+            epoch=new_model_epoch,
+            save_format=save_format,
+        )
+        new_model_path = Path(model_save_dir) / new_model_filename
+
+        # Append model to the retrieved models...
+        model_info_list.append(
+            {
+                "filepath": str(new_model_path),
+                "filename": new_model_filename,
+                "segment_subject": segment_subject,
+                "traindata_id": traindata_id,
+                "architecture_id": architecture_id,
+                "trainparams_id": trainparams_id,
+                "monitor_metric_accuracy": new_model_monitor_accuracy,
+                "epoch": new_model_epoch,
+                "save_format": save_format,
+            }
+        )
+
+    # Loop through all existing models
+    # Remark: the list is sorted descending before iterating it, this way new
+    # modelss are saved bevore deleting the previous best one(s)
+    model_info_df = pd.DataFrame(model_info_list)
+    model_info_sorted_df = model_info_df.sort_values(
+        by="monitor_metric_accuracy", ascending=False
+    )
+    for model_info in model_info_sorted_df.itertuples(index=False):
+
+        # If only the best needs to be kept, check only on monitor_metric_accuracy...
+        keep_model = True
+        better_ones_df = None
+        if save_best_only:
+            better_ones_df = model_info_df[
+                (model_info_df.filepath != model_info.filepath)
+                & (
+                    model_info_df.monitor_metric_accuracy
+                    >= model_info.monitor_metric_accuracy
+                )
+            ]
+            if len(better_ones_df) > 0:
+                keep_model = False
+
+        # If model is (relatively) ok, keep it
+        if keep_model is True:
+            logger.debug(f"KEEP {model_info.filename}")
+
+            # If it is the new model that needs to be kept, keep it or save to disk
+            if (
+                new_model_path is not None
+                and new_model is not None
+                and new_model_epoch is not None
+                and only_report is not True
+                and model_info.filepath == str(new_model_path)
+                and not new_model_path.exists()
+            ):
+                if (
+                    new_model_epoch > save_min_accuracy_ignored_epoch
+                    or model_info.monitor_metric_accuracy > save_min_accuracy
+                ):
+                    logger.debug("Save model start")
+                    if save_weights_only:
+                        if model_template_for_save is not None:
+                            model_template_for_save.save_weights(str(new_model_path))
+                        else:
+                            new_model.save_weights(str(new_model_path))
+                    else:
+                        if model_template_for_save is not None:
+                            model_template_for_save.save(str(new_model_path))
+                        else:
+                            new_model.save(str(new_model_path))
+                    logger.debug("Save model ready")
+                else:
+                    print(
+                        "New model is best, but accuracy < save_min_accuracy: "
+                        f"{new_model_monitor_accuracy} < {save_min_accuracy}"
+                    )
+        else:
+            # Bad model... can be removed (or not saved)
+            if only_report is True:
+                logger.debug(f"DELETE {model_info.filename}")
+            elif Path(model_info.filepath).exists() is True:
+                logger.debug(f"DELETE {model_info.filename}")
+                if Path(model_info.filepath).is_dir() is True:
+                    shutil.rmtree(model_info.filepath)
+                else:
+                    Path(model_info.filepath).unlink()
+
+            if debug is True and better_ones_df is not None:
+                print(f"Better one(s) found for{model_info.filename}:")
+                for better_one in better_ones_df.itertuples(index=False):
+                    print(f"  {better_one.filename}")
+
+    if verbose is True or debug is True:
+        best_model = get_best_model(
+            model_dir=model_save_dir,
+            segment_subject=segment_subject,
+            traindata_id=traindata_id,
+            architecture_id=architecture_id,
+            trainparams_id=trainparams_id,
+        )
+        if best_model is not None:
+            logger.info(
+                f"Current best model for {segment_subject}_{traindata_id}: "
+                f"monitor_metric_accuracy: {best_model['monitor_metric_accuracy']}, "
+                f"epoch: {best_model['epoch']}"
+            )
```

### Comparing `orthoseg-0.4.2/orthoseg/postprocess.py` & `orthoseg-0.4.2a1/orthoseg/postprocess.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# -*- coding: utf-8 -*-
-"""
-Module with functions for post-processing prediction masks towards polygons.
-"""
-
-import argparse
-import logging
-from pathlib import Path
-import shlex
-import sys
-import traceback
-
-import geofileops as gfo
-
-# Because orthoseg isn't installed as package + it is higher in dir hierarchy, add root
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import config_helper as conf
-from orthoseg.helpers import email_helper
-from orthoseg.lib import postprocess_predictions as postp
-import orthoseg.model.model_helper as mh
-from orthoseg.util import log_util
-
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def postprocess_argstr(argstr):
-    args = shlex.split(argstr)
-    postprocess_args(args)
-
-
-def postprocess_args(args):
-
-    # Interprete arguments
-    parser = argparse.ArgumentParser(add_help=False)
-
-    # Required arguments
-    required = parser.add_argument_group("Required arguments")
-    required.add_argument(
-        "-c", "--config", type=str, required=True, help="The config file to use"
-    )
-
-    # Optional arguments
-    optional = parser.add_argument_group("Optional arguments")
-    # Add back help
-    optional.add_argument(
-        "-h",
-        "--help",
-        action="help",
-        default=argparse.SUPPRESS,
-        help="Show this help message and exit",
-    )
-
-    # Interprete arguments
-    args = parser.parse_args(args)
-
-    # Run!
-    postprocess(config_path=Path(args.config))
-
-
-def postprocess(config_path: Path):
-    """
-    Postprocess the output of a prediction for the config specified.
-
-    Args:
-        config_path (Path): Path to the config file.
-    """
-
-    # Init
-    # Load the config and save in a bunch of global variables zo it
-    # is accessible everywhere
-    conf.read_orthoseg_config(config_path)
-
-    # Init logging
-    log_util.clean_log_dir(
-        log_dir=conf.dirs.getpath("log_dir"),
-        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
-    )
-    global logger
-    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
-
-    # Log start + send email
-    message = f"Start postprocess for config {config_path.stem}"
-    logger.info(message)
-    logger.debug(f"Config used: \n{conf.pformat_config()}")
-    email_helper.sendmail(message)
-
-    try:
-
-        # Create base filename of model to use
-        # TODO: is force data version the most logical, or rather implement
-        #       force weights file or ?
-        traindata_id = None
-        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
-        if force_model_traindata_id is not None and force_model_traindata_id > -1:
-            traindata_id = force_model_traindata_id
-
-        # Get the best model that already exists for this train dataset
-        trainparams_id = conf.train.getint("trainparams_id")
-        best_model = mh.get_best_model(
-            model_dir=conf.dirs.getpath("model_dir"),
-            segment_subject=conf.general["segment_subject"],
-            traindata_id=traindata_id,
-            trainparams_id=trainparams_id,
-        )
-        if best_model is None:
-            raise Exception(f"No best model found in {conf.dirs.getpath('model_dir')}")
-
-        # Input file  the "most recent" prediction result dir for this subject
-        output_vector_dir = conf.dirs.getpath("output_vector_dir")
-        output_vector_name = (
-            f"{best_model['basefilename']}_{best_model['epoch']}_"
-            f"{conf.predict['image_layer']}"
-        )
-        output_vector_path = output_vector_dir / f"{output_vector_name}.gpkg"
-
-        # Prepare some parameters for the postprocessing
-        nb_parallel = conf.general.getint("nb_parallel")
-
-        dissolve = conf.postprocess.getboolean("dissolve")
-        dissolve_tiles_path = conf.postprocess.getpath("dissolve_tiles_path")
-        reclassify_query = conf.postprocess.get("reclassify_to_neighbour_query")
-        if reclassify_query is not None:
-            reclassify_query = reclassify_query.replace("\n", " ")
-
-        simplify_algorithm = conf.postprocess.get("simplify_algorithm")
-        if simplify_algorithm is not None:
-            simplify_algorithm = gfo.SimplifyAlgorithm[simplify_algorithm]
-        simplify_tolerance = conf.postprocess.geteval("simplify_tolerance")
-        simplify_lookahead = conf.postprocess.get("simplify_lookahead")
-        if simplify_lookahead is not None:
-            simplify_lookahead = int(simplify_lookahead)
-
-        # Go!
-        postp.postprocess_predictions(
-            input_path=output_vector_path,
-            output_path=output_vector_path,
-            dissolve=dissolve,
-            dissolve_tiles_path=dissolve_tiles_path,
-            reclassify_to_neighbour_query=reclassify_query,
-            simplify_algorithm=simplify_algorithm,
-            simplify_tolerance=simplify_tolerance,
-            simplify_lookahead=simplify_lookahead,
-            nb_parallel=nb_parallel,
-            force=False,
-        )
-
-        # Log and send mail
-        message = f"Completed postprocess for config {config_path.stem}"
-        logger.info(message)
-        email_helper.sendmail(message)
-    except Exception as ex:
-        message = f"ERROR while running postprocess for task {config_path.stem}"
-        logger.exception(message)
-        email_helper.sendmail(
-            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
-        )
-        raise Exception(message) from ex
-
-
-def main():
-    try:
-        postprocess_args(sys.argv[1:])
-    except Exception as ex:
-        logger.exception(f"Error: {ex}")
-        raise
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""
+Module with functions for post-processing prediction masks towards polygons.
+"""
+
+import argparse
+import logging
+from pathlib import Path
+import shlex
+import sys
+import traceback
+
+import geofileops as gfo
+
+# Because orthoseg isn't installed as package + it is higher in dir hierarchy, add root
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import config_helper as conf
+from orthoseg.helpers import email_helper
+from orthoseg.lib import postprocess_predictions as postp
+import orthoseg.model.model_helper as mh
+from orthoseg.util import log_util
+
+# -------------------------------------------------------------
+# First define/init general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def postprocess_argstr(argstr):
+    args = shlex.split(argstr)
+    postprocess_args(args)
+
+
+def postprocess_args(args):
+
+    # Interprete arguments
+    parser = argparse.ArgumentParser(add_help=False)
+
+    # Required arguments
+    required = parser.add_argument_group("Required arguments")
+    required.add_argument(
+        "-c", "--config", type=str, required=True, help="The config file to use"
+    )
+
+    # Optional arguments
+    optional = parser.add_argument_group("Optional arguments")
+    # Add back help
+    optional.add_argument(
+        "-h",
+        "--help",
+        action="help",
+        default=argparse.SUPPRESS,
+        help="Show this help message and exit",
+    )
+
+    # Interprete arguments
+    args = parser.parse_args(args)
+
+    # Run!
+    postprocess(config_path=Path(args.config))
+
+
+def postprocess(config_path: Path):
+    """
+    Postprocess the output of a prediction for the config specified.
+
+    Args:
+        config_path (Path): Path to the config file.
+    """
+
+    # Init
+    # Load the config and save in a bunch of global variables zo it
+    # is accessible everywhere
+    conf.read_orthoseg_config(config_path)
+
+    # Init logging
+    log_util.clean_log_dir(
+        log_dir=conf.dirs.getpath("log_dir"),
+        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
+    )
+    global logger
+    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
+
+    # Log start + send email
+    message = f"Start postprocess for config {config_path.stem}"
+    logger.info(message)
+    logger.debug(f"Config used: \n{conf.pformat_config()}")
+    email_helper.sendmail(message)
+
+    try:
+
+        # Create base filename of model to use
+        # TODO: is force data version the most logical, or rather implement
+        #       force weights file or ?
+        traindata_id = None
+        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
+        if force_model_traindata_id is not None and force_model_traindata_id > -1:
+            traindata_id = force_model_traindata_id
+
+        # Get the best model that already exists for this train dataset
+        trainparams_id = conf.train.getint("trainparams_id")
+        best_model = mh.get_best_model(
+            model_dir=conf.dirs.getpath("model_dir"),
+            segment_subject=conf.general["segment_subject"],
+            traindata_id=traindata_id,
+            trainparams_id=trainparams_id,
+        )
+        if best_model is None:
+            raise Exception(f"No best model found in {conf.dirs.getpath('model_dir')}")
+
+        # Input file  the "most recent" prediction result dir for this subject
+        output_vector_dir = conf.dirs.getpath("output_vector_dir")
+        output_vector_name = (
+            f"{best_model['basefilename']}_{best_model['epoch']}_"
+            f"{conf.predict['image_layer']}"
+        )
+        output_vector_path = output_vector_dir / f"{output_vector_name}.gpkg"
+
+        # Prepare some parameters for the postprocessing
+        nb_parallel = conf.general.getint("nb_parallel")
+
+        dissolve = conf.postprocess.getboolean("dissolve")
+        dissolve_tiles_path = conf.postprocess.getpath("dissolve_tiles_path")
+        reclassify_query = conf.postprocess.get("reclassify_to_neighbour_query")
+        if reclassify_query is not None:
+            reclassify_query = reclassify_query.replace("\n", " ")
+
+        simplify_algorithm = conf.postprocess.get("simplify_algorithm")
+        if simplify_algorithm is not None:
+            simplify_algorithm = gfo.SimplifyAlgorithm[simplify_algorithm]
+        simplify_tolerance = conf.postprocess.geteval("simplify_tolerance")
+        simplify_lookahead = conf.postprocess.get("simplify_lookahead")
+        if simplify_lookahead is not None:
+            simplify_lookahead = int(simplify_lookahead)
+
+        # Go!
+        postp.postprocess_predictions(
+            input_path=output_vector_path,
+            output_path=output_vector_path,
+            dissolve=dissolve,
+            dissolve_tiles_path=dissolve_tiles_path,
+            reclassify_to_neighbour_query=reclassify_query,
+            simplify_algorithm=simplify_algorithm,
+            simplify_tolerance=simplify_tolerance,
+            simplify_lookahead=simplify_lookahead,
+            nb_parallel=nb_parallel,
+            force=False,
+        )
+
+        # Log and send mail
+        message = f"Completed postprocess for config {config_path.stem}"
+        logger.info(message)
+        email_helper.sendmail(message)
+    except Exception as ex:
+        message = f"ERROR while running postprocess for task {config_path.stem}"
+        logger.exception(message)
+        email_helper.sendmail(
+            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
+        )
+        raise Exception(message) from ex
+
+
+def main():
+    try:
+        postprocess_args(sys.argv[1:])
+    except Exception as ex:
+        logger.exception(f"Error: {ex}")
+        raise
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    main()
```

### Comparing `orthoseg-0.4.2/orthoseg/predict.py` & `orthoseg-0.4.2a1/orthoseg/predict.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,319 +1,319 @@
-# -*- coding: utf-8 -*-
-"""
-High-level API to run a segmentation.
-"""
-
-import argparse
-import logging
-import os
-from pathlib import Path
-import pprint
-import shlex
-import sys
-import traceback
-
-import geofileops as gfo
-
-# import os
-# os.environ["CUDA_VISIBLE_DEVICES"] = "-1" # Disable using GPU
-import tensorflow as tf
-
-# orthoseg is higher in dir hierarchy, add root to sys.path
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import config_helper as conf
-from orthoseg.helpers import email_helper
-from orthoseg.lib import predicter
-import orthoseg.model.model_factory as mf
-import orthoseg.model.model_helper as mh
-from orthoseg.util import log_util
-
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def predict_argstr(argstr):
-    args = shlex.split(argstr)
-    predict_args(args)
-
-
-def predict_args(args):
-
-    # Interprete arguments
-    parser = argparse.ArgumentParser(add_help=False)
-
-    # Required arguments
-    required = parser.add_argument_group("Required arguments")
-    required.add_argument(
-        "-c", "--config", type=str, required=True, help="The config file to use"
-    )
-
-    # Optional arguments
-    optional = parser.add_argument_group("Optional arguments")
-    # Add back help
-    optional.add_argument(
-        "-h",
-        "--help",
-        action="help",
-        default=argparse.SUPPRESS,
-        help="Show this help message and exit",
-    )
-
-    # Interprete arguments
-    args = parser.parse_args(args)
-
-    # Run!
-    predict(config_path=Path(args.config))
-
-
-def predict(config_path: Path):
-    """
-    Run a prediction for the config specified.
-
-    Args:
-        config_path (Path): Path to the config file to use.
-    """
-    # Init
-    # Load the config and save in a bunch of global variables zo it
-    # is accessible everywhere
-    conf.read_orthoseg_config(config_path)
-
-    # Init logging
-    log_util.clean_log_dir(
-        log_dir=conf.dirs.getpath("log_dir"),
-        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
-    )
-    global logger
-    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
-
-    # Log start + send email
-    message = f"Start predict for config {config_path.stem}"
-    logger.info(message)
-    logger.debug(f"Config used: \n{conf.pformat_config()}")
-    email_helper.sendmail(message)
-
-    try:
-        # Read some config, and check if values are ok
-        image_layer = conf.image_layers[conf.predict["image_layer"]]
-        if image_layer is None:
-            raise Exception(
-                f"image_layer to predict is not specified in config: {image_layer}"
-            )
-        input_image_dir = conf.dirs.getpath("predict_image_input_dir")
-        if not input_image_dir.exists():
-            raise Exception(f"input image dir doesn't exist: {input_image_dir}")
-
-        # TODO: add something to delete old data, predictions???
-
-        # Create base filename of model to use
-        # TODO: is force data version the most logical, or rather implement
-        #       force weights file or ?
-        traindata_id = None
-        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
-        if force_model_traindata_id is not None and force_model_traindata_id > -1:
-            traindata_id = force_model_traindata_id
-
-        # Get the best model that already exists for this train dataset
-        trainparams_id = conf.train.getint("trainparams_id")
-        best_model = mh.get_best_model(
-            model_dir=conf.dirs.getpath("model_dir"),
-            segment_subject=conf.general["segment_subject"],
-            traindata_id=traindata_id,
-            trainparams_id=trainparams_id,
-        )
-
-        # Check if a model was found
-        if best_model is None:
-            message = (
-                f"No model found in model_dir: {conf.dirs.getpath('model_dir')} for "
-                f"traindata_id: {traindata_id}"
-            )
-            logger.critical(message)
-            raise Exception(message)
-        else:
-            model_weights_filepath = best_model["filepath"]
-            logger.info(f"Best model found: {model_weights_filepath}")
-
-        # Load the hyperparams of the model
-        # TODO: move the hyperparams filename formatting to get_models...
-        hyperparams_path = (
-            best_model["filepath"].parent
-            / f"{best_model['basefilename']}_hyperparams.json"
-        )
-        hyperparams = mh.HyperParams(path=hyperparams_path)
-
-        # Prepare output subdir to be used for predictions
-        predict_out_subdir = f"{best_model['basefilename']}"
-        if trainparams_id > 0:
-            predict_out_subdir += f"_{trainparams_id}"
-        predict_out_subdir += f"_{best_model['epoch']}"
-
-        # Load model to predict with
-        # --------------------------
-        model = None
-        # Try optimizing model with tensorrt. Not supported on Windows
-        # -> disabled for now till I have access again to a linux machine
-        """
-        if os.name != "nt":
-            try:
-                # Try import
-                from tensorflow.python.compiler.tensorrt import trt_convert as trt
-
-                # Import didn't fail, so optimize model
-                logger.info(
-                    "Tensorrt is available, so try to create and use optimized model"
-                )
-                savedmodel_optim_dir = (
-                    best_model["filepath"].parent
-                    / f"{best_model['filepath'].stem}_optim"
-                )
-                if not savedmodel_optim_dir.exists():
-                    # If base model not yet in savedmodel format
-                    savedmodel_dir = (
-                        best_model["filepath"].parent / best_model["filepath"].stem
-                    )
-                    if not savedmodel_dir.exists():
-                        logger.info(
-                            f"SavedModel format not yet available, so load "
-                            f"model + weights from {best_model['filepath']}"
-                        )
-                        model = mf.load_model(best_model["filepath"], compile=False)
-                        logger.info(f"Now save again as savedmodel to {savedmodel_dir}")
-                        tf.saved_model.save(model, str(savedmodel_dir))
-                        model = None
-
-                    # Now optimize model
-                    logger.info(f"Optimize + save model to {savedmodel_optim_dir}")
-                    converter = trt.TrtGraphConverterV2(
-                        input_saved_model_dir=str(savedmodel_dir),
-                        is_dynamic_op=True,
-                        precision_mode="FP16",
-                    )
-                    converter.convert()
-                    converter.save(savedmodel_optim_dir)
-
-                logger.info(
-                    f"Load optimized model + weights from {savedmodel_optim_dir}"
-                )
-                model = tf.keras.models.load_model(str(savedmodel_optim_dir))
-
-            except ImportError:
-                logger.info("Tensorrt is not available, so load unoptimized model")
-            except Exception as ex:
-                logger.info(
-                    "An error occured trying to use tensorrt, "
-                    f"so load unoptimized model. Error: {ex}"
-                )
-        """
-
-        # If model isn't loaded yet... load!
-        if model is None:
-            model = mf.load_model(best_model["filepath"], compile=False)
-
-        # Prepare the model for predicting
-        nb_gpu = len(tf.config.experimental.list_physical_devices("GPU"))
-        batch_size = conf.predict.getint("batch_size")
-        if nb_gpu <= 1:
-            model_for_predict = model
-            logger.info(f"Predict using single GPU or CPU, with nb_gpu: {nb_gpu}")
-        else:
-            # If multiple GPU's available, create multi_gpu_model
-            try:
-                model_for_predict = model
-                logger.warn("Predict using multiple GPUs NOT IMPLEMENTED AT THE MOMENT")
-
-                # logger.info(
-                #     f"Predict using multiple GPUs: {nb_gpu}, batch size becomes: "
-                #     f"{batch_size*nb_gpu}"
-                # )
-                # batch_size *= nb_gpu
-            except ValueError:
-                logger.info("Predict using single GPU or CPU")
-                model_for_predict = model
-
-        # Prepare params for the inline postprocessing of the prediction
-        min_probability = conf.predict.getfloat("min_probability")
-        postprocess = {}
-        simplify_algorithm = conf.predict.get("simplify_algorithm")
-        if simplify_algorithm is not None:
-            postprocess["simplify"] = {}
-            simplify = postprocess["simplify"]
-
-            simplify_algorithm = gfo.SimplifyAlgorithm[simplify_algorithm]
-            simplify["simplify_algorithm"] = simplify_algorithm
-            simplify["simplify_tolerance"] = conf.predict.geteval("simplify_tolerance")
-            simplify["simplify_lookahead"] = conf.predict.getint("simplify_lookahead")
-            simplify["simplify_topological"] = conf.predict.getboolean_ext(
-                "simplify_topological"
-            )
-        postprocess["filter_background_modal_size"] = conf.predict.getint(
-            "filter_background_modal_size"
-        )
-        query = conf.predict.get("reclassify_to_neighbour_query")
-        if query is not None:
-            query = query.replace("\n", " ")
-        postprocess["reclassify_to_neighbour_query"] = query
-        logger.info(f"Inline postprocessing:\n{pprint.pformat(postprocess)}")
-
-        # Prepare the output dirs/paths
-        predict_output_dir = Path(
-            f"{str(conf.dirs.getpath('predict_image_output_basedir'))}_"
-            f"{predict_out_subdir}"
-        )
-        output_vector_dir = conf.dirs.getpath("output_vector_dir")
-        output_vector_name = (
-            f"{best_model['basefilename']}_{best_model['epoch']}_"
-            f"{conf.predict['image_layer']}"
-        )
-        output_vector_path = output_vector_dir / f"{output_vector_name}.gpkg"
-
-        # Predict for entire dataset
-        nb_parallel = conf.general.getint("nb_parallel")
-        predicter.predict_dir(
-            model=model_for_predict,  # type: ignore
-            input_image_dir=input_image_dir,
-            output_image_dir=predict_output_dir,
-            output_vector_path=output_vector_path,
-            classes=hyperparams.architecture.classes,
-            min_probability=min_probability,
-            postprocess=postprocess,
-            border_pixels_to_ignore=conf.predict.getint("image_pixels_overlap"),
-            projection_if_missing=image_layer["projection"],
-            input_mask_dir=None,
-            batch_size=batch_size,
-            evaluate_mode=False,
-            cancel_filepath=conf.files.getpath("cancel_filepath"),
-            nb_parallel_postprocess=nb_parallel,
-            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-        )
-
-        # Log and send mail
-        message = f"Completed predict for config {config_path.stem}"
-        logger.info(message)
-        email_helper.sendmail(message)
-    except Exception as ex:
-        message = f"ERROR while running predict for task {config_path.stem}"
-        logger.exception(message)
-        email_helper.sendmail(
-            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
-        )
-        raise Exception(message) from ex
-
-
-def main():
-    try:
-        predict_args(sys.argv[1:])
-    except Exception as ex:
-        logger.exception(f"Error: {ex}")
-        raise
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""
+High-level API to run a segmentation.
+"""
+
+import argparse
+import logging
+import os
+from pathlib import Path
+import pprint
+import shlex
+import sys
+import traceback
+
+import geofileops as gfo
+
+# import os
+# os.environ["CUDA_VISIBLE_DEVICES"] = "-1" # Disable using GPU
+import tensorflow as tf
+
+# orthoseg is higher in dir hierarchy, add root to sys.path
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import config_helper as conf
+from orthoseg.helpers import email_helper
+from orthoseg.lib import predicter
+import orthoseg.model.model_factory as mf
+import orthoseg.model.model_helper as mh
+from orthoseg.util import log_util
+
+# -------------------------------------------------------------
+# First define/init general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def predict_argstr(argstr):
+    args = shlex.split(argstr)
+    predict_args(args)
+
+
+def predict_args(args):
+
+    # Interprete arguments
+    parser = argparse.ArgumentParser(add_help=False)
+
+    # Required arguments
+    required = parser.add_argument_group("Required arguments")
+    required.add_argument(
+        "-c", "--config", type=str, required=True, help="The config file to use"
+    )
+
+    # Optional arguments
+    optional = parser.add_argument_group("Optional arguments")
+    # Add back help
+    optional.add_argument(
+        "-h",
+        "--help",
+        action="help",
+        default=argparse.SUPPRESS,
+        help="Show this help message and exit",
+    )
+
+    # Interprete arguments
+    args = parser.parse_args(args)
+
+    # Run!
+    predict(config_path=Path(args.config))
+
+
+def predict(config_path: Path):
+    """
+    Run a prediction for the config specified.
+
+    Args:
+        config_path (Path): Path to the config file to use.
+    """
+    # Init
+    # Load the config and save in a bunch of global variables zo it
+    # is accessible everywhere
+    conf.read_orthoseg_config(config_path)
+
+    # Init logging
+    log_util.clean_log_dir(
+        log_dir=conf.dirs.getpath("log_dir"),
+        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
+    )
+    global logger
+    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
+
+    # Log start + send email
+    message = f"Start predict for config {config_path.stem}"
+    logger.info(message)
+    logger.debug(f"Config used: \n{conf.pformat_config()}")
+    email_helper.sendmail(message)
+
+    try:
+        # Read some config, and check if values are ok
+        image_layer = conf.image_layers[conf.predict["image_layer"]]
+        if image_layer is None:
+            raise Exception(
+                f"image_layer to predict is not specified in config: {image_layer}"
+            )
+        input_image_dir = conf.dirs.getpath("predict_image_input_dir")
+        if not input_image_dir.exists():
+            raise Exception(f"input image dir doesn't exist: {input_image_dir}")
+
+        # TODO: add something to delete old data, predictions???
+
+        # Create base filename of model to use
+        # TODO: is force data version the most logical, or rather implement
+        #       force weights file or ?
+        traindata_id = None
+        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
+        if force_model_traindata_id is not None and force_model_traindata_id > -1:
+            traindata_id = force_model_traindata_id
+
+        # Get the best model that already exists for this train dataset
+        trainparams_id = conf.train.getint("trainparams_id")
+        best_model = mh.get_best_model(
+            model_dir=conf.dirs.getpath("model_dir"),
+            segment_subject=conf.general["segment_subject"],
+            traindata_id=traindata_id,
+            trainparams_id=trainparams_id,
+        )
+
+        # Check if a model was found
+        if best_model is None:
+            message = (
+                f"No model found in model_dir: {conf.dirs.getpath('model_dir')} for "
+                f"traindata_id: {traindata_id}"
+            )
+            logger.critical(message)
+            raise Exception(message)
+        else:
+            model_weights_filepath = best_model["filepath"]
+            logger.info(f"Best model found: {model_weights_filepath}")
+
+        # Load the hyperparams of the model
+        # TODO: move the hyperparams filename formatting to get_models...
+        hyperparams_path = (
+            best_model["filepath"].parent
+            / f"{best_model['basefilename']}_hyperparams.json"
+        )
+        hyperparams = mh.HyperParams(path=hyperparams_path)
+
+        # Prepare output subdir to be used for predictions
+        predict_out_subdir = f"{best_model['basefilename']}"
+        if trainparams_id > 0:
+            predict_out_subdir += f"_{trainparams_id}"
+        predict_out_subdir += f"_{best_model['epoch']}"
+
+        # Load model to predict with
+        # --------------------------
+        model = None
+        # Try optimizing model with tensorrt. Not supported on Windows
+        # -> disabled for now till I have access again to a linux machine
+        """
+        if os.name != "nt":
+            try:
+                # Try import
+                from tensorflow.python.compiler.tensorrt import trt_convert as trt
+
+                # Import didn't fail, so optimize model
+                logger.info(
+                    "Tensorrt is available, so try to create and use optimized model"
+                )
+                savedmodel_optim_dir = (
+                    best_model["filepath"].parent
+                    / f"{best_model['filepath'].stem}_optim"
+                )
+                if not savedmodel_optim_dir.exists():
+                    # If base model not yet in savedmodel format
+                    savedmodel_dir = (
+                        best_model["filepath"].parent / best_model["filepath"].stem
+                    )
+                    if not savedmodel_dir.exists():
+                        logger.info(
+                            f"SavedModel format not yet available, so load "
+                            f"model + weights from {best_model['filepath']}"
+                        )
+                        model = mf.load_model(best_model["filepath"], compile=False)
+                        logger.info(f"Now save again as savedmodel to {savedmodel_dir}")
+                        tf.saved_model.save(model, str(savedmodel_dir))
+                        model = None
+
+                    # Now optimize model
+                    logger.info(f"Optimize + save model to {savedmodel_optim_dir}")
+                    converter = trt.TrtGraphConverterV2(
+                        input_saved_model_dir=str(savedmodel_dir),
+                        is_dynamic_op=True,
+                        precision_mode="FP16",
+                    )
+                    converter.convert()
+                    converter.save(savedmodel_optim_dir)
+
+                logger.info(
+                    f"Load optimized model + weights from {savedmodel_optim_dir}"
+                )
+                model = tf.keras.models.load_model(str(savedmodel_optim_dir))
+
+            except ImportError:
+                logger.info("Tensorrt is not available, so load unoptimized model")
+            except Exception as ex:
+                logger.info(
+                    "An error occured trying to use tensorrt, "
+                    f"so load unoptimized model. Error: {ex}"
+                )
+        """
+
+        # If model isn't loaded yet... load!
+        if model is None:
+            model = mf.load_model(best_model["filepath"], compile=False)
+
+        # Prepare the model for predicting
+        nb_gpu = len(tf.config.experimental.list_physical_devices("GPU"))
+        batch_size = conf.predict.getint("batch_size")
+        if nb_gpu <= 1:
+            model_for_predict = model
+            logger.info(f"Predict using single GPU or CPU, with nb_gpu: {nb_gpu}")
+        else:
+            # If multiple GPU's available, create multi_gpu_model
+            try:
+                model_for_predict = model
+                logger.warn("Predict using multiple GPUs NOT IMPLEMENTED AT THE MOMENT")
+
+                # logger.info(
+                #     f"Predict using multiple GPUs: {nb_gpu}, batch size becomes: "
+                #     f"{batch_size*nb_gpu}"
+                # )
+                # batch_size *= nb_gpu
+            except ValueError:
+                logger.info("Predict using single GPU or CPU")
+                model_for_predict = model
+
+        # Prepare params for the inline postprocessing of the prediction
+        min_probability = conf.predict.getfloat("min_probability")
+        postprocess = {}
+        simplify_algorithm = conf.predict.get("simplify_algorithm")
+        if simplify_algorithm is not None:
+            postprocess["simplify"] = {}
+            simplify = postprocess["simplify"]
+
+            simplify_algorithm = gfo.SimplifyAlgorithm[simplify_algorithm]
+            simplify["simplify_algorithm"] = simplify_algorithm
+            simplify["simplify_tolerance"] = conf.predict.geteval("simplify_tolerance")
+            simplify["simplify_lookahead"] = conf.predict.getint("simplify_lookahead")
+            simplify["simplify_topological"] = conf.predict.getboolean_ext(
+                "simplify_topological"
+            )
+        postprocess["filter_background_modal_size"] = conf.predict.getint(
+            "filter_background_modal_size"
+        )
+        query = conf.predict.get("reclassify_to_neighbour_query")
+        if query is not None:
+            query = query.replace("\n", " ")
+        postprocess["reclassify_to_neighbour_query"] = query
+        logger.info(f"Inline postprocessing:\n{pprint.pformat(postprocess)}")
+
+        # Prepare the output dirs/paths
+        predict_output_dir = Path(
+            f"{str(conf.dirs.getpath('predict_image_output_basedir'))}_"
+            f"{predict_out_subdir}"
+        )
+        output_vector_dir = conf.dirs.getpath("output_vector_dir")
+        output_vector_name = (
+            f"{best_model['basefilename']}_{best_model['epoch']}_"
+            f"{conf.predict['image_layer']}"
+        )
+        output_vector_path = output_vector_dir / f"{output_vector_name}.gpkg"
+
+        # Predict for entire dataset
+        nb_parallel = conf.general.getint("nb_parallel")
+        predicter.predict_dir(
+            model=model_for_predict,  # type: ignore
+            input_image_dir=input_image_dir,
+            output_image_dir=predict_output_dir,
+            output_vector_path=output_vector_path,
+            classes=hyperparams.architecture.classes,
+            min_probability=min_probability,
+            postprocess=postprocess,
+            border_pixels_to_ignore=conf.predict.getint("image_pixels_overlap"),
+            projection_if_missing=image_layer["projection"],
+            input_mask_dir=None,
+            batch_size=batch_size,
+            evaluate_mode=False,
+            cancel_filepath=conf.files.getpath("cancel_filepath"),
+            nb_parallel_postprocess=nb_parallel,
+            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+        )
+
+        # Log and send mail
+        message = f"Completed predict for config {config_path.stem}"
+        logger.info(message)
+        email_helper.sendmail(message)
+    except Exception as ex:
+        message = f"ERROR while running predict for task {config_path.stem}"
+        logger.exception(message)
+        email_helper.sendmail(
+            subject=message, body=f"Exception: {ex}\n\n {traceback.format_exc()}"
+        )
+        raise Exception(message) from ex
+
+
+def main():
+    try:
+        predict_args(sys.argv[1:])
+    except Exception as ex:
+        logger.exception(f"Error: {ex}")
+        raise
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    main()
```

### Comparing `orthoseg-0.4.2/orthoseg/project_defaults.ini` & `orthoseg-0.4.2a1/orthoseg/project_defaults.ini`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,442 +1,442 @@
-# This config file contains the default settings for all orthoseg projects.
-#
-# The config used for an orthoseg project is loaded in the following order:
-#   1) the project defaults as "hardcoded" in orthoseg (project_defaults.ini)
-#   2) any .ini files specified in the general.extra_config_files_to_load 
-#      parameter (in this file).
-#   3) the project config file
-# Parameters specified in a config file loaded later in the order above
-# overrule the corresponding parameter values specified in a previously 
-# loaded config file.
-
-# General settings.
-[general]
-# Extra config files to load for the project. They will be loaded in the 
-# order specified and can be specified one path per line, comma seperated.
-# If a relative path is used it will be resolved towards the parent dir of 
-# the project config file.
-extra_config_files_to_load =
-
-# The subject that will be segmented -> must be overruled in the project 
-# specific config file!!!
-segment_subject = MUST_OVERRIDE
-
-# Set the way certificates of ssl requests are verified:
-#   * True: use the default certificate bundle as installed on your system
-#   * False: disable certificate validation (NOT recommended!)
-#   * path to a certificate bundle file (.pem) to specify the certificate 
-#     bundle to be used. In corporate networks using a proxy server this is 
-#     often needed when requests give CERTIFICATE_VERIFY_FAILED errors.
-ssl_verify = True
-
-# Specify the number of cpu's to use while doing heavy processing. If -1, it 
-# uses all available processors.
-nb_parallel = -1
-
-# Settings regarding the download action
-[download]
-# Schedule to control when images can be downloaded. If not specified there is 
-# no time limitation.  
-cron_schedule
-
-# Settings concerning the neural network model you want to use for the 
-# segmentation. 
-[model]
-# The id of the architecture used. 
-# Only needs to be changed if you want to compare the results of different  
-# architectures on the same training data. 
-# Reason: OrthoSeg will only train one model per traindata_id, architecture_id 
-# and hyperparams_id.
-# So if you want to compare different architectures, give each architecture a 
-# unique id.
-# Remark: if the architecture_id is 0, it won't be included in the file name 
-# of trained models.
-architecture_id = 0
-
-# The segmentation architecture to use. 
-# 
-# The architectures currently supported by orthoseg follow the encoder-decoder 
-# principle:
-#   * an encoder: a (deep) neural network that detects features on object level
-#   * a decoder: a (deep) neural network that converts the detected features 
-#     on object level to a segmentation on pixel level
-#
-# To configure an encoder/decoder architecture in orthoseg, specify the it in 
-# the following way: architecture = {encoder}+{decoder}
-#
-# There are a lot of encoders and decoders supported.
-# For starters, the following encoder/decoder combinations are available:
-#   * decoder: unet
-#   * encoder: unet, ternaus 
-# In the configuration, this can be specified as such, eg.:
-#   * architecture = standard+unet
-#
-# Additionally, all encoders/decoders as provided by the 'segmentation_models'
-# project (https://github.com/qubvel/segmentation_models#models-and-backbones) 
-# can be used. 
-# In the configuration below, use the "backbone" as encoder, and the "model" 
-# as decoder, eg.:
-#   * architecture = inceptionresnetv2+unet
-architecture = inceptionresnetv2+unet
-
-# The number of channels of the images to train on
-nb_channels = 3
-
-# Settings concerning the train process.
-[train]
-# Preload model -> only overrule in local_overrule.ini!
-preload_with_previous_traindata = False
-# Force to use a model trained on this traindata version (-1 to disable)
-force_model_traindata_id = -1
-# When training, resume training on the current best existing model
-resume_train = False
-# Train a model, even if a model exists already
-force_train = False
-
-# Pattern how the file paths of the label files should be formatted.
-# The image_layer to get the images from is extracted from the file path. 
-labelpolygons_pattern = ${dirs:labels_dir}/${general:segment_subject}_{image_layer}_polygons.gpkg
-labellocations_pattern = ${dirs:labels_dir}/${general:segment_subject}_{image_layer}_locations.gpkg
-
-# Column where the labels for each training polygon is available. If the column
-# name configured here is not available columns "label_name" is tried as well. 
-labelname_column = classname
-
-# Info about the images used to train on
-image_pixel_width = 512
-image_pixel_height = 512
-image_pixel_x_size = 0.25
-image_pixel_y_size = 0.25
-
-# The id of the set of hyper parameters to use while training. 
-# Only needs to be changed if you want to compare the results of different  
-# hyperparameter sets on the same training data. 
-# Reason: OrthoSeg will only train one model per traindata_id, architecture_id and hyperparams_id.
-# So if you want to compare different hyperparameters, give each set a unique id.
-# If the hyperparams_id is 0, it won't be included in the file name of trained models.
-trainparams_id = 0
-
-# Image augmentations in json format
-image_augmentations = { "fill_mode": "constant",
-                        "cval": 0,
-                        "rescale": 0.0039215686274509803921568627451,
-                        "rotation_range": 359.0,
-                        "width_shift_range": 0.05,
-                        "height_shift_range": 0.05,
-                        "zoom_range": 0.1,
-                        "brightness_range": [0.95, 1.05]
-                    }
-
-# Mask augmentations in json format. 
-# Remarks: 
-#   * the number of randomized values must be the same as for the image, 
-#     otherwise the random augentation factors aren't the same as the image!
-#   * augmentations to translate, rotate,... should be the same as for the image!
-#   * the mask generally shouldn't be rescaled!
-#   * cval values should always be 0 for the mask, even if it is different for 
-#     the image, as the cval of the mask refers to these locations being 
-#     of class "background".
-mask_augmentations = { "fill_mode": "constant",
-                        "cval": 0,
-                        "rescale": 1,
-                        "rotation_range": 359.0,
-                        "width_shift_range": 0.05,
-                        "height_shift_range": 0.05,
-                        "zoom_range": 0.1,
-                        "brightness_range": [1.0, 1.0]
-                    }
-
-# In json format, the classes to train/predict and for each class:
-#     * the label names in the training data to use for this class  
-#     * the weight to use when training
-classes =   {   "background": {
-                    "labelnames": ["ignore_for_train", "background"],
-                    "weight": 1
-                },
-                "${general:segment_subject}": {
-                    "labelnames": ["${general:segment_subject}"],
-                    "weight": 1
-                }
-            }
-
-# The batch size to use during fit of model. 
-# Depends on available hardware, model used and image size.
-batch_size_fit = 6
-# The batch size to use while predicting in the train process. 
-# Depends on available hardware, model used and image size.
-batch_size_predict = 20
-
-# Optimizer to use + params
-optimizer = adam
-optimizer_params = { "learning_rate": 0.0001 } 
-
-# Loss function to use: if not specified: automatic: 
-#   - if weights specified in the classes: weighted_categorical_crossentropy
-#   - if no weights are specified: categorical_crossentropy
-loss_function
-
-# The metric(s) to monitor to evaluate which network is best during the 
-# training. This can be a single metric or a formula with placeholders 
-# to calculate a value based on multiple metrics. Available metrics:
-#   - one_hot_mean_iou: intersection over union on the training dataset
-#   - val_one_hot_mean_iou: intersection over union on the validation dataset
-#   - categorical_accuracy: accuracy on the training dataset
-#   - val_categorical_accuracy: accuracy on the validation dataset
-monitor_metric = ({one_hot_mean_iou}+{val_one_hot_mean_iou})/2
-# Use max to keep the models with a high monitor_metric. Otherwise use min.
-monitor_metric_mode = max
-
-# Format to save the trained model in. Options are h5 or tf.
-save_format = h5
-# True to only keep the best model during training
-save_best_only = True
-# Minimum accuracy to save, (0 = always save)
-save_min_accuracy = 0.80
-
-# Number of epochs to train with some frozen layers. Keeps pretrained layers 
-# intact, which is especially usefull for the first few (2-10) epochs when 
-# big adjustments are made to the network. Training is also 20% faster during 
-# these epochs.   
-nb_epoch_with_freeze = 20
-# Maximum number of epochs to train (without frozen layers). 
-# These epochs are in addition to nb_epoch_with_freeze.
-max_epoch = 1000
-
-# Stop training if earlystop_monitor_metric hasn't improved for 
-# earlystop_patience epochs
-earlystop_patience = 100
-# Options for the earlystop metric: categorical_accuracy, one_hot_mean_iou
-earlystop_monitor_metric = one_hot_mean_iou
-# Use max if the monitor_metric should be high. Otherwise use min.
-earlystop_monitor_metric_mode = max
-
-# True to activate tensorboard style logging 
-log_tensorboard = False
-# True to activate csv logging 
-log_csv = True
-
-# Subdir name to save augmented images to while training (only for debugging)
-save_augmented_subdir
-
-# Settings concerning the prediction process.
-[predict]
-# The batch size to use. 
-# Depends on available hardware, model used and image size.
-batch_size = 4
-
-# Info about the source images that need to be segmented.
-# The image_layer must be specified to be able to predict.
-image_layer = MUST_OVERRIDE
-image_pixel_width = 2048
-image_pixel_height = 2048
-image_pixel_x_size = 0.25
-image_pixel_y_size = 0.25
-image_pixels_overlap = 128
-
-# The minimum probability that a pixel needs to obtain for a class not to be treated as
-# background.
-min_probability = 0.5
-
-# Maximum errors that can occur during prediction before prediction process is stopped.
-max_prediction_errors = 100
-
-# Config for the cleanup operations that are done on the predictions on-the-fly.
-
-# Apply a filter to the background pixels and replace background by the most occuring
-# value in a rectangle around the background pixel of the size specified.
-filter_background_modal_size = 0
-
-# Reclassify all detected polygons that comply to the query provided to the class of
-# the neighbour with the longest border with it.
-# The query need to be in the form to be used by pandas.DataFrame.query() and the
-# following columns are available to query on:
-#   - area: the area of the polygon, as calculated by GeoSeries.area .
-#   - perimeter: the perimeter of the polygon, as calculated by GeoSeries.length .
-#   - onborder: 1 if the polygon touches the border of the tile being predicted, 0 if
-#     it doesn't. It is often useful to filter with onborder == 0 to avoid eg. polygons
-#     being reclassified because they are small due to being on the border.
-# Eg.: reclassify_to_neighbour_query = (onborder == 0 and area <= 5)
-reclassify_to_neighbour_query
-
-# Algorithm to use if vector simplification needs to be executed:
-#   * RAMER_DOUGLAS_PEUCKER: 
-#       * simplify_tolerance: extra, mandatory parameter: specifies the distance 
-#         tolerance to be used.
-#   * VISVALINGAM_WHYATT: 
-#       * simplify_tolerance: extra, mandatory parameter: specifies the area 
-#         tolerance to be used.
-#   * LANG: seems to give best results: best cleaning with few deformation.
-#       * simplify_tolerance: extra, mandatory parameter: specifies the distance 
-#         tolerance to be used.
-#       * simplify_lookahead: extra, mandatory parameter: specifies the number  
-#         of points the algorithm looks ahead during simplify.
-#   * If simplify_algorithm is not specified, no simplification is applied.  
-simplify_algorithm = LANG
-
-# Tolerance to use for the simplification. 
-# Remark: you can use simple math expressions, eg. 1.5*5 
-simplify_tolerance = ${image_pixel_x_size}*1.5
-# For algorythms that need this, specifies the number of points to look ahead
-# during simplify. Used for LANG.
-simplify_lookahead = 8
-# If True, the resulting polygons of the classification are converted to topologies so
-# no gaps are introduced in polygons that are next to each other. If not specified
-# (= None), a multi-class classification will be simplified topologically, a single
-# class will be simplified the standard way.
-simplify_topological
-
-# Settings concerning the postprocessing after the prediction.
-[postprocess]
-
-# If dissolve is true, the result is dissolved.
-dissolve = True
-# If a path is provided, the result of the dissolve will be tiled on the tiles 
-# provided.
-dissolve_tiles_path
-
-# Reclassify all detected polygons that comply to the query provided to the class of
-# the neighbour with the longest border with it.
-# The query need to be in the form to be used by pandas.DataFrame.query() and the
-# following columns are available to query on:
-#   - area: the area of the polygon, as calculated by GeoSeries.area.
-#   - perimeter: the perimeter of the polygon, as calculated by GeoSeries.length.
-# Eg.: reclassify_to_neighbour_query = (area <= 5)
-reclassify_to_neighbour_query
-
-# Apply simplify (also) after dissolve. For more information, check out the 
-# documentation at parameter predict:simplify_algorithm
-simplify_algorithm
-
-# Tolerance to use for the postprocess simplification. 
-# Remark: you can use simple math expressions, eg. 1.5*5 
-simplify_tolerance = ${predict:image_pixel_x_size}*2
-
-# For algorythms that need this, specifies the number of points to look ahead
-# during simplify. Used for LANG.
-simplify_lookahead = 8
-
-# Settings concerning the directories where input/output data is found/put.
-[dirs]
-# Remarks: 
-#   * UNC paths are not supported on Windows, always use mapped drive letters!
-#   * always use forward slashes, even on Windows systems
-#   * in all paths, it is possible to use the {tempdir} placeholder, which will 
-#     be replaced by the default system temp dir. 
-
-# The base projects dir, where multiple orthoseg projects can be stored. Can either be 
-#   * an absolute path 
-#   * OR a relative path starting from the location of the specific projectconfig file of the project
-# Eg.: ".." means: projects_dir is the parent dir of the dir containing the project config file
-projects_dir = ..
-
-# The project directory for this subject
-project_dir = ${projects_dir}/${general:segment_subject}
-
-# Log dir
-log_dir = ${project_dir}/log
-
-# Dir containing the label data
-labels_dir = ${project_dir}/labels
-
-# Dirs used to put data during training 
-training_dir = ${project_dir}/training
-
-# Model dir
-model_dir = ${project_dir}/models
-
-# Output vector dir
-output_vector_dir = ${project_dir}/output_vector/${predict:image_layer}
-
-# Dir with the images we want predictions for
-base_image_dir = ${projects_dir}/_image_cache
-predict_image_input_subdir = ${predict:image_pixel_width}x${predict:image_pixel_height}_${predict:image_pixels_overlap}pxOverlap
-predict_image_input_dir = ${base_image_dir}/${predict:image_layer}/${predict_image_input_subdir}
-predict_image_output_basedir = ${predict_image_input_dir}
-
-# Dir with sample images for use during training
-# Remark: these samples are meant to check the training quality, so by default
-#         the train image size is used!!! 
-predictsample_image_input_subdir = ${train:image_pixel_width}x${train:image_pixel_height}
-predictsample_image_input_dir = ${base_image_dir}/${predict:image_layer}_testsample/${predictsample_image_input_subdir}
-predictsample_image_output_basedir = ${predictsample_image_input_dir}
-
-# Settings concerning some specific file paths.
-[files]
-# File path that will be used to save/load the keras model definition
-model_json_filepath = ${dirs:model_dir}/${model:architecture}.json
-image_layers_config_filepath = ${dirs:projects_dir}/imagelayers.ini
-
-# File path of file that if it exists cancels the current processing
-cancel_filepath = ${dirs:projects_dir}/cancel.txt
-
-# Email config to use to send progress info to. 
-[email]
-# Set enabled to True to enable sending mails
-enabled = False
-# Email address to send task status info from
-from = sample@samplemail.be
-# Email address to send task status info to
-to = sample@samplemail.be
-# Smtp server to use 
-smtp_server = server.for.emails.be
-# Username to use to login to smtp server (in some cases optional)
-mail_server_username = 
-# Password to use to login to smtp server (in some cases optional)
-mail_server_password = 
-
-# Logging configuration. 
-[logging]
-# The number of log files to keep in a log dir
-nb_logfiles_tokeep = 10
-
-# Config to use for the logging. This config is in json, following the 
-# conventions as required by logging.dictConfig.
-# https://docs.python.org/3/library/logging.config.html#logging-config-dictschema 
-# 
-# Mind: the location for file logging 
-logconfig = {
-        "version": 1,
-        "disable_existing_loggers": true,
-        "formatters": {
-            "console": {
-                "format": "%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s", 
-                "datefmt": "%H:%M:%S"
-                },
-            "file": {
-                "format": "%(asctime)s|%(levelname)s|%(name)s|%(message)s", 
-                "datefmt": null
-            }
-        },
-        "handlers": {
-            "console": {
-                "level": "INFO",
-                "class": "logging.StreamHandler",
-                "formatter": "console",
-                "stream": "ext://sys.stdout"
-            },
-            "file": {
-                "level": "INFO",
-                "class": "logging.handlers.RotatingFileHandler",
-                "formatter": "file",
-                "filename": "_log/{iso_datetime}.log",
-                "maxBytes": 10000000,
-                "backupCount": 3
-            }
-        },
-        "loggers": {
-            "geofile_ops": {
-                "level": "INFO",
-                "handlers": ["console"],
-                "propagate": false
-            },
-            "geofile_ops.geofile_ops": {
-                "level": "DEBUG",
-                "handlers": ["console"],
-                "propagate": false
-            }        
-        },
-        "root": {
-            "level": "INFO",
-            "handlers": ["console", "file"]
-        }
+# This config file contains the default settings for all orthoseg projects.
+#
+# The config used for an orthoseg project is loaded in the following order:
+#   1) the project defaults as "hardcoded" in orthoseg (project_defaults.ini)
+#   2) any .ini files specified in the general.extra_config_files_to_load 
+#      parameter (in this file).
+#   3) the project config file
+# Parameters specified in a config file loaded later in the order above
+# overrule the corresponding parameter values specified in a previously 
+# loaded config file.
+
+# General settings.
+[general]
+# Extra config files to load for the project. They will be loaded in the 
+# order specified and can be specified one path per line, comma seperated.
+# If a relative path is used it will be resolved towards the parent dir of 
+# the project config file.
+extra_config_files_to_load =
+
+# The subject that will be segmented -> must be overruled in the project 
+# specific config file!!!
+segment_subject = MUST_OVERRIDE
+
+# Set the way certificates of ssl requests are verified:
+#   * True: use the default certificate bundle as installed on your system
+#   * False: disable certificate validation (NOT recommended!)
+#   * path to a certificate bundle file (.pem) to specify the certificate 
+#     bundle to be used. In corporate networks using a proxy server this is 
+#     often needed when requests give CERTIFICATE_VERIFY_FAILED errors.
+ssl_verify = True
+
+# Specify the number of cpu's to use while doing heavy processing. If -1, it 
+# uses all available processors.
+nb_parallel = -1
+
+# Settings regarding the download action
+[download]
+# Schedule to control when images can be downloaded. If not specified there is 
+# no time limitation.  
+cron_schedule
+
+# Settings concerning the neural network model you want to use for the 
+# segmentation. 
+[model]
+# The id of the architecture used. 
+# Only needs to be changed if you want to compare the results of different  
+# architectures on the same training data. 
+# Reason: OrthoSeg will only train one model per traindata_id, architecture_id 
+# and hyperparams_id.
+# So if you want to compare different architectures, give each architecture a 
+# unique id.
+# Remark: if the architecture_id is 0, it won't be included in the file name 
+# of trained models.
+architecture_id = 0
+
+# The segmentation architecture to use. 
+# 
+# The architectures currently supported by orthoseg follow the encoder-decoder 
+# principle:
+#   * an encoder: a (deep) neural network that detects features on object level
+#   * a decoder: a (deep) neural network that converts the detected features 
+#     on object level to a segmentation on pixel level
+#
+# To configure an encoder/decoder architecture in orthoseg, specify the it in 
+# the following way: architecture = {encoder}+{decoder}
+#
+# There are a lot of encoders and decoders supported.
+# For starters, the following encoder/decoder combinations are available:
+#   * decoder: unet
+#   * encoder: unet, ternaus 
+# In the configuration, this can be specified as such, eg.:
+#   * architecture = standard+unet
+#
+# Additionally, all encoders/decoders as provided by the 'segmentation_models'
+# project (https://github.com/qubvel/segmentation_models#models-and-backbones) 
+# can be used. 
+# In the configuration below, use the "backbone" as encoder, and the "model" 
+# as decoder, eg.:
+#   * architecture = inceptionresnetv2+unet
+architecture = inceptionresnetv2+unet
+
+# The number of channels of the images to train on
+nb_channels = 3
+
+# Settings concerning the train process.
+[train]
+# Preload model -> only overrule in local_overrule.ini!
+preload_with_previous_traindata = False
+# Force to use a model trained on this traindata version (-1 to disable)
+force_model_traindata_id = -1
+# When training, resume training on the current best existing model
+resume_train = False
+# Train a model, even if a model exists already
+force_train = False
+
+# Pattern how the file paths of the label files should be formatted.
+# The image_layer to get the images from is extracted from the file path. 
+labelpolygons_pattern = ${dirs:labels_dir}/${general:segment_subject}_{image_layer}_polygons.gpkg
+labellocations_pattern = ${dirs:labels_dir}/${general:segment_subject}_{image_layer}_locations.gpkg
+
+# Column where the labels for each training polygon is available. If the column
+# name configured here is not available columns "label_name" is tried as well. 
+labelname_column = classname
+
+# Info about the images used to train on
+image_pixel_width = 512
+image_pixel_height = 512
+image_pixel_x_size = 0.25
+image_pixel_y_size = 0.25
+
+# The id of the set of hyper parameters to use while training. 
+# Only needs to be changed if you want to compare the results of different  
+# hyperparameter sets on the same training data. 
+# Reason: OrthoSeg will only train one model per traindata_id, architecture_id and hyperparams_id.
+# So if you want to compare different hyperparameters, give each set a unique id.
+# If the hyperparams_id is 0, it won't be included in the file name of trained models.
+trainparams_id = 0
+
+# Image augmentations in json format
+image_augmentations = { "fill_mode": "constant",
+                        "cval": 0,
+                        "rescale": 0.0039215686274509803921568627451,
+                        "rotation_range": 359.0,
+                        "width_shift_range": 0.05,
+                        "height_shift_range": 0.05,
+                        "zoom_range": 0.1,
+                        "brightness_range": [0.95, 1.05]
+                    }
+
+# Mask augmentations in json format. 
+# Remarks: 
+#   * the number of randomized values must be the same as for the image, 
+#     otherwise the random augentation factors aren't the same as the image!
+#   * augmentations to translate, rotate,... should be the same as for the image!
+#   * the mask generally shouldn't be rescaled!
+#   * cval values should always be 0 for the mask, even if it is different for 
+#     the image, as the cval of the mask refers to these locations being 
+#     of class "background".
+mask_augmentations = { "fill_mode": "constant",
+                        "cval": 0,
+                        "rescale": 1,
+                        "rotation_range": 359.0,
+                        "width_shift_range": 0.05,
+                        "height_shift_range": 0.05,
+                        "zoom_range": 0.1,
+                        "brightness_range": [1.0, 1.0]
+                    }
+
+# In json format, the classes to train/predict and for each class:
+#     * the label names in the training data to use for this class  
+#     * the weight to use when training
+classes =   {   "background": {
+                    "labelnames": ["ignore_for_train", "background"],
+                    "weight": 1
+                },
+                "${general:segment_subject}": {
+                    "labelnames": ["${general:segment_subject}"],
+                    "weight": 1
+                }
+            }
+
+# The batch size to use during fit of model. 
+# Depends on available hardware, model used and image size.
+batch_size_fit = 6
+# The batch size to use while predicting in the train process. 
+# Depends on available hardware, model used and image size.
+batch_size_predict = 20
+
+# Optimizer to use + params
+optimizer = adam
+optimizer_params = { "learning_rate": 0.0001 } 
+
+# Loss function to use: if not specified: automatic: 
+#   - if weights specified in the classes: weighted_categorical_crossentropy
+#   - if no weights are specified: categorical_crossentropy
+loss_function
+
+# The metric(s) to monitor to evaluate which network is best during the 
+# training. This can be a single metric or a formula with placeholders 
+# to calculate a value based on multiple metrics. Available metrics:
+#   - one_hot_mean_iou: intersection over union on the training dataset
+#   - val_one_hot_mean_iou: intersection over union on the validation dataset
+#   - categorical_accuracy: accuracy on the training dataset
+#   - val_categorical_accuracy: accuracy on the validation dataset
+monitor_metric = ({one_hot_mean_iou}+{val_one_hot_mean_iou})/2
+# Use max to keep the models with a high monitor_metric. Otherwise use min.
+monitor_metric_mode = max
+
+# Format to save the trained model in. Options are h5 or tf.
+save_format = h5
+# True to only keep the best model during training
+save_best_only = True
+# Minimum accuracy to save, (0 = always save)
+save_min_accuracy = 0.80
+
+# Number of epochs to train with some frozen layers. Keeps pretrained layers 
+# intact, which is especially usefull for the first few (2-10) epochs when 
+# big adjustments are made to the network. Training is also 20% faster during 
+# these epochs.   
+nb_epoch_with_freeze = 20
+# Maximum number of epochs to train (without frozen layers). 
+# These epochs are in addition to nb_epoch_with_freeze.
+max_epoch = 1000
+
+# Stop training if earlystop_monitor_metric hasn't improved for 
+# earlystop_patience epochs
+earlystop_patience = 100
+# Options for the earlystop metric: categorical_accuracy, one_hot_mean_iou
+earlystop_monitor_metric = one_hot_mean_iou
+# Use max if the monitor_metric should be high. Otherwise use min.
+earlystop_monitor_metric_mode = max
+
+# True to activate tensorboard style logging 
+log_tensorboard = False
+# True to activate csv logging 
+log_csv = True
+
+# Subdir name to save augmented images to while training (only for debugging)
+save_augmented_subdir
+
+# Settings concerning the prediction process.
+[predict]
+# The batch size to use. 
+# Depends on available hardware, model used and image size.
+batch_size = 4
+
+# Info about the source images that need to be segmented.
+# The image_layer must be specified to be able to predict.
+image_layer = MUST_OVERRIDE
+image_pixel_width = 2048
+image_pixel_height = 2048
+image_pixel_x_size = 0.25
+image_pixel_y_size = 0.25
+image_pixels_overlap = 128
+
+# The minimum probability that a pixel needs to obtain for a class not to be treated as
+# background.
+min_probability = 0.5
+
+# Maximum errors that can occur during prediction before prediction process is stopped.
+max_prediction_errors = 100
+
+# Config for the cleanup operations that are done on the predictions on-the-fly.
+
+# Apply a filter to the background pixels and replace background by the most occuring
+# value in a rectangle around the background pixel of the size specified.
+filter_background_modal_size = 0
+
+# Reclassify all detected polygons that comply to the query provided to the class of
+# the neighbour with the longest border with it.
+# The query need to be in the form to be used by pandas.DataFrame.query() and the
+# following columns are available to query on:
+#   - area: the area of the polygon, as calculated by GeoSeries.area .
+#   - perimeter: the perimeter of the polygon, as calculated by GeoSeries.length .
+#   - onborder: 1 if the polygon touches the border of the tile being predicted, 0 if
+#     it doesn't. It is often useful to filter with onborder == 0 to avoid eg. polygons
+#     being reclassified because they are small due to being on the border.
+# Eg.: reclassify_to_neighbour_query = (onborder == 0 and area <= 5)
+reclassify_to_neighbour_query
+
+# Algorithm to use if vector simplification needs to be executed:
+#   * RAMER_DOUGLAS_PEUCKER: 
+#       * simplify_tolerance: extra, mandatory parameter: specifies the distance 
+#         tolerance to be used.
+#   * VISVALINGAM_WHYATT: 
+#       * simplify_tolerance: extra, mandatory parameter: specifies the area 
+#         tolerance to be used.
+#   * LANG: seems to give best results: best cleaning with few deformation.
+#       * simplify_tolerance: extra, mandatory parameter: specifies the distance 
+#         tolerance to be used.
+#       * simplify_lookahead: extra, mandatory parameter: specifies the number  
+#         of points the algorithm looks ahead during simplify.
+#   * If simplify_algorithm is not specified, no simplification is applied.  
+simplify_algorithm = LANG
+
+# Tolerance to use for the simplification. 
+# Remark: you can use simple math expressions, eg. 1.5*5 
+simplify_tolerance = ${image_pixel_x_size}*1.5
+# For algorythms that need this, specifies the number of points to look ahead
+# during simplify. Used for LANG.
+simplify_lookahead = 8
+# If True, the resulting polygons of the classification are converted to topologies so
+# no gaps are introduced in polygons that are next to each other. If not specified
+# (= None), a multi-class classification will be simplified topologically, a single
+# class will be simplified the standard way.
+simplify_topological
+
+# Settings concerning the postprocessing after the prediction.
+[postprocess]
+
+# If dissolve is true, the result is dissolved.
+dissolve = True
+# If a path is provided, the result of the dissolve will be tiled on the tiles 
+# provided.
+dissolve_tiles_path
+
+# Reclassify all detected polygons that comply to the query provided to the class of
+# the neighbour with the longest border with it.
+# The query need to be in the form to be used by pandas.DataFrame.query() and the
+# following columns are available to query on:
+#   - area: the area of the polygon, as calculated by GeoSeries.area.
+#   - perimeter: the perimeter of the polygon, as calculated by GeoSeries.length.
+# Eg.: reclassify_to_neighbour_query = (area <= 5)
+reclassify_to_neighbour_query
+
+# Apply simplify (also) after dissolve. For more information, check out the 
+# documentation at parameter predict:simplify_algorithm
+simplify_algorithm
+
+# Tolerance to use for the postprocess simplification. 
+# Remark: you can use simple math expressions, eg. 1.5*5 
+simplify_tolerance = ${predict:image_pixel_x_size}*2
+
+# For algorythms that need this, specifies the number of points to look ahead
+# during simplify. Used for LANG.
+simplify_lookahead = 8
+
+# Settings concerning the directories where input/output data is found/put.
+[dirs]
+# Remarks: 
+#   * UNC paths are not supported on Windows, always use mapped drive letters!
+#   * always use forward slashes, even on Windows systems
+#   * in all paths, it is possible to use the {tempdir} placeholder, which will 
+#     be replaced by the default system temp dir. 
+
+# The base projects dir, where multiple orthoseg projects can be stored. Can either be 
+#   * an absolute path 
+#   * OR a relative path starting from the location of the specific projectconfig file of the project
+# Eg.: ".." means: projects_dir is the parent dir of the dir containing the project config file
+projects_dir = ..
+
+# The project directory for this subject
+project_dir = ${projects_dir}/${general:segment_subject}
+
+# Log dir
+log_dir = ${project_dir}/log
+
+# Dir containing the label data
+labels_dir = ${project_dir}/labels
+
+# Dirs used to put data during training 
+training_dir = ${project_dir}/training
+
+# Model dir
+model_dir = ${project_dir}/models
+
+# Output vector dir
+output_vector_dir = ${project_dir}/output_vector/${predict:image_layer}
+
+# Dir with the images we want predictions for
+base_image_dir = ${projects_dir}/_image_cache
+predict_image_input_subdir = ${predict:image_pixel_width}x${predict:image_pixel_height}_${predict:image_pixels_overlap}pxOverlap
+predict_image_input_dir = ${base_image_dir}/${predict:image_layer}/${predict_image_input_subdir}
+predict_image_output_basedir = ${predict_image_input_dir}
+
+# Dir with sample images for use during training
+# Remark: these samples are meant to check the training quality, so by default
+#         the train image size is used!!! 
+predictsample_image_input_subdir = ${train:image_pixel_width}x${train:image_pixel_height}
+predictsample_image_input_dir = ${base_image_dir}/${predict:image_layer}_testsample/${predictsample_image_input_subdir}
+predictsample_image_output_basedir = ${predictsample_image_input_dir}
+
+# Settings concerning some specific file paths.
+[files]
+# File path that will be used to save/load the keras model definition
+model_json_filepath = ${dirs:model_dir}/${model:architecture}.json
+image_layers_config_filepath = ${dirs:projects_dir}/imagelayers.ini
+
+# File path of file that if it exists cancels the current processing
+cancel_filepath = ${dirs:projects_dir}/cancel.txt
+
+# Email config to use to send progress info to. 
+[email]
+# Set enabled to True to enable sending mails
+enabled = False
+# Email address to send task status info from
+from = sample@samplemail.be
+# Email address to send task status info to
+to = sample@samplemail.be
+# Smtp server to use 
+smtp_server = server.for.emails.be
+# Username to use to login to smtp server (in some cases optional)
+mail_server_username = 
+# Password to use to login to smtp server (in some cases optional)
+mail_server_password = 
+
+# Logging configuration. 
+[logging]
+# The number of log files to keep in a log dir
+nb_logfiles_tokeep = 10
+
+# Config to use for the logging. This config is in json, following the 
+# conventions as required by logging.dictConfig.
+# https://docs.python.org/3/library/logging.config.html#logging-config-dictschema 
+# 
+# Mind: the location for file logging 
+logconfig = {
+        "version": 1,
+        "disable_existing_loggers": true,
+        "formatters": {
+            "console": {
+                "format": "%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s", 
+                "datefmt": "%H:%M:%S"
+                },
+            "file": {
+                "format": "%(asctime)s|%(levelname)s|%(name)s|%(message)s", 
+                "datefmt": null
+            }
+        },
+        "handlers": {
+            "console": {
+                "level": "INFO",
+                "class": "logging.StreamHandler",
+                "formatter": "console",
+                "stream": "ext://sys.stdout"
+            },
+            "file": {
+                "level": "INFO",
+                "class": "logging.handlers.RotatingFileHandler",
+                "formatter": "file",
+                "filename": "_log/{iso_datetime}.log",
+                "maxBytes": 10000000,
+                "backupCount": 3
+            }
+        },
+        "loggers": {
+            "geofile_ops": {
+                "level": "INFO",
+                "handlers": ["console"],
+                "propagate": false
+            },
+            "geofile_ops.geofile_ops": {
+                "level": "DEBUG",
+                "handlers": ["console"],
+                "propagate": false
+            }        
+        },
+        "root": {
+            "level": "INFO",
+            "handlers": ["console", "file"]
+        }
     }
```

### Comparing `orthoseg-0.4.2/orthoseg/scriptrunner_defaults.ini` & `orthoseg-0.4.2a1/orthoseg/scriptrunner_defaults.ini`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# This config file contains the default settings for scriptrunner.
-#
-# The config used for scriptrunner project is loaded in the following order:
-#   1) the project defaults as "hardcoded" in scriptrunner (scriptrunner_defaults.ini)
-#   2) any config file specified when starting scriptrunner
-# 
-# Parameters specified in a config file loaded later in the order above
-# overrule the corresponding parameter values specified in a previously 
-# loaded config file.
-
-# General settings.
-[general]
-# The files in the script_dir that should be treated as scripts to be executed.
-script_patterns = *.bat, *.sh
-
-# Settings concerning the directories where input/output data is found/put.
-[dirs]
-# Remarks: 
-#   * UNC paths are not supported on Windows, always use mapped drive letters!
-#   * always use forward slashes, even on Windows systems
-
-# The scripts_dir, the folder to look for script to execute in. Can either be 
-#   * an absolute path 
-#   * OR a relative path starting from the location of a specified config file
-#   * OR the script_dir can be specified using the command line parameter. 
-#     This will override the setting in the config file(s)
-script_dir = ./
-
-# Log dir
-log_dir = ${script_dir}/log
-# Done dir
-done_dir = ${script_dir}/done
-# Error dir
-error_dir = ${script_dir}/error
-
-# Logging configuration. 
-[logging]
-# The number of log files to keep in a log dir
-nb_logfiles_tokeep = 10
-
-# Config to use for the logging. This config is in json, following the 
-# conventions as required by logging.dictConfig.
-# https://docs.python.org/3/library/logging.config.html#logging-config-dictschema 
-# 
-# Mind: the location for file logging 
-logconfig = {
-        "version": 1,
-        "disable_existing_loggers": true,
-        "formatters": {
-            "console": {
-                "format": "%(message)s", 
-                "datefmt": "%H:%M:%S"
-                },
-            "file": {
-                "format": "%(message)s", 
-                "datefmt": null
-            }
-        },
-        "handlers": {
-            "console": {
-                "level": "INFO",
-                "class": "logging.StreamHandler",
-                "formatter": "console",
-                "stream": "ext://sys.stdout"
-            },
-            "file": {
-                "level": "INFO",
-                "class": "logging.handlers.RotatingFileHandler",
-                "formatter": "file",
-                "filename": "log/{iso_datetime}.log",
-                "maxBytes": 10000000,
-                "backupCount": 3
-            }
-        },
-        "root": {
-            "level": "INFO",
-            "handlers": ["console", "file"]
-        }
+# This config file contains the default settings for scriptrunner.
+#
+# The config used for scriptrunner project is loaded in the following order:
+#   1) the project defaults as "hardcoded" in scriptrunner (scriptrunner_defaults.ini)
+#   2) any config file specified when starting scriptrunner
+# 
+# Parameters specified in a config file loaded later in the order above
+# overrule the corresponding parameter values specified in a previously 
+# loaded config file.
+
+# General settings.
+[general]
+# The files in the script_dir that should be treated as scripts to be executed.
+script_patterns = *.bat, *.sh
+
+# Settings concerning the directories where input/output data is found/put.
+[dirs]
+# Remarks: 
+#   * UNC paths are not supported on Windows, always use mapped drive letters!
+#   * always use forward slashes, even on Windows systems
+
+# The scripts_dir, the folder to look for script to execute in. Can either be 
+#   * an absolute path 
+#   * OR a relative path starting from the location of a specified config file
+#   * OR the script_dir can be specified using the command line parameter. 
+#     This will override the setting in the config file(s)
+script_dir = ./
+
+# Log dir
+log_dir = ${script_dir}/log
+# Done dir
+done_dir = ${script_dir}/done
+# Error dir
+error_dir = ${script_dir}/error
+
+# Logging configuration. 
+[logging]
+# The number of log files to keep in a log dir
+nb_logfiles_tokeep = 10
+
+# Config to use for the logging. This config is in json, following the 
+# conventions as required by logging.dictConfig.
+# https://docs.python.org/3/library/logging.config.html#logging-config-dictschema 
+# 
+# Mind: the location for file logging 
+logconfig = {
+        "version": 1,
+        "disable_existing_loggers": true,
+        "formatters": {
+            "console": {
+                "format": "%(message)s", 
+                "datefmt": "%H:%M:%S"
+                },
+            "file": {
+                "format": "%(message)s", 
+                "datefmt": null
+            }
+        },
+        "handlers": {
+            "console": {
+                "level": "INFO",
+                "class": "logging.StreamHandler",
+                "formatter": "console",
+                "stream": "ext://sys.stdout"
+            },
+            "file": {
+                "level": "INFO",
+                "class": "logging.handlers.RotatingFileHandler",
+                "formatter": "file",
+                "filename": "log/{iso_datetime}.log",
+                "maxBytes": 10000000,
+                "backupCount": 3
+            }
+        },
+        "root": {
+            "level": "INFO",
+            "handlers": ["console", "file"]
+        }
     }
```

### Comparing `orthoseg-0.4.2/orthoseg/train.py` & `orthoseg-0.4.2a1/orthoseg/train.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,568 +1,568 @@
-# -*- coding: utf-8 -*-
-"""
-Module to make it easy to start a training session.
-"""
-
-import argparse
-import gc
-import logging
-import os
-from pathlib import Path
-import re
-import shlex
-import sys
-import traceback
-from typing import List
-
-from tensorflow import keras as kr
-
-# orthoseg is higher in dir hierarchy, add root to sys.path
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import config_helper as conf
-from orthoseg.helpers import email_helper
-from orthoseg.lib import prepare_traindatasets as prep
-from orthoseg.lib import predicter
-from orthoseg.lib import trainer
-from orthoseg.model import model_factory as mf
-from orthoseg.model import model_helper as mh
-from orthoseg.util import log_util
-
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def _train_argstr(argstr):
-    args = shlex.split(argstr)
-    _train_args(args)
-
-
-def _train_args(args):
-
-    # Interprete arguments
-    parser = argparse.ArgumentParser(add_help=False)
-
-    # Required arguments
-    required = parser.add_argument_group("Required arguments")
-    required.add_argument(
-        "-c", "--config", type=str, required=True, help="The config file to use"
-    )
-
-    # Optional arguments
-    optional = parser.add_argument_group("Optional arguments")
-    # Add back help
-    optional.add_argument(
-        "-h",
-        "--help",
-        action="help",
-        default=argparse.SUPPRESS,
-        help="Show this help message and exit",
-    )
-
-    # Interprete arguments
-    args = parser.parse_args(args)
-
-    # Run!
-    train(config_path=Path(args.config))
-
-
-def train(config_path: Path):
-    """
-    Run a training session for the config specified.
-
-    Args:
-        config_path (Path): Path to the config file to use.
-    """
-    # Init
-    # Load the config and save in a bunch of global variables zo it
-    # is accessible everywhere
-    conf.read_orthoseg_config(config_path)
-
-    # Init logging
-    log_util.clean_log_dir(
-        log_dir=conf.dirs.getpath("log_dir"),
-        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
-    )
-    global logger
-    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
-
-    # Log start
-    logger.info(f"Start train for config {config_path.stem}")
-    logger.debug(f"Config used: \n{conf.pformat_config()}")
-
-    try:
-
-        # First check if the segment_subject has a valid name
-        segment_subject = conf.general["segment_subject"]
-        if segment_subject == "MUST_OVERRIDE":
-            raise Exception(
-                "segment_subject must be overridden in the subject specific config file"
-            )
-        elif "_" in segment_subject:
-            raise Exception(f"segment_subject cannot contain '_': {segment_subject}")
-
-        # Create the output dir's if they don't exist yet...
-        for dir in [
-            conf.dirs.getpath("project_dir"),
-            conf.dirs.getpath("training_dir"),
-        ]:
-            if dir and not dir.exists():
-                dir.mkdir()
-
-        # If the training data doesn't exist yet, create it
-        # Get the label input info
-        label_files_dict = conf.train.getdict("label_datasources", None)
-        label_infos = []
-        if label_files_dict is not None:
-            for label_file_key in label_files_dict:
-                label_file = label_files_dict[label_file_key]
-                # Add as LabelInfo objects to list
-                label_infos.append(
-                    prep.LabelInfo(
-                        locations_path=Path(label_file["locations_path"]),
-                        polygons_path=Path(label_file["data_path"]),
-                        image_layer=label_file["image_layer"],
-                    )
-                )
-            if label_infos is None or len(label_infos) == 0:
-                raise Exception(
-                    "label_datasources is defined in config but contains invalid info!"
-                )
-        else:
-            # Search for the files based on the file name patterns...
-            labelpolygons_pattern = conf.train.getpath("labelpolygons_pattern")
-            labellocations_pattern = conf.train.getpath("labellocations_pattern")
-            label_infos = _search_label_files(
-                labelpolygons_pattern, labellocations_pattern
-            )
-            if label_infos is None or len(label_infos) == 0:
-                raise Exception(
-                    f"No label files found with patterns {labellocations_pattern} and "
-                    f"{labelpolygons_pattern}"
-                )
-
-        # Determine the projection of (the first) train layer... it will be used for all
-        train_image_layer = label_infos[0].image_layer
-        train_projection = conf.image_layers[train_image_layer]["projection"]
-
-        # Determine classes
-        try:
-            classes = conf.train.getdict("classes")
-
-            # If the burn_value property isn't supplied for the classes, add them
-            for class_id, (classname) in enumerate(classes):
-                if "burn_value" not in classes[classname]:
-                    classes[classname]["burn_value"] = class_id
-        except Exception as ex:
-            raise Exception(
-                f"Error reading classes: {conf.train.get('classes')}"
-            ) from ex
-
-        # Now create the train datasets (train, validation, test)
-        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
-        if force_model_traindata_id > -1:
-            training_dir = (
-                conf.dirs.getpath("training_dir") / f"{force_model_traindata_id:02d}"
-            )
-            traindata_id = force_model_traindata_id
-        else:
-            logger.info("Prepare train, validation and test data")
-            training_dir, traindata_id = prep.prepare_traindatasets(
-                label_infos=label_infos,
-                classes=classes,
-                image_layers=conf.image_layers,
-                training_dir=conf.dirs.getpath("training_dir"),
-                labelname_column=conf.train.get("labelname_column"),
-                image_pixel_x_size=conf.train.getfloat("image_pixel_x_size"),
-                image_pixel_y_size=conf.train.getfloat("image_pixel_y_size"),
-                image_pixel_width=conf.train.getint("image_pixel_width"),
-                image_pixel_height=conf.train.getint("image_pixel_height"),
-                ssl_verify=conf.general["ssl_verify"],
-            )
-
-        # Send mail that we are starting train
-        email_helper.sendmail(f"Start train for config {config_path.stem}")
-        logger.info(
-            f"Traindata dir to use is {training_dir}, with traindata_id: {traindata_id}"
-        )
-        traindata_dir = training_dir / "train"
-        validationdata_dir = training_dir / "validation"
-        testdata_dir = training_dir / "test"
-
-        # Check if training is needed
-        # Get hyper parameters from the config
-        # TODO: activation_function should probably not be specified!!!!!!
-        architectureparams = mh.ArchitectureParams(
-            architecture=conf.model["architecture"],
-            classes=[classname for classname in classes],
-            nb_channels=conf.model.getint("nb_channels"),
-            architecture_id=conf.model.getint("architecture_id"),
-            activation_function="softmax",
-        )
-        trainparams = mh.TrainParams(
-            trainparams_id=conf.train.getint("trainparams_id"),
-            image_augmentations=conf.train.getdict("image_augmentations"),
-            mask_augmentations=conf.train.getdict("mask_augmentations"),
-            class_weights=[classes[classname]["weight"] for classname in classes],
-            batch_size=conf.train.getint("batch_size_fit"),
-            optimizer=conf.train.get("optimizer"),
-            optimizer_params=conf.train.getdict("optimizer_params"),
-            loss_function=conf.train.get("loss_function"),
-            monitor_metric=conf.train.get("monitor_metric"),
-            monitor_metric_mode=conf.train.get("monitor_metric_mode"),
-            save_format=conf.train.get("save_format"),
-            save_best_only=conf.train.getboolean("save_best_only"),
-            save_min_accuracy=conf.train.getfloat("save_min_accuracy"),
-            nb_epoch=conf.train.getint("max_epoch"),
-            nb_epoch_with_freeze=conf.train.getint("nb_epoch_with_freeze"),
-            earlystop_patience=conf.train.getint("earlystop_patience"),
-            earlystop_monitor_metric=conf.train.get("earlystop_monitor_metric"),
-            earlystop_monitor_metric_mode=conf.train.get(
-                "earlystop_monitor_metric_mode"
-            ),
-            log_tensorboard=conf.train.getboolean("log_tensorboard"),
-            log_csv=conf.train.getboolean("log_csv"),
-        )
-
-        # Check if there exists already a model for this train dataset + hyperparameters
-        model_dir = conf.dirs.getpath("model_dir")
-        segment_subject = conf.general["segment_subject"]
-        best_model_curr_train_version = mh.get_best_model(
-            model_dir=model_dir,
-            segment_subject=segment_subject,
-            traindata_id=traindata_id,
-            architecture_id=architectureparams.architecture_id,
-            trainparams_id=trainparams.trainparams_id,
-        )
-
-        # Determine if training is needed,...
-        resume_train = conf.train.getboolean("resume_train")
-        if resume_train is False:
-            # If no (best) model found, training needed!
-            if best_model_curr_train_version is None:
-                train_needed = True
-            elif conf.train.getboolean("force_train") is True:
-                train_needed = True
-            else:
-                logger.info(
-                    "JUST PREDICT, no training: resume_train is false + model found"
-                )
-                train_needed = False
-        else:
-            # We want to preload an existing model and models were found
-            if best_model_curr_train_version is not None:
-                logger.info(
-                    "PRELOAD model + continue TRAINING: "
-                    f"{best_model_curr_train_version['filename']}"
-                )
-                train_needed = True
-            else:
-                message = "STOP: preload_existing_model is true but no model was found!"
-                logger.error(message)
-                raise Exception(message)
-
-        # Train!!!
-        min_probability = conf.predict.getfloat("min_probability")
-        if train_needed is True:
-
-            # If a model already exists, use it to predict (possibly new) training and
-            # validation dataset. This way it is possible to have a quick check on
-            # errors in (new) added labels in the datasets.
-
-            # Get the current best model that already exists for this subject
-            best_recent_model = mh.get_best_model(
-                model_dir=model_dir,
-                segment_subject=segment_subject,
-                architecture_id=architectureparams.architecture_id,
-                trainparams_id=trainparams.trainparams_id,
-            )
-            if best_recent_model is not None:
-                try:
-                    # TODO: move the hyperparams filename formatting to get_models...
-                    logger.info(
-                        f"Load model + weights from {best_recent_model['filepath']}"
-                    )
-                    best_model = mf.load_model(
-                        best_recent_model["filepath"], compile=False
-                    )
-                    best_hyperparams_path = (
-                        best_recent_model["filepath"].parent
-                        / f"{best_recent_model['basefilename']}_hyperparams.json"
-                    )
-                    best_hyperparams = mh.HyperParams(path=best_hyperparams_path)
-                    logger.info("Loaded model, weights and params")
-
-                    # Prepare output subdir to be used for predictions
-                    predict_out_subdir, _ = os.path.splitext(
-                        best_recent_model["filename"]
-                    )
-
-                    # Predict training dataset
-                    predicter.predict_dir(
-                        model=best_model,
-                        input_image_dir=traindata_dir / "image",
-                        output_image_dir=traindata_dir / predict_out_subdir,
-                        output_vector_path=None,
-                        projection_if_missing=train_projection,
-                        input_mask_dir=traindata_dir / "mask",
-                        batch_size=conf.train.getint("batch_size_predict"),
-                        evaluate_mode=True,
-                        classes=best_hyperparams.architecture.classes,
-                        min_probability=min_probability,
-                        cancel_filepath=conf.files.getpath("cancel_filepath"),
-                        max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-                    )
-
-                    # Predict validation dataset
-                    predicter.predict_dir(
-                        model=best_model,
-                        input_image_dir=validationdata_dir / "image",
-                        output_image_dir=validationdata_dir / predict_out_subdir,
-                        output_vector_path=None,
-                        projection_if_missing=train_projection,
-                        input_mask_dir=validationdata_dir / "mask",
-                        batch_size=conf.train.getint("batch_size_predict"),
-                        evaluate_mode=True,
-                        classes=best_hyperparams.architecture.classes,
-                        min_probability=min_probability,
-                        cancel_filepath=conf.files.getpath("cancel_filepath"),
-                        max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-                    )
-                    del best_model
-                except Exception as ex:
-                    logger.warn(f"Exception trying to predict with old model: {ex}")
-
-            # Now we can really start training
-            logger.info("Start training")
-            model_preload_filepath = None
-            if best_model_curr_train_version is not None:
-                model_preload_filepath = best_model_curr_train_version["filepath"]
-            elif conf.train.getboolean("preload_with_previous_traindata"):
-                best_model_for_architecture = mh.get_best_model(
-                    model_dir=model_dir, segment_subject=segment_subject
-                )
-                if best_model_for_architecture is not None:
-                    model_preload_filepath = best_model_for_architecture["filepath"]
-
-            # Combine all hyperparameters in hyperparams object
-            hyperparams = mh.HyperParams(
-                architecture=architectureparams, train=trainparams
-            )
-
-            trainer.train(
-                traindata_dir=traindata_dir,
-                validationdata_dir=validationdata_dir,
-                model_save_dir=model_dir,
-                segment_subject=segment_subject,
-                traindata_id=traindata_id,
-                hyperparams=hyperparams,
-                model_preload_filepath=model_preload_filepath,
-                image_width=conf.train.getint("image_pixel_width"),
-                image_height=conf.train.getint("image_pixel_height"),
-                save_augmented_subdir=conf.train.get("save_augmented_subdir"),
-            )
-
-            # Now get the best model found during training
-            best_model_curr_train_version = mh.get_best_model(
-                model_dir=model_dir,
-                segment_subject=segment_subject,
-                traindata_id=traindata_id,
-            )
-
-        # Assert to evade typing warnings
-        assert best_model_curr_train_version is not None
-
-        # Now predict on the train,... data
-        logger.info(
-            "PREDICT test data with best model: "
-            f"{best_model_curr_train_version['filename']}"
-        )
-
-        # Load prediction model...
-        logger.info(
-            f"Load model + weights from {best_model_curr_train_version['filepath']}"
-        )
-        model = mf.load_model(best_model_curr_train_version["filepath"], compile=False)
-        logger.info("Loaded model + weights")
-
-        # Prepare output subdir to be used for predictions
-        predict_out_subdir, _ = os.path.splitext(
-            best_model_curr_train_version["filename"]
-        )
-
-        # Predict training dataset
-        predicter.predict_dir(
-            model=model,
-            input_image_dir=traindata_dir / "image",
-            output_image_dir=traindata_dir / predict_out_subdir,
-            output_vector_path=None,
-            projection_if_missing=train_projection,
-            input_mask_dir=traindata_dir / "mask",
-            batch_size=conf.train.getint("batch_size_predict"),
-            evaluate_mode=True,
-            classes=classes,
-            min_probability=min_probability,
-            cancel_filepath=conf.files.getpath("cancel_filepath"),
-            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-        )
-
-        # Predict validation dataset
-        predicter.predict_dir(
-            model=model,
-            input_image_dir=validationdata_dir / "image",
-            output_image_dir=validationdata_dir / predict_out_subdir,
-            output_vector_path=None,
-            projection_if_missing=train_projection,
-            input_mask_dir=validationdata_dir / "mask",
-            batch_size=conf.train.getint("batch_size_predict"),
-            evaluate_mode=True,
-            classes=classes,
-            min_probability=min_probability,
-            cancel_filepath=conf.files.getpath("cancel_filepath"),
-            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-        )
-
-        # Predict test dataset, if it exists
-        if testdata_dir is not None and testdata_dir.exists():
-            predicter.predict_dir(
-                model=model,
-                input_image_dir=testdata_dir / "image",
-                output_image_dir=testdata_dir / predict_out_subdir,
-                output_vector_path=None,
-                projection_if_missing=train_projection,
-                input_mask_dir=testdata_dir / "mask",
-                batch_size=conf.train.getint("batch_size_predict"),
-                evaluate_mode=True,
-                classes=classes,
-                min_probability=min_probability,
-                cancel_filepath=conf.files.getpath("cancel_filepath"),
-                max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-            )
-
-        # Predict extra test dataset with random images in the roi, to add to
-        # train and/or validation dataset if inaccuracies are found
-        # -> this is very useful to find false positives to improve the datasets
-        if conf.dirs.getpath("predictsample_image_input_dir").exists():
-            predicter.predict_dir(
-                model=model,
-                input_image_dir=conf.dirs.getpath("predictsample_image_input_dir"),
-                output_image_dir=conf.dirs.getpath("predictsample_image_output_basedir")
-                / predict_out_subdir,
-                output_vector_path=None,
-                projection_if_missing=train_projection,
-                batch_size=conf.train.getint("batch_size_predict"),
-                evaluate_mode=True,
-                classes=classes,
-                min_probability=min_probability,
-                cancel_filepath=conf.files.getpath("cancel_filepath"),
-                max_prediction_errors=conf.predict.getint("max_prediction_errors"),
-            )
-
-        # Free resources...
-        logger.debug("Free resources")
-        if model is not None:
-            del model
-        kr.backend.clear_session()
-        gc.collect()
-
-        # Log and send mail
-        message = f"Completed train for config {config_path.stem}"
-        logger.info(message)
-        email_helper.sendmail(message)
-    except Exception as ex:
-        message = f"ERROR while running train for task {config_path.stem}"
-        logger.exception(message)
-        if isinstance(ex, prep.ValidationError):
-            message_body = f"Validation error: {ex.to_html()}"
-        else:
-            message_body = f"Exception: {ex}<br/><br/>{traceback.format_exc()}"
-        email_helper.sendmail(subject=message, body=message_body)
-        raise Exception(message) from ex
-
-
-def _search_label_files(
-    labelpolygons_pattern: Path, labellocations_pattern: Path
-) -> List[prep.LabelInfo]:
-    label_infos = []
-
-    labelpolygons_pattern_searchpath = Path(
-        str(labelpolygons_pattern).format(image_layer="*")
-    )
-    labelpolygons_paths = list(
-        labelpolygons_pattern_searchpath.parent.glob(
-            labelpolygons_pattern_searchpath.name
-        )
-    )
-    labellocations_pattern_searchpath = Path(
-        str(labellocations_pattern).format(image_layer="*")
-    )
-    labellocations_paths = list(
-        labellocations_pattern_searchpath.parent.glob(
-            labellocations_pattern_searchpath.name
-        )
-    )
-
-    # Loop through all labellocation files
-    for labellocations_path in labellocations_paths:
-        tokens = _unformat(labellocations_path.stem, labellocations_pattern.stem)
-        if "image_layer" not in tokens:
-            raise Exception(
-                f"image_layer token not found in {labellocations_path} using pattern "
-                f"{labellocations_pattern}"
-            )
-        image_layer = tokens["image_layer"]
-
-        # Look for the matching (= same image_layer) data file
-        found = False
-        for labelpolygons_path in labelpolygons_paths:
-            tokens = _unformat(labelpolygons_path.stem, labelpolygons_pattern.stem)
-            if "image_layer" not in tokens:
-                raise Exception(
-                    f"image_layer token not found in {labelpolygons_path} using "
-                    f"pattern {labelpolygons_pattern}"
-                )
-
-            if tokens["image_layer"] == image_layer:
-                found = True
-                label_infos.append(
-                    prep.LabelInfo(
-                        locations_path=labellocations_path,
-                        polygons_path=labelpolygons_path,
-                        image_layer=image_layer,
-                    )
-                )
-        if found is False:
-            raise Exception(f"No matching data file found for {labellocations_path}")
-
-    return label_infos
-
-
-def _unformat(string: str, pattern: str) -> dict:
-    regex = re.sub(r"{(.+?)}", r"(?P<_\1>.+)", pattern)
-    regex_result = re.search(regex, string)
-    if regex_result is not None:
-        values = list(regex_result.groups())
-        keys = re.findall(r"{(.+?)}", pattern)
-        _dict = dict(zip(keys, values))
-        return _dict
-    else:
-        raise Exception(f"Error: pattern {pattern} not found in {string}")
-
-
-def main():
-    try:
-        _train_args(sys.argv[1:])
-    except Exception as ex:
-        logger.exception(f"Error: {ex}")
-        raise
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""
+Module to make it easy to start a training session.
+"""
+
+import argparse
+import gc
+import logging
+import os
+from pathlib import Path
+import re
+import shlex
+import sys
+import traceback
+from typing import List
+
+from tensorflow import keras as kr
+
+# orthoseg is higher in dir hierarchy, add root to sys.path
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import config_helper as conf
+from orthoseg.helpers import email_helper
+from orthoseg.lib import prepare_traindatasets as prep
+from orthoseg.lib import predicter
+from orthoseg.lib import trainer
+from orthoseg.model import model_factory as mf
+from orthoseg.model import model_helper as mh
+from orthoseg.util import log_util
+
+# -------------------------------------------------------------
+# First define/init general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def _train_argstr(argstr):
+    args = shlex.split(argstr)
+    _train_args(args)
+
+
+def _train_args(args):
+
+    # Interprete arguments
+    parser = argparse.ArgumentParser(add_help=False)
+
+    # Required arguments
+    required = parser.add_argument_group("Required arguments")
+    required.add_argument(
+        "-c", "--config", type=str, required=True, help="The config file to use"
+    )
+
+    # Optional arguments
+    optional = parser.add_argument_group("Optional arguments")
+    # Add back help
+    optional.add_argument(
+        "-h",
+        "--help",
+        action="help",
+        default=argparse.SUPPRESS,
+        help="Show this help message and exit",
+    )
+
+    # Interprete arguments
+    args = parser.parse_args(args)
+
+    # Run!
+    train(config_path=Path(args.config))
+
+
+def train(config_path: Path):
+    """
+    Run a training session for the config specified.
+
+    Args:
+        config_path (Path): Path to the config file to use.
+    """
+    # Init
+    # Load the config and save in a bunch of global variables zo it
+    # is accessible everywhere
+    conf.read_orthoseg_config(config_path)
+
+    # Init logging
+    log_util.clean_log_dir(
+        log_dir=conf.dirs.getpath("log_dir"),
+        nb_logfiles_tokeep=conf.logging.getint("nb_logfiles_tokeep"),
+    )
+    global logger
+    logger = log_util.main_log_init(conf.dirs.getpath("log_dir"), __name__)
+
+    # Log start
+    logger.info(f"Start train for config {config_path.stem}")
+    logger.debug(f"Config used: \n{conf.pformat_config()}")
+
+    try:
+
+        # First check if the segment_subject has a valid name
+        segment_subject = conf.general["segment_subject"]
+        if segment_subject == "MUST_OVERRIDE":
+            raise Exception(
+                "segment_subject must be overridden in the subject specific config file"
+            )
+        elif "_" in segment_subject:
+            raise Exception(f"segment_subject cannot contain '_': {segment_subject}")
+
+        # Create the output dir's if they don't exist yet...
+        for dir in [
+            conf.dirs.getpath("project_dir"),
+            conf.dirs.getpath("training_dir"),
+        ]:
+            if dir and not dir.exists():
+                dir.mkdir()
+
+        # If the training data doesn't exist yet, create it
+        # Get the label input info
+        label_files_dict = conf.train.getdict("label_datasources", None)
+        label_infos = []
+        if label_files_dict is not None:
+            for label_file_key in label_files_dict:
+                label_file = label_files_dict[label_file_key]
+                # Add as LabelInfo objects to list
+                label_infos.append(
+                    prep.LabelInfo(
+                        locations_path=Path(label_file["locations_path"]),
+                        polygons_path=Path(label_file["data_path"]),
+                        image_layer=label_file["image_layer"],
+                    )
+                )
+            if label_infos is None or len(label_infos) == 0:
+                raise Exception(
+                    "label_datasources is defined in config but contains invalid info!"
+                )
+        else:
+            # Search for the files based on the file name patterns...
+            labelpolygons_pattern = conf.train.getpath("labelpolygons_pattern")
+            labellocations_pattern = conf.train.getpath("labellocations_pattern")
+            label_infos = _search_label_files(
+                labelpolygons_pattern, labellocations_pattern
+            )
+            if label_infos is None or len(label_infos) == 0:
+                raise Exception(
+                    f"No label files found with patterns {labellocations_pattern} and "
+                    f"{labelpolygons_pattern}"
+                )
+
+        # Determine the projection of (the first) train layer... it will be used for all
+        train_image_layer = label_infos[0].image_layer
+        train_projection = conf.image_layers[train_image_layer]["projection"]
+
+        # Determine classes
+        try:
+            classes = conf.train.getdict("classes")
+
+            # If the burn_value property isn't supplied for the classes, add them
+            for class_id, (classname) in enumerate(classes):
+                if "burn_value" not in classes[classname]:
+                    classes[classname]["burn_value"] = class_id
+        except Exception as ex:
+            raise Exception(
+                f"Error reading classes: {conf.train.get('classes')}"
+            ) from ex
+
+        # Now create the train datasets (train, validation, test)
+        force_model_traindata_id = conf.train.getint("force_model_traindata_id")
+        if force_model_traindata_id > -1:
+            training_dir = (
+                conf.dirs.getpath("training_dir") / f"{force_model_traindata_id:02d}"
+            )
+            traindata_id = force_model_traindata_id
+        else:
+            logger.info("Prepare train, validation and test data")
+            training_dir, traindata_id = prep.prepare_traindatasets(
+                label_infos=label_infos,
+                classes=classes,
+                image_layers=conf.image_layers,
+                training_dir=conf.dirs.getpath("training_dir"),
+                labelname_column=conf.train.get("labelname_column"),
+                image_pixel_x_size=conf.train.getfloat("image_pixel_x_size"),
+                image_pixel_y_size=conf.train.getfloat("image_pixel_y_size"),
+                image_pixel_width=conf.train.getint("image_pixel_width"),
+                image_pixel_height=conf.train.getint("image_pixel_height"),
+                ssl_verify=conf.general["ssl_verify"],
+            )
+
+        # Send mail that we are starting train
+        email_helper.sendmail(f"Start train for config {config_path.stem}")
+        logger.info(
+            f"Traindata dir to use is {training_dir}, with traindata_id: {traindata_id}"
+        )
+        traindata_dir = training_dir / "train"
+        validationdata_dir = training_dir / "validation"
+        testdata_dir = training_dir / "test"
+
+        # Check if training is needed
+        # Get hyper parameters from the config
+        # TODO: activation_function should probably not be specified!!!!!!
+        architectureparams = mh.ArchitectureParams(
+            architecture=conf.model["architecture"],
+            classes=[classname for classname in classes],
+            nb_channels=conf.model.getint("nb_channels"),
+            architecture_id=conf.model.getint("architecture_id"),
+            activation_function="softmax",
+        )
+        trainparams = mh.TrainParams(
+            trainparams_id=conf.train.getint("trainparams_id"),
+            image_augmentations=conf.train.getdict("image_augmentations"),
+            mask_augmentations=conf.train.getdict("mask_augmentations"),
+            class_weights=[classes[classname]["weight"] for classname in classes],
+            batch_size=conf.train.getint("batch_size_fit"),
+            optimizer=conf.train.get("optimizer"),
+            optimizer_params=conf.train.getdict("optimizer_params"),
+            loss_function=conf.train.get("loss_function"),
+            monitor_metric=conf.train.get("monitor_metric"),
+            monitor_metric_mode=conf.train.get("monitor_metric_mode"),
+            save_format=conf.train.get("save_format"),
+            save_best_only=conf.train.getboolean("save_best_only"),
+            save_min_accuracy=conf.train.getfloat("save_min_accuracy"),
+            nb_epoch=conf.train.getint("max_epoch"),
+            nb_epoch_with_freeze=conf.train.getint("nb_epoch_with_freeze"),
+            earlystop_patience=conf.train.getint("earlystop_patience"),
+            earlystop_monitor_metric=conf.train.get("earlystop_monitor_metric"),
+            earlystop_monitor_metric_mode=conf.train.get(
+                "earlystop_monitor_metric_mode"
+            ),
+            log_tensorboard=conf.train.getboolean("log_tensorboard"),
+            log_csv=conf.train.getboolean("log_csv"),
+        )
+
+        # Check if there exists already a model for this train dataset + hyperparameters
+        model_dir = conf.dirs.getpath("model_dir")
+        segment_subject = conf.general["segment_subject"]
+        best_model_curr_train_version = mh.get_best_model(
+            model_dir=model_dir,
+            segment_subject=segment_subject,
+            traindata_id=traindata_id,
+            architecture_id=architectureparams.architecture_id,
+            trainparams_id=trainparams.trainparams_id,
+        )
+
+        # Determine if training is needed,...
+        resume_train = conf.train.getboolean("resume_train")
+        if resume_train is False:
+            # If no (best) model found, training needed!
+            if best_model_curr_train_version is None:
+                train_needed = True
+            elif conf.train.getboolean("force_train") is True:
+                train_needed = True
+            else:
+                logger.info(
+                    "JUST PREDICT, no training: resume_train is false + model found"
+                )
+                train_needed = False
+        else:
+            # We want to preload an existing model and models were found
+            if best_model_curr_train_version is not None:
+                logger.info(
+                    "PRELOAD model + continue TRAINING: "
+                    f"{best_model_curr_train_version['filename']}"
+                )
+                train_needed = True
+            else:
+                message = "STOP: preload_existing_model is true but no model was found!"
+                logger.error(message)
+                raise Exception(message)
+
+        # Train!!!
+        min_probability = conf.predict.getfloat("min_probability")
+        if train_needed is True:
+
+            # If a model already exists, use it to predict (possibly new) training and
+            # validation dataset. This way it is possible to have a quick check on
+            # errors in (new) added labels in the datasets.
+
+            # Get the current best model that already exists for this subject
+            best_recent_model = mh.get_best_model(
+                model_dir=model_dir,
+                segment_subject=segment_subject,
+                architecture_id=architectureparams.architecture_id,
+                trainparams_id=trainparams.trainparams_id,
+            )
+            if best_recent_model is not None:
+                try:
+                    # TODO: move the hyperparams filename formatting to get_models...
+                    logger.info(
+                        f"Load model + weights from {best_recent_model['filepath']}"
+                    )
+                    best_model = mf.load_model(
+                        best_recent_model["filepath"], compile=False
+                    )
+                    best_hyperparams_path = (
+                        best_recent_model["filepath"].parent
+                        / f"{best_recent_model['basefilename']}_hyperparams.json"
+                    )
+                    best_hyperparams = mh.HyperParams(path=best_hyperparams_path)
+                    logger.info("Loaded model, weights and params")
+
+                    # Prepare output subdir to be used for predictions
+                    predict_out_subdir, _ = os.path.splitext(
+                        best_recent_model["filename"]
+                    )
+
+                    # Predict training dataset
+                    predicter.predict_dir(
+                        model=best_model,
+                        input_image_dir=traindata_dir / "image",
+                        output_image_dir=traindata_dir / predict_out_subdir,
+                        output_vector_path=None,
+                        projection_if_missing=train_projection,
+                        input_mask_dir=traindata_dir / "mask",
+                        batch_size=conf.train.getint("batch_size_predict"),
+                        evaluate_mode=True,
+                        classes=best_hyperparams.architecture.classes,
+                        min_probability=min_probability,
+                        cancel_filepath=conf.files.getpath("cancel_filepath"),
+                        max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+                    )
+
+                    # Predict validation dataset
+                    predicter.predict_dir(
+                        model=best_model,
+                        input_image_dir=validationdata_dir / "image",
+                        output_image_dir=validationdata_dir / predict_out_subdir,
+                        output_vector_path=None,
+                        projection_if_missing=train_projection,
+                        input_mask_dir=validationdata_dir / "mask",
+                        batch_size=conf.train.getint("batch_size_predict"),
+                        evaluate_mode=True,
+                        classes=best_hyperparams.architecture.classes,
+                        min_probability=min_probability,
+                        cancel_filepath=conf.files.getpath("cancel_filepath"),
+                        max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+                    )
+                    del best_model
+                except Exception as ex:
+                    logger.warn(f"Exception trying to predict with old model: {ex}")
+
+            # Now we can really start training
+            logger.info("Start training")
+            model_preload_filepath = None
+            if best_model_curr_train_version is not None:
+                model_preload_filepath = best_model_curr_train_version["filepath"]
+            elif conf.train.getboolean("preload_with_previous_traindata"):
+                best_model_for_architecture = mh.get_best_model(
+                    model_dir=model_dir, segment_subject=segment_subject
+                )
+                if best_model_for_architecture is not None:
+                    model_preload_filepath = best_model_for_architecture["filepath"]
+
+            # Combine all hyperparameters in hyperparams object
+            hyperparams = mh.HyperParams(
+                architecture=architectureparams, train=trainparams
+            )
+
+            trainer.train(
+                traindata_dir=traindata_dir,
+                validationdata_dir=validationdata_dir,
+                model_save_dir=model_dir,
+                segment_subject=segment_subject,
+                traindata_id=traindata_id,
+                hyperparams=hyperparams,
+                model_preload_filepath=model_preload_filepath,
+                image_width=conf.train.getint("image_pixel_width"),
+                image_height=conf.train.getint("image_pixel_height"),
+                save_augmented_subdir=conf.train.get("save_augmented_subdir"),
+            )
+
+            # Now get the best model found during training
+            best_model_curr_train_version = mh.get_best_model(
+                model_dir=model_dir,
+                segment_subject=segment_subject,
+                traindata_id=traindata_id,
+            )
+
+        # Assert to evade typing warnings
+        assert best_model_curr_train_version is not None
+
+        # Now predict on the train,... data
+        logger.info(
+            "PREDICT test data with best model: "
+            f"{best_model_curr_train_version['filename']}"
+        )
+
+        # Load prediction model...
+        logger.info(
+            f"Load model + weights from {best_model_curr_train_version['filepath']}"
+        )
+        model = mf.load_model(best_model_curr_train_version["filepath"], compile=False)
+        logger.info("Loaded model + weights")
+
+        # Prepare output subdir to be used for predictions
+        predict_out_subdir, _ = os.path.splitext(
+            best_model_curr_train_version["filename"]
+        )
+
+        # Predict training dataset
+        predicter.predict_dir(
+            model=model,
+            input_image_dir=traindata_dir / "image",
+            output_image_dir=traindata_dir / predict_out_subdir,
+            output_vector_path=None,
+            projection_if_missing=train_projection,
+            input_mask_dir=traindata_dir / "mask",
+            batch_size=conf.train.getint("batch_size_predict"),
+            evaluate_mode=True,
+            classes=classes,
+            min_probability=min_probability,
+            cancel_filepath=conf.files.getpath("cancel_filepath"),
+            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+        )
+
+        # Predict validation dataset
+        predicter.predict_dir(
+            model=model,
+            input_image_dir=validationdata_dir / "image",
+            output_image_dir=validationdata_dir / predict_out_subdir,
+            output_vector_path=None,
+            projection_if_missing=train_projection,
+            input_mask_dir=validationdata_dir / "mask",
+            batch_size=conf.train.getint("batch_size_predict"),
+            evaluate_mode=True,
+            classes=classes,
+            min_probability=min_probability,
+            cancel_filepath=conf.files.getpath("cancel_filepath"),
+            max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+        )
+
+        # Predict test dataset, if it exists
+        if testdata_dir is not None and testdata_dir.exists():
+            predicter.predict_dir(
+                model=model,
+                input_image_dir=testdata_dir / "image",
+                output_image_dir=testdata_dir / predict_out_subdir,
+                output_vector_path=None,
+                projection_if_missing=train_projection,
+                input_mask_dir=testdata_dir / "mask",
+                batch_size=conf.train.getint("batch_size_predict"),
+                evaluate_mode=True,
+                classes=classes,
+                min_probability=min_probability,
+                cancel_filepath=conf.files.getpath("cancel_filepath"),
+                max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+            )
+
+        # Predict extra test dataset with random images in the roi, to add to
+        # train and/or validation dataset if inaccuracies are found
+        # -> this is very useful to find false positives to improve the datasets
+        if conf.dirs.getpath("predictsample_image_input_dir").exists():
+            predicter.predict_dir(
+                model=model,
+                input_image_dir=conf.dirs.getpath("predictsample_image_input_dir"),
+                output_image_dir=conf.dirs.getpath("predictsample_image_output_basedir")
+                / predict_out_subdir,
+                output_vector_path=None,
+                projection_if_missing=train_projection,
+                batch_size=conf.train.getint("batch_size_predict"),
+                evaluate_mode=True,
+                classes=classes,
+                min_probability=min_probability,
+                cancel_filepath=conf.files.getpath("cancel_filepath"),
+                max_prediction_errors=conf.predict.getint("max_prediction_errors"),
+            )
+
+        # Free resources...
+        logger.debug("Free resources")
+        if model is not None:
+            del model
+        kr.backend.clear_session()
+        gc.collect()
+
+        # Log and send mail
+        message = f"Completed train for config {config_path.stem}"
+        logger.info(message)
+        email_helper.sendmail(message)
+    except Exception as ex:
+        message = f"ERROR while running train for task {config_path.stem}"
+        logger.exception(message)
+        if isinstance(ex, prep.ValidationError):
+            message_body = f"Validation error: {ex.to_html()}"
+        else:
+            message_body = f"Exception: {ex}<br/><br/>{traceback.format_exc()}"
+        email_helper.sendmail(subject=message, body=message_body)
+        raise Exception(message) from ex
+
+
+def _search_label_files(
+    labelpolygons_pattern: Path, labellocations_pattern: Path
+) -> List[prep.LabelInfo]:
+    label_infos = []
+
+    labelpolygons_pattern_searchpath = Path(
+        str(labelpolygons_pattern).format(image_layer="*")
+    )
+    labelpolygons_paths = list(
+        labelpolygons_pattern_searchpath.parent.glob(
+            labelpolygons_pattern_searchpath.name
+        )
+    )
+    labellocations_pattern_searchpath = Path(
+        str(labellocations_pattern).format(image_layer="*")
+    )
+    labellocations_paths = list(
+        labellocations_pattern_searchpath.parent.glob(
+            labellocations_pattern_searchpath.name
+        )
+    )
+
+    # Loop through all labellocation files
+    for labellocations_path in labellocations_paths:
+        tokens = _unformat(labellocations_path.stem, labellocations_pattern.stem)
+        if "image_layer" not in tokens:
+            raise Exception(
+                f"image_layer token not found in {labellocations_path} using pattern "
+                f"{labellocations_pattern}"
+            )
+        image_layer = tokens["image_layer"]
+
+        # Look for the matching (= same image_layer) data file
+        found = False
+        for labelpolygons_path in labelpolygons_paths:
+            tokens = _unformat(labelpolygons_path.stem, labelpolygons_pattern.stem)
+            if "image_layer" not in tokens:
+                raise Exception(
+                    f"image_layer token not found in {labelpolygons_path} using "
+                    f"pattern {labelpolygons_pattern}"
+                )
+
+            if tokens["image_layer"] == image_layer:
+                found = True
+                label_infos.append(
+                    prep.LabelInfo(
+                        locations_path=labellocations_path,
+                        polygons_path=labelpolygons_path,
+                        image_layer=image_layer,
+                    )
+                )
+        if found is False:
+            raise Exception(f"No matching data file found for {labellocations_path}")
+
+    return label_infos
+
+
+def _unformat(string: str, pattern: str) -> dict:
+    regex = re.sub(r"{(.+?)}", r"(?P<_\1>.+)", pattern)
+    regex_result = re.search(regex, string)
+    if regex_result is not None:
+        values = list(regex_result.groups())
+        keys = re.findall(r"{(.+?)}", pattern)
+        _dict = dict(zip(keys, values))
+        return _dict
+    else:
+        raise Exception(f"Error: pattern {pattern} not found in {string}")
+
+
+def main():
+    try:
+        _train_args(sys.argv[1:])
+    except Exception as ex:
+        logger.exception(f"Error: {ex}")
+        raise
+
+
+# If the script is ran directly...
+if __name__ == "__main__":
+    main()
```

### Comparing `orthoseg-0.4.2/orthoseg/util/general_util.py` & `orthoseg-0.4.2a1/orthoseg/util/general_util.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# -*- coding: utf-8 -*-
-"""
-Module containing some general utilities.
-"""
-
-import datetime
-import logging
-import os
-from typing import Optional
-
-import psutil
-
-################################################################################
-# Some init
-################################################################################
-
-logger = logging.getLogger(__name__)
-
-
-class MissingRuntimeDependencyError(Exception):
-    """
-    Exception raised when an unsupported SQL statement is passed.
-
-    Attributes:
-        message (str): Exception message
-    """
-
-    def __init__(self, message):
-        self.message = message
-        super().__init__(self.message)
-
-
-################################################################################
-# The real work
-################################################################################
-
-
-def report_progress(
-    start_time: datetime.datetime,
-    nb_done: int,
-    nb_todo: int,
-    operation: Optional[str] = None,
-    nb_parallel: int = 1,
-):
-    # Init
-    time_passed = (datetime.datetime.now() - start_time).total_seconds()
-    pct_progress = 100.0 - (nb_todo - nb_done) * 100 / nb_todo
-
-    # If we haven't really started yet, don't report time estimate yet
-    if nb_done == 0:
-        message = (
-            f"\r  ?: ? left to do {operation} on {(nb_todo-nb_done):8d} "
-            f"of {nb_todo:8d} ({pct_progress:3.2f}%)    "
-        )
-        print(message, end="", flush=True)
-    elif time_passed > 0:
-        # Else, report progress properly...
-        processed_per_hour = (nb_done / time_passed) * 3600
-        # Correct the nb processed per hour if running parallel
-        if nb_done < nb_parallel:
-            processed_per_hour = round(processed_per_hour * nb_parallel / nb_done)
-        hours_to_go = (int)((nb_todo - nb_done) / processed_per_hour)
-        min_to_go = (int)((((nb_todo - nb_done) / processed_per_hour) % 1) * 60)
-        pct_progress = 100.0 - (nb_todo - nb_done) * 100 / nb_todo
-        if pct_progress < 100:
-            message = (
-                f"\r{hours_to_go:3d}:{min_to_go:2d} left to do {operation} on "
-                f"{(nb_todo-nb_done):8d} of {nb_todo:8d} ({pct_progress:3.2f}%)    "
-            )
-        else:
-            message = (
-                f"\r{hours_to_go:3d}:{min_to_go:2d} left to do {operation} on "
-                f"{(nb_todo-nb_done):8d} of {nb_todo:8d} ({pct_progress:3.2f}%)    \n"
-            )
-        print(message, end="", flush=True)
-
-
-def formatbytes(bytes: float):
-    """
-    Return the given bytes as a human friendly KB, MB, GB, or TB string
-    """
-
-    bytes_float = float(bytes)
-    KB = float(1024)
-    MB = float(KB**2)  # 1,048,576
-    GB = float(KB**3)  # 1,073,741,824
-    TB = float(KB**4)  # 1,099,511,627,776
-
-    if bytes_float < KB:
-        return "{0} {1}".format(bytes_float, "Bytes" if bytes_float > 1 else "Byte")
-    elif KB <= bytes_float < MB:
-        return "{0:.2f} KB".format(bytes_float / KB)
-    elif MB <= bytes_float < GB:
-        return "{0:.2f} MB".format(bytes_float / MB)
-    elif GB <= bytes_float < TB:
-        return "{0:.2f} GB".format(bytes_float / GB)
-    elif TB <= bytes_float:
-        return "{0:.2f} TB".format(bytes_float / TB)
-
-
-def process_nice_to_priority_class(nice_value: int) -> int:
-    if nice_value <= -15:
-        return psutil.REALTIME_PRIORITY_CLASS
-    elif nice_value <= -10:
-        return psutil.HIGH_PRIORITY_CLASS
-    elif nice_value <= -5:
-        return psutil.ABOVE_NORMAL_PRIORITY_CLASS
-    elif nice_value <= 0:
-        return psutil.NORMAL_PRIORITY_CLASS
-    elif nice_value <= 10:
-        return psutil.BELOW_NORMAL_PRIORITY_CLASS
-    else:
-        return psutil.IDLE_PRIORITY_CLASS
-
-
-def setprocessnice(nice_value: int):
-    p = psutil.Process(os.getpid())
-    if os.name == "nt":
-        p.nice(process_nice_to_priority_class(nice_value))
-    else:
-        p.nice(nice_value)
-
-
-def getprocessnice() -> int:
-    p = psutil.Process(os.getpid())
-    nice_value = p.nice()
-    if os.name == "nt":
-        if nice_value == psutil.REALTIME_PRIORITY_CLASS:
-            return -20
-        elif nice_value == psutil.HIGH_PRIORITY_CLASS:
-            return -10
-        elif nice_value == psutil.ABOVE_NORMAL_PRIORITY_CLASS:
-            return -5
-        elif nice_value == psutil.NORMAL_PRIORITY_CLASS:
-            return 0
-        elif nice_value == psutil.BELOW_NORMAL_PRIORITY_CLASS:
-            return 10
-        elif nice_value == psutil.IDLE_PRIORITY_CLASS:
-            return 20
-        else:
-            return 0
-    else:
-        return int(nice_value)
+# -*- coding: utf-8 -*-
+"""
+Module containing some general utilities.
+"""
+
+import datetime
+import logging
+import os
+from typing import Optional
+
+import psutil
+
+################################################################################
+# Some init
+################################################################################
+
+logger = logging.getLogger(__name__)
+
+
+class MissingRuntimeDependencyError(Exception):
+    """
+    Exception raised when an unsupported SQL statement is passed.
+
+    Attributes:
+        message (str): Exception message
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+
+################################################################################
+# The real work
+################################################################################
+
+
+def report_progress(
+    start_time: datetime.datetime,
+    nb_done: int,
+    nb_todo: int,
+    operation: Optional[str] = None,
+    nb_parallel: int = 1,
+):
+    # Init
+    time_passed = (datetime.datetime.now() - start_time).total_seconds()
+    pct_progress = 100.0 - (nb_todo - nb_done) * 100 / nb_todo
+
+    # If we haven't really started yet, don't report time estimate yet
+    if nb_done == 0:
+        message = (
+            f"\r  ?: ? left to do {operation} on {(nb_todo-nb_done):8d} "
+            f"of {nb_todo:8d} ({pct_progress:3.2f}%)    "
+        )
+        print(message, end="", flush=True)
+    elif time_passed > 0:
+        # Else, report progress properly...
+        processed_per_hour = (nb_done / time_passed) * 3600
+        # Correct the nb processed per hour if running parallel
+        if nb_done < nb_parallel:
+            processed_per_hour = round(processed_per_hour * nb_parallel / nb_done)
+        hours_to_go = (int)((nb_todo - nb_done) / processed_per_hour)
+        min_to_go = (int)((((nb_todo - nb_done) / processed_per_hour) % 1) * 60)
+        pct_progress = 100.0 - (nb_todo - nb_done) * 100 / nb_todo
+        if pct_progress < 100:
+            message = (
+                f"\r{hours_to_go:3d}:{min_to_go:2d} left to do {operation} on "
+                f"{(nb_todo-nb_done):8d} of {nb_todo:8d} ({pct_progress:3.2f}%)    "
+            )
+        else:
+            message = (
+                f"\r{hours_to_go:3d}:{min_to_go:2d} left to do {operation} on "
+                f"{(nb_todo-nb_done):8d} of {nb_todo:8d} ({pct_progress:3.2f}%)    \n"
+            )
+        print(message, end="", flush=True)
+
+
+def formatbytes(bytes: float):
+    """
+    Return the given bytes as a human friendly KB, MB, GB, or TB string
+    """
+
+    bytes_float = float(bytes)
+    KB = float(1024)
+    MB = float(KB**2)  # 1,048,576
+    GB = float(KB**3)  # 1,073,741,824
+    TB = float(KB**4)  # 1,099,511,627,776
+
+    if bytes_float < KB:
+        return "{0} {1}".format(bytes_float, "Bytes" if bytes_float > 1 else "Byte")
+    elif KB <= bytes_float < MB:
+        return "{0:.2f} KB".format(bytes_float / KB)
+    elif MB <= bytes_float < GB:
+        return "{0:.2f} MB".format(bytes_float / MB)
+    elif GB <= bytes_float < TB:
+        return "{0:.2f} GB".format(bytes_float / GB)
+    elif TB <= bytes_float:
+        return "{0:.2f} TB".format(bytes_float / TB)
+
+
+def process_nice_to_priority_class(nice_value: int) -> int:
+    if nice_value <= -15:
+        return psutil.REALTIME_PRIORITY_CLASS
+    elif nice_value <= -10:
+        return psutil.HIGH_PRIORITY_CLASS
+    elif nice_value <= -5:
+        return psutil.ABOVE_NORMAL_PRIORITY_CLASS
+    elif nice_value <= 0:
+        return psutil.NORMAL_PRIORITY_CLASS
+    elif nice_value <= 10:
+        return psutil.BELOW_NORMAL_PRIORITY_CLASS
+    else:
+        return psutil.IDLE_PRIORITY_CLASS
+
+
+def setprocessnice(nice_value: int):
+    p = psutil.Process(os.getpid())
+    if os.name == "nt":
+        p.nice(process_nice_to_priority_class(nice_value))
+    else:
+        p.nice(nice_value)
+
+
+def getprocessnice() -> int:
+    p = psutil.Process(os.getpid())
+    nice_value = p.nice()
+    if os.name == "nt":
+        if nice_value == psutil.REALTIME_PRIORITY_CLASS:
+            return -20
+        elif nice_value == psutil.HIGH_PRIORITY_CLASS:
+            return -10
+        elif nice_value == psutil.ABOVE_NORMAL_PRIORITY_CLASS:
+            return -5
+        elif nice_value == psutil.NORMAL_PRIORITY_CLASS:
+            return 0
+        elif nice_value == psutil.BELOW_NORMAL_PRIORITY_CLASS:
+            return 10
+        elif nice_value == psutil.IDLE_PRIORITY_CLASS:
+            return 20
+        else:
+            return 0
+    else:
+        return int(nice_value)
```

### Comparing `orthoseg-0.4.2/orthoseg/util/git_downloader.py` & `orthoseg-0.4.2a1/orthoseg/util/git_downloader.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-#!/usr/bin/python3
-# Based on https://github.com/sdushantha/gitdir/blob/master/gitdir/gitdir.py
-
-import re
-import os
-import ssl
-import time
-from typing import Union
-import urllib.request
-import json
-from pathlib import Path
-
-
-def create_url(url):
-    """
-    From the given url, produce a URL that is compatible with Github's REST API.
-    Can handle blob or tree paths.
-    """
-
-    # extract the branch name from the given url (e.g master)
-    branch = re.findall(r"/tree/(.*?)/", url)
-    api_url = url.replace("https://github.com", "https://api.github.com/repos")
-    if len(branch) == 0:
-        branch = re.findall(r"/blob/(.*?)/", url)[0]
-        download_dirs = re.findall(r"/blob/" + branch + r"/(.*)", url)[0]
-        api_url = re.sub(r"/blob/.*?/", "/contents/", api_url)
-    else:
-        branch = branch[0]
-        download_dirs = re.findall(r"/tree/" + branch + r"/(.*)", url)[0]
-        api_url = re.sub(r"/tree/.*?/", "/contents/", api_url)
-
-    api_url = api_url + "?ref=" + branch
-    return api_url, download_dirs
-
-
-def download(
-    repo_url: str,
-    output_dir: Path,
-    ssl_verify: Union[bool, str, None] = None,
-    limit_rate: bool = True,
-):
-    """
-    Downloads the files and directories in repo_url.
-
-    Args
-        repo_url (str): url to the repository to download.
-        output_dir (Path): directory to download the repository to.
-        ssl_verify (bool or str, optional): True or None to use the default
-            certificate bundle as installed on your system. False disables
-            certificate validation (NOT recommended!). If a path to a
-            certificate bundle file (.pem) is passed, this will be used.
-            In corporate networks using a proxy server this is often needed
-            to evade CERTIFICATE_VERIFY_FAILED errors. Defaults to None.
-        limit_rate (bool, optional): If True, limit the rate requests are done to
-            github to the maximum level allowed for unauthenticated users.
-            Defaults to True.
-    """
-    context = None
-    if ssl_verify is not None:
-        # If it is a string, make sure it isn't actually a bool
-        if isinstance(ssl_verify, str):
-            if ssl_verify.lower() == "true":
-                context = None
-            elif ssl_verify.lower() == "false":
-                ssl_verify = False
-            else:
-                context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-                context.load_verify_locations(ssl_verify)
-
-        if isinstance(ssl_verify, bool) and not ssl_verify:
-            context = ssl._create_unverified_context()
-            print("SSL VERIFICATION IS TURNED OFF!!!")
-
-    # Generate the url which returns the JSON data
-    api_url, download_dirs = create_url(repo_url)
-
-    # To handle file names.
-    if len(download_dirs.split(".")) == 0:
-        dir_out = output_dir / download_dirs
-    else:
-        dir_out = output_dir / "/".join(download_dirs.split("/")[0:-1])
-
-    # Download the file
-    # If limit_rate enabled, always sleep 1 second before doing a request!
-    if limit_rate:
-        time.sleep(1)
-    with urllib.request.urlopen(api_url, context=context) as u:
-        # Make a directory with the name which is taken from
-        # the actual repo
-        dir_out.mkdir(parents=True, exist_ok=True)
-
-        # Total files count
-        total_files = 0
-        raw_data = u.read()
-        data = json.loads(raw_data)
-
-        # Get the total number of files
-        total_files += len(data)
-
-        # If the data is a file, download it as one.
-        if isinstance(data, dict) and data["type"] == "file":
-            # Download the file
-            if limit_rate:
-                time.sleep(1)
-            with urllib.request.urlopen(
-                data["download_url"], context=context
-            ) as u, open(dir_out / data["name"], "wb") as f:
-                f.write(u.read())
-            return total_files
-
-        # Loop over all files/dirs found
-        for file in data:
-            file_url = file["download_url"]
-            path = output_dir / file["path"]
-            os.makedirs(path.parent, exist_ok=True)
-
-            # If it is a file, download it, if dir, start recursively
-            if file_url is not None:
-                if limit_rate:
-                    time.sleep(1)
-                with urllib.request.urlopen(file_url, context=context) as u, open(
-                    path, "wb"
-                ) as f:
-                    f.write(u.read())
-            else:
-                download(file["html_url"], output_dir)
-
-    return total_files
+#!/usr/bin/python3
+# Based on https://github.com/sdushantha/gitdir/blob/master/gitdir/gitdir.py
+
+import re
+import os
+import ssl
+import time
+from typing import Union
+import urllib.request
+import json
+from pathlib import Path
+
+
+def create_url(url):
+    """
+    From the given url, produce a URL that is compatible with Github's REST API.
+    Can handle blob or tree paths.
+    """
+
+    # extract the branch name from the given url (e.g master)
+    branch = re.findall(r"/tree/(.*?)/", url)
+    api_url = url.replace("https://github.com", "https://api.github.com/repos")
+    if len(branch) == 0:
+        branch = re.findall(r"/blob/(.*?)/", url)[0]
+        download_dirs = re.findall(r"/blob/" + branch + r"/(.*)", url)[0]
+        api_url = re.sub(r"/blob/.*?/", "/contents/", api_url)
+    else:
+        branch = branch[0]
+        download_dirs = re.findall(r"/tree/" + branch + r"/(.*)", url)[0]
+        api_url = re.sub(r"/tree/.*?/", "/contents/", api_url)
+
+    api_url = api_url + "?ref=" + branch
+    return api_url, download_dirs
+
+
+def download(
+    repo_url: str,
+    output_dir: Path,
+    ssl_verify: Union[bool, str, None] = None,
+    limit_rate: bool = True,
+):
+    """
+    Downloads the files and directories in repo_url.
+
+    Args
+        repo_url (str): url to the repository to download.
+        output_dir (Path): directory to download the repository to.
+        ssl_verify (bool or str, optional): True or None to use the default
+            certificate bundle as installed on your system. False disables
+            certificate validation (NOT recommended!). If a path to a
+            certificate bundle file (.pem) is passed, this will be used.
+            In corporate networks using a proxy server this is often needed
+            to evade CERTIFICATE_VERIFY_FAILED errors. Defaults to None.
+        limit_rate (bool, optional): If True, limit the rate requests are done to
+            github to the maximum level allowed for unauthenticated users.
+            Defaults to True.
+    """
+    context = None
+    if ssl_verify is not None:
+        # If it is a string, make sure it isn't actually a bool
+        if isinstance(ssl_verify, str):
+            if ssl_verify.lower() == "true":
+                context = None
+            elif ssl_verify.lower() == "false":
+                ssl_verify = False
+            else:
+                context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+                context.load_verify_locations(ssl_verify)
+
+        if isinstance(ssl_verify, bool) and not ssl_verify:
+            context = ssl._create_unverified_context()
+            print("SSL VERIFICATION IS TURNED OFF!!!")
+
+    # Generate the url which returns the JSON data
+    api_url, download_dirs = create_url(repo_url)
+
+    # To handle file names.
+    if len(download_dirs.split(".")) == 0:
+        dir_out = output_dir / download_dirs
+    else:
+        dir_out = output_dir / "/".join(download_dirs.split("/")[0:-1])
+
+    # Download the file
+    # If limit_rate enabled, always sleep 1 second before doing a request!
+    if limit_rate:
+        time.sleep(1)
+    with urllib.request.urlopen(api_url, context=context) as u:
+        # Make a directory with the name which is taken from
+        # the actual repo
+        dir_out.mkdir(parents=True, exist_ok=True)
+
+        # Total files count
+        total_files = 0
+        raw_data = u.read()
+        data = json.loads(raw_data)
+
+        # Get the total number of files
+        total_files += len(data)
+
+        # If the data is a file, download it as one.
+        if isinstance(data, dict) and data["type"] == "file":
+            # Download the file
+            if limit_rate:
+                time.sleep(1)
+            with urllib.request.urlopen(
+                data["download_url"], context=context
+            ) as u, open(dir_out / data["name"], "wb") as f:
+                f.write(u.read())
+            return total_files
+
+        # Loop over all files/dirs found
+        for file in data:
+            file_url = file["download_url"]
+            path = output_dir / file["path"]
+            os.makedirs(path.parent, exist_ok=True)
+
+            # If it is a file, download it, if dir, start recursively
+            if file_url is not None:
+                if limit_rate:
+                    time.sleep(1)
+                with urllib.request.urlopen(file_url, context=context) as u, open(
+                    path, "wb"
+                ) as f:
+                    f.write(u.read())
+            else:
+                download(file["html_url"], output_dir)
+
+    return total_files
```

### Comparing `orthoseg-0.4.2/orthoseg/util/log_util.py` & `orthoseg-0.4.2a1/orthoseg/util/log_util.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# -*- coding: utf-8 -*-
-"""
-Module with specific helper functions to manage the logging of orthoseg.
-
-TODO: maybe it is cleaner to replace most code here by a config dict?
-"""
-
-import json
-import logging
-import logging.config
-import datetime
-from pathlib import Path
-import tempfile
-from typing import Optional
-
-# -------------------------------------------------------------
-# Log helpers
-# -------------------------------------------------------------
-
-
-class LoggingContext:
-    def __init__(self, logger, level=None, handler=None, close=True):
-        self.logger = logger
-        self.level = level
-        self.handler = handler
-        self.close = close
-
-    def __enter__(self):
-        if self.level is not None:
-            self.old_level = self.logger.level
-            self.logger.setLevel(self.level)
-        if self.handler:
-            self.logger.addHandler(self.handler)
-
-    def __exit__(self, et, ev, tb):
-        if self.level is not None:
-            self.logger.setLevel(self.old_level)
-        if self.handler:
-            self.logger.removeHandler(self.handler)
-        if self.handler and self.close:
-            self.handler.close()
-        # implicit return of None => don't swallow exceptions
-
-
-# -------------------------------------------------------------
-# Init logging
-# -------------------------------------------------------------
-
-
-def init_logging_dictConfig(
-    logconfig_path: Optional[Path] = None,
-    logconfig_dict: Optional[dict] = None,
-    log_basedir: Optional[Path] = None,
-    loggername: Optional[str] = None,
-) -> logging.Logger:
-    """
-    Initializes the logging based on input in dictConfig format.
-
-    The input can be a dict or a json file.
-
-    The added value of this function is:
-        - it will format {iso_datetime} placeholders in handlers.*.filename
-        - it will resolve relative file paths in handlers.*.filename to tempdir.
-
-    Args:
-        logconfig_path (Path, optional): Json file containing the dictConfig info.
-            Defaults to None.
-        logconfig_dict (dict, optional): Dict containing the dictConfig info.
-            Defaults to None.
-    """
-    # Init logging
-    if logconfig_dict is None:
-        if logconfig_path is not None and logconfig_path.exists():
-            # Load from json file
-            with open(logconfig_path, "r") as logconfig_file:
-                logconfig_dict = json.load(logconfig_file)
-        else:
-            raise Exception(
-                "If the logconfig_dict is None, the logconfig_path should point to "
-                f"an existing file: {logconfig_path}"
-            )
-
-    # If there are file handlers, replace placeholders + make sure log dir exists
-    assert logconfig_dict is not None
-    for handler in logconfig_dict["handlers"]:
-        if "filename" in logconfig_dict["handlers"][handler]:
-            # Format the filename
-            log_path = Path(
-                logconfig_dict["handlers"][handler]["filename"].format(
-                    iso_datetime=f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}"
-                )
-            )
-
-            # If the log_path is a relative path, resolve it to temp dir.
-            if not log_path.is_absolute():
-                if log_basedir is not None:
-                    log_path = log_basedir / log_path
-                else:
-                    log_path = Path(tempfile.gettempdir()) / log_path
-                print(
-                    f"Parameter logconfig.handlers.{handler}.filename was relative, "
-                    f"so is now resolved to {log_path}"
-                )
-
-            logconfig_dict["handlers"][handler]["filename"] = str(log_path)
-
-            # Also make sure the log dir exists
-            log_path.parent.mkdir(parents=True, exist_ok=True)
-
-    # Now load the log config
-    logging.config.dictConfig(logconfig_dict)  # type: ignore
-
-    return logging.getLogger(loggername)
-
-
-def main_log_init(log_dir: Path, log_basefilename: str):
-
-    # Check input parameters
-    if not log_dir:
-        raise Exception("Error: log_dir is mandatory!")
-
-    # Make sure the log dir exists
-    if not log_dir.exists():
-        log_dir.mkdir(parents=True, exist_ok=True)
-
-    # Get root logger
-    logger = logging.getLogger("")
-
-    # Set the general maximum log level...
-    logger.setLevel(logging.INFO)
-    for handler in logger.handlers:
-        handler.flush()
-        handler.close()
-
-    # Remove all handlers and add the ones I want again, so a new log file is created
-    # for each run
-    # Remark: the function removehandler doesn't seem to work?
-    logger.handlers = []
-
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
-    # ch.setFormatter(logging.Formatter('%(levelname)s|%(name)s|%(message)s'))
-    # ch.setFormatter(logging.Formatter('%(asctime)s|%(levelname)s|%(name)s|%(message)s',
-    #                                  datefmt='%H:%M:%S,uuu'))
-    ch.setFormatter(
-        logging.Formatter(
-            fmt="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
-            datefmt="%H:%M:%S",
-        )
-    )
-    logger.addHandler(ch)
-
-    log_filepath = (
-        log_dir / f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}_{log_basefilename}.log"
-    )
-    fh = logging.FileHandler(filename=str(log_filepath))
-    fh.setLevel(logging.INFO)
-    fh.setFormatter(logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s"))
-    logger.addHandler(fh)
-
-    return logger
-
-
-def clean_log_dir(log_dir: Path, nb_logfiles_tokeep: int, pattern: str = "*.*"):
-    """
-    Clean a log dir.
-
-    Args:
-        log_dir (Path): dir with log files to clean.
-        nb_logfiles_tokeep (int): the number of log files to keep.
-        pattern (str, optional): pattern of the file names of the log files.
-            Defaults to '*.*'.
-    """
-    # Check input params
-    if log_dir is None or log_dir.exists() is False or nb_logfiles_tokeep is None:
-        return
-
-    # List log files and remove the ones that are too much
-    files = sorted(list(log_dir.glob(pattern)), reverse=True)
-    if len(files) > nb_logfiles_tokeep:
-        for file_index in range(nb_logfiles_tokeep, len(files)):
-            files[file_index].unlink()
+# -*- coding: utf-8 -*-
+"""
+Module with specific helper functions to manage the logging of orthoseg.
+
+TODO: maybe it is cleaner to replace most code here by a config dict?
+"""
+
+import json
+import logging
+import logging.config
+import datetime
+from pathlib import Path
+import tempfile
+from typing import Optional
+
+# -------------------------------------------------------------
+# Log helpers
+# -------------------------------------------------------------
+
+
+class LoggingContext:
+    def __init__(self, logger, level=None, handler=None, close=True):
+        self.logger = logger
+        self.level = level
+        self.handler = handler
+        self.close = close
+
+    def __enter__(self):
+        if self.level is not None:
+            self.old_level = self.logger.level
+            self.logger.setLevel(self.level)
+        if self.handler:
+            self.logger.addHandler(self.handler)
+
+    def __exit__(self, et, ev, tb):
+        if self.level is not None:
+            self.logger.setLevel(self.old_level)
+        if self.handler:
+            self.logger.removeHandler(self.handler)
+        if self.handler and self.close:
+            self.handler.close()
+        # implicit return of None => don't swallow exceptions
+
+
+# -------------------------------------------------------------
+# Init logging
+# -------------------------------------------------------------
+
+
+def init_logging_dictConfig(
+    logconfig_path: Optional[Path] = None,
+    logconfig_dict: Optional[dict] = None,
+    log_basedir: Optional[Path] = None,
+    loggername: Optional[str] = None,
+) -> logging.Logger:
+    """
+    Initializes the logging based on input in dictConfig format.
+
+    The input can be a dict or a json file.
+
+    The added value of this function is:
+        - it will format {iso_datetime} placeholders in handlers.*.filename
+        - it will resolve relative file paths in handlers.*.filename to tempdir.
+
+    Args:
+        logconfig_path (Path, optional): Json file containing the dictConfig info.
+            Defaults to None.
+        logconfig_dict (dict, optional): Dict containing the dictConfig info.
+            Defaults to None.
+    """
+    # Init logging
+    if logconfig_dict is None:
+        if logconfig_path is not None and logconfig_path.exists():
+            # Load from json file
+            with open(logconfig_path, "r") as logconfig_file:
+                logconfig_dict = json.load(logconfig_file)
+        else:
+            raise Exception(
+                "If the logconfig_dict is None, the logconfig_path should point to "
+                f"an existing file: {logconfig_path}"
+            )
+
+    # If there are file handlers, replace placeholders + make sure log dir exists
+    assert logconfig_dict is not None
+    for handler in logconfig_dict["handlers"]:
+        if "filename" in logconfig_dict["handlers"][handler]:
+            # Format the filename
+            log_path = Path(
+                logconfig_dict["handlers"][handler]["filename"].format(
+                    iso_datetime=f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}"
+                )
+            )
+
+            # If the log_path is a relative path, resolve it to temp dir.
+            if not log_path.is_absolute():
+                if log_basedir is not None:
+                    log_path = log_basedir / log_path
+                else:
+                    log_path = Path(tempfile.gettempdir()) / log_path
+                print(
+                    f"Parameter logconfig.handlers.{handler}.filename was relative, "
+                    f"so is now resolved to {log_path}"
+                )
+
+            logconfig_dict["handlers"][handler]["filename"] = str(log_path)
+
+            # Also make sure the log dir exists
+            log_path.parent.mkdir(parents=True, exist_ok=True)
+
+    # Now load the log config
+    logging.config.dictConfig(logconfig_dict)  # type: ignore
+
+    return logging.getLogger(loggername)
+
+
+def main_log_init(log_dir: Path, log_basefilename: str):
+
+    # Check input parameters
+    if not log_dir:
+        raise Exception("Error: log_dir is mandatory!")
+
+    # Make sure the log dir exists
+    if not log_dir.exists():
+        log_dir.mkdir(parents=True, exist_ok=True)
+
+    # Get root logger
+    logger = logging.getLogger("")
+
+    # Set the general maximum log level...
+    logger.setLevel(logging.INFO)
+    for handler in logger.handlers:
+        handler.flush()
+        handler.close()
+
+    # Remove all handlers and add the ones I want again, so a new log file is created
+    # for each run
+    # Remark: the function removehandler doesn't seem to work?
+    logger.handlers = []
+
+    ch = logging.StreamHandler()
+    ch.setLevel(logging.INFO)
+    # ch.setFormatter(logging.Formatter('%(levelname)s|%(name)s|%(message)s'))
+    # ch.setFormatter(logging.Formatter('%(asctime)s|%(levelname)s|%(name)s|%(message)s',
+    #                                  datefmt='%H:%M:%S,uuu'))
+    ch.setFormatter(
+        logging.Formatter(
+            fmt="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
+            datefmt="%H:%M:%S",
+        )
+    )
+    logger.addHandler(ch)
+
+    log_filepath = (
+        log_dir / f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}_{log_basefilename}.log"
+    )
+    fh = logging.FileHandler(filename=str(log_filepath))
+    fh.setLevel(logging.INFO)
+    fh.setFormatter(logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s"))
+    logger.addHandler(fh)
+
+    return logger
+
+
+def clean_log_dir(log_dir: Path, nb_logfiles_tokeep: int, pattern: str = "*.*"):
+    """
+    Clean a log dir.
+
+    Args:
+        log_dir (Path): dir with log files to clean.
+        nb_logfiles_tokeep (int): the number of log files to keep.
+        pattern (str, optional): pattern of the file names of the log files.
+            Defaults to '*.*'.
+    """
+    # Check input params
+    if log_dir is None or log_dir.exists() is False or nb_logfiles_tokeep is None:
+        return
+
+    # List log files and remove the ones that are too much
+    files = sorted(list(log_dir.glob(pattern)), reverse=True)
+    if len(files) > nb_logfiles_tokeep:
+        for file_index in range(nb_logfiles_tokeep, len(files)):
+            files[file_index].unlink()
```

### Comparing `orthoseg-0.4.2/orthoseg/util/progress_util.py` & `orthoseg-0.4.2a1/orthoseg/util/progress_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# -*- coding: utf-8 -*-
-"""
-Module with functions to manage progress logging.
-"""
-
-import datetime
-import logging
-from typing import Optional
-
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-
-class ProgressLogger:
-    first_reporting_done = False
-
-    def __init__(
-        self,
-        message: str,
-        nb_steps_total: int,
-        nb_steps_done: int = 0,
-        start_time: Optional[datetime.datetime] = None,
-        time_between_reporting_s: int = 60,
-        calculate_eta_since_lastreporting: bool = True,
-    ):
-        self.message = message
-        if start_time is None:
-            self.start_time = datetime.datetime.now()
-        else:
-            self.start_time = start_time
-        self.start_time_lastreporting = self.start_time
-        self.nb_steps_total = nb_steps_total
-        self.nb_steps_done = nb_steps_done
-        self.nb_steps_done_lastreporting = nb_steps_done
-        self.time_between_reporting_s = time_between_reporting_s
-        self.calculate_eta_since_lastreporting = calculate_eta_since_lastreporting
-
-    def step(self, message: Optional[str] = None, nb_steps: int = 1):
-
-        # Increase done counter
-        self.nb_steps_done += nb_steps
-
-        # Calculate time since last reporting
-        time_now = datetime.datetime.now()
-        time_passed_lastprogress_s = (
-            time_now - self.start_time_lastreporting
-        ).total_seconds()
-
-        # Calculate the time_passed and nb_done we want to use to calculate ETA
-        if self.calculate_eta_since_lastreporting is True:
-            time_passed_for_eta_s = (
-                time_now - self.start_time_lastreporting
-            ).total_seconds()
-            nb_steps_done_eta = self.nb_steps_done - self.nb_steps_done_lastreporting
-        else:
-            time_passed_for_eta_s = (time_now - self.start_time).total_seconds()
-            nb_steps_done_eta = self.nb_steps_done
-
-        # Print progress on first step or if time between reporting has passed
-        if (
-            time_passed_lastprogress_s >= self.time_between_reporting_s
-            or self.first_reporting_done is False
-        ):
-            # Evade divisions by zero
-            if time_passed_for_eta_s == 0 or nb_steps_done_eta == 0:
-                return
-
-            nb_per_hour = (nb_steps_done_eta / time_passed_for_eta_s) * 3600
-            hours_to_go = (int)(
-                (self.nb_steps_total - self.nb_steps_done) / nb_per_hour
-            )
-            min_to_go = (int)(
-                (((self.nb_steps_total - self.nb_steps_done) / nb_per_hour) % 1) * 60
-            )
-            if message is not None:
-                progress_message = (
-                    f"{message}, {self.nb_steps_done}/{self.nb_steps_total}, "
-                    f"{hours_to_go:3d}:{min_to_go:2d} left at {nb_per_hour:0.0f}/h"
-                )
-            else:
-                progress_message = (
-                    f"{self.message}, {self.nb_steps_done}/{self.nb_steps_total}, "
-                    f"{hours_to_go:3d}:{min_to_go:2d} left at {nb_per_hour:0.0f}/h"
-                )
-            logger.info(progress_message)
-
-            self.start_time_lastreporting = time_now
-            self.nb_steps_done_lastreporting = self.nb_steps_done
-            if self.first_reporting_done is False:
-                self.first_reporting_done = True
+# -*- coding: utf-8 -*-
+"""
+Module with functions to manage progress logging.
+"""
+
+import datetime
+import logging
+from typing import Optional
+
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+
+class ProgressLogger:
+    first_reporting_done = False
+
+    def __init__(
+        self,
+        message: str,
+        nb_steps_total: int,
+        nb_steps_done: int = 0,
+        start_time: Optional[datetime.datetime] = None,
+        time_between_reporting_s: int = 60,
+        calculate_eta_since_lastreporting: bool = True,
+    ):
+        self.message = message
+        if start_time is None:
+            self.start_time = datetime.datetime.now()
+        else:
+            self.start_time = start_time
+        self.start_time_lastreporting = self.start_time
+        self.nb_steps_total = nb_steps_total
+        self.nb_steps_done = nb_steps_done
+        self.nb_steps_done_lastreporting = nb_steps_done
+        self.time_between_reporting_s = time_between_reporting_s
+        self.calculate_eta_since_lastreporting = calculate_eta_since_lastreporting
+
+    def step(self, message: Optional[str] = None, nb_steps: int = 1):
+
+        # Increase done counter
+        self.nb_steps_done += nb_steps
+
+        # Calculate time since last reporting
+        time_now = datetime.datetime.now()
+        time_passed_lastprogress_s = (
+            time_now - self.start_time_lastreporting
+        ).total_seconds()
+
+        # Calculate the time_passed and nb_done we want to use to calculate ETA
+        if self.calculate_eta_since_lastreporting is True:
+            time_passed_for_eta_s = (
+                time_now - self.start_time_lastreporting
+            ).total_seconds()
+            nb_steps_done_eta = self.nb_steps_done - self.nb_steps_done_lastreporting
+        else:
+            time_passed_for_eta_s = (time_now - self.start_time).total_seconds()
+            nb_steps_done_eta = self.nb_steps_done
+
+        # Print progress on first step or if time between reporting has passed
+        if (
+            time_passed_lastprogress_s >= self.time_between_reporting_s
+            or self.first_reporting_done is False
+        ):
+            # Evade divisions by zero
+            if time_passed_for_eta_s == 0 or nb_steps_done_eta == 0:
+                return
+
+            nb_per_hour = (nb_steps_done_eta / time_passed_for_eta_s) * 3600
+            hours_to_go = (int)(
+                (self.nb_steps_total - self.nb_steps_done) / nb_per_hour
+            )
+            min_to_go = (int)(
+                (((self.nb_steps_total - self.nb_steps_done) / nb_per_hour) % 1) * 60
+            )
+            if message is not None:
+                progress_message = (
+                    f"{message}, {self.nb_steps_done}/{self.nb_steps_total}, "
+                    f"{hours_to_go:3d}:{min_to_go:2d} left at {nb_per_hour:0.0f}/h"
+                )
+            else:
+                progress_message = (
+                    f"{self.message}, {self.nb_steps_done}/{self.nb_steps_total}, "
+                    f"{hours_to_go:3d}:{min_to_go:2d} left at {nb_per_hour:0.0f}/h"
+                )
+            logger.info(progress_message)
+
+            self.start_time_lastreporting = time_now
+            self.nb_steps_done_lastreporting = self.nb_steps_done
+            if self.first_reporting_done is False:
+                self.first_reporting_done = True
```

### Comparing `orthoseg-0.4.2/orthoseg/util/vector_util.py` & `orthoseg-0.4.2a1/orthoseg/util/vector_util.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,384 +1,384 @@
-# -*- coding: utf-8 -*-
-"""
-Modile with generic Utility functions for vector manipulations.
-"""
-
-import copy
-import logging
-from typing import Optional, Tuple
-
-import geofileops as gfo
-from geofileops.util import geometry_util
-from geofileops.util import geoseries_util
-import geopandas as gpd
-import numpy as np
-import pandas as pd
-import pygeos
-from shapely import geometry as sh_geom
-import topojson
-import topojson.ops
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def is_onborder(
-    gdf: gpd.GeoDataFrame,
-    border_bounds: Tuple[float, float, float, float],
-    onborder_column_name: str = "onborder",
-) -> gpd.GeoDataFrame:
-    """
-    Add/update a column to the GeoDataFrame with:
-        * 0 if the polygon isn't on the border and
-        * 1 if it is.
-
-    Args
-        geoms_gdf: input GeoDataFrame
-        border_bounds: the bounds (tupple with (xmin, ymin, xmax, ymax)
-                       to check against to determine onborder
-        onborder_column_name: the column name of the onborder column
-
-    """
-    if gdf is None or len(gdf.index) == 0:
-        return gdf
-
-    result_gdf = gdf.copy()  # type: ignore
-    result_gdf[onborder_column_name] = 0
-
-    # Check
-    for i, geom_row in result_gdf.iterrows():
-        if geom_row["geometry"] is not None and not geom_row["geometry"].is_empty:
-            # Check if the geom is on the border of the tile
-            geom_bounds = geom_row["geometry"].bounds  # type: ignore
-            if (
-                geom_bounds[0] <= border_bounds[0]
-                or geom_bounds[1] <= border_bounds[1]
-                or geom_bounds[2] >= border_bounds[2]
-                or geom_bounds[3] >= border_bounds[3]
-            ):
-                result_gdf.loc[i, onborder_column_name] = 1  # type: ignore
-
-    assert isinstance(result_gdf, gpd.GeoDataFrame)
-    return result_gdf
-
-
-def is_valid_reason(geoseries) -> pd.Series:
-    # Remark: should be moved to geofileops (till available in geopandas)!!!
-    return pd.Series(
-        data=pygeos.is_valid_reason(geoseries.array.data), index=geoseries.index
-    )  # type: ignore
-
-
-def reclassify_neighbours(
-    gdf: gpd.GeoDataFrame,
-    reclassify_column: str,
-    query: str,
-    border_bounds: Optional[Tuple[float, float, float, float]],
-    class_background: str = "background",
-) -> gpd.GeoDataFrame:
-    """
-    For features that comply to the query, if they have a neighbour (touch/overlap),
-    change their classname to that of the neighbour with the longest intersection and
-    dissolve to merge them.
-
-    The query should follow the syntax of pandas.query queries and can us the following
-    fields:
-        - onborder (0 or 1): does the feature touch/overlap the border_bounds. If this
-          field is used in the query, the border_bounds parameter is mandatory.
-        - area (float): the area of the geometry.
-        - perimeter (float): the perimeter of the geometry.
-
-    Args:
-        gdf (gpd.GeoDataFrame): input
-        reclassify_column (str): column to reclassify.
-        query (str): th query to find the features to reclassify.
-        border_bounds (Optional[Tuple[float, float, float, float]]): the bounds of the
-            border to use for th onborder field in the query.
-        class_background (str, optional): the classname to treat as background.
-            Defaults to "background".
-        aggfunc ()
-
-    Raises:
-        ValueError: raised if incompatible parameters are passed.
-
-    Returns:
-        gpd.GeoDataFrame: the reclassified result
-    """
-    # Init column info
-    columns_orig = [col for col in gdf.columns]
-
-    # Init query + needed data
-    query = query.replace("\n", " ")
-
-    def _add_needed_columns(
-        inner_gdf: gpd.GeoDataFrame,
-        inner_query: str,
-        inner_border_bounds: Optional[Tuple[float, float, float, float]],
-    ) -> gpd.GeoDataFrame:
-        gdf_result = inner_gdf.copy()
-
-        # Always add area to know which neighbour is largest
-        gdf_result["area"] = gdf_result.geometry.area
-        if "perimeter" in inner_query:
-            gdf_result["perimeter"] = gdf_result.geometry.length
-        if "onborder" in inner_query:
-            if inner_border_bounds is None:
-                raise ValueError(
-                    "query contains onborder, but border_bounds parameter is None"
-                )
-            gdf_result = is_onborder(gdf_result, inner_border_bounds)  # type: ignore
-
-        # Return result
-        assert isinstance(gdf_result, gpd.GeoDataFrame)
-        return gdf_result
-
-    result_gdf = _add_needed_columns(gdf, query, border_bounds)
-
-    # First remove background polygons that don't match the reclassify query
-    nobackground_query = (
-        f"{reclassify_column} != '{class_background}' or "
-        f"({reclassify_column} == '{class_background}' and "
-        f"({query}))"
-    )
-    # Use copy() to avoid view-versus-copy warnings
-    result_gdf = result_gdf.query(nobackground_query).copy()
-
-    # Keep looking for polygons that comply with query and give the same class
-    # as neighbour till no changes can be made anymore.
-    # Stop after 5 iterations to be sure never to end up in endless loop
-    reclassify_max = 5
-    result_gdf["no_neighbours"] = 0
-    query = f"no_neighbours == 0 and ({query})"
-    for reclassify_counter in range(reclassify_max):
-        # Loop till no features were changed anymore
-        if reclassify_counter > 0:
-            assert isinstance(result_gdf, gpd.GeoDataFrame)
-            result_gdf = _add_needed_columns(result_gdf, query, border_bounds)
-
-        # Use copy() to avoid view-versus-copy warnings
-        result_reclass_gdf = result_gdf.query(query).copy()
-        if len(result_reclass_gdf) == 0:
-            break
-        # Order by area to treat the features found from small to large
-        result_reclass_gdf = result_reclass_gdf.sort_values(by=["area"])
-
-        for row in result_reclass_gdf.itertuples():
-            # Find neighbours (query returns iloc's, not indexes!)
-            neighbours_ilocs = result_gdf.geometry.sindex.query(
-                row.geometry, predicate="intersects"
-            ).tolist()
-            if len(neighbours_ilocs) <= 1:
-                result_gdf.loc[[row.Index], ["no_neighbours"]] = 1
-                continue
-
-            # Remove yourself
-            row_loc = result_gdf.index.get_loc(row.Index)
-            neighbours_ilocs.remove(row_loc)
-
-            # Find neighbour with longest intersection
-            neighbours_gdf = result_gdf.iloc[neighbours_ilocs]
-            inters_geoseries = neighbours_gdf.geometry.intersection(  # type: ignore
-                row.geometry
-            )
-            max_length_index = inters_geoseries.length.idxmax()
-
-            # Change the class of the smallest one to the oher's class
-            class_curr = result_gdf.at[row.Index, reclassify_column]
-            class_neighbour = result_gdf.at[max_length_index, reclassify_column]
-            if class_curr != class_neighbour:
-                # If the neighbour is not a reclass feature or if its area is larger
-                # than the current feature, use its class
-                if (
-                    max_length_index not in result_reclass_gdf.index
-                    or result_gdf.at[max_length_index, "area"] >= row.area
-                ):
-                    result_gdf.loc[[row.Index], [reclassify_column]] = class_neighbour
-                else:
-                    result_gdf.loc[[max_length_index], [reclassify_column]] = class_curr
-
-        # Remove temp columns + dissolve
-        result_gdf = result_gdf[columns_orig + ["no_neighbours"]]
-        dissolve_columns = [reclassify_column, "no_neighbours"]
-        # If there are extra columns, use aggfunc join to concatenate values
-        if len(columns_orig) > 2:
-            result_gdf = result_gdf.dissolve(
-                by=dissolve_columns, as_index=False, aggfunc=", ".join
-            )
-        else:
-            result_gdf = result_gdf.dissolve(by=dissolve_columns, as_index=False)
-
-        result_gdf = result_gdf.explode(ignore_index=True)  # type: ignore
-
-    # Finalize + make sure there is no background in the output
-    result_gdf = result_gdf[columns_orig]
-    # Use copy() to avoid view-versus-copy warnings
-    result_gdf = result_gdf.query(f"{reclassify_column} != '{class_background}'").copy()
-    assert isinstance(result_gdf, gpd.GeoDataFrame)
-    return result_gdf
-
-
-def simplify_topo_orthoseg(
-    geoseries: gpd.GeoSeries,
-    tolerance: float,
-    algorithm: gfo.SimplifyAlgorithm = gfo.SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
-    lookahead: int = 8,
-    keep_points_on: Optional[sh_geom.base.BaseGeometry] = None,
-) -> gpd.GeoSeries:
-    """
-    Applies simplify while retaining common boundaries between geometries in the
-    geoseries.
-
-    This is a specific version for orthoseg that, when algorithm is LANG, applies rdp
-    simplify with halve the tolerance first.
-
-    Args:
-        geoseries (gpd.GeoSeries): the geoseries to simplify.
-        algorithm (SimplifyAlgorithm): algorithm to use.
-        tolerance (float): tolerance to use for simplify
-        lookahead (int, optional): lookahead value for algorithms that use this.
-            Defaults to 8.
-        keep_points_on (Optional[sh_geom.base.BaseGeometry], optional): points that
-            intersect with this geometry won't be removed by the simplification.
-            Defaults to None.
-
-    Returns:
-        gpd.GeoSeries: the simplified geoseries
-    """
-    # Just return empty geoseries
-    if len(geoseries) == 0:
-        return geoseries
-
-    # Copy geoseries
-    geoseries_copy = geoseries.copy()  # type: ignore
-
-    # Set empty geometries to None, if no geometries are left, return
-    empty_idxs = pygeos.is_empty(geoseries_copy.array.data).nonzero()  # type: ignore
-    if len(empty_idxs) > 0:
-        geoseries_copy.iloc[empty_idxs] = None
-    if len(geoseries_copy[geoseries_copy != np.array(None)]) == 0:
-        return geoseries
-
-    topo = topojson.Topology(geoseries_copy, prequantize=False, shared_coords=False)
-    # 46889.5, 211427.5
-    # 46932.5, 211391.5
-
-    def simplify_topolines(
-        _topolines: list,
-        _algorithm: gfo.SimplifyAlgorithm,
-        _tolerance: float,
-        _lookahead: int,
-        _keep_points_on: Optional[sh_geom.base.BaseGeometry],
-    ) -> list:
-        """
-        Internal function that takes care of some plumbing specific to simplifying
-        the lines in the topologies.
-
-        Args:
-            _topolines (list): _description_
-            _algorithm (gfo.SimplifyAlgorithm): _description_
-            _tolerance (float): _description_
-            _lookahead (int): _description_
-            _keep_points_on (Optional[sh_geom.base.BaseGeometry]): _description_
-
-        Returns:
-            list: _description_
-        """
-        topolines_geom = sh_geom.MultiLineString(_topolines)
-        topolines_simpl = geometry_util.simplify_ext(
-            geometry=topolines_geom,
-            tolerance=_tolerance,
-            algorithm=_algorithm,
-            lookahead=_lookahead,
-            keep_points_on=_keep_points_on,
-            preserve_topology=True,
-        )
-        assert topolines_simpl is not None
-
-        # Copy the results of the simplified lines
-        if _algorithm == gfo.SimplifyAlgorithm.LANG:
-            # For LANG, a simple copy is OK
-            if isinstance(topolines_simpl, sh_geom.LineString):
-                return [list(topolines_simpl.coords)]
-            else:
-                assert isinstance(topolines_simpl, sh_geom.MultiLineString)
-                return [list(geom.coords) for geom in topolines_simpl.geoms]
-        else:
-            # For RDP, only overwrite the lines that have a valid result
-            topolines_copy = copy.deepcopy(_topolines)
-            for index in range(len(topolines_copy)):
-                # Get the coordinates of the simplified version
-                if isinstance(topolines_simpl, sh_geom.base.BaseMultipartGeometry):
-                    topoline_simpl = topolines_simpl.geoms[index].coords  # type: ignore
-                else:
-                    topoline_simpl = topolines_simpl.coords
-                # If the result of the simplify is a point, keep original
-                if len(topoline_simpl) < 2:
-                    continue
-                elif (
-                    list(topoline_simpl[0]) != topolines_copy[index][0]
-                    or list(topoline_simpl[-1]) != topolines_copy[index][-1]
-                ):
-                    # Start or end point of the simplified version is not the same
-                    # anymore
-                    continue
-                else:
-                    topolines_copy[index] = list(topoline_simpl)
-
-            return topolines_copy
-
-    if algorithm == gfo.SimplifyAlgorithm.LANG:
-        # For lang, first pre-simplify using rdp
-        topolines_simplified = simplify_topolines(
-            _topolines=topo.output["arcs"],
-            _algorithm=gfo.SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
-            _tolerance=tolerance / 2,
-            _lookahead=lookahead,
-            _keep_points_on=keep_points_on,
-        )
-        for line_id in range(len(topo.output["arcs"])):
-            topo.output["arcs"][line_id] = topolines_simplified[line_id]
-
-        topolines_simplified = simplify_topolines(
-            _topolines=topo.output["arcs"],
-            _algorithm=algorithm,
-            _tolerance=tolerance,
-            _lookahead=lookahead,
-            _keep_points_on=keep_points_on,
-        )
-        for line_id in range(len(topo.output["arcs"])):
-            topo.output["arcs"][line_id] = topolines_simplified[line_id]
-    else:
-        topolines_simplified = simplify_topolines(
-            _topolines=topo.output["arcs"],
-            _algorithm=algorithm,
-            _tolerance=tolerance,
-            _lookahead=lookahead,
-            _keep_points_on=keep_points_on,
-        )
-        for line_id in range(len(topo.output["arcs"])):
-            topo.output["arcs"][line_id] = topolines_simplified[line_id]
-
-    topo_simpl_geoseries = topo.to_gdf(crs=geoseries.crs).geometry
-    assert isinstance(topo_simpl_geoseries, gpd.GeoSeries)
-    topo_simpl_geoseries.array.data = pygeos.make_valid(  # type: ignore
-        topo_simpl_geoseries.array.data  # type: ignore
-    )
-    geometry_types_orig = geoseries.type.unique()
-    geometry_types_orig = geometry_types_orig[geometry_types_orig != None]  # noqa: E711
-    geometry_types_simpl = topo_simpl_geoseries.type.unique()
-    if len(geometry_types_orig) == 1 and (
-        len(geometry_types_simpl) > 1
-        or geometry_types_orig[0] != geometry_types_simpl[0]
-    ):
-        topo_simpl_geoseries = geoseries_util.geometry_collection_extract(
-            topo_simpl_geoseries,
-            gfo.GeometryType(geometry_types_orig[0]).to_primitivetype,
-        )
-    return topo_simpl_geoseries
+# -*- coding: utf-8 -*-
+"""
+Modile with generic Utility functions for vector manipulations.
+"""
+
+import copy
+import logging
+from typing import Optional, Tuple
+
+import geofileops as gfo
+from geofileops.util import geometry_util
+from geofileops.util import geoseries_util
+import geopandas as gpd
+import numpy as np
+import pandas as pd
+import pygeos
+from shapely import geometry as sh_geom
+import topojson
+import topojson.ops
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def is_onborder(
+    gdf: gpd.GeoDataFrame,
+    border_bounds: Tuple[float, float, float, float],
+    onborder_column_name: str = "onborder",
+) -> gpd.GeoDataFrame:
+    """
+    Add/update a column to the GeoDataFrame with:
+        * 0 if the polygon isn't on the border and
+        * 1 if it is.
+
+    Args
+        geoms_gdf: input GeoDataFrame
+        border_bounds: the bounds (tupple with (xmin, ymin, xmax, ymax)
+                       to check against to determine onborder
+        onborder_column_name: the column name of the onborder column
+
+    """
+    if gdf is None or len(gdf.index) == 0:
+        return gdf
+
+    result_gdf = gdf.copy()  # type: ignore
+    result_gdf[onborder_column_name] = 0
+
+    # Check
+    for i, geom_row in result_gdf.iterrows():
+        if geom_row["geometry"] is not None and not geom_row["geometry"].is_empty:
+            # Check if the geom is on the border of the tile
+            geom_bounds = geom_row["geometry"].bounds  # type: ignore
+            if (
+                geom_bounds[0] <= border_bounds[0]
+                or geom_bounds[1] <= border_bounds[1]
+                or geom_bounds[2] >= border_bounds[2]
+                or geom_bounds[3] >= border_bounds[3]
+            ):
+                result_gdf.loc[i, onborder_column_name] = 1  # type: ignore
+
+    assert isinstance(result_gdf, gpd.GeoDataFrame)
+    return result_gdf
+
+
+def is_valid_reason(geoseries) -> pd.Series:
+    # Remark: should be moved to geofileops (till available in geopandas)!!!
+    return pd.Series(
+        data=pygeos.is_valid_reason(geoseries.array.data), index=geoseries.index
+    )  # type: ignore
+
+
+def reclassify_neighbours(
+    gdf: gpd.GeoDataFrame,
+    reclassify_column: str,
+    query: str,
+    border_bounds: Optional[Tuple[float, float, float, float]],
+    class_background: str = "background",
+) -> gpd.GeoDataFrame:
+    """
+    For features that comply to the query, if they have a neighbour (touch/overlap),
+    change their classname to that of the neighbour with the longest intersection and
+    dissolve to merge them.
+
+    The query should follow the syntax of pandas.query queries and can us the following
+    fields:
+        - onborder (0 or 1): does the feature touch/overlap the border_bounds. If this
+          field is used in the query, the border_bounds parameter is mandatory.
+        - area (float): the area of the geometry.
+        - perimeter (float): the perimeter of the geometry.
+
+    Args:
+        gdf (gpd.GeoDataFrame): input
+        reclassify_column (str): column to reclassify.
+        query (str): th query to find the features to reclassify.
+        border_bounds (Optional[Tuple[float, float, float, float]]): the bounds of the
+            border to use for th onborder field in the query.
+        class_background (str, optional): the classname to treat as background.
+            Defaults to "background".
+        aggfunc ()
+
+    Raises:
+        ValueError: raised if incompatible parameters are passed.
+
+    Returns:
+        gpd.GeoDataFrame: the reclassified result
+    """
+    # Init column info
+    columns_orig = [col for col in gdf.columns]
+
+    # Init query + needed data
+    query = query.replace("\n", " ")
+
+    def _add_needed_columns(
+        inner_gdf: gpd.GeoDataFrame,
+        inner_query: str,
+        inner_border_bounds: Optional[Tuple[float, float, float, float]],
+    ) -> gpd.GeoDataFrame:
+        gdf_result = inner_gdf.copy()
+
+        # Always add area to know which neighbour is largest
+        gdf_result["area"] = gdf_result.geometry.area
+        if "perimeter" in inner_query:
+            gdf_result["perimeter"] = gdf_result.geometry.length
+        if "onborder" in inner_query:
+            if inner_border_bounds is None:
+                raise ValueError(
+                    "query contains onborder, but border_bounds parameter is None"
+                )
+            gdf_result = is_onborder(gdf_result, inner_border_bounds)  # type: ignore
+
+        # Return result
+        assert isinstance(gdf_result, gpd.GeoDataFrame)
+        return gdf_result
+
+    result_gdf = _add_needed_columns(gdf, query, border_bounds)
+
+    # First remove background polygons that don't match the reclassify query
+    nobackground_query = (
+        f"{reclassify_column} != '{class_background}' or "
+        f"({reclassify_column} == '{class_background}' and "
+        f"({query}))"
+    )
+    # Use copy() to avoid view-versus-copy warnings
+    result_gdf = result_gdf.query(nobackground_query).copy()
+
+    # Keep looking for polygons that comply with query and give the same class
+    # as neighbour till no changes can be made anymore.
+    # Stop after 5 iterations to be sure never to end up in endless loop
+    reclassify_max = 5
+    result_gdf["no_neighbours"] = 0
+    query = f"no_neighbours == 0 and ({query})"
+    for reclassify_counter in range(reclassify_max):
+        # Loop till no features were changed anymore
+        if reclassify_counter > 0:
+            assert isinstance(result_gdf, gpd.GeoDataFrame)
+            result_gdf = _add_needed_columns(result_gdf, query, border_bounds)
+
+        # Use copy() to avoid view-versus-copy warnings
+        result_reclass_gdf = result_gdf.query(query).copy()
+        if len(result_reclass_gdf) == 0:
+            break
+        # Order by area to treat the features found from small to large
+        result_reclass_gdf = result_reclass_gdf.sort_values(by=["area"])
+
+        for row in result_reclass_gdf.itertuples():
+            # Find neighbours (query returns iloc's, not indexes!)
+            neighbours_ilocs = result_gdf.geometry.sindex.query(
+                row.geometry, predicate="intersects"
+            ).tolist()
+            if len(neighbours_ilocs) <= 1:
+                result_gdf.loc[[row.Index], ["no_neighbours"]] = 1
+                continue
+
+            # Remove yourself
+            row_loc = result_gdf.index.get_loc(row.Index)
+            neighbours_ilocs.remove(row_loc)
+
+            # Find neighbour with longest intersection
+            neighbours_gdf = result_gdf.iloc[neighbours_ilocs]
+            inters_geoseries = neighbours_gdf.geometry.intersection(  # type: ignore
+                row.geometry
+            )
+            max_length_index = inters_geoseries.length.idxmax()
+
+            # Change the class of the smallest one to the oher's class
+            class_curr = result_gdf.at[row.Index, reclassify_column]
+            class_neighbour = result_gdf.at[max_length_index, reclassify_column]
+            if class_curr != class_neighbour:
+                # If the neighbour is not a reclass feature or if its area is larger
+                # than the current feature, use its class
+                if (
+                    max_length_index not in result_reclass_gdf.index
+                    or result_gdf.at[max_length_index, "area"] >= row.area
+                ):
+                    result_gdf.loc[[row.Index], [reclassify_column]] = class_neighbour
+                else:
+                    result_gdf.loc[[max_length_index], [reclassify_column]] = class_curr
+
+        # Remove temp columns + dissolve
+        result_gdf = result_gdf[columns_orig + ["no_neighbours"]]
+        dissolve_columns = [reclassify_column, "no_neighbours"]
+        # If there are extra columns, use aggfunc join to concatenate values
+        if len(columns_orig) > 2:
+            result_gdf = result_gdf.dissolve(
+                by=dissolve_columns, as_index=False, aggfunc=", ".join
+            )
+        else:
+            result_gdf = result_gdf.dissolve(by=dissolve_columns, as_index=False)
+
+        result_gdf = result_gdf.explode(ignore_index=True)  # type: ignore
+
+    # Finalize + make sure there is no background in the output
+    result_gdf = result_gdf[columns_orig]
+    # Use copy() to avoid view-versus-copy warnings
+    result_gdf = result_gdf.query(f"{reclassify_column} != '{class_background}'").copy()
+    assert isinstance(result_gdf, gpd.GeoDataFrame)
+    return result_gdf
+
+
+def simplify_topo_orthoseg(
+    geoseries: gpd.GeoSeries,
+    tolerance: float,
+    algorithm: gfo.SimplifyAlgorithm = gfo.SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
+    lookahead: int = 8,
+    keep_points_on: Optional[sh_geom.base.BaseGeometry] = None,
+) -> gpd.GeoSeries:
+    """
+    Applies simplify while retaining common boundaries between geometries in the
+    geoseries.
+
+    This is a specific version for orthoseg that, when algorithm is LANG, applies rdp
+    simplify with halve the tolerance first.
+
+    Args:
+        geoseries (gpd.GeoSeries): the geoseries to simplify.
+        algorithm (SimplifyAlgorithm): algorithm to use.
+        tolerance (float): tolerance to use for simplify
+        lookahead (int, optional): lookahead value for algorithms that use this.
+            Defaults to 8.
+        keep_points_on (Optional[sh_geom.base.BaseGeometry], optional): points that
+            intersect with this geometry won't be removed by the simplification.
+            Defaults to None.
+
+    Returns:
+        gpd.GeoSeries: the simplified geoseries
+    """
+    # Just return empty geoseries
+    if len(geoseries) == 0:
+        return geoseries
+
+    # Copy geoseries
+    geoseries_copy = geoseries.copy()  # type: ignore
+
+    # Set empty geometries to None, if no geometries are left, return
+    empty_idxs = pygeos.is_empty(geoseries_copy.array.data).nonzero()  # type: ignore
+    if len(empty_idxs) > 0:
+        geoseries_copy.iloc[empty_idxs] = None
+    if len(geoseries_copy[geoseries_copy != np.array(None)]) == 0:
+        return geoseries
+
+    topo = topojson.Topology(geoseries_copy, prequantize=False, shared_coords=False)
+    # 46889.5, 211427.5
+    # 46932.5, 211391.5
+
+    def simplify_topolines(
+        _topolines: list,
+        _algorithm: gfo.SimplifyAlgorithm,
+        _tolerance: float,
+        _lookahead: int,
+        _keep_points_on: Optional[sh_geom.base.BaseGeometry],
+    ) -> list:
+        """
+        Internal function that takes care of some plumbing specific to simplifying
+        the lines in the topologies.
+
+        Args:
+            _topolines (list): _description_
+            _algorithm (gfo.SimplifyAlgorithm): _description_
+            _tolerance (float): _description_
+            _lookahead (int): _description_
+            _keep_points_on (Optional[sh_geom.base.BaseGeometry]): _description_
+
+        Returns:
+            list: _description_
+        """
+        topolines_geom = sh_geom.MultiLineString(_topolines)
+        topolines_simpl = geometry_util.simplify_ext(
+            geometry=topolines_geom,
+            tolerance=_tolerance,
+            algorithm=_algorithm,
+            lookahead=_lookahead,
+            keep_points_on=_keep_points_on,
+            preserve_topology=True,
+        )
+        assert topolines_simpl is not None
+
+        # Copy the results of the simplified lines
+        if _algorithm == gfo.SimplifyAlgorithm.LANG:
+            # For LANG, a simple copy is OK
+            if isinstance(topolines_simpl, sh_geom.LineString):
+                return [list(topolines_simpl.coords)]
+            else:
+                assert isinstance(topolines_simpl, sh_geom.MultiLineString)
+                return [list(geom.coords) for geom in topolines_simpl.geoms]
+        else:
+            # For RDP, only overwrite the lines that have a valid result
+            topolines_copy = copy.deepcopy(_topolines)
+            for index in range(len(topolines_copy)):
+                # Get the coordinates of the simplified version
+                if isinstance(topolines_simpl, sh_geom.base.BaseMultipartGeometry):
+                    topoline_simpl = topolines_simpl.geoms[index].coords  # type: ignore
+                else:
+                    topoline_simpl = topolines_simpl.coords
+                # If the result of the simplify is a point, keep original
+                if len(topoline_simpl) < 2:
+                    continue
+                elif (
+                    list(topoline_simpl[0]) != topolines_copy[index][0]
+                    or list(topoline_simpl[-1]) != topolines_copy[index][-1]
+                ):
+                    # Start or end point of the simplified version is not the same
+                    # anymore
+                    continue
+                else:
+                    topolines_copy[index] = list(topoline_simpl)
+
+            return topolines_copy
+
+    if algorithm == gfo.SimplifyAlgorithm.LANG:
+        # For lang, first pre-simplify using rdp
+        topolines_simplified = simplify_topolines(
+            _topolines=topo.output["arcs"],
+            _algorithm=gfo.SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
+            _tolerance=tolerance / 2,
+            _lookahead=lookahead,
+            _keep_points_on=keep_points_on,
+        )
+        for line_id in range(len(topo.output["arcs"])):
+            topo.output["arcs"][line_id] = topolines_simplified[line_id]
+
+        topolines_simplified = simplify_topolines(
+            _topolines=topo.output["arcs"],
+            _algorithm=algorithm,
+            _tolerance=tolerance,
+            _lookahead=lookahead,
+            _keep_points_on=keep_points_on,
+        )
+        for line_id in range(len(topo.output["arcs"])):
+            topo.output["arcs"][line_id] = topolines_simplified[line_id]
+    else:
+        topolines_simplified = simplify_topolines(
+            _topolines=topo.output["arcs"],
+            _algorithm=algorithm,
+            _tolerance=tolerance,
+            _lookahead=lookahead,
+            _keep_points_on=keep_points_on,
+        )
+        for line_id in range(len(topo.output["arcs"])):
+            topo.output["arcs"][line_id] = topolines_simplified[line_id]
+
+    topo_simpl_geoseries = topo.to_gdf(crs=geoseries.crs).geometry
+    assert isinstance(topo_simpl_geoseries, gpd.GeoSeries)
+    topo_simpl_geoseries.array.data = pygeos.make_valid(  # type: ignore
+        topo_simpl_geoseries.array.data  # type: ignore
+    )
+    geometry_types_orig = geoseries.type.unique()
+    geometry_types_orig = geometry_types_orig[geometry_types_orig != None]  # noqa: E711
+    geometry_types_simpl = topo_simpl_geoseries.type.unique()
+    if len(geometry_types_orig) == 1 and (
+        len(geometry_types_simpl) > 1
+        or geometry_types_orig[0] != geometry_types_simpl[0]
+    ):
+        topo_simpl_geoseries = geoseries_util.geometry_collection_extract(
+            topo_simpl_geoseries,
+            gfo.GeometryType(geometry_types_orig[0]).to_primitivetype,
+        )
+    return topo_simpl_geoseries
```

### Comparing `orthoseg-0.4.2/orthoseg.egg-info/PKG-INFO` & `orthoseg-0.4.2a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: orthoseg
-Version: 0.4.2
-Summary: Package to make it easier to segment orthophotos.
-Home-page: https://github.com/orthoseg/orthoseg
-Author: Pieter Roggemans
-Author-email: pieter.roggemans@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.MD
-
-# Orthophoto segmentation
-
-[![Actions Status](https://github.com/orthoseg/orthoseg/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/orthoseg/orthoseg/actions?query=workflow%3ATests) 
-[![PyPI version](https://img.shields.io/pypi/v/orthoseg.svg)](https://pypi.org/project/orthoseg)
-
-This project provides a procedure and (python) scripts to make it (relatively) easy to 
-1. create a training dataset for a topic of your choice
-2. train a neural network to segment orthophotos
-3. run the segmentation on a larger area + vectorize the result
-4. apply some basic postprocessing like dissolve,...
-
-Only open source software is needed, eg. QGIS and tensorflow.
-
-Installation and usage instructions can be found in the [orthoseg wiki](https://github.com/orthoseg/orthoseg/wiki)
+Metadata-Version: 2.1
+Name: orthoseg
+Version: 0.4.2a1
+Summary: Package to make it easier to segment orthophotos.
+Home-page: https://github.com/orthoseg/orthoseg
+Author: Pieter Roggemans
+Author-email: pieter.roggemans@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.MD
+
+# Orthophoto segmentation
+
+[![Actions Status](https://github.com/orthoseg/orthoseg/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/orthoseg/orthoseg/actions?query=workflow%3ATests) 
+[![PyPI version](https://img.shields.io/pypi/v/orthoseg.svg)](https://pypi.org/project/orthoseg)
+
+This project provides a procedure and (python) scripts to make it (relatively) easy to 
+1. create a training dataset for a topic of your choice
+2. train a neural network to segment orthophotos
+3. run the segmentation on a larger area + vectorize the result
+4. apply some basic postprocessing like dissolve,...
+
+Only open source software is needed, eg. QGIS and tensorflow.
+
+Installation and usage instructions can be found in the [orthoseg wiki](https://github.com/orthoseg/orthoseg/wiki)
```

### Comparing `orthoseg-0.4.2/orthoseg.egg-info/SOURCES.txt` & `orthoseg-0.4.2a1/orthoseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.2/tests/test_end2end.py` & `orthoseg-0.4.2a1/tests/test_end2end.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.train.
-"""
-
-from datetime import datetime
-import os
-from pathlib import Path
-import shutil
-import sys
-import tempfile
-
-import gdown
-import geofileops as gfo
-import pytest
-
-# Add path so the local orthoseg packages are found
-root_dir = Path(__file__).resolve().parent.parent
-sys.path.insert(0, str(root_dir))
-import orthoseg
-from orthoseg.helpers import config_helper as conf
-import orthoseg.model.model_helper as mh
-
-from tests.test_helper import TestData
-
-# ----------------------------------------------------
-# Init
-# ----------------------------------------------------
-
-testprojects_dir = Path(tempfile.gettempdir()) / "orthoseg_test_end2end/sample_projects"
-footballfields_dir = testprojects_dir / "footballfields"
-projecttemplate_dir = testprojects_dir / "project_template"
-
-# ----------------------------------------------------
-# Tests
-# ----------------------------------------------------
-
-
-def get_testdata_dir() -> Path:
-    return Path(__file__).resolve().parent / "data"
-
-
-def test_1_init_testproject():
-    # Use footballfields sample project for these end to end tests
-    shutil.rmtree(testprojects_dir, ignore_errors=True)
-    shutil.copytree(TestData.sampleprojects_dir, testprojects_dir)
-
-
-@pytest.mark.order(after="test_1_init_testproject")
-def test_2_load_images():
-    # Load project config to init some vars.
-    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
-    conf.read_orthoseg_config(config_path)
-    image_cache_dir = conf.dirs.getpath("predict_image_input_dir")
-
-    # Clean result if it isn't empty yet
-    if image_cache_dir.exists():
-        shutil.rmtree(image_cache_dir)
-        # Make sure is is deleted now!
-        assert not image_cache_dir.exists()
-
-    # Run task to load images
-    orthoseg.load_images(config_path)
-
-    # Check if the right number of files was loaded
-    assert image_cache_dir.exists()
-    files = list(image_cache_dir.glob("**/*.jpg"))
-    assert len(files) == 4
-
-
-@pytest.mark.skipif(
-    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
-    reason="crashes on github CI on windows",
-)
-@pytest.mark.order(after="test_1_init_testproject")
-def test_3_train():
-    # Load project config to init some vars.
-    config_path = footballfields_dir / "footballfields_train.ini"
-    conf.read_orthoseg_config(config_path)
-
-    # Init + cleanup result dirs
-    traindata_id_result = 2
-    training_dir = conf.dirs.getpath("training_dir")
-    training_id_dir = training_dir / f"{traindata_id_result:02d}"
-    if training_id_dir.exists():
-        shutil.rmtree(training_id_dir)
-    model_dir = conf.dirs.getpath("model_dir")
-    if model_dir.exists():
-        modelfile_paths = model_dir.glob(f"footballfields_{traindata_id_result:02d}_*")
-        for modelfile_path in modelfile_paths:
-            modelfile_path.unlink()
-
-    # Make sure the label files in version 01 are older than those in the label dir
-    # so a new model will be trained
-    label_01_path = training_dir / "01/footballfields_BEFL-2019_polygons.gpkg"
-    timestamp_old = datetime(year=2020, month=1, day=1).timestamp()
-    os.utime(label_01_path, (timestamp_old, timestamp_old))
-
-    # Run train session
-    orthoseg.train(config_path)
-
-    # Check if the training (image) data was created
-    assert training_id_dir.exists()
-
-    # Check if the new model was created
-    best_model = mh.get_best_model(
-        model_dir=conf.dirs.getpath("model_dir"),
-        segment_subject=conf.general["segment_subject"],
-        traindata_id=2,
-    )
-
-    assert best_model is not None
-    assert best_model["traindata_id"] == traindata_id_result
-    assert best_model["epoch"] == 0
-
-
-@pytest.mark.skipif(
-    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
-    reason="crashes on github CI on windows",
-)
-@pytest.mark.order(after="test_2_load_images")
-def test_4_predict():
-    # Load project config to init some vars.
-    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
-    conf.read_orthoseg_config(config_path)
-
-    # Cleanup result if it isn't empty yet
-    predict_image_output_basedir = conf.dirs.getpath("predict_image_output_basedir")
-    predict_image_output_dir = (
-        predict_image_output_basedir.parent
-        / f"{predict_image_output_basedir.name}_footballfields_02_0"
-    )
-    if predict_image_output_dir.exists():
-        shutil.rmtree(predict_image_output_dir)
-        # Make sure it is deleted now!
-        assert not predict_image_output_dir.exists()
-    result_vector_dir = conf.dirs.getpath("output_vector_dir")
-    if result_vector_dir.exists():
-        shutil.rmtree(result_vector_dir)
-        # Make sure is is deleted now!
-        assert not result_vector_dir.exists()
-
-    # Download the version 01 model
-    model_dir = conf.dirs.getpath("model_dir")
-    model_dir.mkdir(parents=True, exist_ok=True)
-    model_hdf5_path = model_dir / "footballfields_01_0.97392_201.hdf5"
-    if not model_hdf5_path.exists():
-        gdown.download(
-            id="1UlNorZ74ADCr3pL4MCJ_tnKRNoeZX79g", output=str(model_hdf5_path)
-        )
-    model_hyperparams_path = model_dir / "footballfields_01_hyperparams.json"
-    if not model_hyperparams_path.exists():
-        gdown.download(
-            id="1NwrVVjx9IsjvaioQ4-bkPMrq7S6HeWIo", output=str(model_hyperparams_path)
-        )
-    model_modeljson_path = model_dir / "footballfields_01_model.json"
-    if not model_modeljson_path.exists():
-        gdown.download(
-            id="1LNPLypM5in3aZngBKK_U4Si47Oe97ZWN", output=str(model_modeljson_path)
-        )
-
-    # Run task to predict
-    orthoseg.predict(config_path)
-
-    # Check results
-    result_vector_path = result_vector_dir / "footballfields_01_201_BEFL-2019.gpkg"
-    assert result_vector_path.exists()
-    result_gdf = gfo.read_file(result_vector_path)
-    if os.name == "nt":
-        assert len(result_gdf) == 233
-    else:
-        # Since 2023-02-17, predict result on linux and Mac became different...
-        assert len(result_gdf) == 259
-
-
-@pytest.mark.skipif(
-    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
-    reason="crashes on github CI on windows",
-)
-@pytest.mark.order(after="test_4_predict")
-def test_5_postprocess():
-    # Load project config to init some vars.
-    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
-    conf.read_orthoseg_config(config_path)
-
-    # Cleanup result if it isn't empty yet
-    result_vector_dir = conf.dirs.getpath("output_vector_dir")
-    result_diss_path = (
-        result_vector_dir / "footballfields_01_201_BEFL-2019_dissolve.gpkg"
-    )
-    if result_diss_path.exists():
-        gfo.remove(result_diss_path)
-
-    # Run task to postprocess
-    orthoseg.postprocess(config_path)
-
-    # Check results
-    assert result_diss_path.exists()
-    result_gdf = gfo.read_file(result_diss_path)
-    if os.name == "nt":
-        assert len(result_gdf) == 227
-    else:
-        # Since 2023-02-17, predict result on linux and Mac became different...
-        assert len(result_gdf) == 239
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.train.
+"""
+
+from datetime import datetime
+import os
+from pathlib import Path
+import shutil
+import sys
+import tempfile
+
+import gdown
+import geofileops as gfo
+import pytest
+
+# Add path so the local orthoseg packages are found
+root_dir = Path(__file__).resolve().parent.parent
+sys.path.insert(0, str(root_dir))
+import orthoseg
+from orthoseg.helpers import config_helper as conf
+import orthoseg.model.model_helper as mh
+
+from tests.test_helper import TestData
+
+# ----------------------------------------------------
+# Init
+# ----------------------------------------------------
+
+testprojects_dir = Path(tempfile.gettempdir()) / "orthoseg_test_end2end/sample_projects"
+footballfields_dir = testprojects_dir / "footballfields"
+projecttemplate_dir = testprojects_dir / "project_template"
+
+# ----------------------------------------------------
+# Tests
+# ----------------------------------------------------
+
+
+def get_testdata_dir() -> Path:
+    return Path(__file__).resolve().parent / "data"
+
+
+def test_1_init_testproject():
+    # Use footballfields sample project for these end to end tests
+    shutil.rmtree(testprojects_dir, ignore_errors=True)
+    shutil.copytree(TestData.sampleprojects_dir, testprojects_dir)
+
+
+@pytest.mark.order(after="test_1_init_testproject")
+def test_2_load_images():
+    # Load project config to init some vars.
+    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
+    conf.read_orthoseg_config(config_path)
+    image_cache_dir = conf.dirs.getpath("predict_image_input_dir")
+
+    # Clean result if it isn't empty yet
+    if image_cache_dir.exists():
+        shutil.rmtree(image_cache_dir)
+        # Make sure is is deleted now!
+        assert not image_cache_dir.exists()
+
+    # Run task to load images
+    orthoseg.load_images(config_path)
+
+    # Check if the right number of files was loaded
+    assert image_cache_dir.exists()
+    files = list(image_cache_dir.glob("**/*.jpg"))
+    assert len(files) == 4
+
+
+@pytest.mark.skipif(
+    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
+    reason="crashes on github CI on windows",
+)
+@pytest.mark.order(after="test_1_init_testproject")
+def test_3_train():
+    # Load project config to init some vars.
+    config_path = footballfields_dir / "footballfields_train.ini"
+    conf.read_orthoseg_config(config_path)
+
+    # Init + cleanup result dirs
+    traindata_id_result = 2
+    training_dir = conf.dirs.getpath("training_dir")
+    training_id_dir = training_dir / f"{traindata_id_result:02d}"
+    if training_id_dir.exists():
+        shutil.rmtree(training_id_dir)
+    model_dir = conf.dirs.getpath("model_dir")
+    if model_dir.exists():
+        modelfile_paths = model_dir.glob(f"footballfields_{traindata_id_result:02d}_*")
+        for modelfile_path in modelfile_paths:
+            modelfile_path.unlink()
+
+    # Make sure the label files in version 01 are older than those in the label dir
+    # so a new model will be trained
+    label_01_path = training_dir / "01/footballfields_BEFL-2019_polygons.gpkg"
+    timestamp_old = datetime(year=2020, month=1, day=1).timestamp()
+    os.utime(label_01_path, (timestamp_old, timestamp_old))
+
+    # Run train session
+    orthoseg.train(config_path)
+
+    # Check if the training (image) data was created
+    assert training_id_dir.exists()
+
+    # Check if the new model was created
+    best_model = mh.get_best_model(
+        model_dir=conf.dirs.getpath("model_dir"),
+        segment_subject=conf.general["segment_subject"],
+        traindata_id=2,
+    )
+
+    assert best_model is not None
+    assert best_model["traindata_id"] == traindata_id_result
+    assert best_model["epoch"] == 0
+
+
+@pytest.mark.skipif(
+    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
+    reason="crashes on github CI on windows",
+)
+@pytest.mark.order(after="test_2_load_images")
+def test_4_predict():
+    # Load project config to init some vars.
+    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
+    conf.read_orthoseg_config(config_path)
+
+    # Cleanup result if it isn't empty yet
+    predict_image_output_basedir = conf.dirs.getpath("predict_image_output_basedir")
+    predict_image_output_dir = (
+        predict_image_output_basedir.parent
+        / f"{predict_image_output_basedir.name}_footballfields_02_0"
+    )
+    if predict_image_output_dir.exists():
+        shutil.rmtree(predict_image_output_dir)
+        # Make sure it is deleted now!
+        assert not predict_image_output_dir.exists()
+    result_vector_dir = conf.dirs.getpath("output_vector_dir")
+    if result_vector_dir.exists():
+        shutil.rmtree(result_vector_dir)
+        # Make sure is is deleted now!
+        assert not result_vector_dir.exists()
+
+    # Download the version 01 model
+    model_dir = conf.dirs.getpath("model_dir")
+    model_dir.mkdir(parents=True, exist_ok=True)
+    model_hdf5_path = model_dir / "footballfields_01_0.97392_201.hdf5"
+    if not model_hdf5_path.exists():
+        gdown.download(
+            id="1UlNorZ74ADCr3pL4MCJ_tnKRNoeZX79g", output=str(model_hdf5_path)
+        )
+    model_hyperparams_path = model_dir / "footballfields_01_hyperparams.json"
+    if not model_hyperparams_path.exists():
+        gdown.download(
+            id="1NwrVVjx9IsjvaioQ4-bkPMrq7S6HeWIo", output=str(model_hyperparams_path)
+        )
+    model_modeljson_path = model_dir / "footballfields_01_model.json"
+    if not model_modeljson_path.exists():
+        gdown.download(
+            id="1LNPLypM5in3aZngBKK_U4Si47Oe97ZWN", output=str(model_modeljson_path)
+        )
+
+    # Run task to predict
+    orthoseg.predict(config_path)
+
+    # Check results
+    result_vector_path = result_vector_dir / "footballfields_01_201_BEFL-2019.gpkg"
+    assert result_vector_path.exists()
+    result_gdf = gfo.read_file(result_vector_path)
+    if os.name == "nt":
+        assert len(result_gdf) == 233
+    else:
+        # Since 2023-02-17, predict result on linux and Mac became different...
+        assert len(result_gdf) == 259
+
+
+@pytest.mark.skipif(
+    "GITHUB_ACTIONS" in os.environ and os.name == "nt",
+    reason="crashes on github CI on windows",
+)
+@pytest.mark.order(after="test_4_predict")
+def test_5_postprocess():
+    # Load project config to init some vars.
+    config_path = footballfields_dir / "footballfields_BEFL-2019.ini"
+    conf.read_orthoseg_config(config_path)
+
+    # Cleanup result if it isn't empty yet
+    result_vector_dir = conf.dirs.getpath("output_vector_dir")
+    result_diss_path = (
+        result_vector_dir / "footballfields_01_201_BEFL-2019_dissolve.gpkg"
+    )
+    if result_diss_path.exists():
+        gfo.remove(result_diss_path)
+
+    # Run task to postprocess
+    orthoseg.postprocess(config_path)
+
+    # Check results
+    assert result_diss_path.exists()
+    result_gdf = gfo.read_file(result_diss_path)
+    if os.name == "nt":
+        assert len(result_gdf) == 227
+    else:
+        # Since 2023-02-17, predict result on linux and Mac became different...
+        assert len(result_gdf) == 239
```

### Comparing `orthoseg-0.4.2/tests/test_helper.py` & `orthoseg-0.4.2a1/tests/test_helper.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-# -*- coding: utf-8 -*-
-"""
-Helper functions for all tests.
-"""
-
-import logging
-from pathlib import Path
-import sys
-import tempfile
-from typing import Optional
-
-import geopandas as gpd
-from shapely import geometry as sh_geom
-
-# Add path so the local geofileops packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-
-
-class TestData:
-    testdata_dir = Path(__file__).resolve().parent / "data"
-    sampleprojects_dir = Path(__file__).resolve().parent.parent / "sample_projects"
-
-    classes = {
-        "background": {
-            "labelnames": ["ignore_for_train", "background"],
-            "weight": 1,
-            "burn_value": 0,
-        },
-        "test_classname1": {"labelnames": ["testlabel1"], "weight": 1, "burn_value": 1},
-        "test_classname2": {"labelnames": ["testlabel2"], "weight": 1, "burn_value": 1},
-    }
-    image_pixel_x_size = 0.25
-    image_pixel_y_size = 0.25
-    image_pixel_width = 512
-    image_pixel_height = 512
-    image_crs_width = image_pixel_width * image_pixel_x_size
-    image_crs_height = image_pixel_height * image_pixel_y_size
-    crs_xmin = 150000
-    crs_ymin = 150000
-    crs = "EPSG:31370"
-    location = sh_geom.box(
-        crs_xmin,
-        crs_ymin,
-        crs_xmin + (image_pixel_width * image_pixel_x_size),
-        crs_ymin + (image_pixel_height * image_pixel_y_size),
-    )
-    location_invalid = sh_geom.Polygon(
-        [
-            (crs_xmin, crs_ymin),
-            (crs_xmin + image_crs_width, crs_ymin),
-            (crs_xmin + image_crs_width, crs_ymin + image_crs_height),
-            (crs_xmin, crs_ymin + image_crs_height),
-            (
-                crs_xmin + image_pixel_x_size,
-                crs_ymin + image_crs_height + image_pixel_y_size,
-            ),
-            (crs_xmin, crs_ymin),
-        ]
-    )
-    polygon = location
-    polygon_invalid = location_invalid
-    locations_gdf = gpd.GeoDataFrame(
-        {
-            "geometry": [location, location, location, location],
-            "traindata_type": ["train", "validation", "test", "todo"],
-            "path": "/tmp/locations.gdf",
-        },
-        crs="epsg:31370",
-    )  # type: ignore
-    polygons_gdf = gpd.GeoDataFrame(
-        {
-            "geometry": [polygon, polygon],
-            "classname": ["testlabel1", "testlabel2"],
-            "path": "/tmp/polygons.gdf",
-        },
-        crs="epsg:31370",
-    )  # type: ignore
-
-
-def create_tempdir(base_dirname: str, parent_dir: Optional[Path] = None) -> Path:
-    # Parent
-    if parent_dir is None:
-        parent_dir = Path(tempfile.gettempdir())
-
-    for i in range(1, 999999):
-        try:
-            tempdir = parent_dir / f"{base_dirname}_{i:06d}"
-            tempdir.mkdir(parents=True)
-            return Path(tempdir)
-        except FileExistsError:
-            continue
-
-    raise Exception(
-        "Wasn't able to create a temporary dir with basedir: "
-        f"{parent_dir / base_dirname}"
-    )
-
-
-def init_test_for_debug(test_module_name: str) -> Path:
-    # Init logging
-    logging.basicConfig(
-        format="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
-        datefmt="%H:%M:%S",
-        level=logging.INFO,
-    )
-
-    # Prepare tmpdir
-    tmp_basedir = Path(tempfile.gettempdir()) / test_module_name
-    tmpdir = create_tempdir(parent_dir=tmp_basedir, base_dirname="debugrun")
-
-    """
-    if tmpdir.exists():
-        shutil.rmtree(tmpdir)
-    tmpdir.mkdir(parents=True, exist_ok=True)
-    """
-
-    return tmpdir
+# -*- coding: utf-8 -*-
+"""
+Helper functions for all tests.
+"""
+
+import logging
+from pathlib import Path
+import sys
+import tempfile
+from typing import Optional
+
+import geopandas as gpd
+from shapely import geometry as sh_geom
+
+# Add path so the local geofileops packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+
+
+class TestData:
+    testdata_dir = Path(__file__).resolve().parent / "data"
+    sampleprojects_dir = Path(__file__).resolve().parent.parent / "sample_projects"
+
+    classes = {
+        "background": {
+            "labelnames": ["ignore_for_train", "background"],
+            "weight": 1,
+            "burn_value": 0,
+        },
+        "test_classname1": {"labelnames": ["testlabel1"], "weight": 1, "burn_value": 1},
+        "test_classname2": {"labelnames": ["testlabel2"], "weight": 1, "burn_value": 1},
+    }
+    image_pixel_x_size = 0.25
+    image_pixel_y_size = 0.25
+    image_pixel_width = 512
+    image_pixel_height = 512
+    image_crs_width = image_pixel_width * image_pixel_x_size
+    image_crs_height = image_pixel_height * image_pixel_y_size
+    crs_xmin = 150000
+    crs_ymin = 150000
+    crs = "EPSG:31370"
+    location = sh_geom.box(
+        crs_xmin,
+        crs_ymin,
+        crs_xmin + (image_pixel_width * image_pixel_x_size),
+        crs_ymin + (image_pixel_height * image_pixel_y_size),
+    )
+    location_invalid = sh_geom.Polygon(
+        [
+            (crs_xmin, crs_ymin),
+            (crs_xmin + image_crs_width, crs_ymin),
+            (crs_xmin + image_crs_width, crs_ymin + image_crs_height),
+            (crs_xmin, crs_ymin + image_crs_height),
+            (
+                crs_xmin + image_pixel_x_size,
+                crs_ymin + image_crs_height + image_pixel_y_size,
+            ),
+            (crs_xmin, crs_ymin),
+        ]
+    )
+    polygon = location
+    polygon_invalid = location_invalid
+    locations_gdf = gpd.GeoDataFrame(
+        {
+            "geometry": [location, location, location, location],
+            "traindata_type": ["train", "validation", "test", "todo"],
+            "path": "/tmp/locations.gdf",
+        },
+        crs="epsg:31370",
+    )  # type: ignore
+    polygons_gdf = gpd.GeoDataFrame(
+        {
+            "geometry": [polygon, polygon],
+            "classname": ["testlabel1", "testlabel2"],
+            "path": "/tmp/polygons.gdf",
+        },
+        crs="epsg:31370",
+    )  # type: ignore
+
+
+def create_tempdir(base_dirname: str, parent_dir: Optional[Path] = None) -> Path:
+    # Parent
+    if parent_dir is None:
+        parent_dir = Path(tempfile.gettempdir())
+
+    for i in range(1, 999999):
+        try:
+            tempdir = parent_dir / f"{base_dirname}_{i:06d}"
+            tempdir.mkdir(parents=True)
+            return Path(tempdir)
+        except FileExistsError:
+            continue
+
+    raise Exception(
+        "Wasn't able to create a temporary dir with basedir: "
+        f"{parent_dir / base_dirname}"
+    )
+
+
+def init_test_for_debug(test_module_name: str) -> Path:
+    # Init logging
+    logging.basicConfig(
+        format="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
+        datefmt="%H:%M:%S",
+        level=logging.INFO,
+    )
+
+    # Prepare tmpdir
+    tmp_basedir = Path(tempfile.gettempdir()) / test_module_name
+    tmpdir = create_tempdir(parent_dir=tmp_basedir, base_dirname="debugrun")
+
+    """
+    if tmpdir.exists():
+        shutil.rmtree(tmpdir)
+    tmpdir.mkdir(parents=True, exist_ok=True)
+    """
+
+    return tmpdir
```

### Comparing `orthoseg-0.4.2/tests/test_load_sampleprojects.py` & `orthoseg-0.4.2a1/tests/test_load_sampleprojects.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.train.
-"""
-
-import os
-from pathlib import Path
-import platform
-import shutil
-import sys
-
-import pytest
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg import load_sampleprojects
-
-# ----------------------------------------------------
-# Tests
-# ----------------------------------------------------
-
-
-def get_testdata_dir() -> Path:
-    return Path(__file__).resolve().parent / "data"
-
-
-@pytest.mark.skipif(
-    "GITHUB_ACTIONS" in os.environ
-    and not (
-        platform.system() == "Linux"
-        and sys.version_info.major == 3
-        and sys.version_info.minor == 10
-    ),
-    reason="on github CI, run this only in one env to avoid rate limit exceeded",
-)
-def test_load_sampleprojects(tmp_path):
-    sampleprojects_dir = tmp_path / "sample_projects"
-    shutil.rmtree(sampleprojects_dir, ignore_errors=True)
-    load_sampleprojects.load_sampleprojects(dest_dir=sampleprojects_dir.parent)
-
-    # Check if the files were correctly loaded
-    assert sampleprojects_dir.exists()
-    assert (sampleprojects_dir / "imagelayers.ini").exists()
-    assert (sampleprojects_dir / "project_defaults_overrule.ini").exists()
-    assert (sampleprojects_dir / "run_footballfields.py").exists()
-
-    footballfields_dir = sampleprojects_dir / "footballfields"
-    assert footballfields_dir.exists()
-    files = list((footballfields_dir).glob("**/*.ini"))
-    assert len(files) > 0
-    files = list((footballfields_dir / "labels").glob("**/*.gpkg"))
-    assert len(files) == 2
-    model_path = footballfields_dir / "models" / "footballfields_01_0.92512_242.hdf5"
-    assert model_path.exists()
-    # The model should be larger than 50 MB, otherwise not normal
-    assert model_path.stat().st_size > 50 * 1024 * 1024
-
-    projecttemplate_dir = sampleprojects_dir / "project_template"
-    assert projecttemplate_dir.exists()
-    files = list((projecttemplate_dir).glob("**/*.ini"))
-    assert len(files) > 0
-    files = list((projecttemplate_dir / "labels").glob("**/*.gpkg"))
-    assert len(files) == 2
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.train.
+"""
+
+import os
+from pathlib import Path
+import platform
+import shutil
+import sys
+
+import pytest
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg import load_sampleprojects
+
+# ----------------------------------------------------
+# Tests
+# ----------------------------------------------------
+
+
+def get_testdata_dir() -> Path:
+    return Path(__file__).resolve().parent / "data"
+
+
+@pytest.mark.skipif(
+    "GITHUB_ACTIONS" in os.environ
+    and not (
+        platform.system() == "Linux"
+        and sys.version_info.major == 3
+        and sys.version_info.minor == 10
+    ),
+    reason="on github CI, run this only in one env to avoid rate limit exceeded",
+)
+def test_load_sampleprojects(tmp_path):
+    sampleprojects_dir = tmp_path / "sample_projects"
+    shutil.rmtree(sampleprojects_dir, ignore_errors=True)
+    load_sampleprojects.load_sampleprojects(dest_dir=sampleprojects_dir.parent)
+
+    # Check if the files were correctly loaded
+    assert sampleprojects_dir.exists()
+    assert (sampleprojects_dir / "imagelayers.ini").exists()
+    assert (sampleprojects_dir / "project_defaults_overrule.ini").exists()
+    assert (sampleprojects_dir / "run_footballfields.py").exists()
+
+    footballfields_dir = sampleprojects_dir / "footballfields"
+    assert footballfields_dir.exists()
+    files = list((footballfields_dir).glob("**/*.ini"))
+    assert len(files) > 0
+    files = list((footballfields_dir / "labels").glob("**/*.gpkg"))
+    assert len(files) == 2
+    model_path = footballfields_dir / "models" / "footballfields_01_0.92512_242.hdf5"
+    assert model_path.exists()
+    # The model should be larger than 50 MB, otherwise not normal
+    assert model_path.stat().st_size > 50 * 1024 * 1024
+
+    projecttemplate_dir = sampleprojects_dir / "project_template"
+    assert projecttemplate_dir.exists()
+    files = list((projecttemplate_dir).glob("**/*.ini"))
+    assert len(files) > 0
+    files = list((projecttemplate_dir / "labels").glob("**/*.gpkg"))
+    assert len(files) == 2
```

### Comparing `orthoseg-0.4.2/tests/test_model_factory.py` & `orthoseg-0.4.2a1/tests/test_model_factory.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.model.model_factory.
-"""
-from pathlib import Path
-import sys
-from typing import Optional
-
-import pytest
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.model import model_factory
-
-
-@pytest.mark.parametrize(
-    "decoder, input_width, input_height, expected_error",
-    [
-        ["linknet", 100, 100, "for decoder linknet"],
-        ["linknet", 256, 256, None],
-        ["pspnet", 144, 144, None],
-        ["unet", 256, 256, None],
-    ],
-)
-def test_check_image_size(
-    decoder: str, input_width: int, input_height: int, expected_error: Optional[str]
-):
-    if expected_error is not None:
-        with pytest.raises(ValueError, match=expected_error):
-            model_factory.check_image_size(
-                decoder=decoder, input_width=input_width, input_height=input_height
-            )
-    else:
-        model_factory.check_image_size(
-            decoder=decoder, input_width=input_width, input_height=input_height
-        )
-
-
-@pytest.mark.parametrize(
-    "architecture, input_width, input_height",
-    [
-        ["mobilenetv2+linknet", 256, 256],
-        ["mobilenetv2+pspnet", 144, 144],
-        ["mobilenetv2+unet", 256, 256],
-    ],
-)
-def test_get_compile_save_load_model(
-    tmp_path, architecture: str, input_width: int, input_height: int
-):
-    # Get model
-    model = model_factory.get_model(
-        architecture=architecture,
-        input_width=input_width,
-        input_height=input_height,
-        nb_classes=5,
-    )
-    assert model is not None
-
-    # Compile model
-    model = model_factory.compile_model(
-        model,
-        optimizer="adam",
-        optimizer_params={"learning_rate": 0.0001},
-        loss="categorical_crossentropy",
-    )
-    assert model is not None
-
-    # Now save model
-    model_path = tmp_path / f"{architecture}.hdf5"
-    model.save(str(model_path))
-    model = None
-
-    # Load model again
-    model = model_factory.load_model(model_path)
-    assert model is not None
-
-
-@pytest.mark.parametrize("architecture", ["mobilenetv2+unknown"])
-def test_get_model_unknown_decoder(architecture: str):
-    with pytest.raises(ValueError, match="Unknown decoder architecture:"):
-        _ = model_factory.get_model(
-            architecture=architecture,
-        )
-
-
-@pytest.mark.parametrize("architecture", ["unknown+unet"])
-def test_get_model_unknown_encoder(architecture: str):
-    # Error is raised by segmentation_models library
-    with pytest.raises(ValueError, match="No such model"):
-        _ = model_factory.get_model(
-            architecture=architecture,
-        )
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.model.model_factory.
+"""
+from pathlib import Path
+import sys
+from typing import Optional
+
+import pytest
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.model import model_factory
+
+
+@pytest.mark.parametrize(
+    "decoder, input_width, input_height, expected_error",
+    [
+        ["linknet", 100, 100, "for decoder linknet"],
+        ["linknet", 256, 256, None],
+        ["pspnet", 144, 144, None],
+        ["unet", 256, 256, None],
+    ],
+)
+def test_check_image_size(
+    decoder: str, input_width: int, input_height: int, expected_error: Optional[str]
+):
+    if expected_error is not None:
+        with pytest.raises(ValueError, match=expected_error):
+            model_factory.check_image_size(
+                decoder=decoder, input_width=input_width, input_height=input_height
+            )
+    else:
+        model_factory.check_image_size(
+            decoder=decoder, input_width=input_width, input_height=input_height
+        )
+
+
+@pytest.mark.parametrize(
+    "architecture, input_width, input_height",
+    [
+        ["mobilenetv2+linknet", 256, 256],
+        ["mobilenetv2+pspnet", 144, 144],
+        ["mobilenetv2+unet", 256, 256],
+    ],
+)
+def test_get_compile_save_load_model(
+    tmp_path, architecture: str, input_width: int, input_height: int
+):
+    # Get model
+    model = model_factory.get_model(
+        architecture=architecture,
+        input_width=input_width,
+        input_height=input_height,
+        nb_classes=5,
+    )
+    assert model is not None
+
+    # Compile model
+    model = model_factory.compile_model(
+        model,
+        optimizer="adam",
+        optimizer_params={"learning_rate": 0.0001},
+        loss="categorical_crossentropy",
+    )
+    assert model is not None
+
+    # Now save model
+    model_path = tmp_path / f"{architecture}.hdf5"
+    model.save(str(model_path))
+    model = None
+
+    # Load model again
+    model = model_factory.load_model(model_path)
+    assert model is not None
+
+
+@pytest.mark.parametrize("architecture", ["mobilenetv2+unknown"])
+def test_get_model_unknown_decoder(architecture: str):
+    with pytest.raises(ValueError, match="Unknown decoder architecture:"):
+        _ = model_factory.get_model(
+            architecture=architecture,
+        )
+
+
+@pytest.mark.parametrize("architecture", ["unknown+unet"])
+def test_get_model_unknown_encoder(architecture: str):
+    # Error is raised by segmentation_models library
+    with pytest.raises(ValueError, match="No such model"):
+        _ = model_factory.get_model(
+            architecture=architecture,
+        )
```

### Comparing `orthoseg-0.4.2/tests/test_ows_util.py` & `orthoseg-0.4.2a1/tests/test_ows_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.train.
-"""
-
-from pathlib import Path
-import sys
-
-import owslib
-import owslib.wms
-import owslib.util
-import pyproj
-import pytest
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.util import ows_util
-
-
-@pytest.mark.parametrize(
-    "crs_epsg, has_switched_axes",
-    [
-        [4326, False],
-        [31370, False],
-        [3059, True],
-        [31468, True],
-    ],
-)
-def test_has_switched_axes(crs_epsg: int, has_switched_axes: bool):
-    assert ows_util._has_switched_axes(pyproj.CRS(crs_epsg)) is has_switched_axes
-
-
-def test_getmap_to_file(tmpdir):
-    # Init some stuff
-    tmpdir = Path(tmpdir)
-    projection = "epsg:31370"
-    pixelsize_x = 0.25
-    pixelsize_y = pixelsize_x
-    image_pixel_width = 512
-    image_pixel_height = image_pixel_width
-    xmin = 160000
-    ymin = 170000
-    bbox = (
-        xmin,
-        ymin,
-        xmin + image_pixel_width * pixelsize_x,
-        ymin + image_pixel_height * pixelsize_y,
-    )
-
-    # Test getting a standard 3 band image from a WMS layer
-    wms_server_url = (
-        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/omw/wms?"
-    )
-    wms_version = "1.3.0"
-    auth = owslib.util.Authentication()
-    wms_service = owslib.wms.WebMapService(
-        wms_server_url, version=wms_version, auth=auth
-    )
-
-    # Two different layers, just use the 1st band from each of them
-    layersources = []
-    layersources.append(
-        ows_util.LayerSource(
-            wms_service=wms_service, layernames=["OMWRGB20VL"], layerstyles=["default"]
-        )
-    )
-
-    # Now get the image...
-    image_filepath = ows_util.getmap_to_file(
-        layersources=layersources,
-        output_dir=tmpdir,
-        crs=projection,
-        bbox=bbox,
-        size=(image_pixel_width, image_pixel_height),
-        image_format=ows_util.FORMAT_PNG,
-        # image_format_save=ows_util.FORMAT_TIFF,
-        image_pixels_ignore_border=0,
-        transparent=False,
-        layername_in_filename=True,
-    )
-
-    assert image_filepath is not None
-    assert image_filepath.exists() is True
-
-    # Test creating greyscale image
-    wms_version = "1.3.0"
-    auth = owslib.util.Authentication()
-    # WMS server for skyview and hillshade
-    wms_server_url_dhm = (
-        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/DHMV/wms?"
-    )
-    wms_service_dhm = owslib.wms.WebMapService(
-        wms_server_url_dhm, version=wms_version, auth=auth
-    )
-    # WMS server for rgb images taken together with dhm2
-    wms_server_url_dhm_ortho = (
-        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/ogw/wms?"
-    )
-    wms_service_dhm_ortho = owslib.wms.WebMapService(
-        wms_server_url_dhm_ortho, version=wms_version, auth=auth
-    )
-
-    # Three different layers, just use one band from each of them
-    layersources = []
-    layersources.append(
-        ows_util.LayerSource(
-            wms_service=wms_service_dhm_ortho, layernames=["OGWRGB13_15VL"], bands=[-1]
-        )
-    )
-
-    # Now get the image...
-    image_filepath = ows_util.getmap_to_file(
-        layersources=layersources,
-        output_dir=tmpdir,
-        crs=projection,
-        bbox=bbox,
-        size=(image_pixel_width, image_pixel_height),
-        image_format=ows_util.FORMAT_PNG,
-        # image_format_save=ows_util.FORMAT_TIFF,
-        image_pixels_ignore_border=0,
-        transparent=False,
-        layername_in_filename=True,
-    )
-
-    assert image_filepath is not None
-    assert image_filepath.exists() is True
-
-    # Test combining bands of 3 different WMS layers
-    wms_version = "1.3.0"
-    auth = owslib.util.Authentication()
-    # WMS server for skyview and hillshade
-    wms_server_url_dhm = (
-        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/DHMV/wms?"
-    )
-    wms_service_dhm = owslib.wms.WebMapService(
-        wms_server_url_dhm, version=wms_version, auth=auth
-    )
-    # WMS server for rgb images taken together with dhm2
-    wms_server_url_dhm_ortho = (
-        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/ogw/wms?"
-    )
-    wms_service_dhm_ortho = owslib.wms.WebMapService(
-        wms_server_url_dhm_ortho, version=wms_version, auth=auth
-    )
-
-    # Three different layers, just use one band from each of them
-    layersources = []
-    layersources.append(
-        ows_util.LayerSource(
-            wms_service=wms_service_dhm, layernames=["DHMV_II_SVF_25cm"], bands=[0]
-        )
-    )
-    layersources.append(
-        ows_util.LayerSource(
-            wms_service=wms_service_dhm, layernames=["DHMV_II_HILL_25cm"], bands=[0]
-        )
-    )
-    layersources.append(
-        ows_util.LayerSource(
-            wms_service=wms_service_dhm_ortho, layernames=["OGWRGB13_15VL"], bands=[-1]
-        )
-    )
-
-    # Now get the image...
-    image_filepath = ows_util.getmap_to_file(
-        layersources=layersources,
-        output_dir=tmpdir,
-        crs=projection,
-        bbox=bbox,
-        size=(image_pixel_width, image_pixel_height),
-        image_format=ows_util.FORMAT_PNG,
-        # image_format_save=ows_util.FORMAT_TIFF,
-        image_pixels_ignore_border=0,
-        transparent=False,
-        layername_in_filename=True,
-    )
-
-    assert image_filepath is not None
-    assert image_filepath.exists() is True
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.train.
+"""
+
+from pathlib import Path
+import sys
+
+import owslib
+import owslib.wms
+import owslib.util
+import pyproj
+import pytest
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.util import ows_util
+
+
+@pytest.mark.parametrize(
+    "crs_epsg, has_switched_axes",
+    [
+        [4326, False],
+        [31370, False],
+        [3059, True],
+        [31468, True],
+    ],
+)
+def test_has_switched_axes(crs_epsg: int, has_switched_axes: bool):
+    assert ows_util._has_switched_axes(pyproj.CRS(crs_epsg)) is has_switched_axes
+
+
+def test_getmap_to_file(tmpdir):
+    # Init some stuff
+    tmpdir = Path(tmpdir)
+    projection = "epsg:31370"
+    pixelsize_x = 0.25
+    pixelsize_y = pixelsize_x
+    image_pixel_width = 512
+    image_pixel_height = image_pixel_width
+    xmin = 160000
+    ymin = 170000
+    bbox = (
+        xmin,
+        ymin,
+        xmin + image_pixel_width * pixelsize_x,
+        ymin + image_pixel_height * pixelsize_y,
+    )
+
+    # Test getting a standard 3 band image from a WMS layer
+    wms_server_url = (
+        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/omw/wms?"
+    )
+    wms_version = "1.3.0"
+    auth = owslib.util.Authentication()
+    wms_service = owslib.wms.WebMapService(
+        wms_server_url, version=wms_version, auth=auth
+    )
+
+    # Two different layers, just use the 1st band from each of them
+    layersources = []
+    layersources.append(
+        ows_util.LayerSource(
+            wms_service=wms_service, layernames=["OMWRGB20VL"], layerstyles=["default"]
+        )
+    )
+
+    # Now get the image...
+    image_filepath = ows_util.getmap_to_file(
+        layersources=layersources,
+        output_dir=tmpdir,
+        crs=projection,
+        bbox=bbox,
+        size=(image_pixel_width, image_pixel_height),
+        image_format=ows_util.FORMAT_PNG,
+        # image_format_save=ows_util.FORMAT_TIFF,
+        image_pixels_ignore_border=0,
+        transparent=False,
+        layername_in_filename=True,
+    )
+
+    assert image_filepath is not None
+    assert image_filepath.exists() is True
+
+    # Test creating greyscale image
+    wms_version = "1.3.0"
+    auth = owslib.util.Authentication()
+    # WMS server for skyview and hillshade
+    wms_server_url_dhm = (
+        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/DHMV/wms?"
+    )
+    wms_service_dhm = owslib.wms.WebMapService(
+        wms_server_url_dhm, version=wms_version, auth=auth
+    )
+    # WMS server for rgb images taken together with dhm2
+    wms_server_url_dhm_ortho = (
+        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/ogw/wms?"
+    )
+    wms_service_dhm_ortho = owslib.wms.WebMapService(
+        wms_server_url_dhm_ortho, version=wms_version, auth=auth
+    )
+
+    # Three different layers, just use one band from each of them
+    layersources = []
+    layersources.append(
+        ows_util.LayerSource(
+            wms_service=wms_service_dhm_ortho, layernames=["OGWRGB13_15VL"], bands=[-1]
+        )
+    )
+
+    # Now get the image...
+    image_filepath = ows_util.getmap_to_file(
+        layersources=layersources,
+        output_dir=tmpdir,
+        crs=projection,
+        bbox=bbox,
+        size=(image_pixel_width, image_pixel_height),
+        image_format=ows_util.FORMAT_PNG,
+        # image_format_save=ows_util.FORMAT_TIFF,
+        image_pixels_ignore_border=0,
+        transparent=False,
+        layername_in_filename=True,
+    )
+
+    assert image_filepath is not None
+    assert image_filepath.exists() is True
+
+    # Test combining bands of 3 different WMS layers
+    wms_version = "1.3.0"
+    auth = owslib.util.Authentication()
+    # WMS server for skyview and hillshade
+    wms_server_url_dhm = (
+        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/DHMV/wms?"
+    )
+    wms_service_dhm = owslib.wms.WebMapService(
+        wms_server_url_dhm, version=wms_version, auth=auth
+    )
+    # WMS server for rgb images taken together with dhm2
+    wms_server_url_dhm_ortho = (
+        "https://geoservices.informatievlaanderen.be/raadpleegdiensten/ogw/wms?"
+    )
+    wms_service_dhm_ortho = owslib.wms.WebMapService(
+        wms_server_url_dhm_ortho, version=wms_version, auth=auth
+    )
+
+    # Three different layers, just use one band from each of them
+    layersources = []
+    layersources.append(
+        ows_util.LayerSource(
+            wms_service=wms_service_dhm, layernames=["DHMV_II_SVF_25cm"], bands=[0]
+        )
+    )
+    layersources.append(
+        ows_util.LayerSource(
+            wms_service=wms_service_dhm, layernames=["DHMV_II_HILL_25cm"], bands=[0]
+        )
+    )
+    layersources.append(
+        ows_util.LayerSource(
+            wms_service=wms_service_dhm_ortho, layernames=["OGWRGB13_15VL"], bands=[-1]
+        )
+    )
+
+    # Now get the image...
+    image_filepath = ows_util.getmap_to_file(
+        layersources=layersources,
+        output_dir=tmpdir,
+        crs=projection,
+        bbox=bbox,
+        size=(image_pixel_width, image_pixel_height),
+        image_format=ows_util.FORMAT_PNG,
+        # image_format_save=ows_util.FORMAT_TIFF,
+        image_pixels_ignore_border=0,
+        transparent=False,
+        layername_in_filename=True,
+    )
+
+    assert image_filepath is not None
+    assert image_filepath.exists() is True
```

### Comparing `orthoseg-0.4.2/tests/test_postprocess_predictions.py` & `orthoseg-0.4.2a1/tests/test_postprocess_predictions.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.lib.postprocess_predictions.
-"""
-import os
-from pathlib import Path
-import sys
-
-import geofileops as gfo
-import pandas as pd
-
-# Make hdf5 version warning non-blocking
-os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.lib import postprocess_predictions as post_pred
-from tests.test_helper import TestData
-
-
-def test_read_prediction_file():
-    # Read + polygonize raster prediction file
-    pred_raster_path = (
-        TestData.testdata_dir / "129568_185248_130592_186272_4096_4096_1_pred.tif"
-    )
-    pred_raster_gdf = post_pred.read_prediction_file(
-        pred_raster_path, border_pixels_to_ignore=128
-    )
-    # gfo.to_file(pred_raster_gdf, get_testdata_dir() / f"{pred_raster_path.stem}.gpkg")
-
-    # Read the comparison file, that contains the result of the polygonize
-    pred_comparison_path = TestData.testdata_dir / f"{pred_raster_path.stem}.gpkg"
-    pred_comparison_gdf = gfo.read_file(pred_comparison_path)
-
-    # Now compare they are the same
-    assert pred_raster_gdf is not None
-    assert len(pred_raster_gdf) == len(pred_comparison_gdf)
-
-
-def test_clean_vectordata(tmpdir):
-    temp_dir = Path(tmpdir)
-
-    # Clean data
-    input1_path = (
-        TestData.testdata_dir / "129568_184288_130592_185312_4096_4096_1_pred.gpkg"
-    )
-    input2_path = (
-        TestData.testdata_dir / "129568_185248_130592_186272_4096_4096_1_pred.gpkg"
-    )
-    input1_gdf = gfo.read_file(input1_path)
-    input2_gdf = gfo.read_file(input2_path)
-    input_gdf = pd.concat([input1_gdf, input2_gdf])
-    assert input1_gdf.crs == input_gdf.crs
-    input_path = temp_dir / "vector_input.gpkg"
-    gfo.to_file(input_gdf, input_path)
-    output_path = temp_dir / input_path.name
-    post_pred.postprocess_predictions(
-        input_path=input_path,
-        output_path=output_path,
-        dissolve=True,
-        dissolve_tiles_path=None,
-        force=True,
-    )
-
-    # Read result and check
-    geoms_simpl_filepath = (
-        output_path.parent / f"{output_path.stem}_dissolve{output_path.suffix}"
-    )
-    result_gdf = gfo.read_file(geoms_simpl_filepath)
-
-    assert len(result_gdf) == 616
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.lib.postprocess_predictions.
+"""
+import os
+from pathlib import Path
+import sys
+
+import geofileops as gfo
+import pandas as pd
+
+# Make hdf5 version warning non-blocking
+os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.lib import postprocess_predictions as post_pred
+from tests.test_helper import TestData
+
+
+def test_read_prediction_file():
+    # Read + polygonize raster prediction file
+    pred_raster_path = (
+        TestData.testdata_dir / "129568_185248_130592_186272_4096_4096_1_pred.tif"
+    )
+    pred_raster_gdf = post_pred.read_prediction_file(
+        pred_raster_path, border_pixels_to_ignore=128
+    )
+    # gfo.to_file(pred_raster_gdf, get_testdata_dir() / f"{pred_raster_path.stem}.gpkg")
+
+    # Read the comparison file, that contains the result of the polygonize
+    pred_comparison_path = TestData.testdata_dir / f"{pred_raster_path.stem}.gpkg"
+    pred_comparison_gdf = gfo.read_file(pred_comparison_path)
+
+    # Now compare they are the same
+    assert pred_raster_gdf is not None
+    assert len(pred_raster_gdf) == len(pred_comparison_gdf)
+
+
+def test_clean_vectordata(tmpdir):
+    temp_dir = Path(tmpdir)
+
+    # Clean data
+    input1_path = (
+        TestData.testdata_dir / "129568_184288_130592_185312_4096_4096_1_pred.gpkg"
+    )
+    input2_path = (
+        TestData.testdata_dir / "129568_185248_130592_186272_4096_4096_1_pred.gpkg"
+    )
+    input1_gdf = gfo.read_file(input1_path)
+    input2_gdf = gfo.read_file(input2_path)
+    input_gdf = pd.concat([input1_gdf, input2_gdf])
+    assert input1_gdf.crs == input_gdf.crs
+    input_path = temp_dir / "vector_input.gpkg"
+    gfo.to_file(input_gdf, input_path)
+    output_path = temp_dir / input_path.name
+    post_pred.postprocess_predictions(
+        input_path=input_path,
+        output_path=output_path,
+        dissolve=True,
+        dissolve_tiles_path=None,
+        force=True,
+    )
+
+    # Read result and check
+    geoms_simpl_filepath = (
+        output_path.parent / f"{output_path.stem}_dissolve{output_path.suffix}"
+    )
+    result_gdf = gfo.read_file(geoms_simpl_filepath)
+
+    assert len(result_gdf) == 616
```

### Comparing `orthoseg-0.4.2/tests/test_prepare_traindata.py` & `orthoseg-0.4.2a1/tests/test_prepare_traindata.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.lib.postprocess_predictions.
-"""
-import os
-from pathlib import Path
-import sys
-from typing import List, Optional, Union
-
-import pytest
-from shapely import geometry as sh_geom
-
-# Make hdf5 version warning non-blocking
-os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
-
-import geopandas as gpd
-import geofileops as gfo
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import config_helper
-from orthoseg.lib import prepare_traindatasets as prep_traindata
-from orthoseg.lib.prepare_traindatasets import ValidationError
-from tests.test_helper import TestData
-
-# ----------------------------------------------------
-# Helper functions to prepare test data
-# ----------------------------------------------------
-
-
-def _prepare_locations_file(
-    tmp_path, locations: Optional[Union[dict, gpd.GeoDataFrame]]
-) -> Path:
-    locations_path = tmp_path / "locations.gpkg"
-    if locations is None:
-        locations = TestData.locations_gdf
-    if isinstance(locations, dict):
-        locations = gpd.GeoDataFrame(locations, crs="EPSG:31370")  # type: ignore
-
-    gfo.to_file(locations, locations_path)
-    return locations_path
-
-
-def _prepare_polygons_file(
-    tmp_path, polygons: Optional[Union[dict, gpd.GeoDataFrame]]
-) -> Path:
-    polygons_path = tmp_path / "polygons.gpkg"
-    if polygons is None:
-        polygons = TestData.polygons_gdf
-    if isinstance(polygons, dict):
-        polygons = gpd.GeoDataFrame(polygons, crs="EPSG:31370")  # type: ignore
-
-    gfo.to_file(polygons, polygons_path)
-    return polygons_path
-
-
-def _prepare_labelinfos(
-    tmp_path,
-    locations: Optional[Union[dict, gpd.GeoDataFrame]] = None,
-    polygons: Optional[Union[dict, gpd.GeoDataFrame]] = None,
-) -> List[prep_traindata.LabelInfo]:
-    locations_path = _prepare_locations_file(tmp_path, locations)
-    polygons_path = _prepare_polygons_file(tmp_path, polygons)
-
-    label_info = prep_traindata.LabelInfo(
-        locations_path=locations_path,
-        polygons_path=polygons_path,
-        image_layer="BEFL-2019",
-    )
-    return [label_info]
-
-
-# Actual tests
-# ------------
-
-
-@pytest.mark.parametrize(
-    "geometry, traindata_type, expected_len_locations",
-    [
-        [TestData.location, "train", 4],
-        [None, "validation", 2],
-        [sh_geom.Polygon(), "validation", 2],
-    ],
-)
-def test_prepare_labeldata_locations(geometry, traindata_type, expected_len_locations):
-    # Prepare test data
-    # Add some extra data to make sure it also works for multiple rows
-    # Prepare test data, by wrapping the parametrized invalid test data by proper data
-    # to make sure the checks work on multiple rows,...
-    locations_gdf = gpd.GeoDataFrame(
-        data={
-            "geometry": [TestData.location, geometry, geometry, TestData.location],
-            "traindata_type": ["train", traindata_type, traindata_type, "validation"],
-            "path": "/tmp/locations.gdf",
-        },
-        crs="EPSG:31370",  # type: ignore
-    )
-    label_info = prep_traindata.LabelInfo(
-        locations_path=Path("locations"),
-        polygons_path=Path("polygons"),
-        image_layer="BEFL-2019",
-        locations_gdf=locations_gdf,
-        polygons_gdf=TestData.polygons_gdf,
-    )
-
-    # Test!
-    labeldata = prep_traindata.prepare_labeldata(
-        label_infos=[label_info],
-        classes=TestData.classes,
-        labelname_column="classname",
-        image_pixel_x_size=TestData.image_pixel_x_size,
-        image_pixel_y_size=TestData.image_pixel_y_size,
-        image_pixel_width=TestData.image_pixel_width,
-        image_pixel_height=TestData.image_pixel_height,
-    )
-    labellocations_gdf, labelpolygons_gdf = labeldata[0]
-
-    assert len(labelpolygons_gdf) == len(TestData.polygons_gdf)
-    assert len(labellocations_gdf) == expected_len_locations
-
-
-@pytest.mark.parametrize(
-    "expected_error, geometry, traindata_type",
-    [
-        ["Invalid geometry ", TestData.location_invalid, "train"],
-        ["Invalid traindata_type ", TestData.location, "invalid_traindata_type"],
-        ["Location geometry too small ", TestData.location.buffer(-5), "train"],
-    ],
-)
-def test_prepare_labeldata_locations_invalid(expected_error, geometry, traindata_type):
-    # Prepare test data, by wrapping the parametrized invalid test data by proper data
-    # to make sure the checks work on multiple rows,...
-    locations_gdf = gpd.GeoDataFrame(
-        data={
-            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
-            "traindata_type": ["train", traindata_type, traindata_type, "validation"],
-            "path": "/tmp/locations.gdf",
-        },
-        crs="EPSG:31370",  # type: ignore
-    )
-    label_info = prep_traindata.LabelInfo(
-        locations_path=Path("locations"),
-        polygons_path=Path("polygons"),
-        image_layer="BEFL-2019",
-        locations_gdf=locations_gdf,
-        polygons_gdf=TestData.polygons_gdf,
-    )
-
-    # Test!
-    with pytest.raises(ValidationError, match="Errors found in label data") as ex:
-        _ = prep_traindata.prepare_labeldata(
-            label_infos=[label_info],
-            classes=TestData.classes,
-            labelname_column="classname",
-            image_pixel_x_size=TestData.image_pixel_x_size,
-            image_pixel_y_size=TestData.image_pixel_y_size,
-            image_pixel_width=TestData.image_pixel_width,
-            image_pixel_height=TestData.image_pixel_height,
-        )
-
-    assert ex.value.errors is not None
-    assert len(ex.value.errors) == 2
-    assert ex.value.errors[0].startswith(expected_error)
-    assert ex.value.errors[1].startswith(expected_error)
-
-
-@pytest.mark.parametrize(
-    "geometry, classname, expected_len_polygons",
-    [
-        [TestData.polygon, "testlabel1", 4],
-        [None, "testlabel1", 2],
-        [sh_geom.Polygon(), "testlabel1", 2],
-    ],
-)
-def test_prepare_labeldata_polygons(geometry, classname, expected_len_polygons):
-    # Prepare test data
-    # Add some extra data to make sure it also works for multiple rows
-    polygons_gdf = gpd.GeoDataFrame(
-        data={
-            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
-            "classname": ["testlabel1", classname, classname, "testlabel2"],
-            "path": "/tmp/polygons.gdf",
-        },
-        crs="EPSG:31370",  # type: ignore
-    )
-    label_info = prep_traindata.LabelInfo(
-        locations_path=Path("locations"),
-        polygons_path=Path("polygons"),
-        image_layer="BEFL-2019",
-        locations_gdf=TestData.locations_gdf,
-        polygons_gdf=polygons_gdf,
-    )
-
-    # Test!
-    labeldata = prep_traindata.prepare_labeldata(
-        label_infos=[label_info],
-        classes=TestData.classes,
-        labelname_column="classname",
-        image_pixel_x_size=TestData.image_pixel_x_size,
-        image_pixel_y_size=TestData.image_pixel_y_size,
-        image_pixel_width=TestData.image_pixel_width,
-        image_pixel_height=TestData.image_pixel_height,
-    )
-    labellocations_gdf, labelpolygons_gdf = labeldata[0]
-
-    assert len(labelpolygons_gdf) == expected_len_polygons
-    assert len(labellocations_gdf) == len(TestData.locations_gdf)
-
-
-@pytest.mark.parametrize(
-    "expected_error, geometry, classname",
-    [
-        ["Invalid geometry ", TestData.polygon_invalid, "testlabel1"],
-        ["Invalid classname ", TestData.polygon, "unknown"],
-    ],
-)
-def test_prepare_labeldata_polygons_invalid(expected_error, geometry, classname):
-    # Prepare test data, by wrapping the parametrized invalid test data by proper data
-    # to make sure the checks work on multiple rows,...
-    polygons_gdf = gpd.GeoDataFrame(
-        data={
-            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
-            "classname": ["testlabel1", classname, classname, "testlabel2"],
-            "path": "/tmp/polygons.gdf",
-        },
-        crs="EPSG:31370",  # type: ignore
-    )
-    label_info = prep_traindata.LabelInfo(
-        locations_path=Path("locations"),
-        polygons_path=Path("polygons"),
-        image_layer="BEFL-2019",
-        locations_gdf=TestData.locations_gdf,
-        polygons_gdf=polygons_gdf,
-    )
-
-    # Test!
-    with pytest.raises(ValidationError, match="Errors found in label data") as ex:
-        _ = prep_traindata.prepare_labeldata(
-            label_infos=[label_info],
-            classes=TestData.classes,
-            labelname_column="classname",
-            image_pixel_x_size=TestData.image_pixel_x_size,
-            image_pixel_y_size=TestData.image_pixel_y_size,
-            image_pixel_width=TestData.image_pixel_width,
-            image_pixel_height=TestData.image_pixel_height,
-        )
-
-    assert ex.value.errors is not None
-    assert len(ex.value.errors) == 2
-    assert ex.value.errors[0].startswith(expected_error)
-    assert ex.value.errors[1].startswith(expected_error)
-
-
-def test_prepare_labeldata_polygons_columnname_backw_compat(tmp_path):
-    # Test bacwards compatibility for old label column name
-    # Prepare test data
-    polygons_gdf = gpd.GeoDataFrame(
-        data={
-            "geometry": [TestData.polygon, TestData.polygon],
-            "label_name": ["testlabel1", "testlabel2"],
-            "path": "/tmp/polygons.gdf",
-        },
-        crs="EPSG:31370",  # type: ignore
-    )
-    label_info = prep_traindata.LabelInfo(
-        locations_path=Path("locations"),
-        polygons_path=Path("polygons"),
-        image_layer="BEFL-2019",
-        locations_gdf=TestData.locations_gdf,
-        polygons_gdf=polygons_gdf,
-    )
-
-    # Test!
-    labeldata = prep_traindata.prepare_labeldata(
-        label_infos=[label_info],
-        classes=TestData.classes,
-        labelname_column="test_columnname",
-        image_pixel_x_size=TestData.image_pixel_x_size,
-        image_pixel_y_size=TestData.image_pixel_y_size,
-        image_pixel_width=TestData.image_pixel_width,
-        image_pixel_height=TestData.image_pixel_height,
-    )
-    locations_gdf, polygons_to_burn_gdf = labeldata[0]
-
-    assert len(polygons_to_burn_gdf) == 2
-
-
-def test_prepare_traindata_full(tmp_path):
-    # Prepare test data
-    classes = TestData.classes
-    image_layers_config_path = TestData.sampleprojects_dir / "imagelayers.ini"
-    image_layers = config_helper.read_layer_config(image_layers_config_path)
-    label_infos = _prepare_labelinfos(tmp_path)
-
-    # Test with the default data...
-    training_dir = tmp_path / "training_dir"
-    training_dir, _ = prep_traindata.prepare_traindatasets(
-        label_infos=label_infos,
-        classes=classes,
-        image_layers=image_layers,
-        training_dir=training_dir,
-        image_pixel_x_size=TestData.image_pixel_x_size,
-        image_pixel_y_size=TestData.image_pixel_y_size,
-        image_pixel_width=TestData.image_pixel_width,
-        image_pixel_height=TestData.image_pixel_height,
-    )
-
-    assert training_dir.exists()
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.lib.postprocess_predictions.
+"""
+import os
+from pathlib import Path
+import sys
+from typing import List, Optional, Union
+
+import pytest
+from shapely import geometry as sh_geom
+
+# Make hdf5 version warning non-blocking
+os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
+
+import geopandas as gpd
+import geofileops as gfo
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import config_helper
+from orthoseg.lib import prepare_traindatasets as prep_traindata
+from orthoseg.lib.prepare_traindatasets import ValidationError
+from tests.test_helper import TestData
+
+# ----------------------------------------------------
+# Helper functions to prepare test data
+# ----------------------------------------------------
+
+
+def _prepare_locations_file(
+    tmp_path, locations: Optional[Union[dict, gpd.GeoDataFrame]]
+) -> Path:
+    locations_path = tmp_path / "locations.gpkg"
+    if locations is None:
+        locations = TestData.locations_gdf
+    if isinstance(locations, dict):
+        locations = gpd.GeoDataFrame(locations, crs="EPSG:31370")  # type: ignore
+
+    gfo.to_file(locations, locations_path)
+    return locations_path
+
+
+def _prepare_polygons_file(
+    tmp_path, polygons: Optional[Union[dict, gpd.GeoDataFrame]]
+) -> Path:
+    polygons_path = tmp_path / "polygons.gpkg"
+    if polygons is None:
+        polygons = TestData.polygons_gdf
+    if isinstance(polygons, dict):
+        polygons = gpd.GeoDataFrame(polygons, crs="EPSG:31370")  # type: ignore
+
+    gfo.to_file(polygons, polygons_path)
+    return polygons_path
+
+
+def _prepare_labelinfos(
+    tmp_path,
+    locations: Optional[Union[dict, gpd.GeoDataFrame]] = None,
+    polygons: Optional[Union[dict, gpd.GeoDataFrame]] = None,
+) -> List[prep_traindata.LabelInfo]:
+    locations_path = _prepare_locations_file(tmp_path, locations)
+    polygons_path = _prepare_polygons_file(tmp_path, polygons)
+
+    label_info = prep_traindata.LabelInfo(
+        locations_path=locations_path,
+        polygons_path=polygons_path,
+        image_layer="BEFL-2019",
+    )
+    return [label_info]
+
+
+# Actual tests
+# ------------
+
+
+@pytest.mark.parametrize(
+    "geometry, traindata_type, expected_len_locations",
+    [
+        [TestData.location, "train", 4],
+        [None, "validation", 2],
+        [sh_geom.Polygon(), "validation", 2],
+    ],
+)
+def test_prepare_labeldata_locations(geometry, traindata_type, expected_len_locations):
+    # Prepare test data
+    # Add some extra data to make sure it also works for multiple rows
+    # Prepare test data, by wrapping the parametrized invalid test data by proper data
+    # to make sure the checks work on multiple rows,...
+    locations_gdf = gpd.GeoDataFrame(
+        data={
+            "geometry": [TestData.location, geometry, geometry, TestData.location],
+            "traindata_type": ["train", traindata_type, traindata_type, "validation"],
+            "path": "/tmp/locations.gdf",
+        },
+        crs="EPSG:31370",  # type: ignore
+    )
+    label_info = prep_traindata.LabelInfo(
+        locations_path=Path("locations"),
+        polygons_path=Path("polygons"),
+        image_layer="BEFL-2019",
+        locations_gdf=locations_gdf,
+        polygons_gdf=TestData.polygons_gdf,
+    )
+
+    # Test!
+    labeldata = prep_traindata.prepare_labeldata(
+        label_infos=[label_info],
+        classes=TestData.classes,
+        labelname_column="classname",
+        image_pixel_x_size=TestData.image_pixel_x_size,
+        image_pixel_y_size=TestData.image_pixel_y_size,
+        image_pixel_width=TestData.image_pixel_width,
+        image_pixel_height=TestData.image_pixel_height,
+    )
+    labellocations_gdf, labelpolygons_gdf = labeldata[0]
+
+    assert len(labelpolygons_gdf) == len(TestData.polygons_gdf)
+    assert len(labellocations_gdf) == expected_len_locations
+
+
+@pytest.mark.parametrize(
+    "expected_error, geometry, traindata_type",
+    [
+        ["Invalid geometry ", TestData.location_invalid, "train"],
+        ["Invalid traindata_type ", TestData.location, "invalid_traindata_type"],
+        ["Location geometry too small ", TestData.location.buffer(-5), "train"],
+    ],
+)
+def test_prepare_labeldata_locations_invalid(expected_error, geometry, traindata_type):
+    # Prepare test data, by wrapping the parametrized invalid test data by proper data
+    # to make sure the checks work on multiple rows,...
+    locations_gdf = gpd.GeoDataFrame(
+        data={
+            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
+            "traindata_type": ["train", traindata_type, traindata_type, "validation"],
+            "path": "/tmp/locations.gdf",
+        },
+        crs="EPSG:31370",  # type: ignore
+    )
+    label_info = prep_traindata.LabelInfo(
+        locations_path=Path("locations"),
+        polygons_path=Path("polygons"),
+        image_layer="BEFL-2019",
+        locations_gdf=locations_gdf,
+        polygons_gdf=TestData.polygons_gdf,
+    )
+
+    # Test!
+    with pytest.raises(ValidationError, match="Errors found in label data") as ex:
+        _ = prep_traindata.prepare_labeldata(
+            label_infos=[label_info],
+            classes=TestData.classes,
+            labelname_column="classname",
+            image_pixel_x_size=TestData.image_pixel_x_size,
+            image_pixel_y_size=TestData.image_pixel_y_size,
+            image_pixel_width=TestData.image_pixel_width,
+            image_pixel_height=TestData.image_pixel_height,
+        )
+
+    assert ex.value.errors is not None
+    assert len(ex.value.errors) == 2
+    assert ex.value.errors[0].startswith(expected_error)
+    assert ex.value.errors[1].startswith(expected_error)
+
+
+@pytest.mark.parametrize(
+    "geometry, classname, expected_len_polygons",
+    [
+        [TestData.polygon, "testlabel1", 4],
+        [None, "testlabel1", 2],
+        [sh_geom.Polygon(), "testlabel1", 2],
+    ],
+)
+def test_prepare_labeldata_polygons(geometry, classname, expected_len_polygons):
+    # Prepare test data
+    # Add some extra data to make sure it also works for multiple rows
+    polygons_gdf = gpd.GeoDataFrame(
+        data={
+            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
+            "classname": ["testlabel1", classname, classname, "testlabel2"],
+            "path": "/tmp/polygons.gdf",
+        },
+        crs="EPSG:31370",  # type: ignore
+    )
+    label_info = prep_traindata.LabelInfo(
+        locations_path=Path("locations"),
+        polygons_path=Path("polygons"),
+        image_layer="BEFL-2019",
+        locations_gdf=TestData.locations_gdf,
+        polygons_gdf=polygons_gdf,
+    )
+
+    # Test!
+    labeldata = prep_traindata.prepare_labeldata(
+        label_infos=[label_info],
+        classes=TestData.classes,
+        labelname_column="classname",
+        image_pixel_x_size=TestData.image_pixel_x_size,
+        image_pixel_y_size=TestData.image_pixel_y_size,
+        image_pixel_width=TestData.image_pixel_width,
+        image_pixel_height=TestData.image_pixel_height,
+    )
+    labellocations_gdf, labelpolygons_gdf = labeldata[0]
+
+    assert len(labelpolygons_gdf) == expected_len_polygons
+    assert len(labellocations_gdf) == len(TestData.locations_gdf)
+
+
+@pytest.mark.parametrize(
+    "expected_error, geometry, classname",
+    [
+        ["Invalid geometry ", TestData.polygon_invalid, "testlabel1"],
+        ["Invalid classname ", TestData.polygon, "unknown"],
+    ],
+)
+def test_prepare_labeldata_polygons_invalid(expected_error, geometry, classname):
+    # Prepare test data, by wrapping the parametrized invalid test data by proper data
+    # to make sure the checks work on multiple rows,...
+    polygons_gdf = gpd.GeoDataFrame(
+        data={
+            "geometry": [TestData.polygon, geometry, geometry, TestData.polygon],
+            "classname": ["testlabel1", classname, classname, "testlabel2"],
+            "path": "/tmp/polygons.gdf",
+        },
+        crs="EPSG:31370",  # type: ignore
+    )
+    label_info = prep_traindata.LabelInfo(
+        locations_path=Path("locations"),
+        polygons_path=Path("polygons"),
+        image_layer="BEFL-2019",
+        locations_gdf=TestData.locations_gdf,
+        polygons_gdf=polygons_gdf,
+    )
+
+    # Test!
+    with pytest.raises(ValidationError, match="Errors found in label data") as ex:
+        _ = prep_traindata.prepare_labeldata(
+            label_infos=[label_info],
+            classes=TestData.classes,
+            labelname_column="classname",
+            image_pixel_x_size=TestData.image_pixel_x_size,
+            image_pixel_y_size=TestData.image_pixel_y_size,
+            image_pixel_width=TestData.image_pixel_width,
+            image_pixel_height=TestData.image_pixel_height,
+        )
+
+    assert ex.value.errors is not None
+    assert len(ex.value.errors) == 2
+    assert ex.value.errors[0].startswith(expected_error)
+    assert ex.value.errors[1].startswith(expected_error)
+
+
+def test_prepare_labeldata_polygons_columnname_backw_compat(tmp_path):
+    # Test bacwards compatibility for old label column name
+    # Prepare test data
+    polygons_gdf = gpd.GeoDataFrame(
+        data={
+            "geometry": [TestData.polygon, TestData.polygon],
+            "label_name": ["testlabel1", "testlabel2"],
+            "path": "/tmp/polygons.gdf",
+        },
+        crs="EPSG:31370",  # type: ignore
+    )
+    label_info = prep_traindata.LabelInfo(
+        locations_path=Path("locations"),
+        polygons_path=Path("polygons"),
+        image_layer="BEFL-2019",
+        locations_gdf=TestData.locations_gdf,
+        polygons_gdf=polygons_gdf,
+    )
+
+    # Test!
+    labeldata = prep_traindata.prepare_labeldata(
+        label_infos=[label_info],
+        classes=TestData.classes,
+        labelname_column="test_columnname",
+        image_pixel_x_size=TestData.image_pixel_x_size,
+        image_pixel_y_size=TestData.image_pixel_y_size,
+        image_pixel_width=TestData.image_pixel_width,
+        image_pixel_height=TestData.image_pixel_height,
+    )
+    locations_gdf, polygons_to_burn_gdf = labeldata[0]
+
+    assert len(polygons_to_burn_gdf) == 2
+
+
+def test_prepare_traindata_full(tmp_path):
+    # Prepare test data
+    classes = TestData.classes
+    image_layers_config_path = TestData.sampleprojects_dir / "imagelayers.ini"
+    image_layers = config_helper.read_layer_config(image_layers_config_path)
+    label_infos = _prepare_labelinfos(tmp_path)
+
+    # Test with the default data...
+    training_dir = tmp_path / "training_dir"
+    training_dir, _ = prep_traindata.prepare_traindatasets(
+        label_infos=label_infos,
+        classes=classes,
+        image_layers=image_layers,
+        training_dir=training_dir,
+        image_pixel_x_size=TestData.image_pixel_x_size,
+        image_pixel_y_size=TestData.image_pixel_y_size,
+        image_pixel_width=TestData.image_pixel_width,
+        image_pixel_height=TestData.image_pixel_height,
+    )
+
+    assert training_dir.exists()
```

### Comparing `orthoseg-0.4.2/tests/test_train.py` & `orthoseg-0.4.2a1/tests/test_train.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.train.
-"""
-
-from pathlib import Path
-import sys
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-import orthoseg
-from tests.test_helper import TestData
-
-
-def test_search_label_files():
-    labeldata_template = (
-        TestData.testdata_dir / "footballfields_{image_layer}_data.gpkg"
-    )
-    labellocation_template = (
-        TestData.testdata_dir / "footballfields_{image_layer}_locations.gpkg"
-    )
-    result = orthoseg._search_label_files(labeldata_template, labellocation_template)
-
-    assert len(result) == 2
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.train.
+"""
+
+from pathlib import Path
+import sys
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+import orthoseg
+from tests.test_helper import TestData
+
+
+def test_search_label_files():
+    labeldata_template = (
+        TestData.testdata_dir / "footballfields_{image_layer}_data.gpkg"
+    )
+    labellocation_template = (
+        TestData.testdata_dir / "footballfields_{image_layer}_locations.gpkg"
+    )
+    result = orthoseg._search_label_files(labeldata_template, labellocation_template)
+
+    assert len(result) == 2
```

### Comparing `orthoseg-0.4.2/tests/test_vector_util.py` & `orthoseg-0.4.2a1/tests/test_vector_util.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.lib.postprocess_predictions.
-"""
-import os
-from pathlib import Path
-import sys
-
-import geopandas as gpd
-from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
-import geofileops as gfo
-import pandas as pd
-from pandas.testing import assert_frame_equal
-import pytest
-from shapely import geometry as sh_geom
-
-# Make hdf5 version warning non-blocking
-os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.util import vector_util
-
-
-@pytest.mark.parametrize("onborder_column_name", ["onborder_custom", "default_value"])
-def test_is_onborder(onborder_column_name: str):
-    # Prepare test data
-    border_bounds = (0.0, 0, 20, 20)
-    expected_onborder_column_name = "expected_onborder"
-    assert expected_onborder_column_name != onborder_column_name
-    columns = ["descr", "geometry", expected_onborder_column_name]
-    testdata = [
-        ["Geom None", None, 0],
-        ["Geom None", None, 0],
-        ["to be removed", None, 0],
-        ["Polygon EMPTY", sh_geom.Polygon(), 0],
-        [
-            "polygon on border",
-            sh_geom.Polygon(shell=[(10, 10), (10, 20), (20, 20), (20, 10), (10, 10)]),
-            1,
-        ],
-        [
-            "polygon not on border",
-            sh_geom.Polygon(shell=[(10, 10), (10, 11), (11, 11), (11, 10), (10, 10)]),
-            0,
-        ],
-    ]
-    df = pd.DataFrame(testdata, columns=columns)
-    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
-    # Remove a row to test if the index is properly maintained
-    testdata_gdf = testdata_gdf.drop([2], axis=0)
-    assert isinstance(testdata_gdf, gpd.GeoDataFrame)
-
-    if onborder_column_name == "default_value":
-        result_gdf = vector_util.is_onborder(testdata_gdf, border_bounds=border_bounds)
-        onborder_column_name = "onborder"
-    else:
-        result_gdf = vector_util.is_onborder(
-            testdata_gdf,
-            border_bounds=border_bounds,
-            onborder_column_name=onborder_column_name,
-        )
-
-    # Compare result with expected result
-    assert onborder_column_name in result_gdf.columns
-    assert onborder_column_name not in testdata_gdf.columns
-    result_gdf[expected_onborder_column_name] = result_gdf[onborder_column_name]
-    result_gdf = result_gdf.drop(columns=[onborder_column_name])
-    assert_geodataframe_equal(testdata_gdf, result_gdf)
-
-    # Test empty GeoDataFrame
-    # --------------------
-    result_gdf = vector_util.is_onborder(
-        gpd.GeoDataFrame(),
-        border_bounds=border_bounds,
-        onborder_column_name=onborder_column_name,
-    )
-    assert result_gdf is not None
-    assert len(result_gdf) == 0
-
-
-def test_reclassify_neighbours():
-    # Prepare test data
-    reclassify_column = "class_name"
-    query = "area <= 20 and onborder == 0"
-    border_bounds = (0.0, 0, 20, 20)
-    columns = ["test_id", "descr", "expected_result", "geometry", reclassify_column]
-    testdata = [
-        ["None1", "Geom None", "disappears", None, "class_1"],
-        ["None2", "Geom None", "disappears", None, "class_1"],
-        ["None3", "to be removed", "disappears", None, "class_1"],
-        ["Empty1", "Polygon EMPTY", "disappears", sh_geom.Polygon(), "class_1"],
-        [
-            "poly1",
-            "large polygon (25m²)",
-            "smaller polygons are added to it",
-            sh_geom.Polygon(shell=[(5, 5), (10, 5), (10, 10), (5, 10), (5, 5)]),
-            "class_1_large",
-        ],
-        [
-            "poly2",
-            "medium (5m²), neighbour of polygon1, onborder",
-            "is onborder, so isn't merged with other things",
-            sh_geom.Polygon(shell=[(0, 5), (0, 6), (5, 6), (5, 5), (0, 5)]),
-            "class_2_medium",
-        ],
-        [
-            "poly3",
-            "small (1m²), neighbour of poly1 and poly4, not onborder",
-            "is merged with poly1",
-            sh_geom.Polygon(shell=[(10, 5), (11, 5), (11, 6), (10, 6), (10, 5)]),
-            "class_3_small",
-        ],
-        [
-            "poly4",
-            "small (1m²), neighbour of poly3, not onborder",
-            "is merged with poly1 and poly3",
-            sh_geom.Polygon(shell=[(11, 5), (12, 5), (12, 6), (11, 6), (11, 5)]),
-            "class_4_small",
-        ],
-        [
-            "poly5",
-            "medium polygon (5m²), larger than neighbour poly6, not onborder",
-            "is merged with poly6 but retains class",
-            sh_geom.Polygon(shell=[(5, 15), (10, 15), (10, 16), (5, 16), (5, 15)]),
-            "class_5_medium",
-        ],
-        [
-            "poly6",
-            "small (1m²), smaller than neighbour poly5, not onborder",
-            "is merged with poly6 and gets its class",
-            sh_geom.Polygon(shell=[(4, 15), (5, 15), (5, 16), (4, 16), (4, 15)]),
-            "class_6_small",
-        ]
-    ]
-    df = pd.DataFrame(testdata, columns=columns)
-    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
-    # Remove a row to test if the index is properly maintained
-    testdata_gdf = testdata_gdf.drop([2], axis=0)
-
-    expected_result_df = pd.DataFrame(
-        [
-            ["poly1, poly3, poly4", "class_1_large"],
-            ["poly2", "class_2_medium"],
-            ["poly5, poly6", "class_5_medium"],
-        ],
-        columns=["test_id", reclassify_column],
-    )
-    # Test with extra column, values are concatenated
-    # -----------------------------------------------
-    # reclassify only supported on gdf with only the reclassify column
-    testdata_prepared_gdf = testdata_gdf[["test_id", "geometry", reclassify_column]]
-    assert isinstance(testdata_prepared_gdf, gpd.GeoDataFrame)
-    result_gdf = vector_util.reclassify_neighbours(
-        testdata_prepared_gdf, reclassify_column, query, border_bounds
-    )
-    assert result_gdf is not None
-    result_df = pd.DataFrame(result_gdf[["test_id", reclassify_column]])
-    assert_frame_equal(result_df, expected_result_df)
-
-    # Test with no extra column
-    # -------------------------
-    expected_result_df = expected_result_df[[reclassify_column]]
-
-    # reclassify only supported on gdf with only the reclassify column
-    testdata_prepared_gdf = testdata_gdf[["geometry", reclassify_column]]
-    assert isinstance(testdata_prepared_gdf, gpd.GeoDataFrame)
-    result_gdf = vector_util.reclassify_neighbours(
-        testdata_prepared_gdf, reclassify_column, query, border_bounds
-    )
-    assert result_gdf is not None
-    result_df = pd.DataFrame(result_gdf[[reclassify_column]])
-    assert_frame_equal(result_df, expected_result_df)
-
-
-def test_simplify_topo_orthoseg():
-    # Test with several different types of geometries
-    # -----------------------------------------------
-    # Prepare test data
-    columns = ["descr", "wkt"]
-    testdata = [
-        ["Geom None", None],
-        ["Geom None", None],
-        ["to be removed", None],
-        ["Polygon EMPTY", "POLYGON(EMPTY)"],
-        [
-            "result=geometrycollection",
-            "POLYGON ((151819.625 213605.125, 151820.625 213605.125, 151820.625 213604.875, 151820.875 213604.875, 151820.875 213604.625, 151821.875 213604.625, 151821.875 213604.375, 151823.125 213604.375, 151823.125 213604.125, 151825.875 213604.125, 151825.875 213603.875, 151828.125 213603.875, 151828.125 213603.625, 151829.375 213603.625, 151829.375 213603.375, 151830.625 213603.375, 151830.625 213603.125, 151831.875 213603.125, 151831.875 213602.875, 151832.625 213602.875, 151832.625 213602.625, 151833.375 213602.625, 151833.375 213602.375, 151834.125 213602.375, 151834.125 213602.125, 151834.375 213602.125, 151834.375 213601.875, 151834.625 213601.875, 151834.625 213601.125, 151834.875 213601.125, 151834.875 213599.875, 151834.625 213599.875, 151834.625 213597.625, 151834.375 213597.625, 151834.375 213594.875, 151834.125 213594.875, 151834.125 213592.125, 151834.375 213592.125, 151834.375 213591.125, 151834.125 213591.125, 151834.125 213590.125, 151833.875 213590.125, 151833.875 213589.375, 151833.625 213589.375, 151833.625 213589.125, 151833.375 213589.125, 151833.375 213588.625, 151833.125 213588.625, 151833.125 213587.875, 151832.875 213587.875, 151832.875 213587.125, 151832.625 213587.125, 151832.625 213585.125, 151832.375 213585.125, 151832.375 213584.625, 151832.125 213584.625, 151832.125 213584.125, 151831.875 213584.125, 151831.875 213583.875, 151831.625 213583.875, 151831.625 213583.125, 151831.375 213583.125, 151831.375 213582.625, 151831.125 213582.625, 151831.125 213582.125, 151830.875 213582.125, 151830.875 213581.875, 151829.375 213581.875, 151829.375 213582.125, 151829.125 213582.125, 151829.125 213582.375, 151828.875 213582.375, 151828.875 213583.125, 151828.625 213583.125, 151828.625 213583.375, 151828.375 213583.375, 151828.375 213583.125, 151827.875 213583.125, 151827.875 213582.875, 151827.625 213582.875, 151827.625 213582.625, 151827.375 213582.625, 151827.375 213582.375, 151826.875 213582.375, 151826.875 213582.125, 151826.625 213582.125, 151826.625 213581.875, 151826.375 213581.875, 151826.375 213581.375, 151826.625 213581.375, 151826.625 213581.125, 151826.875 213581.125, 151826.875 213580.875, 151827.375 213580.875, 151827.375 213581.125, 151829.375 213581.125, 151829.375 213580.875, 151829.875 213580.875, 151829.875 213580.625, 151830.125 213580.625, 151830.125 213580.375, 151830.875 213580.375, 151830.875 213577.875, 151830.625 213577.875, 151830.625 213577.375, 151829.625 213577.375, 151829.625 213577.875, 151829.375 213577.875, 151829.375 213578.125, 151828.875 213578.125, 151828.875 213578.625, 151829.125 213578.625, 151829.125 213579.125, 151828.375 213579.125, 151828.375 213579.375, 151827.875 213579.375, 151827.875 213579.125, 151827.625 213579.125, 151827.625 213578.625, 151827.375 213578.625, 151827.375 213578.375, 151827.125 213578.375, 151827.125 213577.125, 151827.375 213577.125, 151827.375 213576.875, 151827.625 213576.875, 151827.625 213576.625, 151827.875 213576.625, 151827.875 213576.375, 151828.125 213576.375, 151828.125 213576.125, 151828.875 213576.125, 151828.875 213575.875, 151829.125 213575.875, 151829.125 213575.125, 151829.375 213575.125, 151829.375 213574.875, 151828.875 213574.875, 151828.875 213574.625, 151828.375 213574.625, 151828.375 213574.375, 151827.875 213574.375, 151827.875 213574.125, 151827.625 213574.125, 151827.625 213573.875, 151827.375 213573.875, 151827.375 213572.375, 151826.375 213572.375, 151826.375 213572.625, 151825.875 213572.625, 151825.875 213572.875, 151825.625 213572.875, 151825.625 213573.625, 151825.375 213573.625, 151825.375 213574.375, 151824.625 213574.375, 151824.625 213574.125, 151824.125 213574.125, 151824.125 213573.875, 151823.875 213573.875, 151823.875 213574.125, 151823.625 213574.125, 151823.625 213574.375, 151823.125 213574.375, 151823.125 213574.125, 151822.875 213574.125, 151822.875 213573.875, 151822.375 213573.875, 151822.375 213574.125, 151821.125 213574.125, 151821.125 213574.375, 151820.875 213574.375, 151820.875 213574.625, 151819.625 213574.625, 151819.625 213574.875, 151819.125 213574.875, 151819.125 213575.375, 151819.375 213575.375, 151819.375 213575.875, 151819.125 213575.875, 151819.125 213576.125, 151818.375 213576.125, 151818.375 213575.875, 151817.875 213575.875, 151817.875 213575.625, 151817.125 213575.625, 151817.125 213575.375, 151816.625 213575.375, 151816.625 213575.125, 151816.125 213575.125, 151816.125 213575.375, 151815.875 213575.375, 151815.875 213575.125, 151815.625 213575.125, 151815.625 213575.375, 151814.625 213575.375, 151814.625 213575.625, 151814.375 213575.625, 151814.375 213575.875, 151814.625 213575.875, 151814.625 213576.875, 151814.875 213576.875, 151814.875 213578.625, 151815.125 213578.625, 151815.125 213579.375, 151815.375 213579.375, 151815.375 213581.125, 151815.625 213581.125, 151815.625 213583.625, 151815.875 213583.625, 151815.875 213585.125, 151816.125 213585.125, 151816.125 213586.875, 151816.375 213586.875, 151816.375 213588.125, 151816.625 213588.125, 151816.625 213589.375, 151816.875 213589.375, 151816.875 213590.625, 151817.125 213590.625, 151817.125 213592.125, 151817.375 213592.125, 151817.375 213594.125, 151817.625 213594.125, 151817.625 213595.625, 151817.875 213595.625, 151817.875 213597.125, 151818.125 213597.125, 151818.125 213598.375, 151818.375 213598.375, 151818.375 213599.375, 151818.625 213599.375, 151818.625 213599.875, 151818.875 213599.875, 151818.875 213600.375, 151819.125 213600.375, 151819.125 213600.625, 151819.625 213600.625, 151819.625 213600.875, 151819.875 213600.875, 151819.875 213601.375, 151819.625 213601.375, 151819.625 213602.125, 151819.375 213602.125, 151819.375 213602.375, 151819.125 213602.375, 151819.125 213603.625, 151819.375 213603.625, 151819.375 213604.875, 151819.625 213604.875, 151819.625 213605.125), (151828.125 213584.625, 151828.125 213584.375, 151827.625 213584.375, 151827.625 213583.875, 151827.875 213583.875, 151827.875 213583.625, 151828.875 213583.625, 151828.875 213584.375, 151828.375 213584.375, 151828.375 213584.625, 151828.125 213584.625), (151826.375 213573.875, 151826.375 213573.625, 151826.625 213573.625, 151826.625 213573.875, 151826.375 213573.875))",  # noqa: E501
-        ],
-        [
-            "result=linestring",
-            "POLYGON ((6.375 4.375, 6.375 3.875, 6.625 3.875, 6.625 4.375, "
-            "6.375 4.375))",
-        ],
-        [
-            "result=linestring",
-            "POLYGON ((6.625 3.875, 6.625 3.375, 6.875 3.375, 6.875 3.125, "
-            "7.375 3.125, 7.375 3.375, 7.125 3.375, 7.125 3.625, 6.875 3.625, "
-            "6.875 3.875, 6.625 3.875))",
-        ],
-    ]
-    df = pd.DataFrame(testdata, columns=columns)
-    gs = gpd.GeoSeries.from_wkt(df["wkt"])
-    df = df.drop(columns="wkt")
-    testdata_gdf = gpd.GeoDataFrame(df, geometry=gs)  # type: ignore
-    # Remove a row to test if the index is properly maintained in view_angles
-    testdata_gdf = testdata_gdf.drop([2], axis=0)
-
-    simplified_gdf = testdata_gdf.copy()
-    assert isinstance(testdata_gdf.geometry, gpd.GeoSeries)
-    simplified_gdf.geometry = vector_util.simplify_topo_orthoseg(
-        testdata_gdf.geometry, tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
-    )
-    for index, _, geometry in testdata_gdf.itertuples():
-        if geometry is None or geometry.is_empty or index > 4:
-            assert simplified_gdf["geometry"][index] is None
-        else:
-            if index == 4:
-                assert geometry.geom_type == simplified_gdf["geometry"][index].geom_type
-
-    # Test empty geoseries
-    # --------------------
-    result = vector_util.simplify_topo_orthoseg(
-        gpd.GeoSeries(), tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
-    )
-    assert result is not None
-    assert len(result) == 0
-
-    # Test with only empty geometries
-    # -------------------------------
-    # Prepare test data
-    columns = ["descr", "wkt"]
-    testdata = [
-        ["Geom None", None],
-        ["Geom None", None],
-        ["to be removed", None],
-        ["Polygon EMPTY", "POLYGON(EMPTY)"],
-    ]
-    df = pd.DataFrame(testdata, columns=columns)
-    gs = gpd.GeoSeries.from_wkt(df["wkt"])
-    df = df.drop(columns="wkt")
-    testdata_gdf = gpd.GeoDataFrame(df, geometry=gs)  # type: ignore
-    # Remove a row to test if the index is properly maintained in view_angles
-    testdata_gdf = testdata_gdf.drop([2], axis=0)
-
-    simplified_gdf = testdata_gdf.copy()
-    assert isinstance(testdata_gdf.geometry, gpd.GeoSeries)
-    simplified_gdf.geometry = vector_util.simplify_topo_orthoseg(
-        testdata_gdf.geometry, tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
-    )
-    assert_geoseries_equal(testdata_gdf.geometry, simplified_gdf.geometry)
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.lib.postprocess_predictions.
+"""
+import os
+from pathlib import Path
+import sys
+
+import geopandas as gpd
+from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
+import geofileops as gfo
+import pandas as pd
+from pandas.testing import assert_frame_equal
+import pytest
+from shapely import geometry as sh_geom
+
+# Make hdf5 version warning non-blocking
+os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.util import vector_util
+
+
+@pytest.mark.parametrize("onborder_column_name", ["onborder_custom", "default_value"])
+def test_is_onborder(onborder_column_name: str):
+    # Prepare test data
+    border_bounds = (0.0, 0, 20, 20)
+    expected_onborder_column_name = "expected_onborder"
+    assert expected_onborder_column_name != onborder_column_name
+    columns = ["descr", "geometry", expected_onborder_column_name]
+    testdata = [
+        ["Geom None", None, 0],
+        ["Geom None", None, 0],
+        ["to be removed", None, 0],
+        ["Polygon EMPTY", sh_geom.Polygon(), 0],
+        [
+            "polygon on border",
+            sh_geom.Polygon(shell=[(10, 10), (10, 20), (20, 20), (20, 10), (10, 10)]),
+            1,
+        ],
+        [
+            "polygon not on border",
+            sh_geom.Polygon(shell=[(10, 10), (10, 11), (11, 11), (11, 10), (10, 10)]),
+            0,
+        ],
+    ]
+    df = pd.DataFrame(testdata, columns=columns)
+    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
+    # Remove a row to test if the index is properly maintained
+    testdata_gdf = testdata_gdf.drop([2], axis=0)
+    assert isinstance(testdata_gdf, gpd.GeoDataFrame)
+
+    if onborder_column_name == "default_value":
+        result_gdf = vector_util.is_onborder(testdata_gdf, border_bounds=border_bounds)
+        onborder_column_name = "onborder"
+    else:
+        result_gdf = vector_util.is_onborder(
+            testdata_gdf,
+            border_bounds=border_bounds,
+            onborder_column_name=onborder_column_name,
+        )
+
+    # Compare result with expected result
+    assert onborder_column_name in result_gdf.columns
+    assert onborder_column_name not in testdata_gdf.columns
+    result_gdf[expected_onborder_column_name] = result_gdf[onborder_column_name]
+    result_gdf = result_gdf.drop(columns=[onborder_column_name])
+    assert_geodataframe_equal(testdata_gdf, result_gdf)
+
+    # Test empty GeoDataFrame
+    # --------------------
+    result_gdf = vector_util.is_onborder(
+        gpd.GeoDataFrame(),
+        border_bounds=border_bounds,
+        onborder_column_name=onborder_column_name,
+    )
+    assert result_gdf is not None
+    assert len(result_gdf) == 0
+
+
+def test_reclassify_neighbours():
+    # Prepare test data
+    reclassify_column = "class_name"
+    query = "area <= 20 and onborder == 0"
+    border_bounds = (0.0, 0, 20, 20)
+    columns = ["test_id", "descr", "expected_result", "geometry", reclassify_column]
+    testdata = [
+        ["None1", "Geom None", "disappears", None, "class_1"],
+        ["None2", "Geom None", "disappears", None, "class_1"],
+        ["None3", "to be removed", "disappears", None, "class_1"],
+        ["Empty1", "Polygon EMPTY", "disappears", sh_geom.Polygon(), "class_1"],
+        [
+            "poly1",
+            "large polygon (25m²)",
+            "smaller polygons are added to it",
+            sh_geom.Polygon(shell=[(5, 5), (10, 5), (10, 10), (5, 10), (5, 5)]),
+            "class_1_large",
+        ],
+        [
+            "poly2",
+            "medium (5m²), neighbour of polygon1, onborder",
+            "is onborder, so isn't merged with other things",
+            sh_geom.Polygon(shell=[(0, 5), (0, 6), (5, 6), (5, 5), (0, 5)]),
+            "class_2_medium",
+        ],
+        [
+            "poly3",
+            "small (1m²), neighbour of poly1 and poly4, not onborder",
+            "is merged with poly1",
+            sh_geom.Polygon(shell=[(10, 5), (11, 5), (11, 6), (10, 6), (10, 5)]),
+            "class_3_small",
+        ],
+        [
+            "poly4",
+            "small (1m²), neighbour of poly3, not onborder",
+            "is merged with poly1 and poly3",
+            sh_geom.Polygon(shell=[(11, 5), (12, 5), (12, 6), (11, 6), (11, 5)]),
+            "class_4_small",
+        ],
+        [
+            "poly5",
+            "medium polygon (5m²), larger than neighbour poly6, not onborder",
+            "is merged with poly6 but retains class",
+            sh_geom.Polygon(shell=[(5, 15), (10, 15), (10, 16), (5, 16), (5, 15)]),
+            "class_5_medium",
+        ],
+        [
+            "poly6",
+            "small (1m²), smaller than neighbour poly5, not onborder",
+            "is merged with poly6 and gets its class",
+            sh_geom.Polygon(shell=[(4, 15), (5, 15), (5, 16), (4, 16), (4, 15)]),
+            "class_6_small",
+        ]
+    ]
+    df = pd.DataFrame(testdata, columns=columns)
+    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
+    # Remove a row to test if the index is properly maintained
+    testdata_gdf = testdata_gdf.drop([2], axis=0)
+
+    expected_result_df = pd.DataFrame(
+        [
+            ["poly1, poly3, poly4", "class_1_large"],
+            ["poly2", "class_2_medium"],
+            ["poly5, poly6", "class_5_medium"],
+        ],
+        columns=["test_id", reclassify_column],
+    )
+    # Test with extra column, values are concatenated
+    # -----------------------------------------------
+    # reclassify only supported on gdf with only the reclassify column
+    testdata_prepared_gdf = testdata_gdf[["test_id", "geometry", reclassify_column]]
+    assert isinstance(testdata_prepared_gdf, gpd.GeoDataFrame)
+    result_gdf = vector_util.reclassify_neighbours(
+        testdata_prepared_gdf, reclassify_column, query, border_bounds
+    )
+    assert result_gdf is not None
+    result_df = pd.DataFrame(result_gdf[["test_id", reclassify_column]])
+    assert_frame_equal(result_df, expected_result_df)
+
+    # Test with no extra column
+    # -------------------------
+    expected_result_df = expected_result_df[[reclassify_column]]
+
+    # reclassify only supported on gdf with only the reclassify column
+    testdata_prepared_gdf = testdata_gdf[["geometry", reclassify_column]]
+    assert isinstance(testdata_prepared_gdf, gpd.GeoDataFrame)
+    result_gdf = vector_util.reclassify_neighbours(
+        testdata_prepared_gdf, reclassify_column, query, border_bounds
+    )
+    assert result_gdf is not None
+    result_df = pd.DataFrame(result_gdf[[reclassify_column]])
+    assert_frame_equal(result_df, expected_result_df)
+
+
+def test_simplify_topo_orthoseg():
+    # Test with several different types of geometries
+    # -----------------------------------------------
+    # Prepare test data
+    columns = ["descr", "wkt"]
+    testdata = [
+        ["Geom None", None],
+        ["Geom None", None],
+        ["to be removed", None],
+        ["Polygon EMPTY", "POLYGON(EMPTY)"],
+        [
+            "result=geometrycollection",
+            "POLYGON ((151819.625 213605.125, 151820.625 213605.125, 151820.625 213604.875, 151820.875 213604.875, 151820.875 213604.625, 151821.875 213604.625, 151821.875 213604.375, 151823.125 213604.375, 151823.125 213604.125, 151825.875 213604.125, 151825.875 213603.875, 151828.125 213603.875, 151828.125 213603.625, 151829.375 213603.625, 151829.375 213603.375, 151830.625 213603.375, 151830.625 213603.125, 151831.875 213603.125, 151831.875 213602.875, 151832.625 213602.875, 151832.625 213602.625, 151833.375 213602.625, 151833.375 213602.375, 151834.125 213602.375, 151834.125 213602.125, 151834.375 213602.125, 151834.375 213601.875, 151834.625 213601.875, 151834.625 213601.125, 151834.875 213601.125, 151834.875 213599.875, 151834.625 213599.875, 151834.625 213597.625, 151834.375 213597.625, 151834.375 213594.875, 151834.125 213594.875, 151834.125 213592.125, 151834.375 213592.125, 151834.375 213591.125, 151834.125 213591.125, 151834.125 213590.125, 151833.875 213590.125, 151833.875 213589.375, 151833.625 213589.375, 151833.625 213589.125, 151833.375 213589.125, 151833.375 213588.625, 151833.125 213588.625, 151833.125 213587.875, 151832.875 213587.875, 151832.875 213587.125, 151832.625 213587.125, 151832.625 213585.125, 151832.375 213585.125, 151832.375 213584.625, 151832.125 213584.625, 151832.125 213584.125, 151831.875 213584.125, 151831.875 213583.875, 151831.625 213583.875, 151831.625 213583.125, 151831.375 213583.125, 151831.375 213582.625, 151831.125 213582.625, 151831.125 213582.125, 151830.875 213582.125, 151830.875 213581.875, 151829.375 213581.875, 151829.375 213582.125, 151829.125 213582.125, 151829.125 213582.375, 151828.875 213582.375, 151828.875 213583.125, 151828.625 213583.125, 151828.625 213583.375, 151828.375 213583.375, 151828.375 213583.125, 151827.875 213583.125, 151827.875 213582.875, 151827.625 213582.875, 151827.625 213582.625, 151827.375 213582.625, 151827.375 213582.375, 151826.875 213582.375, 151826.875 213582.125, 151826.625 213582.125, 151826.625 213581.875, 151826.375 213581.875, 151826.375 213581.375, 151826.625 213581.375, 151826.625 213581.125, 151826.875 213581.125, 151826.875 213580.875, 151827.375 213580.875, 151827.375 213581.125, 151829.375 213581.125, 151829.375 213580.875, 151829.875 213580.875, 151829.875 213580.625, 151830.125 213580.625, 151830.125 213580.375, 151830.875 213580.375, 151830.875 213577.875, 151830.625 213577.875, 151830.625 213577.375, 151829.625 213577.375, 151829.625 213577.875, 151829.375 213577.875, 151829.375 213578.125, 151828.875 213578.125, 151828.875 213578.625, 151829.125 213578.625, 151829.125 213579.125, 151828.375 213579.125, 151828.375 213579.375, 151827.875 213579.375, 151827.875 213579.125, 151827.625 213579.125, 151827.625 213578.625, 151827.375 213578.625, 151827.375 213578.375, 151827.125 213578.375, 151827.125 213577.125, 151827.375 213577.125, 151827.375 213576.875, 151827.625 213576.875, 151827.625 213576.625, 151827.875 213576.625, 151827.875 213576.375, 151828.125 213576.375, 151828.125 213576.125, 151828.875 213576.125, 151828.875 213575.875, 151829.125 213575.875, 151829.125 213575.125, 151829.375 213575.125, 151829.375 213574.875, 151828.875 213574.875, 151828.875 213574.625, 151828.375 213574.625, 151828.375 213574.375, 151827.875 213574.375, 151827.875 213574.125, 151827.625 213574.125, 151827.625 213573.875, 151827.375 213573.875, 151827.375 213572.375, 151826.375 213572.375, 151826.375 213572.625, 151825.875 213572.625, 151825.875 213572.875, 151825.625 213572.875, 151825.625 213573.625, 151825.375 213573.625, 151825.375 213574.375, 151824.625 213574.375, 151824.625 213574.125, 151824.125 213574.125, 151824.125 213573.875, 151823.875 213573.875, 151823.875 213574.125, 151823.625 213574.125, 151823.625 213574.375, 151823.125 213574.375, 151823.125 213574.125, 151822.875 213574.125, 151822.875 213573.875, 151822.375 213573.875, 151822.375 213574.125, 151821.125 213574.125, 151821.125 213574.375, 151820.875 213574.375, 151820.875 213574.625, 151819.625 213574.625, 151819.625 213574.875, 151819.125 213574.875, 151819.125 213575.375, 151819.375 213575.375, 151819.375 213575.875, 151819.125 213575.875, 151819.125 213576.125, 151818.375 213576.125, 151818.375 213575.875, 151817.875 213575.875, 151817.875 213575.625, 151817.125 213575.625, 151817.125 213575.375, 151816.625 213575.375, 151816.625 213575.125, 151816.125 213575.125, 151816.125 213575.375, 151815.875 213575.375, 151815.875 213575.125, 151815.625 213575.125, 151815.625 213575.375, 151814.625 213575.375, 151814.625 213575.625, 151814.375 213575.625, 151814.375 213575.875, 151814.625 213575.875, 151814.625 213576.875, 151814.875 213576.875, 151814.875 213578.625, 151815.125 213578.625, 151815.125 213579.375, 151815.375 213579.375, 151815.375 213581.125, 151815.625 213581.125, 151815.625 213583.625, 151815.875 213583.625, 151815.875 213585.125, 151816.125 213585.125, 151816.125 213586.875, 151816.375 213586.875, 151816.375 213588.125, 151816.625 213588.125, 151816.625 213589.375, 151816.875 213589.375, 151816.875 213590.625, 151817.125 213590.625, 151817.125 213592.125, 151817.375 213592.125, 151817.375 213594.125, 151817.625 213594.125, 151817.625 213595.625, 151817.875 213595.625, 151817.875 213597.125, 151818.125 213597.125, 151818.125 213598.375, 151818.375 213598.375, 151818.375 213599.375, 151818.625 213599.375, 151818.625 213599.875, 151818.875 213599.875, 151818.875 213600.375, 151819.125 213600.375, 151819.125 213600.625, 151819.625 213600.625, 151819.625 213600.875, 151819.875 213600.875, 151819.875 213601.375, 151819.625 213601.375, 151819.625 213602.125, 151819.375 213602.125, 151819.375 213602.375, 151819.125 213602.375, 151819.125 213603.625, 151819.375 213603.625, 151819.375 213604.875, 151819.625 213604.875, 151819.625 213605.125), (151828.125 213584.625, 151828.125 213584.375, 151827.625 213584.375, 151827.625 213583.875, 151827.875 213583.875, 151827.875 213583.625, 151828.875 213583.625, 151828.875 213584.375, 151828.375 213584.375, 151828.375 213584.625, 151828.125 213584.625), (151826.375 213573.875, 151826.375 213573.625, 151826.625 213573.625, 151826.625 213573.875, 151826.375 213573.875))",  # noqa: E501
+        ],
+        [
+            "result=linestring",
+            "POLYGON ((6.375 4.375, 6.375 3.875, 6.625 3.875, 6.625 4.375, "
+            "6.375 4.375))",
+        ],
+        [
+            "result=linestring",
+            "POLYGON ((6.625 3.875, 6.625 3.375, 6.875 3.375, 6.875 3.125, "
+            "7.375 3.125, 7.375 3.375, 7.125 3.375, 7.125 3.625, 6.875 3.625, "
+            "6.875 3.875, 6.625 3.875))",
+        ],
+    ]
+    df = pd.DataFrame(testdata, columns=columns)
+    gs = gpd.GeoSeries.from_wkt(df["wkt"])
+    df = df.drop(columns="wkt")
+    testdata_gdf = gpd.GeoDataFrame(df, geometry=gs)  # type: ignore
+    # Remove a row to test if the index is properly maintained in view_angles
+    testdata_gdf = testdata_gdf.drop([2], axis=0)
+
+    simplified_gdf = testdata_gdf.copy()
+    assert isinstance(testdata_gdf.geometry, gpd.GeoSeries)
+    simplified_gdf.geometry = vector_util.simplify_topo_orthoseg(
+        testdata_gdf.geometry, tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
+    )
+    for index, _, geometry in testdata_gdf.itertuples():
+        if geometry is None or geometry.is_empty or index > 4:
+            assert simplified_gdf["geometry"][index] is None
+        else:
+            if index == 4:
+                assert geometry.geom_type == simplified_gdf["geometry"][index].geom_type
+
+    # Test empty geoseries
+    # --------------------
+    result = vector_util.simplify_topo_orthoseg(
+        gpd.GeoSeries(), tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
+    )
+    assert result is not None
+    assert len(result) == 0
+
+    # Test with only empty geometries
+    # -------------------------------
+    # Prepare test data
+    columns = ["descr", "wkt"]
+    testdata = [
+        ["Geom None", None],
+        ["Geom None", None],
+        ["to be removed", None],
+        ["Polygon EMPTY", "POLYGON(EMPTY)"],
+    ]
+    df = pd.DataFrame(testdata, columns=columns)
+    gs = gpd.GeoSeries.from_wkt(df["wkt"])
+    df = df.drop(columns="wkt")
+    testdata_gdf = gpd.GeoDataFrame(df, geometry=gs)  # type: ignore
+    # Remove a row to test if the index is properly maintained in view_angles
+    testdata_gdf = testdata_gdf.drop([2], axis=0)
+
+    simplified_gdf = testdata_gdf.copy()
+    assert isinstance(testdata_gdf.geometry, gpd.GeoSeries)
+    simplified_gdf.geometry = vector_util.simplify_topo_orthoseg(
+        testdata_gdf.geometry, tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
+    )
+    assert_geoseries_equal(testdata_gdf.geometry, simplified_gdf.geometry)
```

### Comparing `orthoseg-0.4.2/tests/test_vectorfile_helper.py` & `orthoseg-0.4.2a1/tests/test_vectorfile_helper.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-"""
-Tests for functionalities in orthoseg.lib.postprocess_predictions.
-"""
-import os
-from pathlib import Path
-import sys
-
-import geopandas as gpd
-import geofileops as gfo
-import pandas as pd
-from shapely import geometry as sh_geom
-
-# Make hdf5 version warning non-blocking
-os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
-
-# Add path so the local orthoseg packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.helpers import vectorfile_helper
-
-
-def test_reclassify_neighbours(tmp_path):
-    # Prepare test data
-    reclassify_column = "class_name"
-    query = "area <= 20"
-    columns = ["test_id", "descr", "expected_result", "geometry", reclassify_column]
-    testdata = [
-        ["None1", "Geom None", "disappears", None, "class_1"],
-        ["None2", "Geom None", "disappears", None, "class_1"],
-        ["None3", "to be removed", "disappears", None, "class_1"],
-        ["Empty1", "Polygon EMPTY", "disappears", sh_geom.Polygon(), "class_1"],
-        [
-            "poly1",
-            "large polygon (25m²)",
-            "smaller polygons are added to it",
-            sh_geom.Polygon(shell=[(5, 5), (10, 5), (10, 10), (5, 10), (5, 5)]),
-            "class_1_large",
-        ],
-        [
-            "poly2",
-            "medium (5m²), neighbour of polygon1, onborder",
-            "is onborder, so isn't merged with other things",
-            sh_geom.Polygon(shell=[(0, 5), (0, 6), (5, 6), (5, 5), (0, 5)]),
-            "class_2_medium",
-        ],
-        [
-            "poly3",
-            "neighbour of polygon1, small (1m²), not onborder",
-            "is merged with poly1",
-            sh_geom.Polygon(shell=[(10, 5), (11, 5), (11, 6), (10, 6), (10, 5)]),
-            "class_3_small",
-        ],
-        [
-            "poly4",
-            "neighbour of poly3, small (1m²), not onborder",
-            "is merged with poly1 and poly3",
-            sh_geom.Polygon(shell=[(11, 5), (12, 5), (12, 6), (11, 6), (11, 5)]),
-            "class_4_small",
-        ],
-        [
-            "poly5",
-            "medium polygon (5m²), larger than neighbour poly6, not onborder",
-            "is merged with poly6 but retains class",
-            sh_geom.Polygon(shell=[(5, 15), (10, 15), (10, 16), (5, 16), (5, 15)]),
-            "class_5_medium",
-        ],
-        [
-            "poly6",
-            "small (1m²), smaller than neighbour poly5, not onborder",
-            "is merged with poly6 and gets its class",
-            sh_geom.Polygon(shell=[(4, 15), (5, 15), (5, 16), (4, 16), (4, 15)]),
-            "class_6_small",
-        ]
-    ]
-    df = pd.DataFrame(testdata, columns=columns)
-    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
-    # Remove a row to test if the index is properly maintained
-    testdata_gdf = testdata_gdf.drop([2], axis=0)
-    testdata_path = tmp_path / "testdata.gpkg"
-    gfo.to_file(testdata_gdf, testdata_path)
-
-    # Test
-    result_path = tmp_path / "result.gpkg"
-    vectorfile_helper.reclassify_neighbours(
-        input_path=testdata_path,
-        reclassify_column=reclassify_column, query=query, output_path=result_path
-    )
-    result_gdf = gfo.read_file(result_path)
-    assert result_gdf is not None
-    assert len(result_gdf) == 2
-    assert reclassify_column in result_gdf.columns
-    assert "area" in result_gdf.columns
-    assert "nbcoords" in result_gdf.columns
+# -*- coding: utf-8 -*-
+"""
+Tests for functionalities in orthoseg.lib.postprocess_predictions.
+"""
+import os
+from pathlib import Path
+import sys
+
+import geopandas as gpd
+import geofileops as gfo
+import pandas as pd
+from shapely import geometry as sh_geom
+
+# Make hdf5 version warning non-blocking
+os.environ["HDF5_DISABLE_VERSION_CHECK"] = "1"
+
+# Add path so the local orthoseg packages are found
+sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+from orthoseg.helpers import vectorfile_helper
+
+
+def test_reclassify_neighbours(tmp_path):
+    # Prepare test data
+    reclassify_column = "class_name"
+    query = "area <= 20"
+    columns = ["test_id", "descr", "expected_result", "geometry", reclassify_column]
+    testdata = [
+        ["None1", "Geom None", "disappears", None, "class_1"],
+        ["None2", "Geom None", "disappears", None, "class_1"],
+        ["None3", "to be removed", "disappears", None, "class_1"],
+        ["Empty1", "Polygon EMPTY", "disappears", sh_geom.Polygon(), "class_1"],
+        [
+            "poly1",
+            "large polygon (25m²)",
+            "smaller polygons are added to it",
+            sh_geom.Polygon(shell=[(5, 5), (10, 5), (10, 10), (5, 10), (5, 5)]),
+            "class_1_large",
+        ],
+        [
+            "poly2",
+            "medium (5m²), neighbour of polygon1, onborder",
+            "is onborder, so isn't merged with other things",
+            sh_geom.Polygon(shell=[(0, 5), (0, 6), (5, 6), (5, 5), (0, 5)]),
+            "class_2_medium",
+        ],
+        [
+            "poly3",
+            "neighbour of polygon1, small (1m²), not onborder",
+            "is merged with poly1",
+            sh_geom.Polygon(shell=[(10, 5), (11, 5), (11, 6), (10, 6), (10, 5)]),
+            "class_3_small",
+        ],
+        [
+            "poly4",
+            "neighbour of poly3, small (1m²), not onborder",
+            "is merged with poly1 and poly3",
+            sh_geom.Polygon(shell=[(11, 5), (12, 5), (12, 6), (11, 6), (11, 5)]),
+            "class_4_small",
+        ],
+        [
+            "poly5",
+            "medium polygon (5m²), larger than neighbour poly6, not onborder",
+            "is merged with poly6 but retains class",
+            sh_geom.Polygon(shell=[(5, 15), (10, 15), (10, 16), (5, 16), (5, 15)]),
+            "class_5_medium",
+        ],
+        [
+            "poly6",
+            "small (1m²), smaller than neighbour poly5, not onborder",
+            "is merged with poly6 and gets its class",
+            sh_geom.Polygon(shell=[(4, 15), (5, 15), (5, 16), (4, 16), (4, 15)]),
+            "class_6_small",
+        ]
+    ]
+    df = pd.DataFrame(testdata, columns=columns)
+    testdata_gdf = gpd.GeoDataFrame(df, geometry="geometry")  # type: ignore
+    # Remove a row to test if the index is properly maintained
+    testdata_gdf = testdata_gdf.drop([2], axis=0)
+    testdata_path = tmp_path / "testdata.gpkg"
+    gfo.to_file(testdata_gdf, testdata_path)
+
+    # Test
+    result_path = tmp_path / "result.gpkg"
+    vectorfile_helper.reclassify_neighbours(
+        input_path=testdata_path,
+        reclassify_column=reclassify_column, query=query, output_path=result_path
+    )
+    result_gdf = gfo.read_file(result_path)
+    assert result_gdf is not None
+    assert len(result_gdf) == 2
+    assert reclassify_column in result_gdf.columns
+    assert "area" in result_gdf.columns
+    assert "nbcoords" in result_gdf.columns
```

