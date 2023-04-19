# Comparing `tmp/aac-metrics-0.4.1.tar.gz` & `tmp/aac-metrics-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aac-metrics-0.4.1.tar", last modified: Thu Apr 13 14:21:04 2023, max compression
+gzip compressed data, was "aac-metrics-0.4.2.tar", last modified: Wed Apr 19 15:14:38 2023, max compression
```

## Comparing `aac-metrics-0.4.1.tar` & `aac-metrics-0.4.2.tar`

### file list

```diff
@@ -1,102 +1,106 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.598118 aac-metrics-0.4.1/.github/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/.github/workflows/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1891 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/.github/workflows/python-package-pip.yaml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.1/LICENCE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      135 2022-10-31 09:45:25.000000 aac-metrics-0.4.1/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11098 2023-04-13 14:18:42.000000 aac-metrics-0.4.1/README.md
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/examples/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/examples/example_1.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2022-09-30 12:10:31.000000 aac-metrics-0.4.1/examples/example_2.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/install_spice.sh
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.598118 aac-metrics-0.4.1/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/src/aac_metrics/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-13 14:18:42.000000 aac-metrics-0.4.1/src/aac_metrics/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/src/aac_metrics/classes/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.1/src/aac_metrics/classes/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7654 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/evaluate.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/src/aac_metrics/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/mult_cands.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/src/aac_metrics/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2973 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/utils/checks.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.1/src/aac_metrics/utils/collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.1/src/aac_metrics/utils/imports.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/utils/tokenization.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/src/aac_metrics.egg-info/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4051 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/tests/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/eval_metrics.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_bleu_tchmet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4279 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_compare_cet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3906 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_compare_fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_pickable.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1024 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.317355 aac-metrics-0.4.2/.github/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/.github/workflows/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1958 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/.github/workflows/python-package-pip.yaml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.2/LICENCE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      147 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12241 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11103 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/README.md
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/data/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/data/example_1.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/data/example_2.csv
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/examples/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/examples/example_1.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/examples/example_2.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/install_spice.sh
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/classes/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.2/src/aac_metrics/classes/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7642 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/evaluate.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/mult_cands.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/info.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1559 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/install_spice.sh
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/src/aac_metrics/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3807 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/utils/checks.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.2/src/aac_metrics/utils/collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.2/src/aac_metrics/utils/imports.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/utils/tokenization.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics.egg-info/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12241 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4122 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/tests/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/eval_metrics.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/tests/test_bleu_tchmet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4271 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_compare_cet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3886 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_compare_fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/tests/test_pickable.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1763 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_utils.py
```

### Comparing `aac-metrics-0.4.1/.github/workflows/python-package-pip.yaml` & `aac-metrics-0.4.2/.github/workflows/python-package-pip.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.9"]
         java-version: ["11"]
 
     steps:
     # --- INSTALLATIONS ---
-
     - name: Checkout repository
       uses: actions/checkout@v2
       with:
         submodules: recursive
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
@@ -37,22 +36,22 @@
       with:
         distribution: 'temurin'
         java-version: ${{ matrix.java-version }}
         java-package: jre
 
     - name: Install package
       run: |
-        python -m pip install -e .[dev]
+        python -m pip install "aac-metrics[dev] @ git+https://github.com/Labbeti/aac-metrics@dev"
   
     - name: Load cache of external code and data
       uses: actions/cache@master
       id: cache_external
       with:
         path: /home/runner/.cache/aac-metrics/*
-        key: ${{ runner.os }}-${{ hashFiles('install_spice.sh') }}
+        key: ${{ runner.os }}-${{ hashFiles('src/aac_metrics/download.py') }}
         restore-keys: |
           ${{ runner.os }}-
 
     # --- TESTS ---
     - name: Lint with flake8
       run: |
         python -m flake8 --config .flake8 --exit-zero --show-source --statistics src
@@ -63,15 +62,15 @@
 
     - name: Print install info
       run: |
         aac-metrics-info
 
     - name: Print Java version
       run: |
-        java --version
+        java -version
   
     - name: Install external code if needed
       if: steps.cache_external.outputs.cache-hit != 'true'
       run: |
         aac-metrics-download
   
     - name: Test with pytest
```

### Comparing `aac-metrics-0.4.1/LICENCE` & `aac-metrics-0.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/PKG-INFO` & `aac-metrics-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.1
+Version: 0.4.2
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/
 Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
 Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
@@ -58,15 +58,15 @@
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
@@ -142,15 +142,15 @@
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
-sentence-transformers>=2.2.2
+sentence-transformers >= 2.2.2
 ```
 
 ### External requirements
 - `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
@@ -239,15 +239,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.1},
+    version = {0.4.2},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.1 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.2 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
 repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
@@ -22,16 +22,16 @@
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
 [[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
 sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
 FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
 install aac-metrics ``` Download the external code and models needed for
-METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
-SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE
+and SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
 `$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
 metrics The full evaluation pipeline to compute AAC metrics can be done with
 `aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
 candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
@@ -76,15 +76,15 @@
 **Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
 audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
 Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
 `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 ## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
-numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
+numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers >= 2.2.2 ```
 ### External requirements - `java` **>= 1.8 and <= 1.11** is required to
 compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
@@ -139,9 +139,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.1/README.md` & `aac-metrics-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
@@ -118,15 +118,15 @@
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
-sentence-transformers>=2.2.2
+sentence-transformers >= 2.2.2
 ```
 
 ### External requirements
 - `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
@@ -215,15 +215,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.1},
+    version = {0.4.2},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
 [[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
 sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
 FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
 install aac-metrics ``` Download the external code and models needed for
-METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
-SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE
+and SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
 `$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
 metrics The full evaluation pipeline to compute AAC metrics can be done with
 `aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
 candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
@@ -60,15 +60,15 @@
 **Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
 audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
 Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
 `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 ## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
-numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
+numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers >= 2.2.2 ```
 ### External requirements - `java` **>= 1.8 and <= 1.11** is required to
 compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
@@ -123,9 +123,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.1/examples/example_1.csv` & `aac-metrics-0.4.2/data/example_1.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/examples/example_2.csv` & `aac-metrics-0.4.2/data/example_2.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/install_spice.sh` & `aac-metrics-0.4.2/install_spice.sh`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/pyproject.toml` & `aac-metrics-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/__init__.py` & `aac-metrics-0.4.2/src/aac_metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __name__ = "aac-metrics"
 __author__ = "Etienne Labbé (Labbeti)"
 __author_email__ = "labbeti.pub@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "Etienne Labbé (Labbeti)"
 __status__ = "Development"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 from .classes.base import AACMetric
 from .classes.bleu import BLEU
 from .classes.cider_d import CIDErD
 from .classes.evaluate import AACEvaluate, _get_metric_factory_classes
 from .classes.fense import FENSE
```

### Comparing `aac-metrics-0.4.1/src/aac_metrics/__main__.py` & `aac-metrics-0.4.2/src/aac_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/__init__.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/base.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/base.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/bleu.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/cider_d.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/evaluate.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/fense.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/fluerr.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/fluerr.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/meteor.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/rouge_l.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/sbert_sim.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/sbert_sim.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/spice.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/spider.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/spider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/spider_fl.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/spider_fl.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/classes/spider_max.py` & `aac-metrics-0.4.2/src/aac_metrics/classes/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/download.py` & `aac-metrics-0.4.2/src/aac_metrics/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         # Download JAR files for SPICE metric
         spice_jar_dpath = osp.join(cache_path, osp.dirname(FNAME_SPICE_JAR))
         spice_cache_path = osp.join(cache_path, DNAME_SPICE_CACHE)
 
         os.makedirs(spice_jar_dpath, exist_ok=True)
         os.makedirs(spice_cache_path, exist_ok=True)
 
-        script_path = osp.join(osp.dirname(__file__), "..", "..", "install_spice.sh")
+        script_path = osp.join(osp.dirname(__file__), "install_spice.sh")
         if not osp.isfile(script_path):
             raise FileNotFoundError(
                 f"Cannot find script '{osp.basename(script_path)}'."
             )
 
         if verbose >= 1:
             pylog.info(
@@ -147,15 +147,15 @@
             )
         except (CalledProcessError, PermissionError) as err:
             pylog.error(err)
 
     if fense:
         # Download models files for FENSE metric
         if verbose >= 1:
-            pylog.info("Downloading sBert and Bert error detector for FENSE metric...")
+            pylog.info("Downloading SBERT and BERT error detector for FENSE metric...")
         _ = FENSE(device="cpu")
 
 
 def _get_main_download_args() -> Namespace:
     parser = ArgumentParser(
         description="Download models and external code to evaluate captions."
     )
```

### Comparing `aac-metrics-0.4.1/src/aac_metrics/evaluate.py` & `aac-metrics-0.4.2/src/aac_metrics/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/__init__.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/bleu.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/cider_d.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/evaluate.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/fense.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/fluerr.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/fluerr.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/meteor.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/mult_cands.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/mult_cands.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/rouge_l.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/sbert_sim.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/sbert_sim.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/spice.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/spider.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/spider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/spider_fl.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/spider_fl.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/functional/spider_max.py` & `aac-metrics-0.4.2/src/aac_metrics/functional/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/info.py` & `aac-metrics-0.4.2/src/aac_metrics/info.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/utils/checks.py` & `aac-metrics-0.4.2/src/aac_metrics/utils/checks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
+import re
 import subprocess
 
+from dataclasses import dataclass
 from functools import cache
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Any, Union
 
 
 pylog = logging.getLogger(__name__)
 
+VERSION_PATTERN = r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+).*"
 MIN_JAVA_MAJOR_VERSION = 8
 MAX_JAVA_MAJOR_VERSION = 11
 
 
 def check_metric_inputs(
     candidates: Any,
     mult_references: Any,
@@ -37,50 +40,69 @@
     if not at_least_1_ref_per_cand:
         raise ValueError(
             "Invalid number of references per candidate. (found at least 1 empty list of references)"
         )
 
 
 def check_java_path(java_path: Union[str, Path]) -> bool:
+    version = _get_java_version(str(java_path))
+    valid = _check_java_version(version, MIN_JAVA_MAJOR_VERSION, MAX_JAVA_MAJOR_VERSION)
+    if not valid:
+        pylog.error(
+            f"Using Java version {version} is not officially supported by aac-metrics package and will not work for METEOR and SPICE metrics."
+            f"(expected major version in range [{MIN_JAVA_MAJOR_VERSION}, {MAX_JAVA_MAJOR_VERSION}])"
+        )
+    return valid
+
+
+def _get_java_version(java_path: str) -> str:
     """Returns True if the java path is valid."""
-    if not isinstance(java_path, (str, Path)):
-        return False
+    if not isinstance(java_path, str):
+        raise TypeError(f"Invalid argument type {type(java_path)=}. (expected str)")
 
-    output = ""
+    output = "INVALID"
     try:
         output = subprocess.check_output(
-            [str(java_path), "--version"],
+            [java_path, "-version"],
+            stderr=subprocess.STDOUT,
         )
         output = output.decode().strip()
-        version = output.split("\n")[0]
-        major_version = int(version.split(" ")[1].split(".")[0])
+        version = output.split(" ")[2][1:-1]
 
     except (
         CalledProcessError,
         PermissionError,
         FileNotFoundError,
     ) as err:
-        pylog.error(f"Invalid java path. (from {java_path=} and found error={err})")
-        return False
+        raise ValueError(f"Invalid java path. (from {java_path=} and found {err=})")
 
-    except (
-        IndexError,
-        ValueError,
-    ) as err:
-        pylog.error(f"Invalid java version. (found {output=} and {err=})")
-        return False
+    except IndexError as err:
+        raise ValueError(
+            f"Invalid java version. (from {java_path=} and found {output=} and {err=})"
+        )
 
-    if not (MIN_JAVA_MAJOR_VERSION <= major_version <= MAX_JAVA_MAJOR_VERSION):
-        pylog.error(
-            f"Using Java version {version} is not officially supported by aac-metrics package and could not work for METEOR and SPICE metrics."
-            f"(found {major_version=} but expected in [{MIN_JAVA_MAJOR_VERSION}, {MAX_JAVA_MAJOR_VERSION}])"
+    return version
+
+
+def _check_java_version(version: str, min_major: int, max_major: int) -> bool:
+    result = re.match(VERSION_PATTERN, version)
+    if result is None:
+        raise ValueError(
+            f"Invalid Java version {version=}. (expected version with pattern={VERSION_PATTERN})"
         )
-        return False
 
-    return True
+    major_version = int(result["major"])
+    minor_version = int(result["minor"])
+
+    if (
+        major_version == 1 and minor_version <= 8
+    ):  # java <= 8 use versioning "1.MAJOR.MINOR" and > 8 use "MAJOR.MINOR.PATCH"
+        major_version = minor_version
+
+    return min_major <= major_version <= max_major
 
 
 def is_mono_sents(sents: Any) -> bool:
     """Returns True if input is list[str]."""
     return isinstance(sents, list) and all(isinstance(sent, str) for sent in sents)
```

### Comparing `aac-metrics-0.4.1/src/aac_metrics/utils/collections.py` & `aac-metrics-0.4.2/src/aac_metrics/utils/collections.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics/utils/tokenization.py` & `aac-metrics-0.4.2/src/aac_metrics/utils/tokenization.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/src/aac_metrics.egg-info/PKG-INFO` & `aac-metrics-0.4.2/src/aac_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.1
+Version: 0.4.2
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/
 Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
 Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
@@ -58,15 +58,15 @@
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
@@ -142,15 +142,15 @@
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
-sentence-transformers>=2.2.2
+sentence-transformers >= 2.2.2
 ```
 
 ### External requirements
 - `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
@@ -239,15 +239,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.1},
+    version = {0.4.2},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.1 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.2 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
 repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
@@ -22,16 +22,16 @@
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
 [[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
 sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
 FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
 install aac-metrics ``` Download the external code and models needed for
-METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
-SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERTSim, FluencyError, FENSE
+and SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
 `$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
 metrics The full evaluation pipeline to compute AAC metrics can be done with
 `aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
 candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
@@ -76,15 +76,15 @@
 **Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
 audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
 Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
 `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 ## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
-numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
+numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers >= 2.2.2 ```
 ### External requirements - `java` **>= 1.8 and <= 1.11** is required to
 compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
@@ -139,9 +139,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.1/src/aac_metrics.egg-info/SOURCES.txt` & `aac-metrics-0.4.2/src/aac_metrics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,24 @@
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
 ./tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
 ./tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
+data/example_1.csv
+data/example_2.csv
 examples/example_1.csv
 examples/example_2.csv
 src/aac_metrics/__init__.py
 src/aac_metrics/__main__.py
 src/aac_metrics/download.py
 src/aac_metrics/evaluate.py
 src/aac_metrics/info.py
+src/aac_metrics/install_spice.sh
 src/aac_metrics.egg-info/PKG-INFO
 src/aac_metrics.egg-info/SOURCES.txt
 src/aac_metrics.egg-info/dependency_links.txt
 src/aac_metrics.egg-info/entry_points.txt
 src/aac_metrics.egg-info/requires.txt
 src/aac_metrics.egg-info/top_level.txt
 src/aac_metrics/classes/__init__.py
```

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/caption-evaluation-tools/eval_metrics.py` & `aac-metrics-0.4.2/tests/caption-evaluation-tools/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/test_bleu_tchmet.py` & `aac-metrics-0.4.2/tests/test_bleu_tchmet.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.1/tests/test_compare_cet.py` & `aac-metrics-0.4.2/tests/test_compare_cet.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 
     # Tests methods
     def test_example_0(self) -> None:
         cands, mrefs = self._get_example_0()
         self._test_with_example(cands, mrefs)
 
     def test_example_1(self) -> None:
-        fpath = Path(__file__).parent.parent.joinpath("examples", "example_1.csv")
+        fpath = Path(__file__).parent.parent.joinpath("data", "example_1.csv")
         cands, mrefs = load_csv_file(fpath)
         self._test_with_example(cands, mrefs)
 
     def test_example_2(self) -> None:
-        fpath = Path(__file__).parent.parent.joinpath("examples", "example_2.csv")
+        fpath = Path(__file__).parent.parent.joinpath("data", "example_2.csv")
         cands, mrefs = load_csv_file(fpath)
         self._test_with_example(cands, mrefs)
 
     # Others methods
     def _get_example_0(self) -> tuple[list[str], list[list[str]]]:
         cands = [
             "a man is speaking",
```

### Comparing `aac-metrics-0.4.1/tests/test_compare_fense.py` & `aac-metrics-0.4.2/tests/test_compare_fense.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,31 +50,31 @@
         fense_path = osp.join(osp.dirname(__file__), "fense")
         sys.path.append(fense_path)
         fense_module = importlib.import_module("fense.evaluator")
         return fense_module.Evaluator
 
     # Tests methods
     def test_example_1_fense(self) -> None:
-        fpath = osp.join(osp.dirname(__file__), "..", "examples", "example_1.csv")
+        fpath = osp.join(osp.dirname(__file__), "..", "data", "example_1.csv")
         self._test_with_original_fense(fpath)
 
     def test_example_1_sbert_sim(self) -> None:
-        fpath = osp.join(osp.dirname(__file__), "..", "examples", "example_1.csv")
+        fpath = osp.join(osp.dirname(__file__), "..", "data", "example_1.csv")
         self._test_with_original_sbert_sim(fpath)
 
     def test_example_2_fense(self) -> None:
-        fpath = osp.join(osp.dirname(__file__), "..", "examples", "example_2.csv")
+        fpath = osp.join(osp.dirname(__file__), "..", "data", "example_2.csv")
         self._test_with_original_fense(fpath)
 
     def test_example_2_sbert_sim(self) -> None:
-        fpath = osp.join(osp.dirname(__file__), "..", "examples", "example_2.csv")
+        fpath = osp.join(osp.dirname(__file__), "..", "data", "example_2.csv")
         self._test_with_original_sbert_sim(fpath)
 
     def test_output_size(self) -> None:
-        fpath = osp.join(osp.dirname(__file__), "..", "examples", "example_1.csv")
+        fpath = osp.join(osp.dirname(__file__), "..", "data", "example_1.csv")
         cands, mrefs = load_csv_file(fpath)
 
         self.new_fense._return_all_scores = True
         corpus_scores, sents_scores = self.new_fense(cands, mrefs)
         self.new_fense._return_all_scores = False
 
         for name, score in corpus_scores.items():
```

### Comparing `aac-metrics-0.4.1/tests/test_pickable.py` & `aac-metrics-0.4.2/tests/test_pickable.py`

 * *Files identical despite different names*

