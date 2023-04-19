# Comparing `tmp/toxicTrig-0.1.tar.gz` & `tmp/toxicTrig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toxicTrig-0.1.tar", last modified: Tue Apr 18 17:53:06 2023, max compression
+gzip compressed data, was "toxicTrig-0.3.0.tar", last modified: Wed Apr 19 18:51:22 2023, max compression
```

## Comparing `toxicTrig-0.1.tar` & `toxicTrig-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-18 17:53:06.441765 toxicTrig-0.1/
--rw-r--r--   0 xuhuizhou   (501) staff       (20)     1071 2023-04-18 16:06:43.000000 toxicTrig-0.1/LICENSE
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       33 2023-04-18 16:03:47.000000 toxicTrig-0.1/MANIFEST.in
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      616 2023-04-18 17:53:06.441641 toxicTrig-0.1/PKG-INFO
--rw-r--r--   0 xuhuizhou   (501) staff       (20)     1575 2023-04-18 16:12:05.000000 toxicTrig-0.1/README.md
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       38 2023-04-18 17:53:06.441802 toxicTrig-0.1/setup.cfg
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      730 2023-04-18 17:52:23.000000 toxicTrig-0.1/setup.py
-drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-18 17:53:06.441473 toxicTrig-0.1/toxicTrig.egg-info/
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      616 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/PKG-INFO
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      202 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/SOURCES.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)        1 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/dependency_links.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       18 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/requires.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)        1 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/tests/test_analyze_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/tests/test_get_words.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/toxicTrig/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/toxicTrig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/toxicTrig/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/toxicTrig/data/word_based_bias_list.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-19 18:51:07.000000 toxicTrig-0.3.0/toxicTrig/toxic_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:22.233587 toxicTrig-0.3.0/toxicTrig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-19 18:51:22.000000 toxicTrig-0.3.0/toxicTrig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-19 18:51:22.000000 toxicTrig-0.3.0/toxicTrig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:51:22.000000 toxicTrig-0.3.0/toxicTrig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 18:51:22.000000 toxicTrig-0.3.0/toxicTrig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 18:51:22.000000 toxicTrig-0.3.0/toxicTrig.egg-info/top_level.txt
```

### Comparing `toxicTrig-0.1/LICENSE` & `toxicTrig-0.3.0/LICENSE`

 * *Files identical despite different names*

