# Comparing `tmp/cappr-0.2.1.tar.gz` & `tmp/cappr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappr-0.2.1.tar", last modified: Tue Apr  4 19:36:43 2023, max compression
+gzip compressed data, was "cappr-0.2.2.tar", last modified: Wed Apr 19 02:05:05 2023, max compression
```

## Comparing `cappr-0.2.1.tar` & `cappr-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.985874 cappr-0.2.1/
--rw-rw-rw-   0        0        0    11558 2023-03-25 07:21:05.000000 cappr-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    15477 2023-04-04 19:36:43.978870 cappr-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    15079 2023-04-04 00:36:16.000000 cappr-0.2.1/README.md
--rw-rw-rw-   0        0        0      103 2023-03-30 01:16:14.000000 cappr-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 19:36:43.986871 cappr-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1469 2023-04-04 19:26:57.000000 cappr-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.866070 cappr-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.881696 cappr-0.2.1/src/cappr/
--rw-rw-rw-   0        0        0      237 2023-04-04 19:26:39.000000 cappr-0.2.1/src/cappr/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-03-30 01:16:14.000000 cappr-0.2.1/src/cappr/_example.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.928630 cappr-0.2.1/src/cappr/huggingface/
--rw-rw-rw-   0        0        0      183 2023-04-02 17:50:49.000000 cappr-0.2.1/src/cappr/huggingface/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-03-30 16:08:26.000000 cappr-0.2.1/src/cappr/huggingface/_utils.py
--rw-rw-rw-   0        0        0    34687 2023-04-03 18:16:03.000000 cappr-0.2.1/src/cappr/huggingface/classify.py
--rw-rw-rw-   0        0        0    28624 2023-04-03 18:16:32.000000 cappr-0.2.1/src/cappr/huggingface/classify_no_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.953878 cappr-0.2.1/src/cappr/openai/
--rw-rw-rw-   0        0        0       29 2023-03-30 01:16:14.000000 cappr-0.2.1/src/cappr/openai/__init__.py
--rw-rw-rw-   0        0        0    10084 2023-04-03 21:35:34.000000 cappr-0.2.1/src/cappr/openai/api.py
--rw-rw-rw-   0        0        0    21476 2023-04-03 18:15:27.000000 cappr-0.2.1/src/cappr/openai/classify.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.974876 cappr-0.2.1/src/cappr/utils/
--rw-rw-rw-   0        0        0       40 2023-03-30 01:16:14.000000 cappr-0.2.1/src/cappr/utils/__init__.py
--rw-rw-rw-   0        0        0     3816 2023-03-30 01:16:14.000000 cappr-0.2.1/src/cappr/utils/_batch.py
--rw-rw-rw-   0        0        0      755 2023-04-03 20:56:42.000000 cappr-0.2.1/src/cappr/utils/_check.py
--rw-rw-rw-   0        0        0    12215 2023-04-02 20:27:50.000000 cappr-0.2.1/src/cappr/utils/classify.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:36:43.928630 cappr-0.2.1/src/cappr.egg-info/
--rw-rw-rw-   0        0        0    15477 2023-04-04 19:36:43.000000 cappr-0.2.1/src/cappr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-04-04 19:36:43.000000 cappr-0.2.1/src/cappr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 19:36:43.000000 cappr-0.2.1/src/cappr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      447 2023-04-04 19:36:43.000000 cappr-0.2.1/src/cappr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 19:36:43.000000 cappr-0.2.1/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.966942 cappr-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.970942 cappr-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-19 02:04:53.000000 cappr-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-19 02:04:53.000000 cappr-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 02:04:53.000000 cappr-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 02:04:53.000000 cappr-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:04:53.000000 cappr-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-19 02:05:05.982943 cappr-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-04-19 02:04:53.000000 cappr-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.970942 cappr-0.2.2/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/computational_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/demos/raft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/ade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/b77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/nis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/ose.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/over.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/sot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/sri.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/teh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tos.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/demos/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/superglue/copa.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/superglue/wsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/1_is_for_me.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/2_motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/3_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/4_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/5_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/6_computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/7_future_research.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/github-mark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/scaling_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/scaling_classes/batch_size_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.classify_no_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.utils.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/related_work.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/research.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 02:04:53.000000 cappr-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 02:05:05.982943 cappr-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-19 02:04:53.000000 cappr-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.966942 cappr-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/classify_no_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/huggingface/test_huggingface_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/openai/test_openai_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/utils/test_utils_classify.py
```

### Comparing `cappr-0.2.1/LICENSE` & `cappr-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `cappr-0.2.1/PKG-INFO` & `cappr-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,448 +1,439 @@
-Metadata-Version: 2.1
-Name: cappr
-Version: 0.2.1
-Summary: Zero-shot text classification using autoregressive language models.
-Home-page: https://github.com/kddubey/cappr/
-Author-email: kushdubey63@gmail.com
-License: Apache License 2.0
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: hf
-Provides-Extra: demos
-Provides-Extra: dev
-License-File: LICENSE
-
-# CAPPr: zero-shot text classification using autoregressive language models
-
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
-[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-Perform zero-shot text classification by estimating the probability that an inputted
-completion comes after an inputted prompt. Hence the name:
-
-> **C**ompletion<br>
-  **A**fter<br>
-  **P**rompt<br>
-  **Pr**obability<br>
-
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
-
-## Usage
-
-<details>
-<summary>Use a model from the OpenAI API</summary>
-
-Specifically, this model must be compatible with the
-[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-endpoint.
-
-Let's classify
-[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
-from the OpenAI text completion docs.
-
-```python
-from cappr.openai.classify import predict
-
-tweet = 'I loved the new Batman movie!'
-prompt = f'Tweet: {tweet}\nSentiment:'
-
-class_names = ('positive', 'neutral', 'negative')
-# optional: let's supply a prior distribution over the classes
-prior       = (   1/8    ,    1/8   ,     3/4   )
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='text-ada-001',
-                prior=prior)
-preds
-# ['positive']
-```
-</details>
-
-<details>
-<summary>Use a model from the HuggingFace model hub</summary>
-
-Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
-
-```python
-from cappr.huggingface.classify import predict
-
-prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
-
-class_names = ('Mercury', 'Earth')
-prior = None  # uniform prior
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='gpt2',
-                prior=prior)
-preds
-# ['Mercury']
-```
-</details>
-
-<details>
-<summary>Run in batches</summary>
-
-Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
-instead of the class.
-
-```python
-from cappr.huggingface.classify import predict_proba
-
-prompts = [
-    'Stephen Curry is a',
-    'Martina Navratilova was a',
-    "Dexter, from the TV Series Dexter's Laboratory, is a",
-    'LeBron James is a',    
-]
-
-# each of the prompts could be completed with one of these:
-class_names = (
-    'basketball player',
-    'tennis player',
-    'scientist'
-)
-
-prior = (
-    1/6,  # few
-    1/6,  # few
-    2/3   # there are more
-)
-
-pred_probs = predict_proba(prompts=prompts,
-                           completions=class_names,
-                           model='gpt2',
-                           batch_size=32,  # whatever fits on your CPU/GPU
-                           prior=prior)
-
-# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
-print(pred_probs.round(1))
-# [[0.5 0.3 0.2]
-#  [0.3 0.6 0.2]
-#  [0.1 0.1 0.8]
-#  [0.8 0.2 0. ]]
-
-# for each prompt, which completion is most likely?
-pred_class_idxs = pred_probs.argmax(axis=1)
-print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
-# ['basketball player',
-#  'tennis player',
-#  'scientist',
-#  'basketball player']
-```
-</details>
-
-<details>
-<summary>Run in batches, where each prompt has a different set of possible completions
-</summary>
-
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
-
-```python
-import numpy as np
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-from cappr import Example
-from cappr.huggingface.classify import predict_proba_examples
-
-examples = [
-    Example(prompt='Jodie Foster played',
-            completions=('Clarice Starling', 'Trinity in The Matrix')),
-    Example(prompt='Batman, from Batman: The Animated Series, was played by',
-            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
-            prior=      (     1/3      ,      2/3     ,      0      ))
-]
-
-model_name = 'gpt2'
-model = AutoModelForCausalLM.from_pretrained(model_name)
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-pred_probs = predict_proba_examples(examples,
-                                    model_and_tokenizer=(model, tokenizer))
-
-# pred_probs[i][j] = probability that examples[i].prompt is classified as
-# examples[i].completions[j]
-print([example_pred_probs.round(2)
-       for example_pred_probs in pred_probs])
-# [array([0.7, 0.3]),
-#  array([0.03, 0.97, 0.  ])]
-
-# for each example, which completion is most likely?
-pred_class_idxs = [np.argmax(example_pred_probs)
-                   for example_pred_probs in pred_probs]
-print([example.completions[pred_class_idx]
-       for example, pred_class_idx in zip(examples, pred_class_idxs)])
-# ['Clarice Starling',
-#  'Kevin Conroy']
-```
-</details>
-
-More examples are linked [here in the
-documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
-
-See [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-for a demonstration of a slightly harder classification task.
-
-
-## Documentation
-
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
-
-
-## Setup
-
-If you intend on using OpenAI models, [sign up for the OpenAI API
-here](https://platform.openai.com/signup), and then set the environment variable
-`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
-others. But using them will cost ya 💰!
-
-Install with `pip`:
-
-```
-python -m pip install cappr
-```
-
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
-
-```
-python -m pip install cappr[hf]
-```
-</details>
-
-<details>
-<summary>(Optional) Set up to run demos</summary>
-
-```
-python -m pip install cappr[demos]
-```
-</details>
-
-
-## Motivation
-
-Create a more usable zero-shot text classification interface than
-[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
-
-<details>
-<summary>Short</summary>
-
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
-
-In CAPPr, your job starts and stops at writing up your classification task as a
-`{prompt}{end_of_prompt}{completion}` string.
-</details>
-
-<details>
-<summary>Long</summary>
-
-Please see [this page of the
-documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
-
-</details>
-
-<details>
-<summary>Unstudied</summary>
-
-I'm curious to see how much easier estimation/discrimination is than generation.
-In [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb),
-CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
-accurate.
-
-</details>
-
-<details>
-<summary>Honest</summary>
-
-Keep myself busy
-
-</details>
-
-
-## Results
-
-<details>
-<summary>
-Statistical performance
-</summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
-
-  * [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-  * [`demos/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb)
-</details>
-
-
-<details>
-<summary>
-Computational performance
-</summary>
-
-One concern was that CAPPr requires as many `model()` calls as there are classes. But in
-the CAPPr scheme, we can simply cache each attention block's keys and values for the
-prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
-code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
-the implementation. Note that this caching is not implemented for OpenAI models, as I
-can't control their backend. **This means that when running `cappr.openai` functions,
-you'll be on the *cappr (slow)* line** :-(
-
-![](/docs/source/_static/scaling_classes/batch_size_32.png)
-
-*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
-choices to simulate multi-class classification tasks. [GPT-2
-(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
-
-See the [`demos/computational_analysis.ipynb`
-notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
-
-</details>
-
-
-## Related work
-
-While [benchmarking this
-method](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb) on the Winograd
-Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847) is very
-similar:
-
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
-
-[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
-probabilities to do prompt-completion classification, but these probabilities are
-assumed to come from masked language models like BERT.
-
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
-
-
-## Contributing
-
-TODO
-
-
-## Testing
-
-### Setup
-
-1. Clone the repo
-
-   ```
-   git clone https://github.com/kddubey/cappr.git
-   ```
-
-2. Create a new Python 3.8+ environment
-
-3. Install this package in editable mode, along with development requirements
-
-   ```
-   python -m pip install -e .[dev]
-   ```
-
-### Run tests
-
-```
-pytest
-```
-
-Dumping VS code extensions for development:
-  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
-  Use the numpy format.
-  * [Set Python formatting to
-    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
-  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
-  * [TOML Language
-    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
-
-
-## Todo
-
-(**) = I'm currently working on this or will work on it really soon
-
-<details>
-<summary>Code</summary>
-
-- [ ] Testing
-  - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
-  - [ ] Test input checks
-- [x] Small CPU speed-ups
-  - [x] For constant-completions input, vectorize `agg_log_probs`
-  - [x] For `examples` input, if # completions per prompt is constant, vectorize
-  `posterior_prob`
-- [ ] Add getLogger, basic logging
-- [ ] Make progress bars optional, since inference often isn't batched
-- [ ] Factor out input checks (on prompts and completions)
-- [x] De-automate overzealous auto-docstring stuff :-(
-- [ ] HuggingFace `transformers.AutoModelForCausalLM`
-  - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
-    - [ ] Get to the bottom of why it's slower w/o batching
-  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
-  think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
-  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
-  - [ ] Support [Inference
-    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
-  - [ ] Support priming, as in: cache it
-- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
-- [ ] Allow for multi-label classification
-  - [ ] Pass `normalize` as an argument to predict_proba functions
-  - [ ] For `huggingface`, add note that you'll get faster results by passing all
-  labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
-- [ ] Fill in missing or non-numpy docstrings
-</details>
-
-<details>
-<summary>Research</summary>
-
-Evaluate on more datasets, and understand its relative advantages and disadvantages vs
-other classification methods.
-
-- [ ] RAFT benchmark (**)
-- [ ] Create a user guide, build a table of results comparing competing approaches on
-statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
-  - [ ] Process inputs 1-by-1
-- [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
-- [ ] Calibration
-  - [ ] Is the prior actually effective? Downsample and see
-  - [ ] curves
-- [ ] Compare against few-shot embeddings
-- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
-  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
-  - [ ] Again, compare against sampling
-- [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
-</details>
+# CAPPr: zero-shot text classification using autoregressive language models
+
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
+[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+Perform zero-shot text classification by estimating the probability that an inputted
+completion comes after an inputted prompt. Hence the name:
+
+> **C**ompletion<br>
+  **A**fter<br>
+  **P**rompt<br>
+  **Pr**obability<br>
+
+The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+
+## Usage
+
+<details>
+<summary>Use a model from the OpenAI API</summary>
+
+Specifically, this model must be compatible with the
+[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+endpoint.
+
+Let's classify
+[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
+from the OpenAI text completion docs.
+
+```python
+from cappr.openai.classify import predict
+
+tweet = 'I loved the new Batman movie!'
+prompt = f'Tweet: {tweet}\nSentiment:'
+
+class_names = ('positive', 'neutral', 'negative')
+# optional: let's supply a prior distribution over the classes
+prior       = (   1/8    ,    1/8   ,     3/4   )
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='text-ada-001',
+                prior=prior)
+preds
+# ['positive']
+```
+</details>
+
+<details>
+<summary>Use a model from the HuggingFace model hub</summary>
+
+Specifically, this model must be able to be loaded using
+`transformers.AutoModelForCausalLM.from_pretrained(model)`.
+
+Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+
+```python
+from cappr.huggingface.classify import predict
+
+prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
+
+class_names = ('Mercury', 'Earth')
+prior = None  # uniform prior
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='gpt2',
+                prior=prior)
+preds
+# ['Mercury']
+```
+</details>
+
+<details>
+<summary>Run in batches</summary>
+
+Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
+instead of the class.
+
+```python
+from cappr.huggingface.classify import predict_proba
+
+prompts = [
+    'Stephen Curry is a',
+    'Martina Navratilova was a',
+    "Dexter, from the TV Series Dexter's Laboratory, is a",
+    'LeBron James is a',    
+]
+
+# each of the prompts could be completed with one of these:
+class_names = (
+    'basketball player',
+    'tennis player',
+    'scientist'
+)
+
+prior = (
+    1/6,  # few
+    1/6,  # few
+    2/3   # there are more
+)
+
+pred_probs = predict_proba(prompts=prompts,
+                           completions=class_names,
+                           model='gpt2',
+                           batch_size=32,  # whatever fits on your CPU/GPU
+                           prior=prior)
+
+# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
+print(pred_probs.round(1))
+# [[0.5 0.3 0.2]
+#  [0.3 0.6 0.2]
+#  [0.1 0.1 0.8]
+#  [0.8 0.2 0. ]]
+
+# for each prompt, which completion is most likely?
+pred_class_idxs = pred_probs.argmax(axis=1)
+print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
+# ['basketball player',
+#  'tennis player',
+#  'scientist',
+#  'basketball player']
+```
+</details>
+
+<details>
+<summary>Run in batches, where each prompt has a different set of possible completions
+</summary>
+
+Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
+instantiated model and tokenizer instead of its name. That way, the model isn't
+re-loaded every time you wanna use it.
+
+```python
+import numpy as np
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from cappr import Example
+from cappr.huggingface.classify import predict_proba_examples
+
+examples = [
+    Example(prompt='Jodie Foster played',
+            completions=('Clarice Starling', 'Trinity in The Matrix')),
+    Example(prompt='Batman, from Batman: The Animated Series, was played by',
+            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
+            prior=      (     1/3      ,      2/3     ,      0      ))
+]
+
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+pred_probs = predict_proba_examples(examples,
+                                    model_and_tokenizer=(model, tokenizer))
+
+# pred_probs[i][j] = probability that examples[i].prompt is classified as
+# examples[i].completions[j]
+print([example_pred_probs.round(2)
+       for example_pred_probs in pred_probs])
+# [array([0.7, 0.3]),
+#  array([0.03, 0.97, 0.  ])]
+
+# for each example, which completion is most likely?
+pred_class_idxs = [np.argmax(example_pred_probs)
+                   for example_pred_probs in pred_probs]
+print([example.completions[pred_class_idx]
+       for example, pred_class_idx in zip(examples, pred_class_idxs)])
+# ['Clarice Starling',
+#  'Kevin Conroy']
+```
+</details>
+
+More examples are linked [here in the
+documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
+
+See
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+for a demonstration of a slightly harder classification task.
+
+
+## Documentation
+
+https://cappr.readthedocs.io/en/latest/
+
+Please let me know if you find the writing too dense. The main motivation behind this
+project is simplicity :-)
+
+
+## Setup
+
+If you intend on using OpenAI models, [sign up for the OpenAI API
+here](https://platform.openai.com/signup), and then set the environment variable
+`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
+others. But using them will cost ya 💰!
+
+Install with `pip`:
+
+```
+python -m pip install cappr
+```
+
+<details>
+<summary>(Optional) Install requirements for HuggingFace models</summary>
+
+```
+python -m pip install cappr[hf]
+```
+</details>
+
+<details>
+<summary>(Optional) Set up to run demos</summary>
+
+```
+python -m pip install cappr[demos]
+```
+</details>
+
+
+## Motivation
+
+Create a more usable zero-shot text classification interface than
+[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
+
+<details>
+<summary>Short</summary>
+
+In CVS, your job is to write up your classification task in a `prompt` string, and then
+write custom code to post-process arbitrary `completion`/output strings.
+
+In CAPPr, your job starts and stops at writing up your classification task as a
+`{prompt}{end_of_prompt}{completion}` string.
+</details>
+
+<details>
+<summary>Long</summary>
+
+Please see [this page of the
+documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
+
+</details>
+
+<details>
+<summary>Unstudied</summary>
+
+I'm curious to see how much easier estimation/discrimination is than generation. In
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb),
+CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
+accurate.
+
+</details>
+
+<details>
+<summary>Honest</summary>
+
+Keep myself busy
+
+</details>
+
+
+## Results
+
+<details>
+<summary>
+Statistical performance
+</summary>
+Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
+I need to run it on more ofc. Will update
+
+  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+</details>
+
+
+<details>
+<summary>
+Computational performance
+</summary>
+
+One concern was that CAPPr requires as many `model()` calls as there are classes. But in
+the CAPPr scheme, we can simply cache each attention block's keys and values for the
+prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
+code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
+the implementation. Note that this caching is not implemented for OpenAI models, as I
+can't control their backend. **This means that when running `cappr.openai` functions,
+you'll be on the *cappr (slow)* line** :-(
+
+![](/docs/source/_static/scaling_classes/batch_size_32.png)
+
+*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
+choices to simulate multi-class classification tasks. [GPT-2
+(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
+Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
+processed in batches of size 32. Each point in the graph is a median of 5 runs. For
+classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
+which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
+COPA (and other multiple-choice style prompts), that may result in lower zero-shot
+accuracy, as most of the sampled choices come after the first token.*
+
+See the [`demos/computational_analysis.ipynb`
+notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
+
+</details>
+
+
+## Related work
+
+While [benchmarking this
+method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
+Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
+is very similar:
+
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+
+[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
+probabilities to do prompt-completion classification, but these probabilities are
+assumed to come from masked language models like BERT.
+
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+
+
+## Contributing
+
+TODO
+
+
+## Testing
+
+### Setup
+
+1. Clone the repo
+
+   ```
+   git clone https://github.com/kddubey/cappr.git
+   ```
+
+2. Create a new Python 3.8+ environment
+
+3. Install this package in editable mode, along with development requirements
+
+   ```
+   python -m pip install -e .[dev]
+   ```
+
+### Run tests
+
+```
+pytest
+```
+
+Dumping VS code extensions for development:
+  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
+  Use the numpy format.
+  * [Set Python formatting to
+    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
+  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
+  * [TOML Language
+    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
+
+
+## Todo
+
+(**) = I'm currently working on this or will work on it really soon
+
+<details>
+<summary>Code</summary>
+
+- [ ] Testing
+  - [ ] Increase test cases
+  - [ ] Some more standardization b/t openai and huggingface tests
+  - [x] Add code coverage badge to look cool
+  - [ ] Test input checks
+- [x] Small CPU speed-ups
+  - [x] For constant-completions input, vectorize `agg_log_probs`
+  - [x] For `examples` input, if # completions per prompt is constant, vectorize
+  `posterior_prob`
+- [ ] Make progress bars optional, since inference often isn't batched
+- [ ] Factor out input checks (on prompts and completions)
+- [x] De-automate overzealous auto-docstring stuff :-(
+- [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [x] Optimize backend to enable greater scaling wrt # completions/classes
+  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
+  batching
+    - [ ] Get to the bottom of why it's slower w/o batching
+  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
+  think
+  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
+  - [ ] Consider batchifying the completions again, since they technically don't go in
+  batches of `batch_size`; the actual batch size is the sum of the number of completions
+  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
+  are usually half as long. But it should be configurable at the very least.
+  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
+  - [ ] Support [Inference
+    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
+  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support priming, as in: cache it
+- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
+- [ ] Allow for multi-label classification
+  - [ ] Pass `normalize` as an argument to predict_proba functions
+  - [ ] For `huggingface`, add note that you'll get faster results by passing all
+  labels at once (assuming prompt is identical for each label)
+- [ ] Create a notebook template
+- [ ] Fill in missing or non-numpy docstrings
+</details>
+
+<details>
+<summary>Research</summary>
+
+Evaluate on more datasets, and understand its relative advantages and disadvantages vs
+other classification methods.
+
+- [ ] RAFT benchmark (**)
+  - [x] Zero-shot training scores
+  - [ ] Submit zero-shot test predictions
+  - [ ] Few-shot (priming) training scores
+  - [ ] Submit few-shot test predictions
+- [ ] Create a user guide, build a table of results comparing competing approaches on
+statistical performance, cost, and computation
+- [ ] Make a computational comparison to sampling (**)
+  - [x] Assume I have full freedom to decide how inference works. Demo w/
+  GPT-2. Process inputs in batches.
+  - [ ] Process inputs 1-by-1
+- [ ] More SuperGLUE tasks?
+  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
+- [ ] Calibration
+  - [ ] Is the prior actually effective? Downsample and see
+  - [ ] curves
+- [ ] Compare against few-shot embeddings
+- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
+  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
+  - [ ] Again, compare against sampling
+- [ ] Evaluate a bigger model like GPT-J
+- [ ] Evaluate different aggregation functions. Currently taking mean, but
+there was no good theory for that
+- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
+manipulating position IDs isn't sufficient (I think).
+</details>
```

### Comparing `cappr-0.2.1/README.md` & `cappr-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,434 +1,453 @@
-# CAPPr: zero-shot text classification using autoregressive language models
-
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
-[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-Perform zero-shot text classification by estimating the probability that an inputted
-completion comes after an inputted prompt. Hence the name:
-
-> **C**ompletion<br>
-  **A**fter<br>
-  **P**rompt<br>
-  **Pr**obability<br>
-
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
-
-## Usage
-
-<details>
-<summary>Use a model from the OpenAI API</summary>
-
-Specifically, this model must be compatible with the
-[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-endpoint.
-
-Let's classify
-[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
-from the OpenAI text completion docs.
-
-```python
-from cappr.openai.classify import predict
-
-tweet = 'I loved the new Batman movie!'
-prompt = f'Tweet: {tweet}\nSentiment:'
-
-class_names = ('positive', 'neutral', 'negative')
-# optional: let's supply a prior distribution over the classes
-prior       = (   1/8    ,    1/8   ,     3/4   )
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='text-ada-001',
-                prior=prior)
-preds
-# ['positive']
-```
-</details>
-
-<details>
-<summary>Use a model from the HuggingFace model hub</summary>
-
-Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
-
-```python
-from cappr.huggingface.classify import predict
-
-prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
-
-class_names = ('Mercury', 'Earth')
-prior = None  # uniform prior
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='gpt2',
-                prior=prior)
-preds
-# ['Mercury']
-```
-</details>
-
-<details>
-<summary>Run in batches</summary>
-
-Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
-instead of the class.
-
-```python
-from cappr.huggingface.classify import predict_proba
-
-prompts = [
-    'Stephen Curry is a',
-    'Martina Navratilova was a',
-    "Dexter, from the TV Series Dexter's Laboratory, is a",
-    'LeBron James is a',    
-]
-
-# each of the prompts could be completed with one of these:
-class_names = (
-    'basketball player',
-    'tennis player',
-    'scientist'
-)
-
-prior = (
-    1/6,  # few
-    1/6,  # few
-    2/3   # there are more
-)
-
-pred_probs = predict_proba(prompts=prompts,
-                           completions=class_names,
-                           model='gpt2',
-                           batch_size=32,  # whatever fits on your CPU/GPU
-                           prior=prior)
-
-# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
-print(pred_probs.round(1))
-# [[0.5 0.3 0.2]
-#  [0.3 0.6 0.2]
-#  [0.1 0.1 0.8]
-#  [0.8 0.2 0. ]]
-
-# for each prompt, which completion is most likely?
-pred_class_idxs = pred_probs.argmax(axis=1)
-print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
-# ['basketball player',
-#  'tennis player',
-#  'scientist',
-#  'basketball player']
-```
-</details>
-
-<details>
-<summary>Run in batches, where each prompt has a different set of possible completions
-</summary>
-
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
-
-```python
-import numpy as np
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-from cappr import Example
-from cappr.huggingface.classify import predict_proba_examples
-
-examples = [
-    Example(prompt='Jodie Foster played',
-            completions=('Clarice Starling', 'Trinity in The Matrix')),
-    Example(prompt='Batman, from Batman: The Animated Series, was played by',
-            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
-            prior=      (     1/3      ,      2/3     ,      0      ))
-]
-
-model_name = 'gpt2'
-model = AutoModelForCausalLM.from_pretrained(model_name)
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-pred_probs = predict_proba_examples(examples,
-                                    model_and_tokenizer=(model, tokenizer))
-
-# pred_probs[i][j] = probability that examples[i].prompt is classified as
-# examples[i].completions[j]
-print([example_pred_probs.round(2)
-       for example_pred_probs in pred_probs])
-# [array([0.7, 0.3]),
-#  array([0.03, 0.97, 0.  ])]
-
-# for each example, which completion is most likely?
-pred_class_idxs = [np.argmax(example_pred_probs)
-                   for example_pred_probs in pred_probs]
-print([example.completions[pred_class_idx]
-       for example, pred_class_idx in zip(examples, pred_class_idxs)])
-# ['Clarice Starling',
-#  'Kevin Conroy']
-```
-</details>
-
-More examples are linked [here in the
-documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
-
-See [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-for a demonstration of a slightly harder classification task.
-
-
-## Documentation
-
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
-
-
-## Setup
-
-If you intend on using OpenAI models, [sign up for the OpenAI API
-here](https://platform.openai.com/signup), and then set the environment variable
-`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
-others. But using them will cost ya 💰!
-
-Install with `pip`:
-
-```
-python -m pip install cappr
-```
-
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
-
-```
-python -m pip install cappr[hf]
-```
-</details>
-
-<details>
-<summary>(Optional) Set up to run demos</summary>
-
-```
-python -m pip install cappr[demos]
-```
-</details>
-
-
-## Motivation
-
-Create a more usable zero-shot text classification interface than
-[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
-
-<details>
-<summary>Short</summary>
-
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
-
-In CAPPr, your job starts and stops at writing up your classification task as a
-`{prompt}{end_of_prompt}{completion}` string.
-</details>
-
-<details>
-<summary>Long</summary>
-
-Please see [this page of the
-documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
-
-</details>
-
-<details>
-<summary>Unstudied</summary>
-
-I'm curious to see how much easier estimation/discrimination is than generation.
-In [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb),
-CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
-accurate.
-
-</details>
-
-<details>
-<summary>Honest</summary>
-
-Keep myself busy
-
-</details>
-
-
-## Results
-
-<details>
-<summary>
-Statistical performance
-</summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
-
-  * [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-  * [`demos/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb)
-</details>
-
-
-<details>
-<summary>
-Computational performance
-</summary>
-
-One concern was that CAPPr requires as many `model()` calls as there are classes. But in
-the CAPPr scheme, we can simply cache each attention block's keys and values for the
-prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
-code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
-the implementation. Note that this caching is not implemented for OpenAI models, as I
-can't control their backend. **This means that when running `cappr.openai` functions,
-you'll be on the *cappr (slow)* line** :-(
-
-![](/docs/source/_static/scaling_classes/batch_size_32.png)
-
-*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
-choices to simulate multi-class classification tasks. [GPT-2
-(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
-
-See the [`demos/computational_analysis.ipynb`
-notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
-
-</details>
-
-
-## Related work
-
-While [benchmarking this
-method](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb) on the Winograd
-Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847) is very
-similar:
-
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
-
-[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
-probabilities to do prompt-completion classification, but these probabilities are
-assumed to come from masked language models like BERT.
-
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
-
-
-## Contributing
-
-TODO
-
-
-## Testing
-
-### Setup
-
-1. Clone the repo
-
-   ```
-   git clone https://github.com/kddubey/cappr.git
-   ```
-
-2. Create a new Python 3.8+ environment
-
-3. Install this package in editable mode, along with development requirements
-
-   ```
-   python -m pip install -e .[dev]
-   ```
-
-### Run tests
-
-```
-pytest
-```
-
-Dumping VS code extensions for development:
-  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
-  Use the numpy format.
-  * [Set Python formatting to
-    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
-  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
-  * [TOML Language
-    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
-
-
-## Todo
-
-(**) = I'm currently working on this or will work on it really soon
-
-<details>
-<summary>Code</summary>
-
-- [ ] Testing
-  - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
-  - [ ] Test input checks
-- [x] Small CPU speed-ups
-  - [x] For constant-completions input, vectorize `agg_log_probs`
-  - [x] For `examples` input, if # completions per prompt is constant, vectorize
-  `posterior_prob`
-- [ ] Add getLogger, basic logging
-- [ ] Make progress bars optional, since inference often isn't batched
-- [ ] Factor out input checks (on prompts and completions)
-- [x] De-automate overzealous auto-docstring stuff :-(
-- [ ] HuggingFace `transformers.AutoModelForCausalLM`
-  - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
-    - [ ] Get to the bottom of why it's slower w/o batching
-  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
-  think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
-  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
-  - [ ] Support [Inference
-    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
-  - [ ] Support priming, as in: cache it
-- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
-- [ ] Allow for multi-label classification
-  - [ ] Pass `normalize` as an argument to predict_proba functions
-  - [ ] For `huggingface`, add note that you'll get faster results by passing all
-  labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
-- [ ] Fill in missing or non-numpy docstrings
-</details>
-
-<details>
-<summary>Research</summary>
-
-Evaluate on more datasets, and understand its relative advantages and disadvantages vs
-other classification methods.
-
-- [ ] RAFT benchmark (**)
-- [ ] Create a user guide, build a table of results comparing competing approaches on
-statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
-  - [ ] Process inputs 1-by-1
-- [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
-- [ ] Calibration
-  - [ ] Is the prior actually effective? Downsample and see
-  - [ ] curves
-- [ ] Compare against few-shot embeddings
-- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
-  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
-  - [ ] Again, compare against sampling
-- [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
-</details>
+Metadata-Version: 2.1
+Name: cappr
+Version: 0.2.2
+Summary: Zero-shot text classification using autoregressive language models.
+Home-page: https://github.com/kddubey/cappr/
+Author-email: kushdubey63@gmail.com
+License: Apache License 2.0
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: hf
+Provides-Extra: demos
+Provides-Extra: dev
+License-File: LICENSE
+
+# CAPPr: zero-shot text classification using autoregressive language models
+
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
+[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+Perform zero-shot text classification by estimating the probability that an inputted
+completion comes after an inputted prompt. Hence the name:
+
+> **C**ompletion<br>
+  **A**fter<br>
+  **P**rompt<br>
+  **Pr**obability<br>
+
+The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+
+## Usage
+
+<details>
+<summary>Use a model from the OpenAI API</summary>
+
+Specifically, this model must be compatible with the
+[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+endpoint.
+
+Let's classify
+[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
+from the OpenAI text completion docs.
+
+```python
+from cappr.openai.classify import predict
+
+tweet = 'I loved the new Batman movie!'
+prompt = f'Tweet: {tweet}\nSentiment:'
+
+class_names = ('positive', 'neutral', 'negative')
+# optional: let's supply a prior distribution over the classes
+prior       = (   1/8    ,    1/8   ,     3/4   )
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='text-ada-001',
+                prior=prior)
+preds
+# ['positive']
+```
+</details>
+
+<details>
+<summary>Use a model from the HuggingFace model hub</summary>
+
+Specifically, this model must be able to be loaded using
+`transformers.AutoModelForCausalLM.from_pretrained(model)`.
+
+Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+
+```python
+from cappr.huggingface.classify import predict
+
+prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
+
+class_names = ('Mercury', 'Earth')
+prior = None  # uniform prior
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='gpt2',
+                prior=prior)
+preds
+# ['Mercury']
+```
+</details>
+
+<details>
+<summary>Run in batches</summary>
+
+Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
+instead of the class.
+
+```python
+from cappr.huggingface.classify import predict_proba
+
+prompts = [
+    'Stephen Curry is a',
+    'Martina Navratilova was a',
+    "Dexter, from the TV Series Dexter's Laboratory, is a",
+    'LeBron James is a',    
+]
+
+# each of the prompts could be completed with one of these:
+class_names = (
+    'basketball player',
+    'tennis player',
+    'scientist'
+)
+
+prior = (
+    1/6,  # few
+    1/6,  # few
+    2/3   # there are more
+)
+
+pred_probs = predict_proba(prompts=prompts,
+                           completions=class_names,
+                           model='gpt2',
+                           batch_size=32,  # whatever fits on your CPU/GPU
+                           prior=prior)
+
+# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
+print(pred_probs.round(1))
+# [[0.5 0.3 0.2]
+#  [0.3 0.6 0.2]
+#  [0.1 0.1 0.8]
+#  [0.8 0.2 0. ]]
+
+# for each prompt, which completion is most likely?
+pred_class_idxs = pred_probs.argmax(axis=1)
+print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
+# ['basketball player',
+#  'tennis player',
+#  'scientist',
+#  'basketball player']
+```
+</details>
+
+<details>
+<summary>Run in batches, where each prompt has a different set of possible completions
+</summary>
+
+Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
+instantiated model and tokenizer instead of its name. That way, the model isn't
+re-loaded every time you wanna use it.
+
+```python
+import numpy as np
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from cappr import Example
+from cappr.huggingface.classify import predict_proba_examples
+
+examples = [
+    Example(prompt='Jodie Foster played',
+            completions=('Clarice Starling', 'Trinity in The Matrix')),
+    Example(prompt='Batman, from Batman: The Animated Series, was played by',
+            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
+            prior=      (     1/3      ,      2/3     ,      0      ))
+]
+
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+pred_probs = predict_proba_examples(examples,
+                                    model_and_tokenizer=(model, tokenizer))
+
+# pred_probs[i][j] = probability that examples[i].prompt is classified as
+# examples[i].completions[j]
+print([example_pred_probs.round(2)
+       for example_pred_probs in pred_probs])
+# [array([0.7, 0.3]),
+#  array([0.03, 0.97, 0.  ])]
+
+# for each example, which completion is most likely?
+pred_class_idxs = [np.argmax(example_pred_probs)
+                   for example_pred_probs in pred_probs]
+print([example.completions[pred_class_idx]
+       for example, pred_class_idx in zip(examples, pred_class_idxs)])
+# ['Clarice Starling',
+#  'Kevin Conroy']
+```
+</details>
+
+More examples are linked [here in the
+documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
+
+See
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+for a demonstration of a slightly harder classification task.
+
+
+## Documentation
+
+https://cappr.readthedocs.io/en/latest/
+
+Please let me know if you find the writing too dense. The main motivation behind this
+project is simplicity :-)
+
+
+## Setup
+
+If you intend on using OpenAI models, [sign up for the OpenAI API
+here](https://platform.openai.com/signup), and then set the environment variable
+`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
+others. But using them will cost ya 💰!
+
+Install with `pip`:
+
+```
+python -m pip install cappr
+```
+
+<details>
+<summary>(Optional) Install requirements for HuggingFace models</summary>
+
+```
+python -m pip install cappr[hf]
+```
+</details>
+
+<details>
+<summary>(Optional) Set up to run demos</summary>
+
+```
+python -m pip install cappr[demos]
+```
+</details>
+
+
+## Motivation
+
+Create a more usable zero-shot text classification interface than
+[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
+
+<details>
+<summary>Short</summary>
+
+In CVS, your job is to write up your classification task in a `prompt` string, and then
+write custom code to post-process arbitrary `completion`/output strings.
+
+In CAPPr, your job starts and stops at writing up your classification task as a
+`{prompt}{end_of_prompt}{completion}` string.
+</details>
+
+<details>
+<summary>Long</summary>
+
+Please see [this page of the
+documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
+
+</details>
+
+<details>
+<summary>Unstudied</summary>
+
+I'm curious to see how much easier estimation/discrimination is than generation. In
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb),
+CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
+accurate.
+
+</details>
+
+<details>
+<summary>Honest</summary>
+
+Keep myself busy
+
+</details>
+
+
+## Results
+
+<details>
+<summary>
+Statistical performance
+</summary>
+Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
+I need to run it on more ofc. Will update
+
+  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+</details>
+
+
+<details>
+<summary>
+Computational performance
+</summary>
+
+One concern was that CAPPr requires as many `model()` calls as there are classes. But in
+the CAPPr scheme, we can simply cache each attention block's keys and values for the
+prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
+code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
+the implementation. Note that this caching is not implemented for OpenAI models, as I
+can't control their backend. **This means that when running `cappr.openai` functions,
+you'll be on the *cappr (slow)* line** :-(
+
+![](/docs/source/_static/scaling_classes/batch_size_32.png)
+
+*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
+choices to simulate multi-class classification tasks. [GPT-2
+(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
+Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
+processed in batches of size 32. Each point in the graph is a median of 5 runs. For
+classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
+which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
+COPA (and other multiple-choice style prompts), that may result in lower zero-shot
+accuracy, as most of the sampled choices come after the first token.*
+
+See the [`demos/computational_analysis.ipynb`
+notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
+
+</details>
+
+
+## Related work
+
+While [benchmarking this
+method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
+Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
+is very similar:
+
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+
+[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
+probabilities to do prompt-completion classification, but these probabilities are
+assumed to come from masked language models like BERT.
+
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+
+
+## Contributing
+
+TODO
+
+
+## Testing
+
+### Setup
+
+1. Clone the repo
+
+   ```
+   git clone https://github.com/kddubey/cappr.git
+   ```
+
+2. Create a new Python 3.8+ environment
+
+3. Install this package in editable mode, along with development requirements
+
+   ```
+   python -m pip install -e .[dev]
+   ```
+
+### Run tests
+
+```
+pytest
+```
+
+Dumping VS code extensions for development:
+  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
+  Use the numpy format.
+  * [Set Python formatting to
+    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
+  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
+  * [TOML Language
+    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
+
+
+## Todo
+
+(**) = I'm currently working on this or will work on it really soon
+
+<details>
+<summary>Code</summary>
+
+- [ ] Testing
+  - [ ] Increase test cases
+  - [ ] Some more standardization b/t openai and huggingface tests
+  - [x] Add code coverage badge to look cool
+  - [ ] Test input checks
+- [x] Small CPU speed-ups
+  - [x] For constant-completions input, vectorize `agg_log_probs`
+  - [x] For `examples` input, if # completions per prompt is constant, vectorize
+  `posterior_prob`
+- [ ] Make progress bars optional, since inference often isn't batched
+- [ ] Factor out input checks (on prompts and completions)
+- [x] De-automate overzealous auto-docstring stuff :-(
+- [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [x] Optimize backend to enable greater scaling wrt # completions/classes
+  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
+  batching
+    - [ ] Get to the bottom of why it's slower w/o batching
+  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
+  think
+  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
+  - [ ] Consider batchifying the completions again, since they technically don't go in
+  batches of `batch_size`; the actual batch size is the sum of the number of completions
+  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
+  are usually half as long. But it should be configurable at the very least.
+  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
+  - [ ] Support [Inference
+    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
+  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support priming, as in: cache it
+- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
+- [ ] Allow for multi-label classification
+  - [ ] Pass `normalize` as an argument to predict_proba functions
+  - [ ] For `huggingface`, add note that you'll get faster results by passing all
+  labels at once (assuming prompt is identical for each label)
+- [ ] Create a notebook template
+- [ ] Fill in missing or non-numpy docstrings
+</details>
+
+<details>
+<summary>Research</summary>
+
+Evaluate on more datasets, and understand its relative advantages and disadvantages vs
+other classification methods.
+
+- [ ] RAFT benchmark (**)
+  - [x] Zero-shot training scores
+  - [ ] Submit zero-shot test predictions
+  - [ ] Few-shot (priming) training scores
+  - [ ] Submit few-shot test predictions
+- [ ] Create a user guide, build a table of results comparing competing approaches on
+statistical performance, cost, and computation
+- [ ] Make a computational comparison to sampling (**)
+  - [x] Assume I have full freedom to decide how inference works. Demo w/
+  GPT-2. Process inputs in batches.
+  - [ ] Process inputs 1-by-1
+- [ ] More SuperGLUE tasks?
+  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
+- [ ] Calibration
+  - [ ] Is the prior actually effective? Downsample and see
+  - [ ] curves
+- [ ] Compare against few-shot embeddings
+- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
+  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
+  - [ ] Again, compare against sampling
+- [ ] Evaluate a bigger model like GPT-J
+- [ ] Evaluate different aggregation functions. Currently taking mean, but
+there was no good theory for that
+- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
+manipulating position IDs isn't sufficient (I think).
+</details>
```

### Comparing `cappr-0.2.1/src/cappr/_example.py` & `cappr-0.2.2/src/cappr/_example.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import Optional, Sequence
-
-
-from cappr.utils import _check
-
-
-@dataclass(frozen=True)
-class Example:
-    """
-    Represents a single prompt-completion classification example.
-
-    This data structure is useful when different classification examples may belong to
-    a different set of classes.
-
-    Parameters
-    ----------
-    prompt : str
-        string, which, e.g., contains the text to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after the
-        prompt
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the `prompt`. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-
-    Raises
-    ------
-    TypeError
-        if `prompt` is not a string
-    TypeError
-        if `completions` is not a sequence of strings
-    TypeError
-        if `prior` is not None, or it isn't a sequence
-    ValueError
-        if `prior` is a sequence but isn't 1-D
-    ValueError
-        if `prior` is a sequence but doesn't sum to 1
-    ValueError
-        if `prior` is a sequence but `completions` and `prior` are different lengths
-    """
-
-    prompt: str
-    completions: Sequence[str]
-    prior: Optional[Sequence[float]] = None
-    end_of_prompt: str = " "
-
-    def __post_init__(self):
-        ## Check inputs here so that fxns of Example don't need to check
-        if not isinstance(self.prompt, str):
-            raise TypeError("prompt must be a string.")
-        if isinstance(self.completions, str) or not isinstance(
-            self.completions, Sequence
-        ):
-            raise TypeError("completions must be a Sequence of strings.")
-        _check.prior(self.prior)
-        if self.prior is not None and len(self.completions) != len(self.prior):
-            raise ValueError(
-                "completions and prior are different lengths: "
-                f"{len(self.completions)}, {len(self.prior)}."
-            )
+from __future__ import annotations
+from dataclasses import dataclass
+from typing import Optional, Sequence
+
+
+from cappr.utils import _check
+
+
+@dataclass(frozen=True)
+class Example:
+    """
+    Represents a single prompt-completion classification example.
+
+    This data structure is useful when different classification examples may belong to
+    a different set of classes.
+
+    Parameters
+    ----------
+    prompt : str
+        string, which, e.g., contains the text to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after the
+        prompt
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the `prompt`. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+
+    Raises
+    ------
+    TypeError
+        if `prompt` is not a string
+    TypeError
+        if `completions` is not a sequence of strings
+    TypeError
+        if `prior` is not None, or it isn't a sequence
+    ValueError
+        if `prior` is a sequence but isn't 1-D
+    ValueError
+        if `prior` is a sequence but doesn't sum to 1
+    ValueError
+        if `prior` is a sequence but `completions` and `prior` are different lengths
+    """
+
+    prompt: str
+    completions: Sequence[str]
+    prior: Optional[Sequence[float]] = None
+    end_of_prompt: str = " "
+
+    def __post_init__(self):
+        ## Check inputs here so that fxns of Example don't need to check
+        if not isinstance(self.prompt, str):
+            raise TypeError("prompt must be a string.")
+        if isinstance(self.completions, str) or not isinstance(
+            self.completions, Sequence
+        ):
+            raise TypeError("completions must be a Sequence of strings.")
+        _check.prior(self.prior)
+        if self.prior is not None and len(self.completions) != len(self.prior):
+            raise ValueError(
+                "completions and prior are different lengths: "
+                f"{len(self.completions)}, {len(self.prior)}."
+            )
```

### Comparing `cappr-0.2.1/src/cappr/huggingface/_utils.py` & `cappr-0.2.2/src/cappr/huggingface/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-"""
-YouTils
-"""
-from __future__ import annotations
-
-import torch
-import torch.nn.functional as F
-from transformers import (
-    AutoModelForCausalLM,
-    AutoTokenizer,
-    PreTrainedModel,
-    PreTrainedTokenizer,
-)
-
-
-def logits_to_log_probs(
-    logits: torch.Tensor,
-    input_ids: torch.Tensor,
-    input_ids_start_idx: int,
-    logits_end_idx: int,
-):
-    """
-    TODO: docstring fix
-    Returns a tensor `log_probs` with shape
-
-        `(logits.shape[0], logits.shape[1]-1)`
-
-    where `log_probs[i,j]` is the log-probability of token
-
-        `input_ids[i,j]`
-
-    given its previous tokens
-
-        `input_ids[i,:j]`
-
-    for `j in range(input_ids_start_idx, input_ids.shape[1])`.
-
-    `logits[i,j]` is assumed to be an unnormalized distribution (over tokens in
-    the vocab) given tokens `input_ids[i,:j]`.
-    """
-    ## logits.shape is    (# texts, max # tokens in texts, vocab size)
-    log_probs = F.log_softmax(logits, dim=2)
-
-    ## Only keep the log-prob from the vocab dimension whose index is is the
-    ## next token's input ID.
-    ## input_ids.shape is (# texts, max # tokens in texts)
-    return (
-        log_probs[:, :logits_end_idx, :]
-        .take_along_dim(input_ids[:, input_ids_start_idx:, None], dim=2)
-        .squeeze(-1)
-    )
-
-
-def load_model_and_tokenizer(
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-) -> tuple[PreTrainedModel, PreTrainedTokenizer]:
-    """
-    TODO: docstring
-    """
-    if (model is not None and model_and_tokenizer is not None) or (
-        model is None and model_and_tokenizer is None
-    ):
-        raise ValueError(
-            "One of model and model_and_tokenizer must be None, and the other not None."
-        )
-    from_str = model is not None
-    if from_str:
-        model_: torch.nn.Module = AutoModelForCausalLM.from_pretrained(model)
-        tokenizer = AutoTokenizer.from_pretrained(model)
-    else:
-        model_, tokenizer = model_and_tokenizer
-    ## Prepare model
-    model_.eval()
-    if from_str:
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        model_.to(device)
-    ## Prepare tokenizer
-    if tokenizer.pad_token_id is None:
-        tokenizer.pad_token_id = tokenizer.eos_token_id
-    tokenizer.padding_side = "right"
-    return model_, tokenizer
+"""
+YouTils
+"""
+from __future__ import annotations
+
+import torch
+import torch.nn.functional as F
+from transformers import (
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    PreTrainedModel,
+    PreTrainedTokenizer,
+)
+
+
+def logits_to_log_probs(
+    logits: torch.Tensor,
+    input_ids: torch.Tensor,
+    input_ids_start_idx: int,
+    logits_end_idx: int,
+):
+    """
+    TODO: docstring fix
+    Returns a tensor `log_probs` with shape
+
+        `(logits.shape[0], logits.shape[1]-1)`
+
+    where `log_probs[i,j]` is the log-probability of token
+
+        `input_ids[i,j]`
+
+    given its previous tokens
+
+        `input_ids[i,:j]`
+
+    for `j in range(input_ids_start_idx, input_ids.shape[1])`.
+
+    `logits[i,j]` is assumed to be an unnormalized distribution (over tokens in
+    the vocab) given tokens `input_ids[i,:j]`.
+    """
+    ## logits.shape is    (# texts, max # tokens in texts, vocab size)
+    log_probs = F.log_softmax(logits, dim=2)
+
+    ## Only keep the log-prob from the vocab dimension whose index is is the
+    ## next token's input ID.
+    ## input_ids.shape is (# texts, max # tokens in texts)
+    return (
+        log_probs[:, :logits_end_idx, :]
+        .take_along_dim(input_ids[:, input_ids_start_idx:, None], dim=2)
+        .squeeze(-1)
+    )
+
+
+def load_model_and_tokenizer(
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+) -> tuple[PreTrainedModel, PreTrainedTokenizer]:
+    """
+    TODO: docstring
+    """
+    if (model is not None and model_and_tokenizer is not None) or (
+        model is None and model_and_tokenizer is None
+    ):
+        raise ValueError(
+            "One of model and model_and_tokenizer must be None, and the other not None."
+        )
+    from_str = model is not None
+    if from_str:
+        model_: torch.nn.Module = AutoModelForCausalLM.from_pretrained(model)
+        tokenizer = AutoTokenizer.from_pretrained(model)
+    else:
+        model_, tokenizer = model_and_tokenizer
+    ## Prepare model
+    model_.eval()
+    if from_str:
+        device = "cuda" if torch.cuda.is_available() else "cpu"
+        model_.to(device)
+    ## Prepare tokenizer
+    if tokenizer.pad_token_id is None:
+        tokenizer.pad_token_id = tokenizer.eos_token_id
+    tokenizer.padding_side = "right"
+    return model_, tokenizer
```

### Comparing `cappr-0.2.1/src/cappr/huggingface/classify.py` & `cappr-0.2.2/src/cappr/huggingface/classify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,909 +1,916 @@
-"""
-Perform prompt-completion classification using a ``transformers.AutoModelForCausalLM``.
-Currently, only PyTorch models are supported.
-
-In the implementation, attention block keys and values for prompts are cached and shared
-across completions. See the computational performance `here`_.
-
-.. _here: https://cappr.readthedocs.io/en/latest/6_computational_performance.html
-
-You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
-
-.. warning:: This module currently requires that ``end_of_prompt`` is a whitespace.
-"""
-from __future__ import annotations
-from typing import Mapping, Optional, Sequence, Union
-
-import numpy as np
-import numpy.typing as npt
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer, BatchEncoding
-
-from cappr.utils import _batch, classify
-from cappr import Example
-from cappr import huggingface as hf
-
-
-def _keys_values_prompts(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    num_repeats_per_prompt: Union[int, Sequence[int]],
-) -> tuple[
-    tuple[torch.Tensor, torch.Tensor], BatchEncoding, torch.Tensor, torch.Tensor
-]:
-    """
-    Efficiently performs this procedure:
-
-    1. Repeat-interleave `prompts[i]` `num_repeats_per_prompt[i]` times.
-
-       Or, if `num_repeats_per_prompt` is an integer, repeat-interleave `prompts[i]`
-       `num_repeats_per_prompt` times.
-
-       For example, if there are 2 prompts and `num_repeats_per_prompt=(2,3)`, the
-       repeated prompts look like::
-
-           [prompts[0],
-            prompts[0],
-            prompts[1],
-            prompts[1],
-            prompts[1]]
-
-    2. Apply `tokenizer` to the repeated prompts.
-
-    3. Apply `model`.
-
-    Parameters
-    ----------
-    model : AutoModelForCausalLM
-        an autoregressive transformer language model
-    tokenizer : AutoTokenizer
-        the tokenizer corresponding to `model`
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    num_repeats_per_prompt : Union[int, Sequence[int]]
-        the numer of times to repeat each prompt in `prompts`
-
-    Returns
-    -------
-    past_key_values : tuple[torch.Tensor, torch.Tensor]
-        for each attention block in `model`, the keys and values for each prompt in the
-        repeated prompts
-    encodings : BatchEncoding
-        the tokenizer output for the repeated prompts
-    offsets : torch.Tensor
-        the number of (non-pad) tokens in each of the repeated prompts
-    last_nonpad_token_logits : torch.Tensor
-        next-token logits for the last non-pad token for each of the repeated prompts
-
-    Raises
-    ------
-    ValueError
-        if the `tokenizer` is not using right-padding
-    TypeError
-        if `prompts` is not a `Sequence`
-    ValueError
-        if `num_repeats_per_prompt` is a `Sequence` whose length is not the same as the
-        length of `prompts`
-    """
-    if not tokenizer.padding_side == "right":
-        raise ValueError(
-            "Gotta use right padding to ensure position IDs are " "correct."
-        )
-    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
-        raise TypeError("prompts must be a Sequence of strings.")
-    if isinstance(num_repeats_per_prompt, Sequence):
-        if not len(prompts) == len(num_repeats_per_prompt):
-            raise ValueError(
-                "If num_repeats_per_prompt is a Sequence, then it must be the same "
-                f"length as prompts. Got lengths {len(num_repeats_per_prompt)}, "
-                f"{len(prompts)}."
-            )
-    if not isinstance(num_repeats_per_prompt, int) and not isinstance(
-        num_repeats_per_prompt, torch.Tensor
-    ):
-        num_repeats_per_prompt = torch.tensor(
-            num_repeats_per_prompt, device=model.device
-        )
-
-    ## Batch inference prompts
-    prompts = list(prompts)  ## 0-index in case it's a Series or something
-    # fmt: off
-    encodings: BatchEncoding = (tokenizer(prompts, return_tensors="pt", padding=True)
-                                .to(model.device))
-    # fmt: on
-    with torch.no_grad():
-        out = model(**encodings)
-
-    ## We need to repeat each prompt's keys and values num_repeats_per_prompt times
-    ## For layer i, prompts_out.past_key_values[i] is a tuple (key, value),
-    ## each w/ shape: (batch size=len(prompts),
-    ##                 number of attention heads=12 for gpt2,
-    ##                 encodings.input_ids.shape[-1],
-    ##                 key/value hidden dimension=64 for gpt2)
-    past_key_values = (
-        torch.stack([torch.stack(block) for block in out.past_key_values], dim=0)
-        ## The tuple is now a tensor w/ shape:
-        ## (# layers=12 for gpt2,
-        ##  2 (for key and value),
-        ##  and then the rest as before)
-        ## Repeat along batch size dim so that it aligns downstream w/ completions
-        .repeat_interleave(num_repeats_per_prompt, dim=2)
-    )
-    ## Re-format this tensor to the nested tuple format we'd get if we passed multiple
-    ## copies of the prompt at the same time to the model
-    past_key_values = tuple(
-        [(layer[0], layer[1]) for layer in past_key_values]  ## keys, values
-    )
-
-    ## Repeat stuff
-    # fmt: off
-    encodings["attention_mask"] = (encodings
-                                   .attention_mask
-                                   .repeat_interleave(num_repeats_per_prompt,
-                                                      dim=0))
-    encodings["input_ids"] = (encodings
-                              .input_ids
-                              .repeat_interleave(num_repeats_per_prompt, dim=0))
-    # fmt: on
-
-    ## Need offsets so that position_ids for future tokens are set correctly
-    offsets: torch.Tensor = encodings.attention_mask.sum(dim=1)
-
-    ## Need (next-token) logits from prompts, i.e., last non-pad prompt token, since
-    ## that contains the first completion token's log-probability
-    _last_nonpad_token_idxs = (offsets - 1)[:, None, None]
-    # fmt: off
-    last_nonpad_token_logits: torch.Tensor = (out
-                                              .logits
-                                              .repeat_interleave(
-                                                  num_repeats_per_prompt, dim=0)
-                                              .take_along_dim(
-                                                  _last_nonpad_token_idxs, dim=1))
-    # fmt: on
-
-    return past_key_values, encodings, offsets, last_nonpad_token_logits
-
-
-def _blessed_helper(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    num_completions_per_prompt: Union[int, Sequence[int]],
-    completions_repeats: int,
-) -> tuple[torch.Tensor, BatchEncoding]:
-    """
-    TODO: docstring
-    """
-    if not tokenizer.padding_side == "right":
-        raise ValueError("Gotta use right padding to ensure position IDs are correct.")
-    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
-        raise TypeError("prompts must be a Sequence of strings.")
-    if isinstance(completions, str) or not isinstance(completions, Sequence):
-        raise TypeError("completions must be a Sequence of strings.")
-
-    ## Prepare prompt data
-    (
-        past_key_values,
-        prompts_encodings,
-        offsets,
-        prompts_last_nonpad_token_logits,
-    ) = _keys_values_prompts(model, tokenizer, prompts, num_completions_per_prompt)
-
-    ## Prepare completion data
-    completions = list(completions)  ## 0-index in case it's a Series or somethin
-    # fmt: off
-    completions_encoding = (tokenizer(completions, return_tensors="pt", padding=True)
-                            .to(model.device))
-    completions_input_ids = (completions_encoding
-                             .input_ids
-                             .repeat(completions_repeats, 1))
-    completions_attention_mask = (completions_encoding
-                                  .attention_mask
-                                  .repeat(completions_repeats, 1))
-    # fmt: on
-    ## Set position_ids to what they were had we fed the prompt + completion together w/
-    ## right-padding (right b/c GPT-2 uses absolute position ids)
-    _num_completion_tokens = completions_encoding.input_ids.shape[1]
-    completions_position_ids = (
-        torch.arange(_num_completion_tokens, device=model.device) + offsets[:, None]
-    )
-    ## Need attention_mask to include the prompt since it prolly has padding
-    attention_mask = torch.cat(
-        (prompts_encodings["attention_mask"], completions_attention_mask), dim=1
-    )
-
-    ## Everything should now be aligned 🤞 🙏
-    with torch.no_grad():
-        completions_out = model(
-            input_ids=completions_input_ids,
-            attention_mask=attention_mask,
-            past_key_values=past_key_values,
-            position_ids=completions_position_ids,
-        )
-    ## 😎
-
-    ## You need to be able to ignore pad tokens, so you need this data as well
-    encodings = BatchEncoding(
-        {
-            "input_ids": completions_input_ids,
-            "attention_mask": completions_attention_mask,
-            "offsets": offsets,
-        }
-    )
-
-    ## Let's drop the next-token logits for the last completion token b/c they're not
-    ## useful for our purposes. Moreover, dropping ensures
-    ## logits.shape[:2] == encodings['input_ids'].shape, as one expects.
-    ## Just keep in mind that `logits` are shifted behind.
-    logits = torch.cat(
-        [prompts_last_nonpad_token_logits, completions_out.logits[:, :-1, :]], dim=1
-    )
-
-    return logits, encodings
-
-
-def _logits_completions_given_prompts(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    end_of_prompt: str = " ",
-):
-    """
-    TODO: convert docstring to numpy style
-
-    If `texts` is
-
-    ```python
-    [prompt + end_of_prompt + completions
-     for prompt in prompts
-     for completion in completions]
-    ```
-
-    then this function returns
-
-    1. `logits`: tensor with shape
-
-        (`len(texts)`, max # tokens `completions`, `tokenizer.vocab_size`)
-
-    where `logits[i,j]` are the `model`'s logits for token `j+1` of the completion in
-    `texts[i]` given the prompt in `texts[i]`. This tensor includes logits for
-    right-padded tokens. Use the `encodings.attention_mask` to ignore them before
-    further processing.
-
-    2. `encodings`: `BatchEncoding` containing the input IDs, attention mask,
-    and position offsets.
-    """
-    if end_of_prompt != " ":
-        raise ValueError("end_of_prompt must be ' ' for now. Sorry!")
-    completions = [end_of_prompt + completion.lstrip() for completion in completions]
-    ## TODO: figure out how to do this generally, not just for ' ' end_of_prompt
-    return _blessed_helper(
-        model,
-        tokenizer,
-        prompts,
-        completions,
-        num_completions_per_prompt=len(completions),
-        completions_repeats=len(prompts),
-    )
-
-
-def _logits_completions_given_prompts_examples(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    examples: Sequence[Example],
-):
-    """
-    TODO: convert docstring to numpy style
-
-    If `texts` is
-
-    ```python
-    [example.prompt + example.end_of_prompt + completion
-     for example in examples
-     for completion in example.completions]
-    ```
-    then this function returns
-
-    1. `logits`: tensor with shape
-
-        (`len(texts)`, max # tokens `completions`, `tokenizer.vocab_size`)
-
-    where `logits[i,j]` are the `model`'s logits for token `j+1` of the completion in
-    `texts[i]` given the prompt in `texts[i]`. This tensor includes logits for
-    right-padded tokens. Use the `encodings.attention_mask` to ignore them before
-    further processing.
-
-    2. `encodings`: `BatchEncoding` containing the input IDs, attention mask,
-    and position offsets.
-    """
-    if any([example.end_of_prompt != " " for example in examples]):
-        raise ValueError("Every example's end_of_prompt must be ' ' for now. Sorry!")
-    prompts = [example.prompt for example in examples]
-    completions = [
-        example.end_of_prompt + completion.lstrip()
-        for example in examples
-        for completion in example.completions
-    ]
-    ## TODO: figure out how to do this generally, not just for ' ' end_of_prompt
-    num_completions_per_prompt = [len(example.completions) for example in examples]
-    completions_repeats = 1
-    return _blessed_helper(
-        model,
-        tokenizer,
-        prompts,
-        completions,
-        num_completions_per_prompt=num_completions_per_prompt,
-        completions_repeats=completions_repeats,
-    )
-
-
-def _logits_to_log_probs_completions(
-    logits: torch.Tensor, encodings: Mapping[str, torch.Tensor]
-) -> list[list[float]]:
-    """
-    TODO: convert docstring to numpy style
-
-    Returns a list `log_probs_completions` where `log_probs_completions[i][j]` is the
-    log-probablity of *completion* token
-
-        `encodings['input_ids'][i,j]`
-
-    given its previous tokens
-
-        `encodings['input_ids'][i,:j]`
-
-    Pad tokens, i.e., tokens where `encodings['attention_mask'] == 0` are excluded.
-
-    `logits[i,j]` is assumed to be an unnormalized distribution (over tokens in
-    the vocab) given tokens `input_ids[i,:j]`.
-    """
-    log_probs = hf._utils.logits_to_log_probs(
-        logits, encodings["input_ids"], input_ids_start_idx=None, logits_end_idx=None
-    )
-    last_idx_non_pad = encodings["attention_mask"].sum(dim=1)
-    ## i.e., # of tokens per completion
-    return [
-        log_probs_prompt_completion[:completion_end].tolist()
-        for log_probs_prompt_completion, completion_end in zip(
-            log_probs, last_idx_non_pad
-        )
-    ]
-
-
-def log_probs_conditional(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> list[list[list[float]]]:
-    """
-    Log-probabilities of each completion token conditional on each prompt and previous
-    completion tokens.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
-        log-probability of the completion token in `completions[completion_idx]`,
-        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
-        completion tokens.
-
-    Note
-    ----
-    To efficiently aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs_from_constant_completions`.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify import log_probs_conditional
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        prompts = ['x y', 'a b c']
-        completions = ['z', 'd e']
-
-        # Compute
-        log_probs_completions = log_probs_conditional(
-                                    prompts,
-                                    completions,
-                                    model_and_tokenizer=(model, tokenizer)
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0]
-        # [[-4.5],        [[log Pr(z | x, y)],
-        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1]
-        # [[-9.7],        [[log Pr(z | a, b, c)],
-        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
-    """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
-
-    @_batch.flatten
-    @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs")
-    def log_probs_completions_batch(prompts, batch_size=batch_size):
-        logits, encodings = _logits_completions_given_prompts(
-            model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
-        )
-        return _logits_to_log_probs_completions(logits, encodings)
-
-    log_probs_completions = log_probs_completions_batch(prompts)
-    return list(_batch.constant(log_probs_completions, size=len(completions)))
-
-
-def log_probs_conditional_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> list[list[list[float]]]:
-    """
-    Log-probabilities of each completion token conditional on each prompt and previous
-    completion tokens.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
-        the log-probability of the completion token in
-        `examples[example_idx].completions[completion_idx]`, conditional on
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
-        previous completion tokens.
-
-    Note
-    ----
-    To aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs`.
-
-    Note
-    ----
-    The attribute :attr:`cappr.Example.prior` is unused.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify import log_probs_conditional_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [Example(prompt='x y',   completions=('z', 'd e')),
-                    Example(prompt='a b c', completions=('1 2',))]
-
-        # Compute
-        log_probs_completions = log_probs_conditional_examples(
-                                    examples,
-                                    model_and_tokenizer=(model, tokenizer)
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0] # corresponds to examples[0]
-        # [[-4.5],        [[log Pr(z | x, y)],
-        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1] # corresponds to examples[1]
-        # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
-    """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
-
-    @_batch.flatten
-    @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs")
-    def log_probs_completions_batch(examples, batch_size=batch_size):
-        logits, encodings = _logits_completions_given_prompts_examples(
-            model, tokenizer, examples
-        )
-        return _logits_to_log_probs_completions(logits, encodings)
-
-    log_probs_completions = log_probs_completions_batch(examples)
-    num_completions_per_prompt = [len(example.completions) for example in examples]
-    return list(
-        _batch.variable(log_probs_completions, sizes=num_completions_per_prompt)
-    )
-
-
-@classify._predict_proba
-def predict_proba(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    prior: Optional[Sequence[float]] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> npt.NDArray[np.floating]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    pred_probs : npt.NDArray[np.floating]
-        Array with shape `(len(prompts), len(completions))`.
-        `pred_probs[prompt_idx, completion_idx]` is the model's estimate of the
-        probability that `completions[completion_idx]` comes after
-        `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_proba_examples`.
-
-    Example
-    -------
-    Let's have GPT-2 (small) predict where stuff is in the kitchen. This example also
-    conveys that it's not the greatest model out there::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify import predict_proba
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Define a classification task
-        prompts = ['The tacos are cooking',
-                   'Ice cream is']
-        class_names = ('on the stove', 'in the freezer', 'in the fridge')
-        prior       = (     1/5      ,       2/5       ,       2/5      )
-
-        pred_probs = predict_proba(prompts,
-                                   completions=class_names,
-                                   model_and_tokenizer=(model, tokenizer),
-                                   prior=prior)
-
-        pred_probs = pred_probs.round(1) # just for cleaner output
-
-        # predicted probability that tacos cook on the stove
-        pred_probs[0,0]
-        # 0.4
-
-        # predicted probability that ice cream is in the freezer
-        pred_probs[1,1]
-        # 0.5
-
-        # predicted probability that ice cream is in the fridge
-        pred_probs[1,2]
-        # 0.4
-    """
-    return log_probs_conditional(
-        prompts,
-        completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        end_of_prompt=end_of_prompt,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict_proba_examples
-def predict_proba_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
-        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
-        probability that `examples[example_idx].completions[completion_idx]` comes after
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-        If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
-
-    Example
-    -------
-    GPT-2 (small) doing media trivia::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify import predict_proba_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [
-            Example(prompt='Jodie Foster played',
-                    completions=('Clarice Starling', 'Trinity in The Matrix')),
-            Example(prompt='Batman, from Batman: The Animated Series, was played by',
-                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
-                    prior=      (     2/3      ,      1/3     ,      0      ))
-        ]
-
-        pred_probs = predict_proba_examples(examples,
-                                            model_and_tokenizer=(model, tokenizer))
-
-        # predicted probability that Jodie Foster played Clarice Starling, not Trinity
-        pred_probs[0][0]
-        # 0.7
-
-        # predicted probability that Batman was played by Kevin Conroy
-        pred_probs[0][1]
-        # 0.97
-    """
-    return log_probs_conditional_examples(
-        examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict
-def predict(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    prior: Optional[Sequence[float]] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(prompts)`.
-        `preds[prompt_idx]` is the completion in `completions` which is predicted to
-        follow `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_examples`.
-
-    Example
-    -------
-    Let's have GPT-2 (small) predict where stuff is in the kitchen::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify import predict
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Define a classification task
-        prompts = ['The tacos are cooking', 'Ice cream is']
-        class_names = ('on the stove', 'in the freezer', 'in the fridge')
-        prior       = (     1/5      ,       2/5       ,       2/5      )
-
-        preds = predict(prompts,
-                        completions=class_names,
-                        model_and_tokenizer=(model, tokenizer),
-                        prior=prior)
-        preds
-        # ['on the stove',
-        #  'in the freezer']
-    """
-    return predict_proba(
-        prompts,
-        completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        prior=prior,
-        end_of_prompt=end_of_prompt,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict_examples
-def predict_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(examples)`.
-        `preds[example_idx]` is the completion in `examples[example_idx].completions`
-        which is predicted to follow
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-    Example
-    -------
-    GPT-2 (small) doing media trivia::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify import predict_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [
-            Example(prompt='Jodie Foster played',
-                    completions=('Clarice Starling', 'Trinity in The Matrix')),
-            Example(prompt='Batman, from Batman: The Animated Series, was played by',
-                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
-                    prior=      (     2/3      ,      1/3     ,      0      ))
-        ]
-
-        preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
-        preds
-        # ['Clarice Starling',
-        #  'Kevin Conroy']
-    """
-    return predict_proba_examples(
-        examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        batch_size=batch_size,
-    )
+"""
+Perform prompt-completion classification using a ``transformers.AutoModelForCausalLM``.
+Currently, only PyTorch models are supported.
+
+In the implementation, attention block keys and values for prompts are cached and shared
+across completions. See the computational performance `here`_.
+
+.. _here: https://cappr.readthedocs.io/en/latest/6_computational_performance.html
+
+You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
+
+.. warning:: This module currently requires that ``end_of_prompt`` is a whitespace.
+
+.. warning:: This module doesn't work with ``transformers.BartForCausalLM``, among
+             others probably.
+"""
+from __future__ import annotations
+from typing import Mapping, Optional, Sequence, Union
+
+import numpy as np
+import numpy.typing as npt
+import torch
+from transformers import AutoModelForCausalLM, PreTrainedTokenizer, BatchEncoding
+
+from cappr.utils import _batch, classify
+from cappr import Example
+from cappr import huggingface as hf
+
+
+def _keys_values_prompts(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    num_repeats_per_prompt: Union[int, Sequence[int]],
+) -> tuple[
+    tuple[torch.Tensor, torch.Tensor], BatchEncoding, torch.Tensor, torch.Tensor
+]:
+    """
+    Efficiently performs this procedure:
+
+    1. Repeat-interleave `prompts[i]` `num_repeats_per_prompt[i]` times.
+
+       Or, if `num_repeats_per_prompt` is an integer, repeat-interleave `prompts[i]`
+       `num_repeats_per_prompt` times.
+
+       For example, if there are 2 prompts and `num_repeats_per_prompt=(2,3)`, the
+       repeated prompts look like::
+
+           [prompts[0],
+            prompts[0],
+            prompts[1],
+            prompts[1],
+            prompts[1]]
+
+    2. Apply `tokenizer` to the repeated prompts.
+
+    3. Apply `model`.
+
+    Parameters
+    ----------
+    model : AutoModelForCausalLM
+        an autoregressive transformer language model
+    tokenizer : PreTrainedTokenizer
+        the tokenizer corresponding to `model`
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    num_repeats_per_prompt : Union[int, Sequence[int]]
+        the numer of times to repeat each prompt in `prompts`
+
+    Returns
+    -------
+    past_key_values : tuple[torch.Tensor, torch.Tensor]
+        for each attention block in `model`, the keys and values for each prompt in the
+        repeated prompts
+    encodings : BatchEncoding
+        the tokenizer output for the repeated prompts
+    offsets : torch.Tensor
+        the number of (non-pad) tokens in each of the repeated prompts
+    last_nonpad_token_logits : torch.Tensor
+        next-token logits for the last non-pad token for each of the repeated prompts
+
+    Raises
+    ------
+    ValueError
+        if the `tokenizer` is not using right-padding
+    TypeError
+        if `prompts` is not a `Sequence`
+    ValueError
+        if `num_repeats_per_prompt` is a `Sequence` whose length is not the same as the
+        length of `prompts`
+    """
+    if not tokenizer.padding_side == "right":
+        raise ValueError(
+            "Gotta use right padding to ensure position IDs are correct. "
+            "Run tokenizer.padding_side = 'right' if sensible."
+        )
+    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
+        raise TypeError("prompts must be a Sequence of strings.")
+    if isinstance(num_repeats_per_prompt, Sequence):
+        if not len(prompts) == len(num_repeats_per_prompt):
+            raise ValueError(
+                "If num_repeats_per_prompt is a Sequence, then it must be the same "
+                f"length as prompts. Got lengths {len(num_repeats_per_prompt)}, "
+                f"{len(prompts)}."
+            )
+    if not isinstance(num_repeats_per_prompt, int) and not isinstance(
+        num_repeats_per_prompt, torch.Tensor
+    ):
+        num_repeats_per_prompt = torch.tensor(
+            num_repeats_per_prompt, device=model.device
+        )
+
+    ## Batch inference prompts
+    prompts = list(prompts)  ## 0-index in case it's a Series or something
+    # fmt: off
+    encodings: BatchEncoding = (tokenizer(prompts, return_tensors="pt", padding=True)
+                                .to(model.device))
+    # fmt: on
+    with torch.no_grad():
+        out = model(**encodings)
+
+    ## We need to repeat each prompt's keys and values num_repeats_per_prompt times
+    ## For layer i, prompts_out.past_key_values[i] is a tuple (key, value),
+    ## each w/ shape: (batch size=len(prompts),
+    ##                 number of attention heads=12 for gpt2,
+    ##                 encodings.input_ids.shape[-1],
+    ##                 key/value hidden dimension=64 for gpt2)
+    past_key_values = (
+        torch.stack([torch.stack(block) for block in out.past_key_values], dim=0)
+        ## The tuple is now a tensor w/ shape:
+        ## (# layers=12 for gpt2,
+        ##  2 (for key and value),
+        ##  and then the rest as before)
+        ## Repeat along batch size dim so that it aligns downstream w/ completions
+        .repeat_interleave(num_repeats_per_prompt, dim=2)
+    )
+    ## Re-format this tensor to the nested tuple format we'd get if we passed multiple
+    ## copies of the prompt at the same time to the model
+    past_key_values = tuple(
+        [(layer[0], layer[1]) for layer in past_key_values]  ## keys, values
+    )
+
+    ## Repeat stuff
+    # fmt: off
+    encodings["attention_mask"] = (encodings
+                                   .attention_mask
+                                   .repeat_interleave(num_repeats_per_prompt,
+                                                      dim=0))
+    encodings["input_ids"] = (encodings
+                              .input_ids
+                              .repeat_interleave(num_repeats_per_prompt, dim=0))
+    # fmt: on
+
+    ## Need offsets so that position_ids for future tokens are set correctly
+    offsets: torch.Tensor = encodings.attention_mask.sum(dim=1)
+
+    ## Need (next-token) logits from prompts, i.e., last non-pad prompt token, since
+    ## that contains the first completion token's log-probability
+    _last_nonpad_token_idxs = (offsets - 1)[:, None, None]
+    # fmt: off
+    last_nonpad_token_logits: torch.Tensor = (out
+                                              .logits
+                                              .repeat_interleave(
+                                                  num_repeats_per_prompt, dim=0)
+                                              .take_along_dim(
+                                                  _last_nonpad_token_idxs, dim=1))
+    # fmt: on
+
+    return past_key_values, encodings, offsets, last_nonpad_token_logits
+
+
+def _blessed_helper(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    num_completions_per_prompt: Union[int, Sequence[int]],
+    completions_repeats: int,
+) -> tuple[torch.Tensor, BatchEncoding]:
+    """
+    TODO: docstring
+    """
+    if not tokenizer.padding_side == "right":
+        raise ValueError(
+            "Gotta use right padding to ensure position IDs are correct. "
+            "Run tokenizer.padding_side = 'right' if sensible."
+        )
+    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
+        raise TypeError("prompts must be a Sequence of strings.")
+    if isinstance(completions, str) or not isinstance(completions, Sequence):
+        raise TypeError("completions must be a Sequence of strings.")
+
+    ## Prepare prompt data
+    (
+        past_key_values,
+        prompts_encodings,
+        offsets,
+        prompts_last_nonpad_token_logits,
+    ) = _keys_values_prompts(model, tokenizer, prompts, num_completions_per_prompt)
+
+    ## Prepare completion data
+    completions = list(completions)  ## 0-index in case it's a Series or somethin
+    # fmt: off
+    completions_encoding = (tokenizer(completions, return_tensors="pt", padding=True)
+                            .to(model.device))
+    completions_input_ids = (completions_encoding
+                             .input_ids
+                             .repeat(completions_repeats, 1))
+    completions_attention_mask = (completions_encoding
+                                  .attention_mask
+                                  .repeat(completions_repeats, 1))
+    # fmt: on
+    ## Set position_ids to what they were had we fed the prompt + completion together w/
+    ## right-padding (right b/c GPT-2 uses absolute position ids)
+    _num_completion_tokens = completions_encoding.input_ids.shape[1]
+    completions_position_ids = (
+        torch.arange(_num_completion_tokens, device=model.device) + offsets[:, None]
+    )
+    ## Need attention_mask to include the prompt since it prolly has padding
+    attention_mask = torch.cat(
+        (prompts_encodings["attention_mask"], completions_attention_mask), dim=1
+    )
+
+    ## Everything should now be aligned 🤞 🙏
+    with torch.no_grad():
+        completions_out = model(
+            input_ids=completions_input_ids,
+            attention_mask=attention_mask,
+            past_key_values=past_key_values,
+            position_ids=completions_position_ids,
+        )
+    ## 😎
+
+    ## You need to be able to ignore pad tokens, so you need this data as well
+    encodings = BatchEncoding(
+        {
+            "input_ids": completions_input_ids,
+            "attention_mask": completions_attention_mask,
+            "offsets": offsets,
+        }
+    )
+
+    ## Let's drop the next-token logits for the last completion token b/c they're not
+    ## useful for our purposes. Moreover, dropping ensures
+    ## logits.shape[:2] == encodings['input_ids'].shape, as one expects.
+    ## Just keep in mind that `logits` are shifted behind.
+    logits = torch.cat(
+        [prompts_last_nonpad_token_logits, completions_out.logits[:, :-1, :]], dim=1
+    )
+
+    return logits, encodings
+
+
+def _logits_completions_given_prompts(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    end_of_prompt: str = " ",
+):
+    """
+    TODO: convert docstring to numpy style
+
+    If `texts` is
+
+    ```python
+    [prompt + end_of_prompt + completions
+     for prompt in prompts
+     for completion in completions]
+    ```
+
+    then this function returns
+
+    1. `logits`: tensor with shape
+
+        (`len(texts)`, max # tokens `completions`, `tokenizer.vocab_size`)
+
+    where `logits[i,j]` are the `model`'s logits for token `j+1` of the completion in
+    `texts[i]` given the prompt in `texts[i]`. This tensor includes logits for
+    right-padded tokens. Use the `encodings.attention_mask` to ignore them before
+    further processing.
+
+    2. `encodings`: `BatchEncoding` containing the input IDs, attention mask,
+    and position offsets.
+    """
+    if end_of_prompt != " ":
+        raise ValueError("end_of_prompt must be ' ' for now. Sorry!")
+    completions = [end_of_prompt + completion.lstrip() for completion in completions]
+    ## TODO: figure out how to do this generally, not just for ' ' end_of_prompt
+    return _blessed_helper(
+        model,
+        tokenizer,
+        prompts,
+        completions,
+        num_completions_per_prompt=len(completions),
+        completions_repeats=len(prompts),
+    )
+
+
+def _logits_completions_given_prompts_examples(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    examples: Sequence[Example],
+):
+    """
+    TODO: convert docstring to numpy style
+
+    If `texts` is
+
+    ```python
+    [example.prompt + example.end_of_prompt + completion
+     for example in examples
+     for completion in example.completions]
+    ```
+    then this function returns
+
+    1. `logits`: tensor with shape
+
+        (`len(texts)`, max # tokens `completions`, `tokenizer.vocab_size`)
+
+    where `logits[i,j]` are the `model`'s logits for token `j+1` of the completion in
+    `texts[i]` given the prompt in `texts[i]`. This tensor includes logits for
+    right-padded tokens. Use the `encodings.attention_mask` to ignore them before
+    further processing.
+
+    2. `encodings`: `BatchEncoding` containing the input IDs, attention mask,
+    and position offsets.
+    """
+    if any([example.end_of_prompt != " " for example in examples]):
+        raise ValueError("Every example's end_of_prompt must be ' ' for now. Sorry!")
+    prompts = [example.prompt for example in examples]
+    completions = [
+        example.end_of_prompt + completion.lstrip()
+        for example in examples
+        for completion in example.completions
+    ]
+    ## TODO: figure out how to do this generally, not just for ' ' end_of_prompt
+    num_completions_per_prompt = [len(example.completions) for example in examples]
+    completions_repeats = 1
+    return _blessed_helper(
+        model,
+        tokenizer,
+        prompts,
+        completions,
+        num_completions_per_prompt=num_completions_per_prompt,
+        completions_repeats=completions_repeats,
+    )
+
+
+def _logits_to_log_probs_completions(
+    logits: torch.Tensor, encodings: Mapping[str, torch.Tensor]
+) -> list[list[float]]:
+    """
+    TODO: convert docstring to numpy style
+
+    Returns a list `log_probs_completions` where `log_probs_completions[i][j]` is the
+    log-probablity of *completion* token
+
+        `encodings['input_ids'][i,j]`
+
+    given its previous tokens
+
+        `encodings['input_ids'][i,:j]`
+
+    Pad tokens, i.e., tokens where `encodings['attention_mask'] == 0` are excluded.
+
+    `logits[i,j]` is assumed to be an unnormalized distribution (over tokens in
+    the vocab) given tokens `input_ids[i,:j]`.
+    """
+    log_probs = hf._utils.logits_to_log_probs(
+        logits, encodings["input_ids"], input_ids_start_idx=None, logits_end_idx=None
+    )
+    last_idx_non_pad = encodings["attention_mask"].sum(dim=1)
+    ## i.e., # of tokens per completion
+    return [
+        log_probs_prompt_completion[:completion_end].tolist()
+        for log_probs_prompt_completion, completion_end in zip(
+            log_probs, last_idx_non_pad
+        )
+    ]
+
+
+def log_probs_conditional(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> list[list[list[float]]]:
+    """
+    Log-probabilities of each completion token conditional on each prompt and previous
+    completion tokens.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
+        log-probability of the completion token in `completions[completion_idx]`,
+        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
+        completion tokens.
+
+    Note
+    ----
+    To efficiently aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify import log_probs_conditional
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        prompts = ['x y', 'a b c']
+        completions = ['z', 'd e']
+
+        # Compute
+        log_probs_completions = log_probs_conditional(
+                                    prompts,
+                                    completions,
+                                    model_and_tokenizer=(model, tokenizer)
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0]
+        # [[-4.5],        [[log Pr(z | x, y)],
+        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1]
+        # [[-9.7],        [[log Pr(z | a, b, c)],
+        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+    """
+    model, tokenizer = hf._utils.load_model_and_tokenizer(
+        model=model, model_and_tokenizer=model_and_tokenizer
+    )
+
+    @_batch.flatten
+    @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs")
+    def log_probs_completions_batch(prompts, batch_size=batch_size):
+        logits, encodings = _logits_completions_given_prompts(
+            model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
+        )
+        return _logits_to_log_probs_completions(logits, encodings)
+
+    log_probs_completions = log_probs_completions_batch(prompts)
+    return list(_batch.constant(log_probs_completions, size=len(completions)))
+
+
+def log_probs_conditional_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> list[list[list[float]]]:
+    """
+    Log-probabilities of each completion token conditional on each prompt and previous
+    completion tokens.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
+        the log-probability of the completion token in
+        `examples[example_idx].completions[completion_idx]`, conditional on
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
+        previous completion tokens.
+
+    Note
+    ----
+    To aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Note
+    ----
+    The attribute :attr:`cappr.Example.prior` is unused.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify import log_probs_conditional_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [Example(prompt='x y',   completions=('z', 'd e')),
+                    Example(prompt='a b c', completions=('1 2',))]
+
+        # Compute
+        log_probs_completions = log_probs_conditional_examples(
+                                    examples,
+                                    model_and_tokenizer=(model, tokenizer)
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0] # corresponds to examples[0]
+        # [[-4.5],        [[log Pr(z | x, y)],
+        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1] # corresponds to examples[1]
+        # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
+    """
+    model, tokenizer = hf._utils.load_model_and_tokenizer(
+        model=model, model_and_tokenizer=model_and_tokenizer
+    )
+
+    @_batch.flatten
+    @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs")
+    def log_probs_completions_batch(examples, batch_size=batch_size):
+        logits, encodings = _logits_completions_given_prompts_examples(
+            model, tokenizer, examples
+        )
+        return _logits_to_log_probs_completions(logits, encodings)
+
+    log_probs_completions = log_probs_completions_batch(examples)
+    num_completions_per_prompt = [len(example.completions) for example in examples]
+    return list(
+        _batch.variable(log_probs_completions, sizes=num_completions_per_prompt)
+    )
+
+
+@classify._predict_proba
+def predict_proba(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    prior: Optional[Sequence[float]] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> npt.NDArray[np.floating]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    pred_probs : npt.NDArray[np.floating]
+        Array with shape `(len(prompts), len(completions))`.
+        `pred_probs[prompt_idx, completion_idx]` is the model's estimate of the
+        probability that `completions[completion_idx]` comes after
+        `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_proba_examples`.
+
+    Example
+    -------
+    Let's have GPT-2 (small) predict where stuff is in the kitchen. This example also
+    conveys that it's not the greatest model out there::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify import predict_proba
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Define a classification task
+        prompts = ['The tacos are cooking',
+                   'Ice cream is']
+        class_names = ('on the stove', 'in the freezer', 'in the fridge')
+        prior       = (     1/5      ,       2/5       ,       2/5      )
+
+        pred_probs = predict_proba(prompts,
+                                   completions=class_names,
+                                   model_and_tokenizer=(model, tokenizer),
+                                   prior=prior)
+
+        pred_probs = pred_probs.round(1) # just for cleaner output
+
+        # predicted probability that tacos cook on the stove
+        pred_probs[0,0]
+        # 0.4
+
+        # predicted probability that ice cream is in the freezer
+        pred_probs[1,1]
+        # 0.5
+
+        # predicted probability that ice cream is in the fridge
+        pred_probs[1,2]
+        # 0.4
+    """
+    return log_probs_conditional(
+        prompts,
+        completions,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        end_of_prompt=end_of_prompt,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict_proba_examples
+def predict_proba_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
+        probability that `examples[example_idx].completions[completion_idx]` comes after
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+        If the number of completions per example is a constant `k`, then an array with
+        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+
+    Example
+    -------
+    GPT-2 (small) doing media trivia::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify import predict_proba_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [
+            Example(prompt='Jodie Foster played',
+                    completions=('Clarice Starling', 'Trinity in The Matrix')),
+            Example(prompt='Batman, from Batman: The Animated Series, was played by',
+                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
+                    prior=      (     2/3      ,      1/3     ,      0      ))
+        ]
+
+        pred_probs = predict_proba_examples(examples,
+                                            model_and_tokenizer=(model, tokenizer))
+
+        # predicted probability that Jodie Foster played Clarice Starling, not Trinity
+        pred_probs[0][0]
+        # 0.7
+
+        # predicted probability that Batman was played by Kevin Conroy
+        pred_probs[0][1]
+        # 0.97
+    """
+    return log_probs_conditional_examples(
+        examples,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict
+def predict(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    prior: Optional[Sequence[float]] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(prompts)`.
+        `preds[prompt_idx]` is the completion in `completions` which is predicted to
+        follow `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_examples`.
+
+    Example
+    -------
+    Let's have GPT-2 (small) predict where stuff is in the kitchen::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify import predict
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Define a classification task
+        prompts = ['The tacos are cooking', 'Ice cream is']
+        class_names = ('on the stove', 'in the freezer', 'in the fridge')
+        prior       = (     1/5      ,       2/5       ,       2/5      )
+
+        preds = predict(prompts,
+                        completions=class_names,
+                        model_and_tokenizer=(model, tokenizer),
+                        prior=prior)
+        preds
+        # ['on the stove',
+        #  'in the freezer']
+    """
+    return predict_proba(
+        prompts,
+        completions,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        prior=prior,
+        end_of_prompt=end_of_prompt,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict_examples
+def predict_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(examples)`.
+        `preds[example_idx]` is the completion in `examples[example_idx].completions`
+        which is predicted to follow
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+    Example
+    -------
+    GPT-2 (small) doing media trivia::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify import predict_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [
+            Example(prompt='Jodie Foster played',
+                    completions=('Clarice Starling', 'Trinity in The Matrix')),
+            Example(prompt='Batman, from Batman: The Animated Series, was played by',
+                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
+                    prior=      (     2/3      ,      1/3     ,      0      ))
+        ]
+
+        preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
+        preds
+        # ['Clarice Starling',
+        #  'Kevin Conroy']
+    """
+    return predict_proba_examples(
+        examples,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        batch_size=batch_size,
+    )
```

### Comparing `cappr-0.2.1/src/cappr/huggingface/classify_no_cache.py` & `cappr-0.2.2/src/cappr/huggingface/classify_no_cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,750 +1,750 @@
-"""
-Perform prompt-completion classification using a ``transformers.AutoModelForCausalLM``.
-Currently, only PyTorch models are supported.
-
-This module is a mirror of :mod:`cappr.huggingface.classify` which **does not**
-precompute attention block keys and values for prompts. Not precomputing may be faster
-if the batch size is small, as is the case during live inference. See the computational
-performance `here`_.
-
-.. _here: https://cappr.readthedocs.io/en/latest/6_computational_performance.html
-
-You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
-"""
-from __future__ import annotations
-from typing import Mapping, Optional, Sequence, Union
-
-import numpy as np
-import numpy.typing as npt
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer, BatchEncoding
-
-from cappr.utils import _batch, classify
-from cappr import Example
-from cappr import huggingface as hf
-
-
-def _keys_values_prompts(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    num_completions_per_prompt: Union[int, Sequence[int]],
-):
-    """
-    Performs this procedure:
-
-    1. Repeat-interleave `prompts[i]` `num_repeats_per_prompt[i]` times.
-
-       Or, if `num_repeats_per_prompt` is an integer, repeat-interleave `prompts[i]`
-       `num_repeats_per_prompt` times.
-
-       For example, if there are 2 prompts and `num_repeats_per_prompt=(2,3)`, the
-       repeated prompts look like::
-
-           [prompts[0],
-            prompts[0],
-            prompts[1],
-            prompts[1],
-            prompts[1]]
-
-    2. Apply `tokenizer` to the repeated prompts.
-
-    3. Apply `model`.
-
-    Note
-    ----
-    This function is only used to test
-    :func:`cappr.huggingface.classify._keys_values_prompts`.
-
-    Parameters
-    ----------
-    model : AutoModelForCausalLM
-        an autoregressive transformer language model
-    tokenizer : AutoTokenizer
-        the tokenizer corresponding to `model`
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    num_repeats_per_prompt : Union[int, Sequence[int]]
-        the numer of times to repeat each prompt in `prompts`
-
-    Returns
-    -------
-    past_key_values : tuple[torch.Tensor, torch.Tensor]
-        for each attention block in `model`, the keys and values for each prompt in the
-        repeated prompts
-    encodings : BatchEncoding
-        the tokenizer output for the repeated prompts
-    offsets : torch.Tensor
-        the number of (non-pad) tokens in each of the repeated prompts
-    last_nonpad_token_logits : torch.Tensor
-        next-token logits for the last non-pad token for each of the repeated prompts
-
-    Raises
-    ------
-    ValueError
-        if the `tokenizer` is not using right-padding
-    TypeError
-        if `prompts` is not a `Sequence`
-    ValueError
-        if `num_repeats_per_prompt` is a `Sequence` whose length is not the same as the
-        length of `prompts`
-    """
-    if not tokenizer.padding_side == "right":
-        raise ValueError("Gotta use right padding to ensure position IDs are correct.")
-    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
-        raise TypeError("prompts must be a Sequence of strings.")
-    if isinstance(num_completions_per_prompt, Sequence):
-        if not len(prompts) == len(num_completions_per_prompt):
-            raise ValueError(
-                "If num_completions_per_prompt is a Sequence, then it must be the same "
-                f"length as prompts. Got lengths {len(num_completions_per_prompt)}, "
-                f"{len(prompts)}."
-            )
-    if isinstance(num_completions_per_prompt, int):
-        ## For code simplicity, just repeat it
-        num_completions_per_prompt = [num_completions_per_prompt] * len(prompts)
-    prompts_repeated = [
-        prompt
-        for prompt, num_repeats in zip(prompts, num_completions_per_prompt)
-        for _ in range(num_repeats)
-    ]
-    # fmt: off
-    encodings: BatchEncoding = (tokenizer(prompts_repeated, return_tensors="pt",
-                                          padding=True)
-                                .to(model.device))
-    # fmt: on
-    with torch.no_grad():
-        out = model(**encodings)
-
-    offsets: torch.Tensor = encodings.attention_mask.sum(dim=1)
-
-    ## Need (next-token) logits from prompts, i.e., last non-pad prompt token, since
-    ## that contains the first completion token's log-probability
-    _last_nonpad_token_idxs = (offsets - 1)[:, None, None]
-    last_nonpad_token_logits: torch.Tensor = out.logits.take_along_dim(
-        _last_nonpad_token_idxs, dim=1
-    )
-
-    return out.past_key_values, encodings, offsets, last_nonpad_token_logits
-
-
-def _logits_texts(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    texts: Sequence[str],
-) -> tuple[torch.Tensor, BatchEncoding]:
-    encodings = tokenizer(texts, return_tensors="pt", padding=True).to(model.device)
-    with torch.no_grad():
-        out = model(**encodings)
-    return out.logits, encodings
-
-
-def _prompts_offsets(
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    num_completions_per_prompt: Union[int, Sequence[int]],
-) -> torch.Tensor:
-    if not isinstance(num_completions_per_prompt, int) and not isinstance(
-        num_completions_per_prompt, torch.Tensor
-    ):
-        num_completions_per_prompt = torch.tensor(num_completions_per_prompt)
-    return (
-        tokenizer(prompts, return_tensors="pt", padding=True)
-        .attention_mask.repeat_interleave(num_completions_per_prompt, dim=0)
-        .sum(dim=1)
-    )
-
-
-def _logits_completions_given_prompts(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    end_of_prompt: str = " ",
-):
-    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
-        raise TypeError("prompts must be a Sequence of strings.")
-    if isinstance(completions, str) or not isinstance(completions, Sequence):
-        raise TypeError("completions must be a Sequence of strings.")
-    texts = [
-        prompt + end_of_prompt + completion
-        for prompt in prompts
-        for completion in completions
-    ]
-    logits, encodings = _logits_texts(model, tokenizer, texts)
-    ## Need these indices to slice completion tokens
-    encodings["offsets"] = _prompts_offsets(
-        tokenizer, prompts, num_completions_per_prompt=len(completions)
-    ).to(model.device)
-    return logits, encodings
-
-
-def _logits_completions_given_prompts_examples(
-    model: AutoModelForCausalLM,
-    tokenizer: AutoTokenizer,
-    examples: Sequence[Example],
-):
-    texts = [
-        example.prompt + example.end_of_prompt + completion
-        for example in examples
-        for completion in example.completions
-    ]
-    logits, encodings = _logits_texts(model, tokenizer, texts)
-    ## Need these indices to slice completion tokens
-    prompts = [example.prompt for example in examples]
-    num_completions_per_prompt = [len(example.completions) for example in examples]
-    encodings["offsets"] = _prompts_offsets(
-        tokenizer, prompts, num_completions_per_prompt=num_completions_per_prompt
-    )
-    return logits, encodings
-
-
-def _logits_to_log_probs_completions(
-    logits: torch.Tensor, encodings: Mapping[str, torch.Tensor]
-) -> list[list[float]]:
-    log_probs = hf._utils.logits_to_log_probs(
-        logits, encodings["input_ids"], input_ids_start_idx=1, logits_end_idx=-1
-    )
-    last_idx_non_pad = encodings["attention_mask"].sum(dim=1)
-    ## i.e., # of tokens per text
-    return [
-        log_probs_prompt_completion[completion_start:completion_end].tolist()
-        for log_probs_prompt_completion, completion_start, completion_end in zip(
-            log_probs, encodings["offsets"] - 1, last_idx_non_pad - 1
-        )
-    ]
-
-
-def log_probs_conditional(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> list[list[list[float]]]:
-    """
-    Log-probabilities of each completion token conditional on each prompt and previous
-    completion tokens.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
-        log-probability of the completion token in `completions[completion_idx]`,
-        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
-        completion tokens.
-
-    Note
-    ----
-    To efficiently aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs_from_constant_completions`.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify_no_cache import log_probs_conditional
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        prompts = ['x y', 'a b c']
-        completions = ['z', 'd e']
-
-        # Compute
-        log_probs_completions = log_probs_conditional(
-                                    prompts,
-                                    completions,
-                                    model_and_tokenizer=(model, tokenizer)
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0]
-        # [[-4.5],        [[log Pr(z | x, y)],
-        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1]
-        # [[-9.7],        [[log Pr(z | a, b, c)],
-        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
-    """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
-
-    @_batch.flatten
-    @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs (no cache)")
-    def log_probs_completions_batch(prompts, batch_size=batch_size):
-        logits, encodings = _logits_completions_given_prompts(
-            model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
-        )
-        return _logits_to_log_probs_completions(logits, encodings)
-
-    log_probs_completions = log_probs_completions_batch(prompts)
-    return list(_batch.constant(log_probs_completions, size=len(completions)))
-
-
-def log_probs_conditional_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> list[list[list[float]]]:
-    """
-    Log-probabilities of each completion token conditional on each prompt and previous
-    completion tokens.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
-        the log-probability of the completion token in
-        `examples[example_idx].completions[completion_idx]`, conditional on
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
-        previous completion tokens.
-
-    Note
-    ----
-    To aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs`.
-
-    Note
-    ----
-    The attribute :attr:`cappr.Example.prior` is unused.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify_no_cache import log_probs_conditional_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [Example(prompt='x y',   completions=('z', 'd e')),
-                    Example(prompt='a b c', completions=('1 2',))]
-
-        # Compute
-        log_probs_completions = log_probs_conditional_examples(
-                                    examples,
-                                    model_and_tokenizer=(model, tokenizer)
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0] # corresponds to examples[0]
-        # [[-4.5],        [[log Pr(z | x, y)],
-        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1] # corresponds to examples[1]
-        # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
-    """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
-
-    @_batch.flatten
-    @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs (no cache)")
-    def log_probs_completions_batch(examples, batch_size=batch_size):
-        logits, encodings = _logits_completions_given_prompts_examples(
-            model, tokenizer, examples
-        )
-        return _logits_to_log_probs_completions(logits, encodings)
-
-    log_probs_completions = log_probs_completions_batch(examples)
-    num_completions_per_prompt = [len(example.completions) for example in examples]
-    return list(
-        _batch.variable(log_probs_completions, sizes=num_completions_per_prompt)
-    )
-
-
-@classify._predict_proba
-def predict_proba(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> npt.NDArray[np.floating]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    pred_probs : npt.NDArray[np.floating]
-        Array with shape `(len(prompts), len(completions))`.
-        `pred_probs[prompt_idx, completion_idx]` is the model's estimate of the
-        probability that `completions[completion_idx]` comes after
-        `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_proba_examples`.
-
-    Example
-    -------
-    Let's have GPT-2 (small) predict where stuff is in the kitchen. This example also
-    conveys that it's not the greatest model out there::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify_no_cache import predict_proba
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Define a classification task
-        prompts = ['The tacos are cooking',
-                   'Ice cream is']
-        class_names = ('on the stove', 'in the freezer', 'in the fridge')
-        prior       = (     1/5      ,       2/5       ,       2/5      )
-
-        pred_probs = predict_proba(prompts,
-                                   completions=class_names,
-                                   model_and_tokenizer=(model, tokenizer),
-                                   prior=prior)
-
-        pred_probs = pred_probs.round(1) # just for cleaner output
-
-        # predicted probability that tacos cook on the stove
-        pred_probs[0,0]
-        # 0.4
-
-        # predicted probability that ice cream is in the freezer
-        pred_probs[1,1]
-        # 0.5
-
-        # predicted probability that ice cream is in the fridge
-        pred_probs[1,2]
-        # 0.4
-    """
-    return log_probs_conditional(
-        prompts,
-        completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        end_of_prompt=end_of_prompt,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict_proba_examples
-def predict_proba_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
-        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
-        probability that `examples[example_idx].completions[completion_idx]` comes after
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-        If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
-
-    Example
-    -------
-    GPT-2 (small) doing media trivia::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify_no_cache import predict_proba_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [
-            Example(prompt='Jodie Foster played',
-                    completions=('Clarice Starling', 'Trinity in The Matrix')),
-            Example(prompt='Batman, from Batman: The Animated Series, was played by',
-                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
-                    prior=      (     2/3      ,      1/3     ,      0      ))
-        ]
-
-        pred_probs = predict_proba_examples(examples,
-                                            model_and_tokenizer=(model, tokenizer))
-
-        # predicted probability that Jodie Foster played Clarice Starling, not Trinity
-        pred_probs[0][0]
-        # 0.7
-
-        # predicted probability that Batman was played by Kevin Conroy
-        pred_probs[0][1]
-        # 0.97
-    """
-    return log_probs_conditional_examples(
-        examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict
-def predict(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    prior: Optional[Sequence[float]] = None,
-    end_of_prompt: str = " ",
-    batch_size: int = 32,
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(prompts)`.
-        `preds[prompt_idx]` is the completion in `completions` which is predicted to
-        follow `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_examples`.
-
-    Example
-    -------
-    Let's have GPT-2 (small) predict where stuff is in the kitchen::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr.huggingface.classify_no_cache import predict
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Define a classification task
-        prompts = ['The tacos are cooking', 'Ice cream is']
-        class_names = ('on the stove', 'in the freezer', 'in the fridge')
-        prior       = (     1/5      ,       2/5       ,       2/5      )
-
-        preds = predict(prompts,
-                        completions=class_names,
-                        model_and_tokenizer=(model, tokenizer),
-                        prior=prior)
-        preds
-        # ['on the stove',
-        #  'in the freezer']
-    """
-    return predict_proba(
-        prompts,
-        completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        prior=prior,
-        end_of_prompt=end_of_prompt,
-        batch_size=batch_size,
-    )
-
-
-@classify._predict_examples
-def predict_examples(
-    examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, AutoTokenizer] = None,
-    batch_size: int = 32,
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, AutoTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
-    batch_size : int, optional
-        the maximum number of inputs that the model will process in parallel, by default
-        32
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(examples)`.
-        `preds[example_idx]` is the completion in `examples[example_idx].completions`
-        which is predicted to follow
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-    Example
-    -------
-    GPT-2 (small) doing media trivia::
-
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        from cappr import Example
-        from cappr.huggingface.classify_no_cache import predict_examples
-
-        # Load model and tokenizer
-        model = AutoModelForCausalLM.from_pretrained('gpt2')
-        tokenizer = AutoTokenizer.from_pretrained('gpt2')
-
-        # Create data
-        examples = [
-            Example(prompt='Jodie Foster played',
-                    completions=('Clarice Starling', 'Trinity in The Matrix')),
-            Example(prompt='Batman, from Batman: The Animated Series, was played by',
-                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
-                    prior=      (     2/3      ,      1/3     ,      0      ))
-        ]
-
-        preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
-        preds
-        # ['Clarice Starling',
-        #  'Kevin Conroy']
-    """
-    return predict_proba_examples(
-        examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
-        batch_size=batch_size,
-    )
+"""
+Perform prompt-completion classification using a ``transformers.AutoModelForCausalLM``.
+Currently, only PyTorch models are supported.
+
+This module is a mirror of :mod:`cappr.huggingface.classify` which **does not**
+precompute attention block keys and values for prompts.
+
+This module may happen to be compatible with a slightly broader class of
+causal/autoregressive language models, as the model's forward method is only assumed
+take input IDs and the attention mask.
+
+You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
+"""
+from __future__ import annotations
+from typing import Mapping, Optional, Sequence, Union
+
+import numpy as np
+import numpy.typing as npt
+import torch
+from transformers import AutoModelForCausalLM, BatchEncoding, PreTrainedTokenizer
+
+from cappr.utils import _batch, classify
+from cappr import Example
+from cappr import huggingface as hf
+
+
+def _keys_values_prompts(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    num_completions_per_prompt: Union[int, Sequence[int]],
+):
+    """
+    Performs this procedure:
+
+    1. Repeat-interleave `prompts[i]` `num_repeats_per_prompt[i]` times.
+
+       Or, if `num_repeats_per_prompt` is an integer, repeat-interleave `prompts[i]`
+       `num_repeats_per_prompt` times.
+
+       For example, if there are 2 prompts and `num_repeats_per_prompt=(2,3)`, the
+       repeated prompts look like::
+
+           [prompts[0],
+            prompts[0],
+            prompts[1],
+            prompts[1],
+            prompts[1]]
+
+    2. Apply `tokenizer` to the repeated prompts.
+
+    3. Apply `model`.
+
+    Note
+    ----
+    This function is only used to test
+    :func:`cappr.huggingface.classify._keys_values_prompts`.
+
+    Parameters
+    ----------
+    model : AutoModelForCausalLM
+        an autoregressive transformer language model
+    tokenizer : PreTrainedTokenizer
+        the tokenizer corresponding to `model`
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    num_repeats_per_prompt : Union[int, Sequence[int]]
+        the numer of times to repeat each prompt in `prompts`
+
+    Returns
+    -------
+    past_key_values : tuple[torch.Tensor, torch.Tensor]
+        for each attention block in `model`, the keys and values for each prompt in the
+        repeated prompts
+    encodings : BatchEncoding
+        the tokenizer output for the repeated prompts
+    offsets : torch.Tensor
+        the number of (non-pad) tokens in each of the repeated prompts
+    last_nonpad_token_logits : torch.Tensor
+        next-token logits for the last non-pad token for each of the repeated prompts
+
+    Raises
+    ------
+    ValueError
+        if the `tokenizer` is not using right-padding
+    TypeError
+        if `prompts` is not a `Sequence`
+    ValueError
+        if `num_repeats_per_prompt` is a `Sequence` whose length is not the same as the
+        length of `prompts`
+    """
+    if not tokenizer.padding_side == "right":
+        raise ValueError("Gotta use right padding to ensure position IDs are correct.")
+    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
+        raise TypeError("prompts must be a Sequence of strings.")
+    if isinstance(num_completions_per_prompt, Sequence):
+        if not len(prompts) == len(num_completions_per_prompt):
+            raise ValueError(
+                "If num_completions_per_prompt is a Sequence, then it must be the same "
+                f"length as prompts. Got lengths {len(num_completions_per_prompt)}, "
+                f"{len(prompts)}."
+            )
+    if isinstance(num_completions_per_prompt, int):
+        ## For code simplicity, just repeat it
+        num_completions_per_prompt = [num_completions_per_prompt] * len(prompts)
+    prompts_repeated = [
+        prompt
+        for prompt, num_repeats in zip(prompts, num_completions_per_prompt)
+        for _ in range(num_repeats)
+    ]
+    # fmt: off
+    encodings: BatchEncoding = (tokenizer(prompts_repeated, return_tensors="pt",
+                                          padding=True)
+                                .to(model.device))
+    # fmt: on
+    with torch.no_grad():
+        out = model(**encodings)
+
+    offsets: torch.Tensor = encodings.attention_mask.sum(dim=1)
+
+    ## Need (next-token) logits from prompts, i.e., last non-pad prompt token, since
+    ## that contains the first completion token's log-probability
+    _last_nonpad_token_idxs = (offsets - 1)[:, None, None]
+    last_nonpad_token_logits: torch.Tensor = out.logits.take_along_dim(
+        _last_nonpad_token_idxs, dim=1
+    )
+
+    return out.past_key_values, encodings, offsets, last_nonpad_token_logits
+
+
+def _logits_texts(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    texts: Sequence[str],
+) -> tuple[torch.Tensor, BatchEncoding]:
+    encodings = tokenizer(texts, return_tensors="pt", padding=True).to(model.device)
+    with torch.no_grad():
+        out = model(**encodings)
+    return out.logits, encodings
+
+
+def _prompts_offsets(
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    num_completions_per_prompt: Union[int, Sequence[int]],
+) -> torch.Tensor:
+    if not isinstance(num_completions_per_prompt, int) and not isinstance(
+        num_completions_per_prompt, torch.Tensor
+    ):
+        num_completions_per_prompt = torch.tensor(num_completions_per_prompt)
+    return (
+        tokenizer(prompts, return_tensors="pt", padding=True)
+        .attention_mask.repeat_interleave(num_completions_per_prompt, dim=0)
+        .sum(dim=1)
+    )
+
+
+def _logits_completions_given_prompts(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    end_of_prompt: str = " ",
+):
+    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
+        raise TypeError("prompts must be a Sequence of strings.")
+    if isinstance(completions, str) or not isinstance(completions, Sequence):
+        raise TypeError("completions must be a Sequence of strings.")
+    texts = [
+        prompt + end_of_prompt + completion
+        for prompt in prompts
+        for completion in completions
+    ]
+    logits, encodings = _logits_texts(model, tokenizer, texts)
+    ## Need these indices to slice completion tokens
+    encodings["offsets"] = _prompts_offsets(
+        tokenizer, prompts, num_completions_per_prompt=len(completions)
+    ).to(model.device)
+    return logits, encodings
+
+
+def _logits_completions_given_prompts_examples(
+    model: AutoModelForCausalLM,
+    tokenizer: PreTrainedTokenizer,
+    examples: Sequence[Example],
+):
+    texts = [
+        example.prompt + example.end_of_prompt + completion
+        for example in examples
+        for completion in example.completions
+    ]
+    logits, encodings = _logits_texts(model, tokenizer, texts)
+    ## Need these indices to slice completion tokens
+    prompts = [example.prompt for example in examples]
+    num_completions_per_prompt = [len(example.completions) for example in examples]
+    encodings["offsets"] = _prompts_offsets(
+        tokenizer, prompts, num_completions_per_prompt=num_completions_per_prompt
+    )
+    return logits, encodings
+
+
+def _logits_to_log_probs_completions(
+    logits: torch.Tensor, encodings: Mapping[str, torch.Tensor]
+) -> list[list[float]]:
+    log_probs = hf._utils.logits_to_log_probs(
+        logits, encodings["input_ids"], input_ids_start_idx=1, logits_end_idx=-1
+    )
+    last_idx_non_pad = encodings["attention_mask"].sum(dim=1)
+    ## i.e., # of tokens per text
+    return [
+        log_probs_prompt_completion[completion_start:completion_end].tolist()
+        for log_probs_prompt_completion, completion_start, completion_end in zip(
+            log_probs, encodings["offsets"] - 1, last_idx_non_pad - 1
+        )
+    ]
+
+
+def log_probs_conditional(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> list[list[list[float]]]:
+    """
+    Log-probabilities of each completion token conditional on each prompt and previous
+    completion tokens.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
+        log-probability of the completion token in `completions[completion_idx]`,
+        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
+        completion tokens.
+
+    Note
+    ----
+    To efficiently aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify_no_cache import log_probs_conditional
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        prompts = ['x y', 'a b c']
+        completions = ['z', 'd e']
+
+        # Compute
+        log_probs_completions = log_probs_conditional(
+                                    prompts,
+                                    completions,
+                                    model_and_tokenizer=(model, tokenizer)
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0]
+        # [[-4.5],        [[log Pr(z | x, y)],
+        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1]
+        # [[-9.7],        [[log Pr(z | a, b, c)],
+        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+    """
+    model, tokenizer = hf._utils.load_model_and_tokenizer(
+        model=model, model_and_tokenizer=model_and_tokenizer
+    )
+
+    @_batch.flatten
+    @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs (no cache)")
+    def log_probs_completions_batch(prompts, batch_size=batch_size):
+        logits, encodings = _logits_completions_given_prompts(
+            model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
+        )
+        return _logits_to_log_probs_completions(logits, encodings)
+
+    log_probs_completions = log_probs_completions_batch(prompts)
+    return list(_batch.constant(log_probs_completions, size=len(completions)))
+
+
+def log_probs_conditional_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> list[list[list[float]]]:
+    """
+    Log-probabilities of each completion token conditional on each prompt and previous
+    completion tokens.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
+        the log-probability of the completion token in
+        `examples[example_idx].completions[completion_idx]`, conditional on
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
+        previous completion tokens.
+
+    Note
+    ----
+    To aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Note
+    ----
+    The attribute :attr:`cappr.Example.prior` is unused.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify_no_cache import log_probs_conditional_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [Example(prompt='x y',   completions=('z', 'd e')),
+                    Example(prompt='a b c', completions=('1 2',))]
+
+        # Compute
+        log_probs_completions = log_probs_conditional_examples(
+                                    examples,
+                                    model_and_tokenizer=(model, tokenizer)
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0] # corresponds to examples[0]
+        # [[-4.5],        [[log Pr(z | x, y)],
+        #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1] # corresponds to examples[1]
+        # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
+    """
+    model, tokenizer = hf._utils.load_model_and_tokenizer(
+        model=model, model_and_tokenizer=model_and_tokenizer
+    )
+
+    @_batch.flatten
+    @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs (no cache)")
+    def log_probs_completions_batch(examples, batch_size=batch_size):
+        logits, encodings = _logits_completions_given_prompts_examples(
+            model, tokenizer, examples
+        )
+        return _logits_to_log_probs_completions(logits, encodings)
+
+    log_probs_completions = log_probs_completions_batch(examples)
+    num_completions_per_prompt = [len(example.completions) for example in examples]
+    return list(
+        _batch.variable(log_probs_completions, sizes=num_completions_per_prompt)
+    )
+
+
+@classify._predict_proba
+def predict_proba(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> npt.NDArray[np.floating]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    pred_probs : npt.NDArray[np.floating]
+        Array with shape `(len(prompts), len(completions))`.
+        `pred_probs[prompt_idx, completion_idx]` is the model's estimate of the
+        probability that `completions[completion_idx]` comes after
+        `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_proba_examples`.
+
+    Example
+    -------
+    Let's have GPT-2 (small) predict where stuff is in the kitchen. This example also
+    conveys that it's not the greatest model out there::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify_no_cache import predict_proba
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Define a classification task
+        prompts = ['The tacos are cooking',
+                   'Ice cream is']
+        class_names = ('on the stove', 'in the freezer', 'in the fridge')
+        prior       = (     1/5      ,       2/5       ,       2/5      )
+
+        pred_probs = predict_proba(prompts,
+                                   completions=class_names,
+                                   model_and_tokenizer=(model, tokenizer),
+                                   prior=prior)
+
+        pred_probs = pred_probs.round(1) # just for cleaner output
+
+        # predicted probability that tacos cook on the stove
+        pred_probs[0,0]
+        # 0.4
+
+        # predicted probability that ice cream is in the freezer
+        pred_probs[1,1]
+        # 0.5
+
+        # predicted probability that ice cream is in the fridge
+        pred_probs[1,2]
+        # 0.4
+    """
+    return log_probs_conditional(
+        prompts,
+        completions,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        end_of_prompt=end_of_prompt,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict_proba_examples
+def predict_proba_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
+        probability that `examples[example_idx].completions[completion_idx]` comes after
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+        If the number of completions per example is a constant `k`, then an array with
+        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+
+    Example
+    -------
+    GPT-2 (small) doing media trivia::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify_no_cache import predict_proba_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [
+            Example(prompt='Jodie Foster played',
+                    completions=('Clarice Starling', 'Trinity in The Matrix')),
+            Example(prompt='Batman, from Batman: The Animated Series, was played by',
+                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
+                    prior=      (     2/3      ,      1/3     ,      0      ))
+        ]
+
+        pred_probs = predict_proba_examples(examples,
+                                            model_and_tokenizer=(model, tokenizer))
+
+        # predicted probability that Jodie Foster played Clarice Starling, not Trinity
+        pred_probs[0][0]
+        # 0.7
+
+        # predicted probability that Batman was played by Kevin Conroy
+        pred_probs[0][1]
+        # 0.97
+    """
+    return log_probs_conditional_examples(
+        examples,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict
+def predict(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    prior: Optional[Sequence[float]] = None,
+    end_of_prompt: str = " ",
+    batch_size: int = 32,
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(prompts)`.
+        `preds[prompt_idx]` is the completion in `completions` which is predicted to
+        follow `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_examples`.
+
+    Example
+    -------
+    Let's have GPT-2 (small) predict where stuff is in the kitchen::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr.huggingface.classify_no_cache import predict
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Define a classification task
+        prompts = ['The tacos are cooking', 'Ice cream is']
+        class_names = ('on the stove', 'in the freezer', 'in the fridge')
+        prior       = (     1/5      ,       2/5       ,       2/5      )
+
+        preds = predict(prompts,
+                        completions=class_names,
+                        model_and_tokenizer=(model, tokenizer),
+                        prior=prior)
+        preds
+        # ['on the stove',
+        #  'in the freezer']
+    """
+    return predict_proba(
+        prompts,
+        completions,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        prior=prior,
+        end_of_prompt=end_of_prompt,
+        batch_size=batch_size,
+    )
+
+
+@classify._predict_examples
+def predict_examples(
+    examples: Sequence[Example],
+    model: str = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    batch_size: int = 32,
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Note
+    ----
+    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
+    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
+    See the Example.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : str, optional
+        the name of an `AutoModelForCausalLM`, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
+        an instantiated model and its corresponding tokenizer, by default None
+    batch_size : int, optional
+        the maximum number of inputs that the model will process in parallel, by default
+        32
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(examples)`.
+        `preds[example_idx]` is the completion in `examples[example_idx].completions`
+        which is predicted to follow
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+    Example
+    -------
+    GPT-2 (small) doing media trivia::
+
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from cappr import Example
+        from cappr.huggingface.classify_no_cache import predict_examples
+
+        # Load model and tokenizer
+        model = AutoModelForCausalLM.from_pretrained('gpt2')
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+        # Create data
+        examples = [
+            Example(prompt='Jodie Foster played',
+                    completions=('Clarice Starling', 'Trinity in The Matrix')),
+            Example(prompt='Batman, from Batman: The Animated Series, was played by',
+                    completions=('Kevin Conroy', 'Pete Holmes', 'Spongebob!'),
+                    prior=      (     2/3      ,      1/3     ,      0      ))
+        ]
+
+        preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
+        preds
+        # ['Clarice Starling',
+        #  'Kevin Conroy']
+    """
+    return predict_proba_examples(
+        examples,
+        model=model,
+        model_and_tokenizer=model_and_tokenizer,
+        batch_size=batch_size,
+    )
```

### Comparing `cappr-0.2.1/src/cappr/openai/api.py` & `cappr-0.2.2/src/cappr/openai/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,286 +1,289 @@
-"""
-Helpers for interacting with the OpenAI API.
-"""
-from __future__ import annotations
-import logging
-import os
-import time
-from typing import Any, Callable, Literal, Mapping, Optional, Sequence, get_args
-
-import openai
-import tiktoken
-from tqdm.auto import tqdm
-
-from cappr.utils import _batch
-
-
-logger = logging.getLogger(__name__)
-
-
-openai.api_key = os.getenv("OPENAI_API_KEY")
-
-
-end_of_prompt = "\n\n###\n\n"
-## https://platform.openai.com/docs/guides/fine-tuning/data-formatting
-
-
-Model = Literal[
-    "text-ada-001",
-    "ada",
-    "text-babbage-001",
-    "babbage",
-    "text-curie-001",
-    "curie",
-    "text-davinci-003",
-    "text-davinci-002",
-    "davinci",
-]
-## https://platform.openai.com/docs/models/model-endpoint-compatibility
-_costs = [0.0004, 0.0004, 0.0005, 0.0005, 0.002, 0.002, 0.02, 0.02, 0.02]
-## https://openai.com/api/pricing/
-## TODO: figure out how to get this automatically from openai, if possible
-model_to_cost_per_1k: dict[Model, float] = dict(zip(get_args(Model), _costs))
-
-
-def openai_method_retry(
-    openai_method: Callable,
-    max_num_tries: int = 5,
-    sleep_sec: float = 10,
-    retry_errors: tuple = (
-        openai.error.ServiceUnavailableError,
-        openai.error.RateLimitError,
-    ),
-    **openai_method_kwargs,
-) -> Any:
-    """
-    Wrapper around OpenAI API calls which automatically retries and sleeps if requests
-    fail. Logs at level INFO when requests fail, and level ERROR if an exception is
-    raised.
-
-    Parameters
-    ----------
-    openai_method : Callable
-        a function or method whose inputs are `openai_method_kwargs`
-    max_num_tries : int, optional
-        maximum number of times to retry the request before raising the exception, by
-        default 5
-    sleep_sec : float, optional
-        number of seconds to sleep before re-submitting the request, by default 10
-    retry_errors : tuple[Exception], optional
-        if one of these exceptions is raised by the request, then retry, else the
-        exception is immediately raised.
-        By default
-        ``(openai.error.ServiceUnavailableError, openai.error.RateLimitError)``
-
-    Returns
-    -------
-    Any
-        `openai_method(**openai_method_kwargs)`
-
-    Raises
-    ------
-    Exception
-        if `max_num_tries` is exceeded or an exception not in `retry_errors` is raised
-    """
-    num_tries = 0
-    while num_tries < max_num_tries:
-        try:
-            return openai_method(**openai_method_kwargs)
-        except retry_errors as e:
-            num_tries += 1
-            logger.info(f"openai error: {e}")
-            logger.info(f"Try {num_tries}. Sleeping for {sleep_sec} sec.")
-            time.sleep(sleep_sec)
-            exception = e  ## allow it to be referenced later
-    logger.error(f"Max retries exceeded. openai error: {exception}")
-    raise exception
-
-
-class _UserCanceled(Exception):
-    pass
-
-
-def _openai_api_call_is_ok(
-    model: Model,
-    texts: list[str],
-    max_tokens: int = 0,
-    cost_per_1k_tokens: Optional[float] = None,
-):
-    """
-    After displaying the cost (usually an upper bound) of hitting the OpenAI API
-    text completion endpoint, prompt the user to manually input ``y`` or ``n`` to
-    indicate whether the program can proceed.
-
-    Parameters
-    ----------
-    model : Model
-        name of the OpenAI API text completion model
-    texts : list[str]
-        texts or prompts inputted to the `model` OpenAI API call
-    max_tokens : int, optional
-        maximum number of tokens to generate, by default 0
-    cost_per_1k_tokens : Optional[float], optional
-        OpenAI API dollar cost for processing 1k tokens. If unset,
-        `cappr.openai.api.model_to_cost_per_1k[model]` is used. If it's still unknown,
-        the cost will be displayed as `unknown`. By default None
-
-    Raises
-    ------
-    _UserCanceled
-        if the user inputs ``n`` when prompted to give the go-ahead
-    """
-    texts = list(texts)
-    try:
-        tokenizer = tiktoken.encoding_for_model(model)
-    except KeyError:  ## that's fine, we just need an approximation
-        tokenizer = tiktoken.get_encoding("gpt2")
-    _num_tokens_prompts = sum(len(tokens) for tokens in tokenizer.encode_batch(texts))
-    _num_tokens_completions = len(texts) * max_tokens  ## upper bound ofc
-    num_tokens = _num_tokens_prompts + _num_tokens_completions
-    cost_per_1k_tokens = cost_per_1k_tokens or model_to_cost_per_1k.get(model)
-    if cost_per_1k_tokens is None:
-        cost = "unknown (see https://openai.com/api/pricing/)"
-    else:
-        cost = round(num_tokens * cost_per_1k_tokens / 1_000, 2)
-    output = None
-    while output not in {"y", "n"}:
-        output = input(
-            f"This API call will cost you about ${cost} "
-            f"({num_tokens:_} tokens). Proceed? (y/n): "
-        )
-    if output == "n":
-        raise _UserCanceled("No API requests will be submitted.")
-
-
-def gpt_complete(
-    texts: Sequence[str],
-    model: Model,
-    ask_if_ok: bool = False,
-    progress_bar_desc: str = "log-probs",
-    max_tokens: int = 0,
-    **openai_completion_kwargs,
-) -> list[Mapping[str, Any]]:
-    """
-    Wrapper around the OpenAI text completion endpoint which automatically batches
-    texts for greater efficiency, retries requests that fail, and displays a progress
-    bar.
-
-    OpenAI API text completion reference:
-    https://platform.openai.com/docs/api-reference/completions
-
-    Warning
-    -------
-    By default, no tokens will be generated/sampled.
-
-    Parameters
-    ----------
-    texts : Sequence[str]
-        these are passed as the `prompt` argument in a text completion request
-    model : Model
-        which text completion model to use
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-    progress_bar_desc: str, optional
-        description of the progress bar that's displayed, by default ``'log-probs'``
-    max_tokens : int, optional
-        maximum number of tokens to generate, by default 0
-    **openai_completion_kwargs
-        other arguments passed to the text completion endpoint, e.g., `logprobs=1`
-
-    Returns
-    -------
-    list[Mapping[str, Any]]
-        (flat) list of the `choices` mappings which the text completion endpoint
-        returns. More specifically, it's a list of
-        ``openai.openai_object.OpenAIObject``
-    """
-    _batch_size = 20  ## max that the API can currently handle
-    if isinstance(texts, str):
-        ## Passing in a string will silently but majorly fail. Handle it
-        texts = [texts]
-    if ask_if_ok:
-        _openai_api_call_is_ok(model, texts, max_tokens=max_tokens)
-    choices = []
-    with tqdm(total=len(texts), desc=progress_bar_desc) as progress_bar:
-        for texts_batch in _batch.constant(texts, _batch_size):
-            response = openai_method_retry(
-                openai.Completion.create,
-                prompt=texts_batch,
-                model=model,
-                max_tokens=max_tokens,
-                **openai_completion_kwargs,
-            )
-            choices.extend(response["choices"])
-            progress_bar.update(len(texts_batch))
-    return choices
-
-
-def gpt_chat_complete(
-    texts: Sequence[str],
-    model: str = "gpt-3.5-turbo",
-    ask_if_ok: bool = False,
-    max_tokens: int = 5,
-    system_msg: str = ("You are an assistant which classifies text."),
-    **openai_chat_kwargs,
-) -> list[Mapping[str, Any]]:
-    """
-    Wrapper around the OpenAI chat completion endpoint which retries requests that fail
-    and displays a progress bar. It does not batch inputs, so this may take a while.
-
-    OpenAI API chat completion reference:
-    https://platform.openai.com/docs/api-reference/chat
-
-    Warning
-    -------
-    By default, the `system_msg` asks ChatGPT to perform text classification.
-
-    Parameters
-    ----------
-    texts : Sequence[str]
-        texts which are passed in one by one immediately after the system content as
-        ``{"role": "user", "content": text}``
-    model : str, optional
-        one of the chat model names, by default "gpt-3.5-turbo"
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-    max_tokens : int, optional
-        maximum number of tokens to generate, by default 5
-    system_msg : str, optional
-        text which is passed in 1-by-1 immediately before every piece of
-        user content in `texts` as ``{"role": "system", "content": system_msg}``. By
-        default ``"You are an assistant which classifies text."``
-    **openai_chat_kwargs
-        other arguments passed to the chat completion endpoint, e.g., `temperature=0.8`
-
-    Returns
-    -------
-    list[Mapping[str, Any]]
-        (flat) list of the `choices` mappings which the chat completion endpoint
-        returns. More specifically, it's a list of
-        ``openai.openai_object.OpenAIObject``
-    """
-    ## TODO: batch, if possible
-    if isinstance(texts, str):
-        texts = [texts]
-    if ask_if_ok:
-        _openai_api_call_is_ok(model=model, texts=texts, max_tokens=max_tokens)
-    choices = []
-    for text in tqdm(texts, total=len(texts), desc="Completing chats"):
-        messages = [
-            {"role": "system", "content": system_msg},
-            {"role": "user", "content": text},
-        ]
-        response = openai_method_retry(
-            openai.ChatCompletion.create,
-            model=model,
-            messages=messages,
-            max_tokens=max_tokens,
-            temperature=0,
-            **openai_chat_kwargs,
-        )
-        choices.extend(response["choices"])
-    return choices
+"""
+Helpers for interacting with the OpenAI API.
+"""
+from __future__ import annotations
+import logging
+import os
+import time
+from typing import Any, Callable, Literal, Mapping, Optional, Sequence, get_args
+
+import openai
+import tiktoken
+from tqdm.auto import tqdm
+
+from cappr.utils import _batch
+
+
+logger = logging.getLogger(__name__)
+
+
+openai.api_key = os.getenv("OPENAI_API_KEY")
+
+
+end_of_prompt = "\n\n###\n\n"
+## https://platform.openai.com/docs/guides/fine-tuning/data-formatting
+
+
+Model = Literal[
+    "text-ada-001",
+    "ada",
+    "text-babbage-001",
+    "babbage",
+    "text-curie-001",
+    "curie",
+    "text-davinci-003",
+    "text-davinci-002",
+    "davinci",
+]
+## https://platform.openai.com/docs/models/model-endpoint-compatibility
+_costs = [0.0004, 0.0004, 0.0005, 0.0005, 0.002, 0.002, 0.02, 0.02, 0.02]
+## https://openai.com/api/pricing/
+## TODO: figure out how to get this automatically from openai, if possible
+model_to_cost_per_1k: dict[Model, float] = dict(zip(get_args(Model), _costs))
+
+
+def openai_method_retry(
+    openai_method: Callable,
+    max_num_tries: int = 5,
+    sleep_sec: float = 10,
+    retry_errors: tuple = (
+        openai.error.ServiceUnavailableError,
+        openai.error.RateLimitError,
+    ),
+    **openai_method_kwargs,
+) -> Any:
+    """
+    Wrapper around OpenAI API calls which automatically retries and sleeps if requests
+    fail. Logs at level INFO when requests fail, and level ERROR if an exception is
+    raised.
+
+    Parameters
+    ----------
+    openai_method : Callable
+        a function or method whose inputs are `openai_method_kwargs`
+    max_num_tries : int, optional
+        maximum number of times to retry the request before raising the exception, by
+        default 5
+    sleep_sec : float, optional
+        number of seconds to sleep before re-submitting the request, by default 10
+    retry_errors : tuple[Exception], optional
+        if one of these exceptions is raised by the request, then retry, else the
+        exception is immediately raised.
+        By default
+        ``(openai.error.ServiceUnavailableError, openai.error.RateLimitError)``
+
+    Returns
+    -------
+    Any
+        `openai_method(**openai_method_kwargs)`
+
+    Raises
+    ------
+    Exception
+        if `max_num_tries` is exceeded or an exception not in `retry_errors` is raised
+    """
+    num_tries = 0
+    while num_tries < max_num_tries:
+        try:
+            return openai_method(**openai_method_kwargs)
+        except retry_errors as e:
+            num_tries += 1
+            logger.info(f"openai error: {e}")
+            logger.info(f"Try {num_tries}. Sleeping for {sleep_sec} sec.")
+            time.sleep(sleep_sec)
+            exception = e  ## allow it to be referenced later
+    logger.error(f"Max retries exceeded. openai error: {exception}")
+    raise exception
+
+
+class _UserCanceled(Exception):
+    pass
+
+
+def _openai_api_call_is_ok(
+    model: Model,
+    texts: list[str],
+    max_tokens: int = 0,
+    cost_per_1k_tokens: Optional[float] = None,
+):
+    """
+    After displaying the cost (usually an upper bound) of hitting the OpenAI API
+    text completion endpoint, prompt the user to manually input ``y`` or ``n`` to
+    indicate whether the program can proceed.
+
+    Parameters
+    ----------
+    model : Model
+        name of the OpenAI API text completion model
+    texts : list[str]
+        texts or prompts inputted to the `model` OpenAI API call
+    max_tokens : int, optional
+        maximum number of tokens to generate, by default 0
+    cost_per_1k_tokens : Optional[float], optional
+        OpenAI API dollar cost for processing 1k tokens. If unset,
+        `cappr.openai.api.model_to_cost_per_1k[model]` is used. If it's still unknown,
+        the cost will be displayed as `unknown`. By default None
+
+    Raises
+    ------
+    _UserCanceled
+        if the user inputs ``n`` when prompted to give the go-ahead
+    """
+    texts = list(texts)
+    try:
+        tokenizer = tiktoken.encoding_for_model(model)
+    except KeyError:  ## that's fine, we just need an approximation
+        tokenizer = tiktoken.get_encoding("gpt2")
+    _num_tokens_prompts = sum(len(tokens) for tokens in tokenizer.encode_batch(texts))
+    _num_tokens_completions = len(texts) * max_tokens  ## upper bound ofc
+    num_tokens = _num_tokens_prompts + _num_tokens_completions
+    cost_per_1k_tokens = cost_per_1k_tokens or model_to_cost_per_1k.get(model)
+    if cost_per_1k_tokens is None:
+        cost = "unknown (see https://openai.com/api/pricing/)"
+    else:
+        cost = round(num_tokens * cost_per_1k_tokens / 1_000, 2)
+    output = None
+    while output not in {"y", "n"}:
+        output = input(
+            f"This API call will cost you about ${cost} "
+            f"({num_tokens:_} tokens). Proceed? (y/n): "
+        )
+    if output == "n":
+        raise _UserCanceled("No API requests will be submitted.")
+
+
+def gpt_complete(
+    texts: Sequence[str],
+    model: Model,
+    ask_if_ok: bool = False,
+    progress_bar_desc: str = "log-probs",
+    max_tokens: int = 0,
+    **openai_completion_kwargs,
+) -> list[Mapping[str, Any]]:
+    """
+    Wrapper around the OpenAI text completion endpoint which automatically batches
+    texts for greater efficiency, retries requests that fail, and displays a progress
+    bar.
+
+    OpenAI API text completion reference:
+    https://platform.openai.com/docs/api-reference/completions
+
+    Warning
+    -------
+    By default, no tokens will be generated/sampled.
+
+    Parameters
+    ----------
+    texts : Sequence[str]
+        these are passed as the `prompt` argument in a text completion request
+    model : Model
+        which text completion model to use
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+    progress_bar_desc: str, optional
+        description of the progress bar that's displayed, by default ``'log-probs'``
+    max_tokens : int, optional
+        maximum number of tokens to generate, by default 0
+    **openai_completion_kwargs
+        other arguments passed to the text completion endpoint, e.g., `logprobs=1`
+
+    Returns
+    -------
+    list[Mapping[str, Any]]
+        list with the same length as `texts`. Each element is the ``choices`` mapping
+        which the OpenAI text completion endpoint returns.
+    """
+    _batch_size = 20  ## max that the API can currently handle
+    if isinstance(texts, str):
+        ## Passing in a string will silently but majorly fail. Handle it
+        texts = [texts]
+    if ask_if_ok:
+        _openai_api_call_is_ok(model, texts, max_tokens=max_tokens)
+    choices = []
+    with tqdm(total=len(texts), desc=progress_bar_desc) as progress_bar:
+        for texts_batch in _batch.constant(texts, _batch_size):
+            response = openai_method_retry(
+                openai.Completion.create,
+                prompt=texts_batch,
+                model=model,
+                max_tokens=max_tokens,
+                **openai_completion_kwargs,
+            )
+            choices.extend(response["choices"])
+            progress_bar.update(len(texts_batch))
+    return choices
+
+
+def gpt_chat_complete(
+    texts: Sequence[str],
+    model: str = "gpt-3.5-turbo",
+    ask_if_ok: bool = False,
+    system_msg: str = ("You are an assistant which classifies text."),
+    max_tokens: int = 5,
+    temperature: float = 0,
+    **openai_chat_kwargs,
+) -> list[Mapping[str, Any]]:
+    """
+    Wrapper around the OpenAI chat completion endpoint which performs text
+    classification 1-by-1. It retries requests that fail and displays a progress bar.
+
+    OpenAI API chat completion reference:
+    https://platform.openai.com/docs/api-reference/chat
+
+    Warning
+    -------
+    By default, the `system_msg` asks ChatGPT to perform text classification. And the
+    `temperature` is set to 0.
+
+    Parameters
+    ----------
+    texts : Sequence[str]
+        texts which are passed in one by one immediately after the system content as
+        ``{"role": "user", "content": text}``
+    model : str, optional
+        one of the chat model names, by default "gpt-3.5-turbo"
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+    system_msg : str, optional
+        text which is passed in 1-by-1 immediately before every piece of
+        user content in `texts` as ``{"role": "system", "content": system_msg}``. By
+        default ``"You are an assistant which classifies text."``
+    max_tokens : int, optional
+        maximum number of tokens to generate, by default 5
+    temperature : float, optional
+        probability re-scaler to apply before sampling, by default 0
+    **openai_chat_kwargs
+        other arguments passed to the chat completion endpoint
+
+    Returns
+    -------
+    list[Mapping[str, Any]]
+        (flat) list of the `choices` mappings which the chat completion endpoint
+        returns. More specifically, it's a list of
+        ``openai.openai_object.OpenAIObject``
+    """
+    ## TODO: batch, if possible
+    if isinstance(texts, str):
+        texts = [texts]
+    if ask_if_ok:
+        _openai_api_call_is_ok(model=model, texts=texts, max_tokens=max_tokens)
+    choices = []
+    for text in tqdm(texts, total=len(texts), desc="Completing chats"):
+        messages = [
+            {"role": "system", "content": system_msg},
+            {"role": "user", "content": text},
+        ]
+        response = openai_method_retry(
+            openai.ChatCompletion.create,
+            model=model,
+            messages=messages,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            **openai_chat_kwargs,
+        )
+        choices.extend(response["choices"])
+    return choices
```

### Comparing `cappr-0.2.1/src/cappr/openai/classify.py` & `cappr-0.2.2/src/cappr/openai/classify.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,555 +1,597 @@
-"""
-Perform prompt-completion classification using models from OpenAI's text
-completion API.
-
-You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
-"""
-from __future__ import annotations
-from typing import Optional, Sequence, Union
-
-import numpy as np
-import numpy.typing as npt
-import tiktoken
-
-from cappr.utils import _batch, classify
-from cappr import Example
-from cappr import openai
-
-
-def _token_logprobs(
-    texts: Sequence[str], model: openai.api.Model, ask_if_ok: bool = False
-) -> list[list[float]]:
-    """
-    TODO: convert docstring to numpy style
-
-    Returns a list `log_probs` where `log_probs[i]` is the value of
-    `'log_probs' -> 'token_logprobs'` (from the OpenAI Completion endpoint) for
-    `texts[i]` using `model`.
-    """
-    choices = openai.api.gpt_complete(
-        texts,
-        ask_if_ok=ask_if_ok,
-        model=model,
-        ## rest must be hard-coded
-        max_tokens=0,
-        logprobs=1,
-        echo=True,
-    )
-    return [choice["logprobs"]["token_logprobs"] for choice in choices]
-
-
-def _slice_completions(
-    completions: Sequence[str],
-    log_probs: Sequence[Sequence[float]],
-    model: openai.api.Model,
-) -> list[list[float]]:
-    """
-    TODO: convert docstring to numpy style
-
-    Returns a list `log_probs_completions` where `log_probs_completions[i]` is a list of
-    conditional log-probablities for each token in `completions[i]`, extracted by
-    slicing `log_probs[i]`.
-    """
-    if len(completions) != len(log_probs):
-        raise ValueError(
-            "Different number of completions and log_probs: "
-            f"{len(completions)}, {len(log_probs)}."
-        )
-    tokenizer = tiktoken.encoding_for_model(model)
-    completion_lengths = [len(tokens) for tokens in tokenizer.encode_batch(completions)]
-    return [
-        log_probs_text[-num_completion_tokens:]
-        for num_completion_tokens, log_probs_text in zip(completion_lengths, log_probs)
-    ]
-
-
-def log_probs_conditional(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: openai.api.Model,
-    end_of_prompt: str = " ",
-    ask_if_ok: bool = False,
-):
-    """
-    Log-probabilities of each completion token conditional on each prompt and previous
-    completion tokens.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
-        log-probability of the completion token in `completions[completion_idx]`,
-        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
-        completion tokens.
-
-    Note
-    ----
-    To efficiently aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs_from_constant_completions`.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from cappr.openai.classify import log_probs_conditional
-
-        # Create data
-        prompts = ['x y', 'a b c']
-        completions = ['z', 'd e']
-
-        # Compute
-        log_probs_completions = log_probs_conditional(
-                                    prompts,
-                                    completions,
-                                    model='text-ada-001'
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0]
-        # [[-5.5],        [[log Pr(z | x, y)],
-        #  [-8.2, -2.1]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1]
-        # [[-11.6],       [[log Pr(z | a, b, c)],
-        #  [-0.3, -1.2]]   [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
-    """
-    ## str / non-Sequence[str] inputs silently, wastefully, and irreparably fail
-    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
-        raise TypeError("prompts must be a Sequence of strings.")
-    if isinstance(completions, str) or not isinstance(completions, Sequence):
-        raise TypeError("completions must be a Sequence of strings.")
-    ## Flat list of prompts and their completions. Will post-process
-    texts = [
-        prompt + end_of_prompt + completion
-        for prompt in prompts
-        for completion in completions
-    ]
-    log_probs = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
-    ## Since log_probs is a flat list, we'll need to batch them by the size and order of
-    ## completions to fulfill the spec.
-    return [
-        _slice_completions(completions, log_probs_batch, model)
-        for log_probs_batch in _batch.constant(log_probs, size=len(completions))
-    ]
-
-
-def log_probs_conditional_examples(
-    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
-) -> list[list[list[float]]]:
-    """
-    Log-probabilities of each completion token conditional on each prompt.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    log_probs_completions : list[list[list[float]]]
-        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
-        the log-probability of the completion token in
-        `examples[example_idx].completions[completion_idx]`, conditional on
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
-        previous completion tokens.
-
-    Note
-    ----
-    To aggregate `log_probs_completions`, use
-    :func:`cappr.utils.classify.agg_log_probs`.
-
-    Note
-    ----
-    The attribute :attr:`cappr.Example.prior` is unused.
-
-    Example
-    -------
-    Here we'll use single characters (which are of course single tokens) to more clearly
-    demonstrate what this function does::
-
-        from cappr import Example
-        from cappr.openai.classify import log_probs_conditional_examples
-
-        # Create data
-        examples = [Example(prompt='x y',   completions=('z', 'd e')),
-                    Example(prompt='a b c', completions=('1 2',))]
-
-        # Compute
-        log_probs_completions = log_probs_conditional_examples(
-                                    examples,
-                                    model='text-ada-001'
-                                )
-
-        # Outputs (rounded) next to their symbolic representation
-
-        log_probs_completions[0] # corresponds to examples[0]
-        # [[-5.5],        [[log Pr(z | x, y)],
-        #  [-8.2, -2.1]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
-
-        log_probs_completions[1] # corresponds to examples[1]
-        # [[-11.2, -4.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
-    """
-    ## Flat list of prompts and their completions. Will post-process
-    texts = [
-        example.prompt + example.end_of_prompt + completion
-        for example in examples
-        for completion in example.completions
-    ]
-    log_probs_all = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
-    ## Flatten completions in same order as examples were flattened
-    completions_all = [
-        completion for example in examples for completion in example.completions
-    ]
-    log_probs_completions_all = _slice_completions(
-        completions_all, log_probs_all, model
-    )
-    ## Batch by completions to fulfill the spec
-    num_completions_per_prompt = [len(example.completions) for example in examples]
-    return list(
-        _batch.variable(log_probs_completions_all, sizes=num_completions_per_prompt)
-    )
-
-
-@classify._predict_proba
-def predict_proba(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: openai.api.Model,
-    prior: Optional[Sequence[float]] = None,
-    end_of_prompt: str = " ",
-    ask_if_ok: bool = False,
-) -> npt.NDArray[np.floating]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    pred_probs : npt.NDArray[np.floating]
-        Array with shape `(len(prompts), len(completions))`.
-        `pred_probs[prompt_idx, completion_idx]` is the `model`'s estimate of the
-        probability that `completions[completion_idx]` comes after
-        `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_proba_examples`.
-
-    Example
-    -------
-    A more complicated business-y example—classify product reviews::
-
-        from cappr.openai.classify import predict_proba
-
-
-        # Define a classification task
-        feedback_types = ('the product is too expensive',
-                          'the product uses low quality materials',
-                          'the product is difficult to use',
-                          'the product is great')
-        prior = (2/5, 1/5, 1/5, 1/5) # I already expect customers to say it's expensive
-
-
-        # Write a prompt
-        def prompt_func(product_review: str) -> str:
-            return f'''
-        This product review: {product_review}\n
-        is best summarized as:'''
-
-
-        # Supply the texts you wanna classify
-        product_reviews = ["I can't figure out how to integrate it into my setup.",
-                           "Yeah it's pricey, but it's definitely worth it."]
-        prompts = [prompt_func(product_review) for product_review in product_reviews]
-
-
-        pred_probs = predict_proba(prompts,
-                                   completions=feedback_types,
-                                   model='text-curie-001',
-                                   prior=prior)
-
-        pred_probs = pred_probs.round(1) # just for cleaner output
-
-        # predicted probability that 1st product review says it's difficult to use
-        pred_probs[0,2]
-        # 0.9
-
-        # predicted probability that 2nd product review says it's great
-        pred_probs[1,3]
-        # 0.7
-
-        # predicted probability that 2nd product review says it's too expensive
-        pred_probs[1,0]
-        # 0.1
-    """
-    return log_probs_conditional(
-        prompts,
-        completions,
-        model,
-        end_of_prompt=end_of_prompt,
-        ask_if_ok=ask_if_ok,
-    )
-
-
-@classify._predict_proba_examples
-def predict_proba_examples(
-    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
-    """
-    Predict probabilities of each completion coming after each prompt.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
-        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
-        probability that `examples[example_idx].completions[completion_idx]` comes after
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-        If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
-
-    Example
-    -------
-    Let's demo COPA https://people.ict.usc.edu/~gordon/copa.html::
-
-        from cappr import Example
-        from cappr.openai.classify import predict_proba_examples
-
-
-        # Create data from the premises and alternatives
-        examples = [Example(prompt='The man broke his toe because',
-                            completions=('he got a hole in his sock.',
-                                         'he dropped a hammer on his foot.')),
-                    Example(prompt='I tipped the bottle, so',
-                            completions=('the liquid in the bottle froze.',
-                                         'the liquid in the bottle poured out.'))]
-
-
-        pred_probs = predict_proba_examples(examples, model='text-curie-001')
-
-        pred_probs = pred_probs.round(2) # just for cleaner output
-
-        # predicted probability that 'he dropped a hammer on his foot' is the
-        # alternative implied by the 1st premise: 'The man broke his toe'
-        pred_probs[0,1]
-        # 0.53
-
-        # predicted probability that 'the liquid in the bottle poured out' is the
-        # alternative implied by the 2nd premise: 'I tipped the bottle'
-        pred_probs[1,1]
-        # 0.66
-    """
-    return log_probs_conditional_examples(examples, model, ask_if_ok=ask_if_ok)
-
-
-@classify._predict
-def predict(
-    prompts: Sequence[str],
-    completions: Sequence[str],
-    model: openai.api.Model,
-    prior: Optional[Sequence[float]] = None,
-    end_of_prompt: str = " ",
-    ask_if_ok: bool = False,
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Parameters
-    ----------
-    prompts : Sequence[str]
-        strings, where, e.g., each contains the text you want to classify
-    completions : Sequence[str]
-        strings, where, e.g., each one is the name of a class which could come after a
-        prompt
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    prior : Sequence[float], optional
-        a probability distribution over `completions`, representing a belief about their
-        likelihoods regardless of the prompt. By default, each completion in
-        `completions` is assumed to be equally likely
-    end_of_prompt : str, optional
-        the string to tack on at the end of every prompt, by default " "
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(prompts)`.
-        `preds[prompt_idx]` is the completion in `completions` which is predicted to
-        follow `prompts[prompt_idx] + end_of_prompt`.
-
-    Note
-    ----
-    In this function, the set of possible completions which could follow each prompt is
-    the same for every prompt. If instead, each prompt could be followed by a
-    *different* set of completions, then construct a sequence of :class:`cappr.Example`
-    objects and pass them to :func:`predict_examples`.
-
-    Example
-    -------
-    A more complicated business-y example—classify product reviews::
-
-        from cappr.openai.classify import predict
-
-
-        # Define a classification task
-        feedback_types = ('the product is too expensive',
-                          'the product uses low quality materials',
-                          'the product is difficult to use',
-                          'the product is great')
-        prior = (2/5, 1/5, 1/5, 1/5) # I already expect customers to say it's expensive
-
-
-        # Write a prompt
-        def prompt_func(product_review: str) -> str:
-            return f'''
-        This product review: {product_review}\n
-        is best summarized as:'''
-
-
-        # Supply the texts you wanna classify
-        product_reviews = ["I can't figure out how to integrate it into my setup.",
-                           "Yeah it's pricey, but it's definitely worth it."]
-        prompts = [prompt_func(product_review) for product_review in product_reviews]
-
-
-        preds = predict(prompts,
-                        completions=feedback_types,
-                        model='text-curie-001',
-                        prior=prior)
-        preds
-        # ['the product is difficult to use',
-        #  'the product is great']
-    """
-    return predict_proba(
-        prompts,
-        completions,
-        model,
-        prior=prior,
-        end_of_prompt=end_of_prompt,
-        ask_if_ok=ask_if_ok,
-    )
-
-
-@classify._predict_examples
-def predict_examples(
-    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
-) -> list[str]:
-    """
-    Predict which completion is most likely to follow each prompt.
-
-    Parameters
-    ----------
-    examples : Sequence[Example]
-        `Example` objects, where each contains a prompt and its set of possible
-        completions
-    model : cappr.openai.api.Model
-        string for the name of an OpenAI text-completion model, specifically one from
-        the ``/v1/completions`` endpoint:
-        https://platform.openai.com/docs/models/model-endpoint-compatibility
-    ask_if_ok : bool, optional
-        whether or not to prompt you to manually give the go-ahead to run this function,
-        after notifying you of the approximate cost of the OpenAI API calls. By default
-        False
-
-    Returns
-    -------
-    preds : list[str]
-        List with length `len(examples)`.
-        `preds[example_idx]` is the completion in `examples[example_idx].completions`
-        which is predicted to follow
-        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
-
-    Example
-    -------
-    Let's demo COPA https://people.ict.usc.edu/~gordon/copa.html::
-
-        from cappr import Example
-        from cappr.openai.classify import predict_examples
-
-        # Create data from the premises and alternatives
-        examples = [Example(prompt='The man broke his toe because',
-                            completions=('he got a hole in his sock.',
-                                         'he dropped a hammer on his foot.')),
-                    Example(prompt='I tipped the bottle, so',
-                            completions=('the liquid in the bottle froze.',
-                                         'the liquid in the bottle poured out.'))]
-
-        preds = predict_examples(examples, model='text-curie-001')
-        preds
-        # ['he dropped a hammer on his foot',
-        #  'the liquid in the bottle poured out']
-    """
-    return predict_proba_examples(examples, model, ask_if_ok=ask_if_ok)
+"""
+Perform prompt-completion classification using models from OpenAI's text
+completion API.
+
+You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
+"""
+from __future__ import annotations
+from typing import Optional, Sequence, Union
+
+import numpy as np
+import numpy.typing as npt
+import tiktoken
+
+from cappr.utils import _batch, classify
+from cappr import Example
+from cappr import openai
+
+
+def _token_logprobs(
+    texts: Sequence[str], model: openai.api.Model, ask_if_ok: bool = False
+) -> list[list[float]]:
+    """
+    Returns a list `log_probs` where `log_probs[i]` is the value of `'logprobs' ->
+    'token_logprobs'` (from the OpenAI Completion endpoint) for `texts[i]` using
+    `model`. If `texts[i]` is a single token, then `log_probs[i]` is `[None]` (because
+    there's nothing to condition on).
+    """
+    ## Need to handle texts which are single tokens. Set their logprobs to [None]
+    tokenizer = tiktoken.encoding_for_model(model)
+    text_lengths = [len(tokens) for tokens in tokenizer.encode_batch(texts)]
+    idxs_multiple_tokens = [i for i, length in enumerate(text_lengths) if length > 1]
+    choices = openai.api.gpt_complete(
+        texts=[texts[i] for i in idxs_multiple_tokens],
+        ask_if_ok=ask_if_ok,
+        model=model,
+        ## rest must be hard-coded
+        max_tokens=0,
+        logprobs=1,
+        echo=True,
+    )
+    ## Interleave
+    log_probs_texts = [choice["logprobs"]["token_logprobs"] for choice in choices]
+    log_probs = [[None]] * len(texts)
+    for i, log_probs_text in zip(idxs_multiple_tokens, log_probs_texts):
+        log_probs[i] = log_probs_text
+    return log_probs
+
+
+def _slice_completions(
+    completions: Sequence[str],
+    log_probs: Sequence[Sequence[float]],
+    model: openai.api.Model,
+) -> list[list[float]]:
+    """
+    TODO: convert docstring to numpy style
+
+    Returns a list `log_probs_completions` where `log_probs_completions[i]` is a list of
+    conditional log-probablities for each token in `completions[i]`, extracted by
+    slicing `log_probs[i]`.
+    """
+    if len(completions) != len(log_probs):
+        raise ValueError(
+            "Different number of completions and log_probs: "
+            f"{len(completions)}, {len(log_probs)}."
+        )
+    tokenizer = tiktoken.encoding_for_model(model)
+    completion_lengths = [len(tokens) for tokens in tokenizer.encode_batch(completions)]
+    return [
+        log_probs_text[-num_completion_tokens:]
+        for num_completion_tokens, log_probs_text in zip(completion_lengths, log_probs)
+    ]
+
+
+def log_probs_conditional(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: openai.api.Model,
+    end_of_prompt: str = " ",
+    ask_if_ok: bool = False,
+):
+    """
+    Log-probabilities of each completion token conditional on each prompt and previous
+    completion tokens.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[prompt_idx][completion_idx][completion_token_idx]` is the
+        log-probability of the completion token in `completions[completion_idx]`,
+        conditional on `prompts[prompt_idx] + end_of_prompt` and previous
+        completion tokens.
+
+    Note
+    ----
+    To efficiently aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from cappr.openai.classify import log_probs_conditional
+
+        # Create data
+        prompts = ['x y', 'a b c']
+        completions = ['z', 'd e']
+
+        # Compute
+        log_probs_completions = log_probs_conditional(
+                                    prompts,
+                                    completions,
+                                    model='text-ada-001'
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0]
+        # [[-5.5],        [[log Pr(z | x, y)],
+        #  [-8.2, -2.1]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1]
+        # [[-11.6],       [[log Pr(z | a, b, c)],
+        #  [-0.3, -1.2]]   [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+    """
+    ## str / non-Sequence[str] inputs silently, wastefully, and irreparably fail
+    if isinstance(prompts, str) or not isinstance(prompts, Sequence):
+        raise TypeError("prompts must be a Sequence of strings.")
+    if isinstance(completions, str) or not isinstance(completions, Sequence):
+        raise TypeError("completions must be a Sequence of strings.")
+    ## Flat list of prompts and their completions. Will post-process
+    texts = [
+        prompt + end_of_prompt + completion
+        for prompt in prompts
+        for completion in completions
+    ]
+    log_probs = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
+    ## Since log_probs is a flat list, we'll need to batch them by the size and order of
+    ## completions to fulfill the spec.
+    return [
+        _slice_completions(completions, log_probs_batch, model)
+        for log_probs_batch in _batch.constant(log_probs, size=len(completions))
+    ]
+
+
+def log_probs_conditional_examples(
+    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
+) -> list[list[list[float]]]:
+    """
+    Log-probabilities of each completion token conditional on each prompt.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    log_probs_completions : list[list[list[float]]]
+        `log_probs_completions[example_idx][completion_idx][completion_token_idx]` is
+        the log-probability of the completion token in
+        `examples[example_idx].completions[completion_idx]`, conditional on
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt` and
+        previous completion tokens.
+
+    Note
+    ----
+    To aggregate `log_probs_completions`, use
+    :func:`cappr.utils.classify.agg_log_probs`.
+
+    Note
+    ----
+    The attribute :attr:`cappr.Example.prior` is unused.
+
+    Example
+    -------
+    Here we'll use single characters (which are of course single tokens) to more clearly
+    demonstrate what this function does::
+
+        from cappr import Example
+        from cappr.openai.classify import log_probs_conditional_examples
+
+        # Create data
+        examples = [Example(prompt='x y',   completions=('z', 'd e')),
+                    Example(prompt='a b c', completions=('1 2',))]
+
+        # Compute
+        log_probs_completions = log_probs_conditional_examples(
+                                    examples,
+                                    model='text-ada-001'
+                                )
+
+        # Outputs (rounded) next to their symbolic representation
+
+        log_probs_completions[0] # corresponds to examples[0]
+        # [[-5.5],        [[log Pr(z | x, y)],
+        #  [-8.2, -2.1]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
+
+        log_probs_completions[1] # corresponds to examples[1]
+        # [[-11.2, -4.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
+    """
+    ## Flat list of prompts and their completions. Will post-process
+    texts = [
+        example.prompt + example.end_of_prompt + completion
+        for example in examples
+        for completion in example.completions
+    ]
+    log_probs_all = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
+    ## Flatten completions in same order as examples were flattened
+    completions_all = [
+        completion for example in examples for completion in example.completions
+    ]
+    log_probs_completions_all = _slice_completions(
+        completions_all, log_probs_all, model
+    )
+    ## Batch by completions to fulfill the spec
+    num_completions_per_prompt = [len(example.completions) for example in examples]
+    return list(
+        _batch.variable(log_probs_completions_all, sizes=num_completions_per_prompt)
+    )
+
+
+@classify._predict_proba
+def predict_proba(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: openai.api.Model,
+    prior: Optional[Sequence[float]] = None,
+    end_of_prompt: str = " ",
+    discount_completions: float = 0.0,
+    ask_if_ok: bool = False,
+) -> npt.NDArray[np.floating]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    discount_completions : float, optional
+        experimental feature: set it to >0.0 (e.g., 1.0 may work well) if a completion
+        is consistently getting too high predicted probabilities. You could instead
+        fudge the `prior`, but this hyperparameter may be easier to tune than the
+        `prior`. By default 0.0
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    pred_probs : npt.NDArray[np.floating]
+        Array with shape `(len(prompts), len(completions))`.
+        `pred_probs[prompt_idx, completion_idx]` is the `model`'s estimate of the
+        probability that `completions[completion_idx]` comes after
+        `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_proba_examples`.
+
+    Example
+    -------
+    A more complicated business-y example—classify product reviews::
+
+        from cappr.openai.classify import predict_proba
+
+
+        # Define a classification task
+        feedback_types = ('the product is too expensive',
+                          'the product uses low quality materials',
+                          'the product is difficult to use',
+                          'the product is great')
+        prior = (2/5, 1/5, 1/5, 1/5) # I already expect customers to say it's expensive
+
+
+        # Write a prompt
+        def prompt_func(product_review: str) -> str:
+            return f'''
+        This product review: {product_review}\n
+        is best summarized as:'''
+
+
+        # Supply the texts you wanna classify
+        product_reviews = ["I can't figure out how to integrate it into my setup.",
+                           "Yeah it's pricey, but it's definitely worth it."]
+        prompts = [prompt_func(product_review) for product_review in product_reviews]
+
+
+        pred_probs = predict_proba(prompts,
+                                   completions=feedback_types,
+                                   model='text-curie-001',
+                                   prior=prior)
+
+        pred_probs = pred_probs.round(1) # just for cleaner output
+
+        # predicted probability that 1st product review says it's difficult to use
+        pred_probs[0,2]
+        # 0.9
+
+        # predicted probability that 2nd product review says it's great
+        pred_probs[1,3]
+        # 0.7
+
+        # predicted probability that 2nd product review says it's too expensive
+        pred_probs[1,0]
+        # 0.1
+    """
+    if discount_completions < 0.0:
+        raise ValueError(
+            f"discount_completions must be >= 0.0. Got {discount_completions}"
+        )
+    log_probs_completions = log_probs_conditional(
+        prompts,
+        completions,
+        model,
+        end_of_prompt=end_of_prompt,
+        ask_if_ok=ask_if_ok,
+    )
+    if discount_completions == 0.0:
+        return log_probs_completions
+    log_marginal_probs_completions = _token_logprobs(
+        completions, model, ask_if_ok=ask_if_ok
+    )
+    for x in log_marginal_probs_completions:
+        x[0] = 0  ## set it from None to 0, i.e., no discount for the first token
+    return [
+        [
+            np.array(log_probs_prompt_completions[completion_idx])
+            + (
+                discount_completions
+                * np.array(log_marginal_probs_completions[completion_idx])
+            )
+            for completion_idx in range(len(completions))
+        ]
+        for log_probs_prompt_completions in log_probs_completions
+    ]
+
+
+@classify._predict_proba_examples
+def predict_proba_examples(
+    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
+) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+    """
+    Predict probabilities of each completion coming after each prompt.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+        `pred_probs[example_idx][completion_idx]` is the model's estimate of the
+        probability that `examples[example_idx].completions[completion_idx]` comes after
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+        If the number of completions per example is a constant `k`, then an array with
+        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+
+    Example
+    -------
+    Let's demo COPA https://people.ict.usc.edu/~gordon/copa.html::
+
+        from cappr import Example
+        from cappr.openai.classify import predict_proba_examples
+
+
+        # Create data from the premises and alternatives
+        examples = [Example(prompt='The man broke his toe because',
+                            completions=('he got a hole in his sock.',
+                                         'he dropped a hammer on his foot.')),
+                    Example(prompt='I tipped the bottle, so',
+                            completions=('the liquid in the bottle froze.',
+                                         'the liquid in the bottle poured out.'))]
+
+
+        pred_probs = predict_proba_examples(examples, model='text-curie-001')
+
+        pred_probs = pred_probs.round(2) # just for cleaner output
+
+        # predicted probability that 'he dropped a hammer on his foot' is the
+        # alternative implied by the 1st premise: 'The man broke his toe'
+        pred_probs[0,1]
+        # 0.53
+
+        # predicted probability that 'the liquid in the bottle poured out' is the
+        # alternative implied by the 2nd premise: 'I tipped the bottle'
+        pred_probs[1,1]
+        # 0.66
+    """
+    return log_probs_conditional_examples(examples, model, ask_if_ok=ask_if_ok)
+
+
+@classify._predict
+def predict(
+    prompts: Sequence[str],
+    completions: Sequence[str],
+    model: openai.api.Model,
+    prior: Optional[Sequence[float]] = None,
+    end_of_prompt: str = " ",
+    discount_completions: float = 0.0,
+    ask_if_ok: bool = False,
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Parameters
+    ----------
+    prompts : Sequence[str]
+        strings, where, e.g., each contains the text you want to classify
+    completions : Sequence[str]
+        strings, where, e.g., each one is the name of a class which could come after a
+        prompt
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    prior : Sequence[float], optional
+        a probability distribution over `completions`, representing a belief about their
+        likelihoods regardless of the prompt. By default, each completion in
+        `completions` is assumed to be equally likely
+    end_of_prompt : str, optional
+        the string to tack on at the end of every prompt, by default " "
+    discount_completions : float, optional
+        experimental feature: set it to >0.0 (e.g., 1.0 may work well) if a completion
+        is consistently getting over-predicted. You could instead fudge the `prior`, but
+        this hyperparameter may be easier to tune than the `prior`. By default 0.0
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(prompts)`.
+        `preds[prompt_idx]` is the completion in `completions` which is predicted to
+        follow `prompts[prompt_idx] + end_of_prompt`.
+
+    Note
+    ----
+    In this function, the set of possible completions which could follow each prompt is
+    the same for every prompt. If instead, each prompt could be followed by a
+    *different* set of completions, then construct a sequence of :class:`cappr.Example`
+    objects and pass them to :func:`predict_examples`.
+
+    Example
+    -------
+    A more complicated business-y example—classify product reviews::
+
+        from cappr.openai.classify import predict
+
+
+        # Define a classification task
+        feedback_types = ('the product is too expensive',
+                          'the product uses low quality materials',
+                          'the product is difficult to use',
+                          'the product is great')
+        prior = (2/5, 1/5, 1/5, 1/5) # I already expect customers to say it's expensive
+
+
+        # Write a prompt
+        def prompt_func(product_review: str) -> str:
+            return f'''
+        This product review: {product_review}\n
+        is best summarized as:'''
+
+
+        # Supply the texts you wanna classify
+        product_reviews = ["I can't figure out how to integrate it into my setup.",
+                           "Yeah it's pricey, but it's definitely worth it."]
+        prompts = [prompt_func(product_review) for product_review in product_reviews]
+
+
+        preds = predict(prompts,
+                        completions=feedback_types,
+                        model='text-curie-001',
+                        prior=prior)
+        preds
+        # ['the product is difficult to use',
+        #  'the product is great']
+    """
+    return predict_proba(
+        prompts,
+        completions,
+        model,
+        prior=prior,
+        end_of_prompt=end_of_prompt,
+        discount_completions=discount_completions,
+        ask_if_ok=ask_if_ok,
+    )
+
+
+@classify._predict_examples
+def predict_examples(
+    examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
+) -> list[str]:
+    """
+    Predict which completion is most likely to follow each prompt.
+
+    Parameters
+    ----------
+    examples : Sequence[Example]
+        `Example` objects, where each contains a prompt and its set of possible
+        completions
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    preds : list[str]
+        List with length `len(examples)`.
+        `preds[example_idx]` is the completion in `examples[example_idx].completions`
+        which is predicted to follow
+        `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
+
+    Example
+    -------
+    Let's demo COPA https://people.ict.usc.edu/~gordon/copa.html::
+
+        from cappr import Example
+        from cappr.openai.classify import predict_examples
+
+        # Create data from the premises and alternatives
+        examples = [Example(prompt='The man broke his toe because',
+                            completions=('he got a hole in his sock.',
+                                         'he dropped a hammer on his foot.')),
+                    Example(prompt='I tipped the bottle, so',
+                            completions=('the liquid in the bottle froze.',
+                                         'the liquid in the bottle poured out.'))]
+
+        preds = predict_examples(examples, model='text-curie-001')
+        preds
+        # ['he dropped a hammer on his foot',
+        #  'the liquid in the bottle poured out']
+    """
+    return predict_proba_examples(examples, model, ask_if_ok=ask_if_ok)
```

### Comparing `cappr-0.2.1/src/cappr/utils/_batch.py` & `cappr-0.2.2/src/cappr/utils/_batch.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""
-Batch lists into sublists of constant or variable sizes, and batchify functions.
-"""
-from __future__ import annotations
-from functools import wraps
-import inspect
-from typing import Sequence
-
-import numpy as np
-from tqdm.auto import tqdm
-
-
-def constant(lst: list, size: int):
-    """
-    TODO: numpy docstring
-
-    Generates sublists in the order of `lst` which partition `lst`. All sublists (except
-    potentially the last) have length `size`.
-    """
-    if size <= 0:
-        raise ValueError("size must be positive.")
-    lst = list(lst)  ## 0-index whatever was passed, or fully evaluate generator
-    n = len(lst)
-    for ndx in range(0, n, size):
-        yield lst[ndx : (ndx + size)]
-
-
-def variable(lst: list, sizes: Sequence[int]):
-    """
-    TODO: numpy docstring
-
-    Generates sublists in the order of `lst` which partition `lst`. The `i`'th generated
-    sublist has length `sizes[i]`.
-    """
-    sizes: np.ndarray = np.array(sizes)
-    if np.any(sizes <= 0):
-        raise ValueError("sizes must all be positive.")
-    if len(sizes.shape) != 1:
-        raise ValueError("sizes must be 1-D.")
-    cumulative_sizes = np.cumsum(sizes)
-    if cumulative_sizes[-1] != len(lst):
-        raise ValueError("sizes must sum to len(lst).")
-    ## We want start and stop idxs. The first start idx must ofc be 0.
-    cumulative_sizes = np.insert(cumulative_sizes, 0, 0)
-    lst = list(lst)  ## 0-index and/or fully evaluate generator
-    for start, stop in zip(cumulative_sizes[:-1], cumulative_sizes[1:]):
-        yield lst[start:stop]
-
-
-def _kwarg_name_to_value(func):
-    """
-    Returns a dictionary mapping keyword arguments in the signature of `func`
-    to their default values.
-    """
-    ## ty https://stackoverflow.com/a/12627202/18758987
-    signature = inspect.signature(func)
-    return {
-        name: value.default
-        for name, value in signature.parameters.items()
-        if value.default is not inspect.Parameter.empty
-    }
-
-
-def batchify(batchable_arg: str, batch_size: int = 32, progress_bar_desc: str = ""):
-    """
-    TODO: numpy docstring
-
-    Returns a decorator which runs the decorated function in batches along its
-    `batchable_arg`, returning a list of the function's outputs for each batch.
-
-    If the function includes a `'batch_size'` keyword argument, then its value is used
-    as the batch size instead of the decorator's default `batch_size`.
-    TODO: allow non-kwarg too.
-    """
-
-    def decorator(func):
-        _arg_names = inspect.getfullargspec(func).args
-        batchable_arg_idx = _arg_names.index(batchable_arg)
-        batch_size_default = _kwarg_name_to_value(func).get("batch_size", batch_size)
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            batchable: Sequence = args[batchable_arg_idx]
-            size = kwargs.get("batch_size", batch_size_default)
-            outputs = []
-            args = list(args)  ## need to modify the batch argument value
-            with tqdm(total=len(batchable), desc=progress_bar_desc) as progress_bar:
-                for batch_ in constant(batchable, size):
-                    args[batchable_arg_idx] = batch_
-                    outputs.append(func(*args, **kwargs))
-                    progress_bar.update(len(batch_))
-            return outputs
-
-        return wrapper
-
-    return decorator
-
-
-def flatten(batchified_func):
-    """
-    TODO: numpy docstring
-
-    Decorates a `cappr.utils._batch.batchify`d function. Flattens the output.
-    """
-
-    @wraps(batchified_func)
-    def wrapper(*args, **kwargs):
-        nested_outputs = batchified_func(*args, **kwargs)
-        return [output for inner_outputs in nested_outputs for output in inner_outputs]
-
-    return wrapper
+"""
+Batch lists into sublists of constant or variable sizes, and batchify functions.
+"""
+from __future__ import annotations
+from functools import wraps
+import inspect
+from typing import Sequence
+
+import numpy as np
+from tqdm.auto import tqdm
+
+
+def constant(lst: list, size: int):
+    """
+    TODO: numpy docstring
+
+    Generates sublists in the order of `lst` which partition `lst`. All sublists (except
+    potentially the last) have length `size`.
+    """
+    if size <= 0:
+        raise ValueError("size must be positive.")
+    lst = list(lst)  ## 0-index whatever was passed, or fully evaluate generator
+    n = len(lst)
+    for ndx in range(0, n, size):
+        yield lst[ndx : (ndx + size)]
+
+
+def variable(lst: list, sizes: Sequence[int]):
+    """
+    TODO: numpy docstring
+
+    Generates sublists in the order of `lst` which partition `lst`. The `i`'th generated
+    sublist has length `sizes[i]`.
+    """
+    sizes: np.ndarray = np.array(sizes)
+    if np.any(sizes <= 0):
+        raise ValueError("sizes must all be positive.")
+    if len(sizes.shape) != 1:
+        raise ValueError("sizes must be 1-D.")
+    cumulative_sizes = np.cumsum(sizes)
+    if cumulative_sizes[-1] != len(lst):
+        raise ValueError("sizes must sum to len(lst).")
+    ## We want start and stop idxs. The first start idx must ofc be 0.
+    cumulative_sizes = np.insert(cumulative_sizes, 0, 0)
+    lst = list(lst)  ## 0-index and/or fully evaluate generator
+    for start, stop in zip(cumulative_sizes[:-1], cumulative_sizes[1:]):
+        yield lst[start:stop]
+
+
+def _kwarg_name_to_value(func):
+    """
+    Returns a dictionary mapping keyword arguments in the signature of `func`
+    to their default values.
+    """
+    ## ty https://stackoverflow.com/a/12627202/18758987
+    signature = inspect.signature(func)
+    return {
+        name: value.default
+        for name, value in signature.parameters.items()
+        if value.default is not inspect.Parameter.empty
+    }
+
+
+def batchify(batchable_arg: str, batch_size: int = 32, progress_bar_desc: str = ""):
+    """
+    TODO: numpy docstring
+
+    Returns a decorator which runs the decorated function in batches along its
+    `batchable_arg`, returning a list of the function's outputs for each batch.
+
+    If the function includes a `'batch_size'` keyword argument, then its value is used
+    as the batch size instead of the decorator's default `batch_size`.
+    TODO: allow non-kwarg too.
+    """
+
+    def decorator(func):
+        _arg_names = inspect.getfullargspec(func).args
+        batchable_arg_idx = _arg_names.index(batchable_arg)
+        batch_size_default = _kwarg_name_to_value(func).get("batch_size", batch_size)
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            batchable: Sequence = args[batchable_arg_idx]
+            size = kwargs.get("batch_size", batch_size_default)
+            outputs = []
+            args = list(args)  ## need to modify the batch argument value
+            with tqdm(total=len(batchable), desc=progress_bar_desc) as progress_bar:
+                for batch_ in constant(batchable, size):
+                    args[batchable_arg_idx] = batch_
+                    outputs.append(func(*args, **kwargs))
+                    progress_bar.update(len(batch_))
+            return outputs
+
+        return wrapper
+
+    return decorator
+
+
+def flatten(batchified_func):
+    """
+    TODO: numpy docstring
+
+    Decorates a `cappr.utils._batch.batchify`d function. Flattens the output.
+    """
+
+    @wraps(batchified_func)
+    def wrapper(*args, **kwargs):
+        nested_outputs = batchified_func(*args, **kwargs)
+        return [output for inner_outputs in nested_outputs for output in inner_outputs]
+
+    return wrapper
```

### Comparing `cappr-0.2.1/src/cappr/utils/_check.py` & `cappr-0.2.2/src/cappr/utils/_check.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from __future__ import annotations
-from typing import Optional, Sequence
-
-import numpy as np
-
-
-def prior(prior: Optional[Sequence[float]] = None):
-    """
-    Raises an error if `prior` is not `None`, or if it's not a 1-D `Sequence` which sums
-    to 1.
-    """
-    if prior is None:  ## it's a uniform prior, no need to check anything
-        return None
-    if not (isinstance(prior, Sequence) or isinstance(prior, np.ndarray)):
-        raise TypeError("prior must be None or a Sequence.")
-    if len(np.shape(prior)) != 1:
-        raise ValueError("prior must be 1-D.")
-    prior_arr = np.array(prior, dtype=float)  ## try casting to float
-    if not np.isclose(prior_arr.sum(), 1):
-        raise ValueError("prior must sum to 1.")
+from __future__ import annotations
+from typing import Optional, Sequence
+
+import numpy as np
+
+
+def prior(prior: Optional[Sequence[float]] = None):
+    """
+    Raises an error if `prior` is not `None`, or if it's not a 1-D `Sequence` which sums
+    to 1.
+    """
+    if prior is None:  ## it's a uniform prior, no need to check anything
+        return
+    if not isinstance(prior, (Sequence, np.ndarray)):
+        raise TypeError("prior must be None or a sequence.")
+    if len(np.shape(prior)) != 1:
+        raise ValueError("prior must be 1-D.")
+    prior_arr = np.array(prior, dtype=float)  ## try casting to float
+    if not np.isclose(prior_arr.sum(), 1):
+        raise ValueError("prior must sum to 1.")
```

### Comparing `cappr-0.2.1/src/cappr/utils/classify.py` & `cappr-0.2.2/src/cappr/utils/classify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,320 +1,304 @@
-"""
-Transform completion token log-probabilites to a probability distribution over
-completions.
-"""
-from __future__ import annotations
-from functools import wraps
-from typing import Callable, Optional, Sequence, Union
-
-import numpy as np
-import numpy.typing as npt
-
-from cappr.utils import _check
-
-
-def agg_log_probs(
-    log_probs: Sequence[Sequence[Sequence[float]]],
-    func: Callable[[Sequence[float]], float] = np.mean,
-) -> list[list[float]]:
-    """
-    Aggregate token log-probabilities along the last dimension into probabilities.
-
-    Note
-    ----
-    If `log_probs` was derived from a constant set of completions, e.g., it's the
-    output of
-    :func:`cappr.openai.classify.log_probs_conditional` or
-    :func:`cappr.huggingface.classify.log_probs_conditional`, then use the more
-    efficient :func:`agg_log_probs_from_constant_completions` function instead of this
-    one.
-
-    Parameters
-    ----------
-    log_probs : Sequence[Sequence[Sequence[float]]]
-        sequences where token log-probabilities are in the last dimension
-    func : Callable[[Sequence[float]], float], optional
-        function which aggregates a sequence of token log-probabilities into a single
-        log-probability, by default np.mean
-
-    Returns
-    -------
-    probs: list[list[float]]
-        Lists of probabilities where::
-
-            probs[i][j] = np.exp(func(log_probs[i][j]))
-    """
-    return [
-        [
-            np.exp(func(log_probs_completion))
-            for log_probs_completion in log_probs_completions
-        ]
-        for log_probs_completions in log_probs
-    ]
-
-
-def agg_log_probs_from_constant_completions(
-    log_probs: Sequence[Sequence[Sequence[float]]],
-    func: Callable[[Sequence[float]], float] = np.mean,
-) -> npt.NDArray[np.floating]:
-    """
-    Aggregate token log-probabilities along the last dimension into probabilities.
-
-    Warning
-    -------
-    If `log_probs` was NOT dervived from a constant set of completions, e.g., it's
-    the output of
-    :func:`cappr.openai.classify.log_probs_conditional_examples` or
-    :func:`cappr.huggingface.classify.log_probs_conditional_examples`, then you must use
-    :func:`agg_log_probs` function instead of this function.
-
-    Parameters
-    ----------
-    log_probs : Sequence[Sequence[Sequence[float]]]
-        sequences where token log-probabilities (from a constant set of completions) are
-        in the last dimension
-    func : Callable[[Sequence[float]], float], optional
-        function which aggregates a sequence of token log-probabilities into a single
-        log-probability **AND** takes an ``axis`` keyword argument, by default np.mean
-
-    Returns
-    -------
-    probs: npt.NDArray[np.floating]
-        Array of probabilities where::
-
-            probs[i,j] = np.exp(func(log_probs[i][j]))
-    """
-    num_completions_per_prompt = [
-        len(log_probs_completions) for log_probs_completions in log_probs
-    ]
-    num_completions_per_prompt_set = set(num_completions_per_prompt)
-    if not len(num_completions_per_prompt_set) == 1:
-        raise ValueError(
-            "log_probs does not have a constant number of completions, i.e., there are "
-            "indices i, j such that len(log_probs[i]) != len(log_probs[j]). Please use "
-            "the slower function, agg_log_probs, instead."
-        )
-    ## Say, e.g., we have 2 completions, ['a b', 'c d e'], and 2 prompts.
-    ## Then log_probs looks like:
-    ## [ [ [a1, b1],      (token log-probs for completion 1 | prompt 1)
-    #      [c1, d1, e1]], (token log-probs for completion 2 | prompt 1)
-    ##   [ [a2, b2],      (token log-probs for completion 1 | prompt 2)
-    ##     [c2, d2, e2]]  (token log-probs for completion 2 | prompt 2)
-    ## ]
-    ## We can re-shape this "jagged" list as a list of (non-jagged) arrays:
-    ## [ array([[a1, b1]],
-    ##         [[a2, b2]]),
-    ##   array([[c1, d1, e1]],
-    ##         [[c2, d2, e2]])
-    ## ]
-    num_completions_per_prompt = list(num_completions_per_prompt_set)[0]
-    array_list = [
-        np.array(  ## raises jagged/inhomogeneous ValueError if non-constant # tokens
-            [
-                log_probs_completions[completion_idx]
-                for log_probs_completions in log_probs
-            ]
-        )
-        for completion_idx in range(num_completions_per_prompt)
-    ]
-    ## Now we can apply the vectorized function to each array in the list
-    likelihoods: npt.NDArray[np.floating] = np.exp(
-        np.array([func(array, axis=1) for array in array_list])
-    )
-    ## likelihoods looks like:
-    ## array([[likelihood_a1b1,   likelihood_a2b2  ],
-    ##        [likelihood_c1d1e1, likelihood_c2d2e2]
-    ##       ])
-    ## Transpose it to fulfill the spec
-    return likelihoods.T
-
-
-def posterior_prob(
-    likelihoods: npt.ArrayLike[float],
-    axis: int,
-    prior: Optional[Union[Sequence[float], npt.ArrayLike[float]]] = None,
-    normalize: Union[bool, Sequence[bool]] = True,
-    check_prior: bool = True,
-) -> npt.NDArray[np.floating]:
-    """
-    Compute posterior probabilities from likelihoods and a prior.
-
-    Parameters
-    ----------
-    likelihoods : npt.ArrayLike[float]
-        2-D array of probabilities of data given a hypothesis
-    axis : int
-        the axis along which the probability distribution should be defined, e.g.,
-        `axis=0` if `likelihoods` is 1-D
-    prior : Optional[Union[Sequence[float], npt.ArrayLike[float]]], optional
-        a probability distribution over the `axis` of `likelihoods`, by default None
-    normalize : Union[bool, Sequence[bool]], optional
-        whether or not to return a normalized probability distribtution for each row, by
-        default True (normalize all rows)
-    check_prior : bool, optional
-        whether or not to check that the `prior` is indeed a probability distribution,
-        by default True
-
-    Returns
-    -------
-    posterior_probs : npt.NDArray[np.floating]
-        2-D array of probabilities of a hypothesis given data. Its shape is the same as
-        `likelihood.shape`
-
-    Raises
-    ------
-    ValueError
-        if `normalize` is a sequence whose length is different than that of
-        `likelihoods`
-    """
-    ## Input checks and preprocessing
-    likelihoods = np.array(likelihoods)  ## it should not be jagged/inhomogenous
-    if not isinstance(normalize, Sequence):
-        ## For code simplicity, just repeat it
-        ## If likelihoods is 1-D, there's only a single probability distr to normalize
-        num_repeats = 1 if len(likelihoods.shape) == 1 else likelihoods.shape[0]
-        normalize = [normalize] * num_repeats
-    elif len(normalize) != len(likelihoods):
-        raise ValueError(
-            "If normalize is a Sequence, it must have the same length as likelihoods. "
-            f"Got {len(normalize)}, {len(likelihoods)}."
-        )
-    normalize = np.array(normalize, dtype=bool)
-    if prior is not None and check_prior:
-        _check.prior(prior)
-
-    ## Apply Bayes' rule, w/ optional normalization per row
-    if prior is None:
-        posteriors_unnorm = likelihoods
-    else:
-        posteriors_unnorm = likelihoods * prior
-    marginals = posteriors_unnorm.sum(axis=axis, keepdims=True)
-    marginals[~normalize] = 1  ## denominator of 1 <=> no normalization
-    return posteriors_unnorm / marginals
-
-
-def _predict_proba(conditional_func):
-    """
-    TODO: docstring
-    """
-
-    @wraps(conditional_func)
-    def wrapper(
-        prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
-    ) -> npt.NDArray[np.floating]:
-        ## Before hitting any APIs ($$), let's check the prior
-        prior = kwargs.get("prior", None)
-        _check.prior(prior)
-        if prior is not None and len(completions) != len(prior):
-            raise ValueError(
-                "completions and prior are different lengths: "
-                f"{len(completions)}, {len(prior)}."
-            )
-
-        log_probs_completions = conditional_func(prompts, completions, *args, **kwargs)
-        likelihoods = agg_log_probs_from_constant_completions(log_probs_completions)
-        ## If there's only 1 completion, normalizing will cause the probability to
-        ## trivially be 1! So let's not normalize in that case, and hope the user knows
-        ## what they're doing
-        normalize = len(completions) > 1
-        return posterior_prob(likelihoods, axis=1, prior=prior, normalize=normalize)
-
-    return wrapper
-
-
-def _predict_proba_examples(conditional_examples_func):
-    """
-    TODO: docstring
-    """
-
-    @wraps(conditional_examples_func)
-    def wrapper(
-        examples, *args, **kwargs
-    ) -> Union[list[list[float]], npt.NDArray[np.floating]]:
-        log_probs_completions = conditional_examples_func(examples, *args, **kwargs)
-        likelihoods = agg_log_probs(log_probs_completions)
-        ## If an example has just 1 completion, normalizing will cause the probability
-        ## to trivially be 1! So let's not normalize in that case, and hope the user
-        ## knows what they're doing
-        num_completions_per_prompt = [len(example.completions) for example in examples]
-        normalize = [num > 1 for num in num_completions_per_prompt]
-        num_completions_per_prompt_set = set(num_completions_per_prompt)
-        if len(num_completions_per_prompt_set) != 1:
-            ## Can't be vectorized :-(
-            return [
-                posterior_prob(
-                    likelihoods_ex,
-                    axis=0,
-                    prior=example.prior,
-                    normalize=normalize_ex,
-                    check_prior=False,  ## already checked during example construction
-                )
-                for likelihoods_ex, example, normalize_ex in zip(
-                    likelihoods, examples, normalize
-                )
-            ]
-        ## Vectorize!
-        if all([example.prior is None for example in examples]):
-            prior = None
-        else:
-            ## For coding simplicity, just supply a prior which is non-None *everywhere*
-            ## It's the same shape as likelihoods
-            prior = np.array(
-                [
-                    example.prior
-                    or [1 / len(example.completions)] * len(example.completions)
-                    for example in examples
-                ]
-            )
-        ## prior cannot be jagged b/c every example has the same # of completions
-        return posterior_prob(
-            likelihoods,
-            axis=1,
-            prior=prior,
-            normalize=normalize,
-            check_prior=False,  ## ## already checked during example construction
-        )
-
-    return wrapper
-
-
-def _predict(predict_proba_func):
-    """
-    TODO: docstring
-    """
-
-    @wraps(predict_proba_func)
-    def wrapper(
-        prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
-    ) -> list[str]:
-        pred_probs: npt.NDArray = predict_proba_func(
-            prompts, completions, *args, **kwargs
-        )
-        pred_class_idxs = pred_probs.argmax(axis=1)
-        return [completions[pred_class_idx] for pred_class_idx in pred_class_idxs]
-
-    return wrapper
-
-
-def _predict_examples(predict_proba_examples_func):
-    """
-    TODO: docstring
-    """
-
-    @wraps(predict_proba_examples_func)
-    def wrapper(examples, *args, **kwargs) -> list[str]:
-        pred_probs: Union[
-            list[list[float]], npt.NDArray[np.floating]
-        ] = predict_proba_examples_func(examples, *args, **kwargs)
-        ## If it's an array, we can call .argmax, which is faster
-        try:
-            pred_class_idxs = pred_probs.argmax(axis=1)
-        except AttributeError:
-            pred_class_idxs = [
-                np.argmax(example_pred_probs) for example_pred_probs in pred_probs
-            ]
-        return [
-            example.completions[pred_class_idx]
-            for example, pred_class_idx in zip(examples, pred_class_idxs)
-        ]
-
-    return wrapper
+"""
+Transform completion token log-probabilites to a probability distribution over
+completions.
+"""
+from __future__ import annotations
+from functools import wraps
+from typing import Callable, Optional, Sequence, Union
+
+import numpy as np
+import numpy.typing as npt
+
+from cappr.utils import _check
+
+
+def _agg_log_probs(
+    log_probs: Sequence[Sequence[Sequence[float]]],
+    func: Callable[[Sequence[float]], float] = np.mean,
+) -> list[list[float]]:
+    """
+    Aggregate using a nested list comprehension.
+    """
+    return [
+        [
+            np.exp(func(log_probs_completion))
+            for log_probs_completion in log_probs_completions
+        ]
+        for log_probs_completions in log_probs
+    ]
+
+
+def _agg_log_probs_from_constant_completions(
+    log_probs: Sequence[Sequence[Sequence[float]]],
+    func: Callable[[Sequence[float]], float] = np.mean,
+) -> npt.NDArray[np.floating]:
+    """
+    Aggregate using a vectorized numpy function `func`.
+    """
+    num_completions_per_prompt = [
+        len(log_probs_completions) for log_probs_completions in log_probs
+    ]
+    num_completions_per_prompt_set = set(num_completions_per_prompt)
+    if not len(num_completions_per_prompt_set) == 1:
+        raise ValueError(
+            "log_probs does not have a constant number of completions, i.e., there are "
+            "indices i, j such that len(log_probs[i]) != len(log_probs[j]). Please use "
+            "the slower function, agg_log_probs, instead."
+        )
+    ## Say, e.g., we have 2 completions, ['a b', 'c d e'], and 2 prompts.
+    ## Then log_probs looks like:
+    ## [ [ [a1, b1],      (token log-probs for completion 1 | prompt 1)
+    #      [c1, d1, e1]], (token log-probs for completion 2 | prompt 1)
+    ##   [ [a2, b2],      (token log-probs for completion 1 | prompt 2)
+    ##     [c2, d2, e2]]  (token log-probs for completion 2 | prompt 2)
+    ## ]
+    ## We can re-shape this "jagged" list as a list of (non-jagged) arrays:
+    ## [ array([[a1, b1]],
+    ##         [[a2, b2]]),
+    ##   array([[c1, d1, e1]],
+    ##         [[c2, d2, e2]])
+    ## ]
+    num_completions_per_prompt = list(num_completions_per_prompt_set)[0]
+    array_list = [
+        np.array(  ## raises jagged/inhomogeneous ValueError if non-constant # tokens
+            [
+                log_probs_completions[completion_idx]
+                for log_probs_completions in log_probs
+            ]
+        )
+        for completion_idx in range(num_completions_per_prompt)
+    ]
+    ## Now we can apply the vectorized function to each array in the list
+    likelihoods: npt.NDArray[np.floating] = np.exp(
+        np.array([func(array, axis=1) for array in array_list])
+    )
+    ## likelihoods looks like:
+    ## array([[likelihood_a1b1,   likelihood_a2b2  ],
+    ##        [likelihood_c1d1e1, likelihood_c2d2e2]
+    ##       ])
+    ## Transpose it to fulfill the spec
+    return likelihoods.T
+
+
+def agg_log_probs(
+    log_probs: Sequence[Sequence[Sequence[float]]],
+    func: Callable[[Sequence[float]], float] = np.mean,
+) -> list[list[float]]:
+    """
+    Aggregate token log-probabilities along the last dimension into probabilities.
+
+    Parameters
+    ----------
+    log_probs : Sequence[Sequence[Sequence[float]]]
+        nested sequences where token log-probabilities are in the last dimension
+    func : Callable[[Sequence[float]], float], optional
+        function which aggregates a sequence of token log-probabilities into a single
+        log-probability. If the function is vectorized, it must take an ``axis``
+        argument. By default, `numpy.mean`
+
+    Returns
+    -------
+    probs: list[list[float]]
+        Lists of probabilities where::
+
+            probs[i][j] = numpy.exp(func(log_probs[i][j]))
+    """
+    try:
+        return _agg_log_probs_from_constant_completions(log_probs, func)
+    except (
+        ValueError,  ## log_probs is jagged
+        TypeError,  ## func doesn't take an axis argument
+    ):
+        return _agg_log_probs(log_probs, func)
+
+
+def posterior_prob(
+    likelihoods: npt.ArrayLike[float],
+    axis: int,
+    prior: Optional[Union[Sequence[float], npt.ArrayLike[float]]] = None,
+    normalize: Union[bool, Sequence[bool]] = True,
+    check_prior: bool = True,
+) -> npt.NDArray[np.floating]:
+    """
+    Compute posterior probabilities from likelihoods and a prior.
+
+    Parameters
+    ----------
+    likelihoods : npt.ArrayLike[float]
+        2-D array of probabilities of data given a hypothesis
+    axis : int
+        the axis along which the probability distribution should be defined, e.g.,
+        `axis=0` if `likelihoods` is 1-D
+    prior : Optional[Union[Sequence[float], npt.ArrayLike[float]]], optional
+        a probability distribution over the `axis` of `likelihoods`, by default None
+    normalize : Union[bool, Sequence[bool]], optional
+        whether or not to return a normalized probability distribtution for each row, by
+        default True (normalize all rows)
+    check_prior : bool, optional
+        whether or not to check that the `prior` is indeed a probability distribution,
+        by default True
+
+    Returns
+    -------
+    posterior_probs : npt.NDArray[np.floating]
+        2-D array of probabilities of a hypothesis given data. Its shape is the same as
+        `likelihood.shape`
+
+    Raises
+    ------
+    ValueError
+        if `normalize` is a sequence whose length is different than that of
+        `likelihoods`
+    """
+    ## Input checks and preprocessing
+    likelihoods = np.array(likelihoods)  ## it should not be jagged/inhomogenous
+    if not isinstance(normalize, (Sequence, np.ndarray)):
+        ## For code simplicity, just repeat it
+        ## If likelihoods is 1-D, there's only a single probability distr to normalize
+        num_repeats = 1 if len(likelihoods.shape) == 1 else likelihoods.shape[0]
+        normalize = [normalize] * num_repeats
+    elif len(normalize) != len(likelihoods):
+        raise ValueError(
+            "If normalize is a Sequence, it must have the same length as likelihoods. "
+            f"Got {len(normalize)}, {len(likelihoods)}."
+        )
+    normalize = np.array(normalize, dtype=bool)
+    if check_prior:
+        _check.prior(prior)
+
+    ## Apply Bayes' rule, w/ optional normalization per row
+    if prior is None:
+        posteriors_unnorm = likelihoods
+    else:
+        posteriors_unnorm = likelihoods * prior
+    marginals = posteriors_unnorm.sum(axis=axis, keepdims=True)
+    marginals[~normalize] = 1  ## denominator of 1 <=> no normalization
+    return posteriors_unnorm / marginals
+
+
+def _predict_proba(conditional_func):
+    """
+    TODO: docstring
+    """
+
+    @wraps(conditional_func)
+    def wrapper(
+        prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
+    ) -> npt.NDArray[np.floating]:
+        ## Before hitting any APIs ($$), let's check the prior
+        prior = kwargs.get("prior", None)
+        _check.prior(prior)
+        if prior is not None and len(completions) != len(prior):
+            raise ValueError(
+                "completions and prior are different lengths: "
+                f"{len(completions)}, {len(prior)}."
+            )
+
+        log_probs_completions = conditional_func(prompts, completions, *args, **kwargs)
+        likelihoods = agg_log_probs(log_probs_completions)
+        ## If there's only 1 completion, normalizing will cause the probability to
+        ## trivially be 1! So let's not normalize in that case, and hope the user knows
+        ## what they're doing
+        normalize = len(completions) > 1
+        return posterior_prob(likelihoods, axis=1, prior=prior, normalize=normalize)
+
+    return wrapper
+
+
+def _predict_proba_examples(conditional_examples_func):
+    """
+    TODO: docstring
+    """
+
+    @wraps(conditional_examples_func)
+    def wrapper(
+        examples, *args, **kwargs
+    ) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+        log_probs_completions = conditional_examples_func(examples, *args, **kwargs)
+        likelihoods = agg_log_probs(log_probs_completions)
+        ## If an example has just 1 completion, normalizing will cause the probability
+        ## to trivially be 1! So let's not normalize in that case, and hope the user
+        ## knows what they're doing
+        num_completions_per_prompt = [len(example.completions) for example in examples]
+        normalize = [num > 1 for num in num_completions_per_prompt]
+        num_completions_per_prompt_set = set(num_completions_per_prompt)
+        if len(num_completions_per_prompt_set) != 1:
+            ## Can't be vectorized :-(
+            return [
+                posterior_prob(
+                    likelihoods_ex,
+                    axis=0,
+                    prior=example.prior,
+                    normalize=normalize_ex,
+                    check_prior=False,  ## already checked during example construction
+                )
+                for likelihoods_ex, example, normalize_ex in zip(
+                    likelihoods, examples, normalize
+                )
+            ]
+        ## Vectorize!
+        if all([example.prior is None for example in examples]):
+            prior = None
+        else:
+            ## For coding simplicity, just supply a prior which is non-None *everywhere*
+            ## It's the same shape as likelihoods
+            prior = np.array(
+                [
+                    example.prior
+                    or [1 / len(example.completions)] * len(example.completions)
+                    for example in examples
+                ]
+            )
+        ## prior cannot be jagged b/c every example has the same # of completions
+        return posterior_prob(
+            likelihoods,
+            axis=1,
+            prior=prior,
+            normalize=normalize,
+            check_prior=False,  ## ## already checked during example construction
+        )
+
+    return wrapper
+
+
+def _predict(predict_proba_func):
+    """
+    TODO: docstring
+    """
+
+    @wraps(predict_proba_func)
+    def wrapper(
+        prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
+    ) -> list[str]:
+        pred_probs: npt.NDArray = predict_proba_func(
+            prompts, completions, *args, **kwargs
+        )
+        pred_class_idxs = pred_probs.argmax(axis=1)
+        return [completions[pred_class_idx] for pred_class_idx in pred_class_idxs]
+
+    return wrapper
+
+
+def _predict_examples(predict_proba_examples_func):
+    """
+    TODO: docstring
+    """
+
+    @wraps(predict_proba_examples_func)
+    def wrapper(examples, *args, **kwargs) -> list[str]:
+        pred_probs: Union[
+            list[list[float]], npt.NDArray[np.floating]
+        ] = predict_proba_examples_func(examples, *args, **kwargs)
+        ## If it's an array, we can call .argmax, which is faster
+        try:
+            pred_class_idxs = pred_probs.argmax(axis=1)
+        except AttributeError:
+            pred_class_idxs = [
+                np.argmax(example_pred_probs) for example_pred_probs in pred_probs
+            ]
+        return [
+            example.completions[pred_class_idx]
+            for example, pred_class_idx in zip(examples, pred_class_idxs)
+        ]
+
+    return wrapper
```

### Comparing `cappr-0.2.1/src/cappr.egg-info/PKG-INFO` & `cappr-0.2.2/src/cappr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,448 +1,453 @@
-Metadata-Version: 2.1
-Name: cappr
-Version: 0.2.1
-Summary: Zero-shot text classification using autoregressive language models.
-Home-page: https://github.com/kddubey/cappr/
-Author-email: kushdubey63@gmail.com
-License: Apache License 2.0
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: hf
-Provides-Extra: demos
-Provides-Extra: dev
-License-File: LICENSE
-
-# CAPPr: zero-shot text classification using autoregressive language models
-
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
-[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-Perform zero-shot text classification by estimating the probability that an inputted
-completion comes after an inputted prompt. Hence the name:
-
-> **C**ompletion<br>
-  **A**fter<br>
-  **P**rompt<br>
-  **Pr**obability<br>
-
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
-
-## Usage
-
-<details>
-<summary>Use a model from the OpenAI API</summary>
-
-Specifically, this model must be compatible with the
-[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-endpoint.
-
-Let's classify
-[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
-from the OpenAI text completion docs.
-
-```python
-from cappr.openai.classify import predict
-
-tweet = 'I loved the new Batman movie!'
-prompt = f'Tweet: {tweet}\nSentiment:'
-
-class_names = ('positive', 'neutral', 'negative')
-# optional: let's supply a prior distribution over the classes
-prior       = (   1/8    ,    1/8   ,     3/4   )
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='text-ada-001',
-                prior=prior)
-preds
-# ['positive']
-```
-</details>
-
-<details>
-<summary>Use a model from the HuggingFace model hub</summary>
-
-Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
-
-```python
-from cappr.huggingface.classify import predict
-
-prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
-
-class_names = ('Mercury', 'Earth')
-prior = None  # uniform prior
-
-preds = predict(prompts=[prompt],
-                completions=class_names,
-                model='gpt2',
-                prior=prior)
-preds
-# ['Mercury']
-```
-</details>
-
-<details>
-<summary>Run in batches</summary>
-
-Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
-instead of the class.
-
-```python
-from cappr.huggingface.classify import predict_proba
-
-prompts = [
-    'Stephen Curry is a',
-    'Martina Navratilova was a',
-    "Dexter, from the TV Series Dexter's Laboratory, is a",
-    'LeBron James is a',    
-]
-
-# each of the prompts could be completed with one of these:
-class_names = (
-    'basketball player',
-    'tennis player',
-    'scientist'
-)
-
-prior = (
-    1/6,  # few
-    1/6,  # few
-    2/3   # there are more
-)
-
-pred_probs = predict_proba(prompts=prompts,
-                           completions=class_names,
-                           model='gpt2',
-                           batch_size=32,  # whatever fits on your CPU/GPU
-                           prior=prior)
-
-# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
-print(pred_probs.round(1))
-# [[0.5 0.3 0.2]
-#  [0.3 0.6 0.2]
-#  [0.1 0.1 0.8]
-#  [0.8 0.2 0. ]]
-
-# for each prompt, which completion is most likely?
-pred_class_idxs = pred_probs.argmax(axis=1)
-print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
-# ['basketball player',
-#  'tennis player',
-#  'scientist',
-#  'basketball player']
-```
-</details>
-
-<details>
-<summary>Run in batches, where each prompt has a different set of possible completions
-</summary>
-
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
-
-```python
-import numpy as np
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-from cappr import Example
-from cappr.huggingface.classify import predict_proba_examples
-
-examples = [
-    Example(prompt='Jodie Foster played',
-            completions=('Clarice Starling', 'Trinity in The Matrix')),
-    Example(prompt='Batman, from Batman: The Animated Series, was played by',
-            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
-            prior=      (     1/3      ,      2/3     ,      0      ))
-]
-
-model_name = 'gpt2'
-model = AutoModelForCausalLM.from_pretrained(model_name)
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-pred_probs = predict_proba_examples(examples,
-                                    model_and_tokenizer=(model, tokenizer))
-
-# pred_probs[i][j] = probability that examples[i].prompt is classified as
-# examples[i].completions[j]
-print([example_pred_probs.round(2)
-       for example_pred_probs in pred_probs])
-# [array([0.7, 0.3]),
-#  array([0.03, 0.97, 0.  ])]
-
-# for each example, which completion is most likely?
-pred_class_idxs = [np.argmax(example_pred_probs)
-                   for example_pred_probs in pred_probs]
-print([example.completions[pred_class_idx]
-       for example, pred_class_idx in zip(examples, pred_class_idxs)])
-# ['Clarice Starling',
-#  'Kevin Conroy']
-```
-</details>
-
-More examples are linked [here in the
-documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
-
-See [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-for a demonstration of a slightly harder classification task.
-
-
-## Documentation
-
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
-
-
-## Setup
-
-If you intend on using OpenAI models, [sign up for the OpenAI API
-here](https://platform.openai.com/signup), and then set the environment variable
-`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
-others. But using them will cost ya 💰!
-
-Install with `pip`:
-
-```
-python -m pip install cappr
-```
-
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
-
-```
-python -m pip install cappr[hf]
-```
-</details>
-
-<details>
-<summary>(Optional) Set up to run demos</summary>
-
-```
-python -m pip install cappr[demos]
-```
-</details>
-
-
-## Motivation
-
-Create a more usable zero-shot text classification interface than
-[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
-
-<details>
-<summary>Short</summary>
-
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
-
-In CAPPr, your job starts and stops at writing up your classification task as a
-`{prompt}{end_of_prompt}{completion}` string.
-</details>
-
-<details>
-<summary>Long</summary>
-
-Please see [this page of the
-documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
-
-</details>
-
-<details>
-<summary>Unstudied</summary>
-
-I'm curious to see how much easier estimation/discrimination is than generation.
-In [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb),
-CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
-accurate.
-
-</details>
-
-<details>
-<summary>Honest</summary>
-
-Keep myself busy
-
-</details>
-
-
-## Results
-
-<details>
-<summary>
-Statistical performance
-</summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
-
-  * [`demos/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/copa.ipynb)
-  * [`demos/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb)
-</details>
-
-
-<details>
-<summary>
-Computational performance
-</summary>
-
-One concern was that CAPPr requires as many `model()` calls as there are classes. But in
-the CAPPr scheme, we can simply cache each attention block's keys and values for the
-prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
-code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
-the implementation. Note that this caching is not implemented for OpenAI models, as I
-can't control their backend. **This means that when running `cappr.openai` functions,
-you'll be on the *cappr (slow)* line** :-(
-
-![](/docs/source/_static/scaling_classes/batch_size_32.png)
-
-*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
-choices to simulate multi-class classification tasks. [GPT-2
-(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
-
-See the [`demos/computational_analysis.ipynb`
-notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
-
-</details>
-
-
-## Related work
-
-While [benchmarking this
-method](https://github.com/kddubey/cappr/blob/main/demos/wsc.ipynb) on the Winograd
-Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847) is very
-similar:
-
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
-
-[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
-probabilities to do prompt-completion classification, but these probabilities are
-assumed to come from masked language models like BERT.
-
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
-
-
-## Contributing
-
-TODO
-
-
-## Testing
-
-### Setup
-
-1. Clone the repo
-
-   ```
-   git clone https://github.com/kddubey/cappr.git
-   ```
-
-2. Create a new Python 3.8+ environment
-
-3. Install this package in editable mode, along with development requirements
-
-   ```
-   python -m pip install -e .[dev]
-   ```
-
-### Run tests
-
-```
-pytest
-```
-
-Dumping VS code extensions for development:
-  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
-  Use the numpy format.
-  * [Set Python formatting to
-    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
-  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
-  * [TOML Language
-    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
-
-
-## Todo
-
-(**) = I'm currently working on this or will work on it really soon
-
-<details>
-<summary>Code</summary>
-
-- [ ] Testing
-  - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
-  - [ ] Test input checks
-- [x] Small CPU speed-ups
-  - [x] For constant-completions input, vectorize `agg_log_probs`
-  - [x] For `examples` input, if # completions per prompt is constant, vectorize
-  `posterior_prob`
-- [ ] Add getLogger, basic logging
-- [ ] Make progress bars optional, since inference often isn't batched
-- [ ] Factor out input checks (on prompts and completions)
-- [x] De-automate overzealous auto-docstring stuff :-(
-- [ ] HuggingFace `transformers.AutoModelForCausalLM`
-  - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
-    - [ ] Get to the bottom of why it's slower w/o batching
-  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
-  think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
-  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
-  - [ ] Support [Inference
-    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
-  - [ ] Support priming, as in: cache it
-- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
-- [ ] Allow for multi-label classification
-  - [ ] Pass `normalize` as an argument to predict_proba functions
-  - [ ] For `huggingface`, add note that you'll get faster results by passing all
-  labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
-- [ ] Fill in missing or non-numpy docstrings
-</details>
-
-<details>
-<summary>Research</summary>
-
-Evaluate on more datasets, and understand its relative advantages and disadvantages vs
-other classification methods.
-
-- [ ] RAFT benchmark (**)
-- [ ] Create a user guide, build a table of results comparing competing approaches on
-statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
-  - [ ] Process inputs 1-by-1
-- [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
-- [ ] Calibration
-  - [ ] Is the prior actually effective? Downsample and see
-  - [ ] curves
-- [ ] Compare against few-shot embeddings
-- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
-  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
-  - [ ] Again, compare against sampling
-- [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
-</details>
+Metadata-Version: 2.1
+Name: cappr
+Version: 0.2.2
+Summary: Zero-shot text classification using autoregressive language models.
+Home-page: https://github.com/kddubey/cappr/
+Author-email: kushdubey63@gmail.com
+License: Apache License 2.0
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: hf
+Provides-Extra: demos
+Provides-Extra: dev
+License-File: LICENSE
+
+# CAPPr: zero-shot text classification using autoregressive language models
+
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
+[![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI - Package Version](https://img.shields.io/pypi/v/cappr?logo=pypi&style=flat&color=orange)](https://pypi.org/project/cappr/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+Perform zero-shot text classification by estimating the probability that an inputted
+completion comes after an inputted prompt. Hence the name:
+
+> **C**ompletion<br>
+  **A**fter<br>
+  **P**rompt<br>
+  **Pr**obability<br>
+
+The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+
+## Usage
+
+<details>
+<summary>Use a model from the OpenAI API</summary>
+
+Specifically, this model must be compatible with the
+[/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+endpoint.
+
+Let's classify
+[this sentiment example](https://platform.openai.com/docs/guides/completion/classification)
+from the OpenAI text completion docs.
+
+```python
+from cappr.openai.classify import predict
+
+tweet = 'I loved the new Batman movie!'
+prompt = f'Tweet: {tweet}\nSentiment:'
+
+class_names = ('positive', 'neutral', 'negative')
+# optional: let's supply a prior distribution over the classes
+prior       = (   1/8    ,    1/8   ,     3/4   )
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='text-ada-001',
+                prior=prior)
+preds
+# ['positive']
+```
+</details>
+
+<details>
+<summary>Use a model from the HuggingFace model hub</summary>
+
+Specifically, this model must be able to be loaded using
+`transformers.AutoModelForCausalLM.from_pretrained(model)`.
+
+Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+
+```python
+from cappr.huggingface.classify import predict
+
+prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
+
+class_names = ('Mercury', 'Earth')
+prior = None  # uniform prior
+
+preds = predict(prompts=[prompt],
+                completions=class_names,
+                model='gpt2',
+                prior=prior)
+preds
+# ['Mercury']
+```
+</details>
+
+<details>
+<summary>Run in batches</summary>
+
+Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
+instead of the class.
+
+```python
+from cappr.huggingface.classify import predict_proba
+
+prompts = [
+    'Stephen Curry is a',
+    'Martina Navratilova was a',
+    "Dexter, from the TV Series Dexter's Laboratory, is a",
+    'LeBron James is a',    
+]
+
+# each of the prompts could be completed with one of these:
+class_names = (
+    'basketball player',
+    'tennis player',
+    'scientist'
+)
+
+prior = (
+    1/6,  # few
+    1/6,  # few
+    2/3   # there are more
+)
+
+pred_probs = predict_proba(prompts=prompts,
+                           completions=class_names,
+                           model='gpt2',
+                           batch_size=32,  # whatever fits on your CPU/GPU
+                           prior=prior)
+
+# pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
+print(pred_probs.round(1))
+# [[0.5 0.3 0.2]
+#  [0.3 0.6 0.2]
+#  [0.1 0.1 0.8]
+#  [0.8 0.2 0. ]]
+
+# for each prompt, which completion is most likely?
+pred_class_idxs = pred_probs.argmax(axis=1)
+print([class_names[pred_class_idx] for pred_class_idx in pred_class_idxs])
+# ['basketball player',
+#  'tennis player',
+#  'scientist',
+#  'basketball player']
+```
+</details>
+
+<details>
+<summary>Run in batches, where each prompt has a different set of possible completions
+</summary>
+
+Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
+instantiated model and tokenizer instead of its name. That way, the model isn't
+re-loaded every time you wanna use it.
+
+```python
+import numpy as np
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from cappr import Example
+from cappr.huggingface.classify import predict_proba_examples
+
+examples = [
+    Example(prompt='Jodie Foster played',
+            completions=('Clarice Starling', 'Trinity in The Matrix')),
+    Example(prompt='Batman, from Batman: The Animated Series, was played by',
+            completions=('Pete Holmes', 'Kevin Conroy', 'Spongebob!'),
+            prior=      (     1/3      ,      2/3     ,      0      ))
+]
+
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+pred_probs = predict_proba_examples(examples,
+                                    model_and_tokenizer=(model, tokenizer))
+
+# pred_probs[i][j] = probability that examples[i].prompt is classified as
+# examples[i].completions[j]
+print([example_pred_probs.round(2)
+       for example_pred_probs in pred_probs])
+# [array([0.7, 0.3]),
+#  array([0.03, 0.97, 0.  ])]
+
+# for each example, which completion is most likely?
+pred_class_idxs = [np.argmax(example_pred_probs)
+                   for example_pred_probs in pred_probs]
+print([example.completions[pred_class_idx]
+       for example, pred_class_idx in zip(examples, pred_class_idxs)])
+# ['Clarice Starling',
+#  'Kevin Conroy']
+```
+</details>
+
+More examples are linked [here in the
+documentation](https://cappr.readthedocs.io/en/latest/5_examples.html).
+
+See
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+for a demonstration of a slightly harder classification task.
+
+
+## Documentation
+
+https://cappr.readthedocs.io/en/latest/
+
+Please let me know if you find the writing too dense. The main motivation behind this
+project is simplicity :-)
+
+
+## Setup
+
+If you intend on using OpenAI models, [sign up for the OpenAI API
+here](https://platform.openai.com/signup), and then set the environment variable
+`OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
+others. But using them will cost ya 💰!
+
+Install with `pip`:
+
+```
+python -m pip install cappr
+```
+
+<details>
+<summary>(Optional) Install requirements for HuggingFace models</summary>
+
+```
+python -m pip install cappr[hf]
+```
+</details>
+
+<details>
+<summary>(Optional) Set up to run demos</summary>
+
+```
+python -m pip install cappr[demos]
+```
+</details>
+
+
+## Motivation
+
+Create a more usable zero-shot text classification interface than
+[classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
+
+<details>
+<summary>Short</summary>
+
+In CVS, your job is to write up your classification task in a `prompt` string, and then
+write custom code to post-process arbitrary `completion`/output strings.
+
+In CAPPr, your job starts and stops at writing up your classification task as a
+`{prompt}{end_of_prompt}{completion}` string.
+</details>
+
+<details>
+<summary>Long</summary>
+
+Please see [this page of the
+documentation](https://cappr.readthedocs.io/en/latest/2_motivation.html).
+
+</details>
+
+<details>
+<summary>Unstudied</summary>
+
+I'm curious to see how much easier estimation/discrimination is than generation. In
+[`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb),
+CVS using OpenAI's `text-curie-001` is less than 50% accurate, while CAPPr is 80%
+accurate.
+
+</details>
+
+<details>
+<summary>Honest</summary>
+
+Keep myself busy
+
+</details>
+
+
+## Results
+
+<details>
+<summary>
+Statistical performance
+</summary>
+Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
+I need to run it on more ofc. Will update
+
+  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
+  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+</details>
+
+
+<details>
+<summary>
+Computational performance
+</summary>
+
+One concern was that CAPPr requires as many `model()` calls as there are classes. But in
+the CAPPr scheme, we can simply cache each attention block's keys and values for the
+prompts. This feature is already supported by `AutoModelForCausalLM`s. See [this
+code](https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py) for
+the implementation. Note that this caching is not implemented for OpenAI models, as I
+can't control their backend. **This means that when running `cappr.openai` functions,
+you'll be on the *cappr (slow)* line** :-(
+
+![](/docs/source/_static/scaling_classes/batch_size_32.png)
+
+*Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
+choices to simulate multi-class classification tasks. [GPT-2
+(small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
+Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
+processed in batches of size 32. Each point in the graph is a median of 5 runs. For
+classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
+which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
+COPA (and other multiple-choice style prompts), that may result in lower zero-shot
+accuracy, as most of the sampled choices come after the first token.*
+
+See the [`demos/computational_analysis.ipynb`
+notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
+
+</details>
+
+
+## Related work
+
+While [benchmarking this
+method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
+Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
+is very similar:
+
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+
+[PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
+probabilities to do prompt-completion classification, but these probabilities are
+assumed to come from masked language models like BERT.
+
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+
+
+## Contributing
+
+TODO
+
+
+## Testing
+
+### Setup
+
+1. Clone the repo
+
+   ```
+   git clone https://github.com/kddubey/cappr.git
+   ```
+
+2. Create a new Python 3.8+ environment
+
+3. Install this package in editable mode, along with development requirements
+
+   ```
+   python -m pip install -e .[dev]
+   ```
+
+### Run tests
+
+```
+pytest
+```
+
+Dumping VS code extensions for development:
+  * [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring).
+  Use the numpy format.
+  * [Set Python formatting to
+    `black`](https://dev.to/adamlombard/how-to-use-the-black-python-code-formatter-in-vscode-3lo0).
+  * [Rewrap](https://stkb.github.io/Rewrap/). Enable Auto Wrap.
+  * [TOML Language
+    Support](https://marketplace.visualstudio.com/items?itemName=be5invis.toml)
+
+
+## Todo
+
+(**) = I'm currently working on this or will work on it really soon
+
+<details>
+<summary>Code</summary>
+
+- [ ] Testing
+  - [ ] Increase test cases
+  - [ ] Some more standardization b/t openai and huggingface tests
+  - [x] Add code coverage badge to look cool
+  - [ ] Test input checks
+- [x] Small CPU speed-ups
+  - [x] For constant-completions input, vectorize `agg_log_probs`
+  - [x] For `examples` input, if # completions per prompt is constant, vectorize
+  `posterior_prob`
+- [ ] Make progress bars optional, since inference often isn't batched
+- [ ] Factor out input checks (on prompts and completions)
+- [x] De-automate overzealous auto-docstring stuff :-(
+- [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [x] Optimize backend to enable greater scaling wrt # completions/classes
+  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
+  batching
+    - [ ] Get to the bottom of why it's slower w/o batching
+  - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
+  think
+  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
+  - [ ] Consider batchifying the completions again, since they technically don't go in
+  batches of `batch_size`; the actual batch size is the sum of the number of completions
+  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
+  are usually half as long. But it should be configurable at the very least.
+  - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
+  - [ ] Support [Inference
+    Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
+  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support priming, as in: cache it
+- [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
+- [ ] Allow for multi-label classification
+  - [ ] Pass `normalize` as an argument to predict_proba functions
+  - [ ] For `huggingface`, add note that you'll get faster results by passing all
+  labels at once (assuming prompt is identical for each label)
+- [ ] Create a notebook template
+- [ ] Fill in missing or non-numpy docstrings
+</details>
+
+<details>
+<summary>Research</summary>
+
+Evaluate on more datasets, and understand its relative advantages and disadvantages vs
+other classification methods.
+
+- [ ] RAFT benchmark (**)
+  - [x] Zero-shot training scores
+  - [ ] Submit zero-shot test predictions
+  - [ ] Few-shot (priming) training scores
+  - [ ] Submit few-shot test predictions
+- [ ] Create a user guide, build a table of results comparing competing approaches on
+statistical performance, cost, and computation
+- [ ] Make a computational comparison to sampling (**)
+  - [x] Assume I have full freedom to decide how inference works. Demo w/
+  GPT-2. Process inputs in batches.
+  - [ ] Process inputs 1-by-1
+- [ ] More SuperGLUE tasks?
+  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
+- [ ] Calibration
+  - [ ] Is the prior actually effective? Downsample and see
+  - [ ] curves
+- [ ] Compare against few-shot embeddings
+- [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
+  - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
+  - [ ] Again, compare against sampling
+- [ ] Evaluate a bigger model like GPT-J
+- [ ] Evaluate different aggregation functions. Currently taking mean, but
+there was no good theory for that
+- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
+manipulating position IDs isn't sufficient (I think).
+</details>
```

