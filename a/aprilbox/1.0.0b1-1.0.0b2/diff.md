# Comparing `tmp/aprilbox-1.0.0b1.tar.gz` & `tmp/aprilbox-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprilbox-1.0.0b1.tar", last modified: Wed Apr 19 10:07:31 2023, max compression
+gzip compressed data, was "aprilbox-1.0.0b2.tar", last modified: Wed Apr 19 10:11:51 2023, max compression
```

## Comparing `aprilbox-1.0.0b1.tar` & `aprilbox-1.0.0b2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1587 2022-12-22 10:24:41.000000 aprilbox-1.0.0b1/LICENSE.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/PKG-INFO
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      706 2023-04-19 06:14:13.000000 aprilbox-1.0.0b1/README.md
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      526 2023-04-19 06:33:58.000000 aprilbox-1.0.0b1/aprilbox/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      314 2023-04-19 06:34:21.000000 aprilbox-1.0.0b1/aprilbox/ai/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      505 2023-04-19 06:17:32.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/activation/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      320 2023-04-19 09:29:33.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/activation/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2991 2023-04-19 09:29:38.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/activation/acon.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2302 2023-04-19 09:29:44.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/activation/smu.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      424 2023-04-10 06:04:03.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7552 2023-04-19 09:30:19.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/lstm.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3084 2023-04-19 09:30:19.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/resnet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4201 2023-04-19 09:30:19.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/unet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    10459 2023-04-19 09:30:19.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/vit.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      328 2023-04-10 06:04:30.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    16473 2023-04-19 09:30:19.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/scinet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1509 2023-04-19 07:01:02.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/simvp.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      497 2023-04-19 09:30:59.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      426 2023-04-19 09:30:27.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1558 2023-04-19 09:30:51.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/lka.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7114 2023-04-19 09:30:50.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/psa.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      852 2023-03-31 08:08:57.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/simple.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3763 2023-04-19 09:30:56.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/split.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1236 2023-04-10 06:05:56.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/cca.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3328 2023-04-19 06:44:54.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/conv.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4526 2023-04-19 06:45:16.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/inception.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4186 2023-04-19 09:31:05.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/block/memory.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      573 2023-04-19 09:31:10.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1172 2023-04-19 09:31:21.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/dice.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4899 2023-04-19 07:02:27.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/efl.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2683 2023-04-19 07:28:33.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/loss.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1506 2023-04-10 05:47:56.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/rmse.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3807 2023-04-17 03:00:51.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/seesaw.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3762 2023-04-19 09:31:21.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/ssim.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1386 2023-04-10 05:58:58.000000 aprilbox-1.0.0b1/aprilbox/ai/dl/loss/ts.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/ml/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      231 2023-04-19 07:03:03.000000 aprilbox-1.0.0b1/aprilbox/ai/ml/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/ai/tools/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      240 2023-04-19 07:26:53.000000 aprilbox-1.0.0b1/aprilbox/ai/tools/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7260 2023-04-19 07:29:05.000000 aprilbox-1.0.0b1/aprilbox/ai/tools/base.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2800 2023-04-19 07:27:43.000000 aprilbox-1.0.0b1/aprilbox/ai/tools/config.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2931 2023-04-19 07:33:34.000000 aprilbox-1.0.0b1/aprilbox/ai/tools/weight.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/data/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:28:00.000000 aprilbox-1.0.0b1/aprilbox/data/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/data/met/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:27:17.000000 aprilbox-1.0.0b1/aprilbox/data/met/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2578 2023-04-19 09:24:47.000000 aprilbox-1.0.0b1/aprilbox/data/met/constant.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    11518 2023-04-19 07:45:35.000000 aprilbox-1.0.0b1/aprilbox/data/met/loader.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/data/preprocess/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      235 2023-04-19 09:27:28.000000 aprilbox-1.0.0b1/aprilbox/data/preprocess/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/eval/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      233 2023-04-19 06:34:40.000000 aprilbox-1.0.0b1/aprilbox/eval/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2379 2023-04-19 09:22:36.000000 aprilbox-1.0.0b1/aprilbox/types.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/utils/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      443 2023-04-19 06:52:00.000000 aprilbox-1.0.0b1/aprilbox/utils/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     6810 2023-04-19 06:48:01.000000 aprilbox-1.0.0b1/aprilbox/utils/interpolate.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/utils/met/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 07:36:09.000000 aprilbox-1.0.0b1/aprilbox/utils/met/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4054 2023-04-19 07:35:45.000000 aprilbox-1.0.0b1/aprilbox/utils/met/distance.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3835 2023-04-19 07:35:45.000000 aprilbox-1.0.0b1/aprilbox/utils/met/factor.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3767 2023-04-19 07:44:00.000000 aprilbox-1.0.0b1/aprilbox/utils/path.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2867 2023-04-19 09:32:01.000000 aprilbox-1.0.0b1/aprilbox/utils/pool.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox/vis/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      287 2023-04-19 06:36:23.000000 aprilbox-1.0.0b1/aprilbox/vis/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      532 2023-04-19 06:20:56.000000 aprilbox-1.0.0b1/aprilbox/vis/base.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1454 2023-04-19 06:37:27.000000 aprilbox-1.0.0b1/aprilbox/vis/precipitation.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/aprilbox.egg-info/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:07:30.000000 aprilbox-1.0.0b1/aprilbox.egg-info/PKG-INFO
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1833 2023-04-19 10:07:30.000000 aprilbox-1.0.0b1/aprilbox.egg-info/SOURCES.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        1 2023-04-19 10:07:30.000000 aprilbox-1.0.0b1/aprilbox.egg-info/dependency_links.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      138 2023-04-19 10:07:30.000000 aprilbox-1.0.0b1/aprilbox.egg-info/requires.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        9 2023-04-19 10:07:30.000000 aprilbox-1.0.0b1/aprilbox.egg-info/top_level.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      421 2023-04-19 10:07:31.000000 aprilbox-1.0.0b1/setup.cfg
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      494 2023-04-19 09:46:04.000000 aprilbox-1.0.0b1/setup.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1587 2022-12-22 10:24:41.000000 aprilbox-1.0.0b2/LICENSE.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/PKG-INFO
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      706 2023-04-19 06:14:13.000000 aprilbox-1.0.0b2/README.md
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      526 2023-04-19 06:33:58.000000 aprilbox-1.0.0b2/aprilbox/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      314 2023-04-19 06:34:21.000000 aprilbox-1.0.0b2/aprilbox/ai/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      505 2023-04-19 06:17:32.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      320 2023-04-19 09:29:33.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2991 2023-04-19 09:29:38.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/acon.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2302 2023-04-19 09:29:44.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/smu.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      424 2023-04-10 06:04:03.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7552 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/lstm.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3084 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/resnet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4201 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/unet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    10459 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/vit.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      328 2023-04-10 06:04:30.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    16473 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/scinet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1509 2023-04-19 07:01:02.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/simvp.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      497 2023-04-19 09:30:59.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      426 2023-04-19 09:30:27.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1558 2023-04-19 09:30:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/lka.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7114 2023-04-19 09:30:50.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/psa.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      852 2023-03-31 08:08:57.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/simple.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3763 2023-04-19 09:30:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/split.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1236 2023-04-10 06:05:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/cca.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3328 2023-04-19 06:44:54.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/conv.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4526 2023-04-19 06:45:16.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/inception.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4186 2023-04-19 09:31:05.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/memory.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      573 2023-04-19 09:31:10.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1172 2023-04-19 09:31:21.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/dice.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4899 2023-04-19 07:02:27.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/efl.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2683 2023-04-19 07:28:33.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/loss.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1506 2023-04-10 05:47:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/rmse.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3807 2023-04-17 03:00:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/seesaw.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3762 2023-04-19 09:31:21.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ssim.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1386 2023-04-10 05:58:58.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ts.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/ml/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      231 2023-04-19 07:03:03.000000 aprilbox-1.0.0b2/aprilbox/ai/ml/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      240 2023-04-19 07:26:53.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7260 2023-04-19 07:29:05.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/base.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2800 2023-04-19 07:27:43.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/config.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2931 2023-04-19 07:33:34.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/weight.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:28:00.000000 aprilbox-1.0.0b2/aprilbox/data/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/met/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:27:17.000000 aprilbox-1.0.0b2/aprilbox/data/met/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2578 2023-04-19 09:24:47.000000 aprilbox-1.0.0b2/aprilbox/data/met/constant.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    11518 2023-04-19 07:45:35.000000 aprilbox-1.0.0b2/aprilbox/data/met/loader.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/preprocess/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      235 2023-04-19 09:27:28.000000 aprilbox-1.0.0b2/aprilbox/data/preprocess/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/eval/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      233 2023-04-19 06:34:40.000000 aprilbox-1.0.0b2/aprilbox/eval/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2379 2023-04-19 09:22:36.000000 aprilbox-1.0.0b2/aprilbox/types.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/utils/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      443 2023-04-19 06:52:00.000000 aprilbox-1.0.0b2/aprilbox/utils/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     6810 2023-04-19 06:48:01.000000 aprilbox-1.0.0b2/aprilbox/utils/interpolate.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/utils/met/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 07:36:09.000000 aprilbox-1.0.0b2/aprilbox/utils/met/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4054 2023-04-19 07:35:45.000000 aprilbox-1.0.0b2/aprilbox/utils/met/distance.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3835 2023-04-19 07:35:45.000000 aprilbox-1.0.0b2/aprilbox/utils/met/factor.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3767 2023-04-19 07:44:00.000000 aprilbox-1.0.0b2/aprilbox/utils/path.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2867 2023-04-19 09:32:01.000000 aprilbox-1.0.0b2/aprilbox/utils/pool.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/vis/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      287 2023-04-19 06:36:23.000000 aprilbox-1.0.0b2/aprilbox/vis/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      532 2023-04-19 06:20:56.000000 aprilbox-1.0.0b2/aprilbox/vis/base.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1454 2023-04-19 06:37:27.000000 aprilbox-1.0.0b2/aprilbox/vis/precipitation.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/PKG-INFO
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1833 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        1 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      140 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/requires.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        9 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/top_level.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      423 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/setup.cfg
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      494 2023-04-19 09:46:04.000000 aprilbox-1.0.0b2/setup.py
```

### Comparing `aprilbox-1.0.0b1/LICENSE.txt` & `aprilbox-1.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/PKG-INFO` & `aprilbox-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprilbox
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Fang Linwanghao
 Author-email: fanglwh@outlook.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `aprilbox-1.0.0b1/README.md` & `aprilbox-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/__init__.py` & `aprilbox-1.0.0b2/aprilbox/__init__.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/activation/acon.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/activation/acon.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/activation/smu.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/activation/smu.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/lstm.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/lstm.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/resnet.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/unet.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/unet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/backbone/vit.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/scinet.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/scinet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/benchmark/simvp.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/simvp.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/lka.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/lka.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/psa.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/psa.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/simple.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/simple.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/attention/split.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/split.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/cca.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/cca.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/conv.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/conv.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/inception.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/inception.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/block/memory.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/block/memory.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/__init__.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/dice.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/dice.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/efl.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/efl.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/loss.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/loss.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/rmse.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/rmse.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/seesaw.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/seesaw.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/ssim.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ssim.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/dl/loss/ts.py` & `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ts.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/tools/base.py` & `aprilbox-1.0.0b2/aprilbox/ai/tools/base.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/tools/config.py` & `aprilbox-1.0.0b2/aprilbox/ai/tools/config.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/ai/tools/weight.py` & `aprilbox-1.0.0b2/aprilbox/ai/tools/weight.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/data/met/constant.py` & `aprilbox-1.0.0b2/aprilbox/data/met/constant.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/data/met/loader.py` & `aprilbox-1.0.0b2/aprilbox/data/met/loader.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/types.py` & `aprilbox-1.0.0b2/aprilbox/types.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/utils/interpolate.py` & `aprilbox-1.0.0b2/aprilbox/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/utils/met/distance.py` & `aprilbox-1.0.0b2/aprilbox/utils/met/distance.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/utils/met/factor.py` & `aprilbox-1.0.0b2/aprilbox/utils/met/factor.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/utils/path.py` & `aprilbox-1.0.0b2/aprilbox/utils/path.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/utils/pool.py` & `aprilbox-1.0.0b2/aprilbox/utils/pool.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/vis/base.py` & `aprilbox-1.0.0b2/aprilbox/vis/base.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox/vis/precipitation.py` & `aprilbox-1.0.0b2/aprilbox/vis/precipitation.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b1/aprilbox.egg-info/PKG-INFO` & `aprilbox-1.0.0b2/aprilbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprilbox
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Fang Linwanghao
 Author-email: fanglwh@outlook.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `aprilbox-1.0.0b1/aprilbox.egg-info/SOURCES.txt` & `aprilbox-1.0.0b2/aprilbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

