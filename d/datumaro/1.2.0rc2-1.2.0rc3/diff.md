# Comparing `tmp/datumaro-1.2.0rc2.tar.gz` & `tmp/datumaro-1.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.2.0rc2.tar", last modified: Mon Apr 17 05:09:49 2023, max compression
+gzip compressed data, was "datumaro-1.2.0rc3.tar", last modified: Wed Apr 19 00:50:44 2023, max compression
```

## Comparing `datumaro-1.2.0rc2.tar` & `datumaro-1.2.0rc3.tar`

### file list

```diff
@@ -1,307 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.538255 datumaro-1.2.0rc2/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.538255 datumaro-1.2.0rc2/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23475 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89324 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.546256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.546256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/synthia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    41229 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89324 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.189725 datumaro-1.2.0rc3/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.189725 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.193724 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/synthia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41240 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/setup.py
```

### Comparing `datumaro-1.2.0rc2/3rd-party.txt` & `datumaro-1.2.0rc3/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/LICENSE` & `datumaro-1.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/PKG-INFO` & `datumaro-1.2.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc2
+Version: 1.2.0rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc2/README.md` & `datumaro-1.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/__init__.py` & `datumaro-1.2.0rc3/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/capi/pybind.cpp` & `datumaro-1.2.0rc3/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/__main__.py` & `datumaro-1.2.0rc3/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/__init__.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/convert.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/detect_format.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/download.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/explain.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/filter.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/generate.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/merge.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/patch.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/diff.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/export.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/info.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/stats.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/transform.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/validate.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/commands/search.py` & `datumaro-1.2.0rc3/datumaro/cli/commands/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,18 +106,17 @@
     subset_list = []
     id_list = []
     result_path_list = []
     log.info("Most similar {} results of query in dataset".format(args.topk))
     for result in results:
         subset_list.append(result.subset)
         id_list.append(result.id)
-        result_path_list.append(result.media.path)
-        log.info(
-            "id: {} | subset: {} | path : {}".format(result.id, result.subset, result.media.path)
-        )
+        path = getattr(result.media, "path", None)
+        result_path_list.append(path)
+        log.info("id: {} | subset: {} | path : {}".format(result.id, result.subset, path))
 
     visualizer = Visualizer(dataset, figsize=(20, 20), alpha=0)
     fig = visualizer.vis_gallery(id_list, subset_list)
 
     if args.save:
         fig.canvas.draw()
         data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
```

### Comparing `datumaro-1.2.0rc2/datumaro/cli/contexts/model.py` & `datumaro-1.2.0rc3/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.2.0rc3/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/contexts/source.py` & `datumaro-1.2.0rc3/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/contexts/util.py` & `datumaro-1.2.0rc3/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/util/__init__.py` & `datumaro-1.2.0rc3/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/util/diff.py` & `datumaro-1.2.0rc3/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/cli/util/project.py` & `datumaro-1.2.0rc3/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/abstracts/merger.py` & `datumaro-1.2.0rc3/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/algorithms/rise.py` & `datumaro-1.2.0rc3/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/annotation.py` & `datumaro-1.2.0rc3/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/annotations/matcher.py` & `datumaro-1.2.0rc3/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/annotations/merger.py` & `datumaro-1.2.0rc3/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/cli_plugin.py` & `datumaro-1.2.0rc3/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/config.py` & `datumaro-1.2.0rc3/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/config_model.py` & `datumaro-1.2.0rc3/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/crypter.py` & `datumaro-1.2.0rc3/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/dataset.py` & `datumaro-1.2.0rc3/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/dataset_base.py` & `datumaro-1.2.0rc3/datumaro/components/dataset_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             "'DatasetItem.point_cloud' is deprecated and will be "
             "removed in future. Use '.media' and '.media_as()' instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         if not isinstance(self.media, PointCloud):
             return None
-        return self.media_as(PointCloud).path
+        return getattr(self.media_as(PointCloud), "path", None)
 
     # Deprecated. Provided for backward compatibility.
     @property
     def related_images(self) -> List[Image]:
         warnings.warn(
             "'DatasetItem.related_images' is deprecated and will be "
             "removed in future. Use '.media' and '.media_as()' instead.",
```

### Comparing `datumaro-1.2.0rc2/datumaro/components/dataset_item_storage.py` & `datumaro-1.2.0rc3/datumaro/components/dataset_item_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         return self.data
 
     def get_annotated_items(self):
         return sum(bool(s.annotations) for s in self._traversal_order.values())
 
     def get_datasetitem_by_path(self, path):
         for s in self._traversal_order.values():
-            if s.media.path == path:
+            if getattr(s.media, "path", None) == path:
                 return s
 
     def get_annotations(self):
         annotations_by_type = {t.name: {"count": 0} for t in AnnotationType}
         for item in self._traversal_order.values():
             for ann in item.annotations:
                 annotations_by_type[ann.type.name]["count"] += 1
```

### Comparing `datumaro-1.2.0rc2/datumaro/components/environment.py` & `datumaro-1.2.0rc3/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/errors.py` & `datumaro-1.2.0rc3/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/exporter.py` & `datumaro-1.2.0rc3/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/extractor_tfds.py` & `datumaro-1.2.0rc3/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/filter.py` & `datumaro-1.2.0rc3/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/format_detection.py` & `datumaro-1.2.0rc3/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/generator.py` & `datumaro-1.2.0rc3/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/hl_ops/__init__.py` & `datumaro-1.2.0rc3/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/importer.py` & `datumaro-1.2.0rc3/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/launcher.py` & `datumaro-1.2.0rc3/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/media.py` & `datumaro-1.2.0rc3/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/media_manager.py` & `datumaro-1.2.0rc3/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/merge/__init__.py` & `datumaro-1.2.0rc3/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/merge/base.py` & `datumaro-1.2.0rc3/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/merge/exact_merge.py` & `datumaro-1.2.0rc3/datumaro/components/merge/exact_merge.py`

 * *Files 13% similar despite different names*

```diff
@@ -122,58 +122,61 @@
             not item_b.media or isinstance(item_b.media, MultiframeImage)
         ):
             media = self._merge_multiframe_images(item_a, item_b)
         elif (not item_a.media or isinstance(item_a.media, MediaElement)) and (
             not item_b.media or isinstance(item_b.media, MediaElement)
         ):
             if isinstance(item_a.media, MediaElement) and isinstance(item_b.media, MediaElement):
-                if (
-                    item_a.media.path
-                    and item_b.media.path
-                    and item_a.media.path != item_b.media.path
-                ):
+                item_a_path = getattr(item_a.media, "path", None)
+                item_b_path = getattr(item_b.media, "path", None)
+
+                if item_a_path and item_b_path and item_a_path != item_b_path:
                     raise MismatchingMediaPathError(
-                        (item_a.id, item_a.subset), item_a.media.path, item_b.media.path
+                        (item_a.id, item_a.subset), item_a_path, item_b_path
+                    )
+                elif item_a_path is None and item_b_path is None:
+                    raise MismatchingMediaError(
+                        (item_a.id, item_a.subset), item_a.media, item_b.media
                     )
 
-                if item_a.media.path:
-                    media = item_a.media
-                else:
-                    media = item_b.media
+                media = item_a.media if item_a_path else item_b.media
 
             elif isinstance(item_a.media, MediaElement):
                 media = item_a.media
             else:
                 media = item_b.media
         else:
             raise MismatchingMediaError((item_a.id, item_a.subset), item_a.media, item_b.media)
         return media
 
     def _merge_images(self, item_a: DatasetItem, item_b: DatasetItem) -> Image:
         media = None
 
         if isinstance(item_a.media, Image) and isinstance(item_b.media, Image):
+            item_a_path = getattr(item_a.media, "path", None)
+            item_b_path = getattr(item_b.media, "path", None)
+
             if (
-                item_a.media.path
-                and item_b.media.path
-                and item_a.media.path != item_b.media.path
+                item_a_path
+                and item_b_path
+                and item_a_path != item_b_path
                 and item_a.media.has_data is item_b.media.has_data
             ):
                 # We use has_data as a replacement for path existence check
                 # - If only one image has data, we'll use it. The other
                 #   one is just a path metainfo, which is not significant
                 #   in this case.
                 # - If both images have data or both don't, we need
                 #   to compare paths.
                 #
                 # Different paths can aclually point to the same file,
                 # but it's not the case we'd like to allow here to be
                 # a "simple" merging strategy used for extractor joining
                 raise MismatchingMediaPathError(
-                    (item_a.id, item_a.subset), item_a.media.path, item_b.media.path
+                    (item_a.id, item_a.subset), item_a_path, item_b_path
                 )
 
             if (
                 item_a.media.has_size
                 and item_b.media.has_size
                 and item_a.media.size != item_b.media.size
             ):
@@ -184,24 +187,24 @@
             # Avoid direct comparison here for better performance
             # If there are 2 "data-only" images, they won't be compared and
             # we just use the first one
             if item_a.media.has_data:
                 media = item_a.media
             elif item_b.media.has_data:
                 media = item_b.media
-            elif item_a.media.path:
+            elif item_a_path:
                 media = item_a.media
-            elif item_b.media.path:
+            elif item_b_path:
                 media = item_b.media
             elif item_a.media.has_size:
                 media = item_a.media
             elif item_b.media.has_size:
                 media = item_b.media
             else:
-                assert False, "Unknown image field combination"
+                raise MismatchingMediaError((item_a.id, item_a.subset), item_a.media, item_b.media)
 
             if not media.has_data or not media.has_size:
                 if item_a.media._size:
                     media._size = item_a.media._size
                 elif item_b.media._size:
                     media._size = item_b.media._size
         elif isinstance(item_a.media, Image):
@@ -211,33 +214,41 @@
 
         return media
 
     def _merge_point_clouds(self, item_a: DatasetItem, item_b: DatasetItem) -> PointCloud:
         media = None
 
         if isinstance(item_a.media, PointCloud) and isinstance(item_b.media, PointCloud):
-            if item_a.media.path and item_b.media.path and item_a.media.path != item_b.media.path:
+            item_a_path = getattr(item_a.media, "path", None)
+            item_b_path = getattr(item_b.media, "path", None)
+
+            if item_a_path and item_b_path and item_a_path != item_b_path:
                 raise MismatchingMediaPathError(
-                    (item_a.id, item_a.subset), item_a.media.path, item_b.media.path
+                    (item_a.id, item_a.subset), item_a_path, item_b_path
                 )
 
-            if item_a.media.path or item_a.media.extra_images:
+            # Avoid direct comparison here for better performance
+            # If there are 2 "data-only" pointclouds, they won't be compared and
+            # we just use the first one
+            if item_a.media.has_data or item_a.media.extra_images:
                 media = item_a.media
 
                 if item_b.media.extra_images:
                     for image in item_b.media.extra_images:
                         if image not in media.extra_images:
                             media.extra_images.append(image)
-            else:
+            elif item_b.media.has_data or item_b.media.extra_images:
                 media = item_b.media
 
                 if item_a.media.extra_images:
                     for image in item_a.media.extra_images:
                         if image not in media.extra_images:
                             media.extra_images.append(image)
+            else:
+                raise MismatchingMediaError((item_a.id, item_a.subset), item_a.media, item_b.media)
 
         elif isinstance(item_a.media, PointCloud):
             media = item_a.media
         else:
             media = item_b.media
 
         return media
```

### Comparing `datumaro-1.2.0rc2/datumaro/components/merge/intersect_merge.py` & `datumaro-1.2.0rc3/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/merge/union_merge.py` & `datumaro-1.2.0rc3/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/operations.py` & `datumaro-1.2.0rc3/datumaro/components/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
     return matches, a_unmatched, b_unmatched
 
 
 class _ItemMatcher:
     @staticmethod
     def _default_item_hash(item: DatasetItem):
         if not item.media or not item.media.has_data:
-            if item.media and item.media.path:
+            if item.media and hasattr(item.media, "path"):
                 return hash(item.media.path)
 
             log.warning(
                 "Item (%s, %s) has no image " "info, counted as unique", item.id, item.subset
             )
             return None
```

### Comparing `datumaro-1.2.0rc2/datumaro/components/progress_reporting.py` & `datumaro-1.2.0rc3/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/project.py` & `datumaro-1.2.0rc3/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/searcher.py` & `datumaro-1.2.0rc3/datumaro/components/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/shift_analyzer.py` & `datumaro-1.2.0rc3/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/transformer.py` & `datumaro-1.2.0rc3/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/validator.py` & `datumaro-1.2.0rc3/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/components/visualizer.py` & `datumaro-1.2.0rc3/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     else {"path": getattr(img, "path", None)}
                     for img in pcd.extra_images
                 ]
 
                 if related_images:
                     item_desc["related_images"] = related_images
             elif isinstance(item.media, MediaElement):
-                item_desc["media"] = {"path": item.media.path}
+                item_desc["media"] = {"path": getattr(item.media, "path", None)}
 
         self.items.append(item_desc)
 
         for ann in item.annotations:
             if isinstance(ann, Label):
                 converted_ann = self._convert_label_object(ann)
             elif isinstance(ann, Mask):
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,17 @@
     def _write_item(self, item, index):
         if not self._reindex:
             index = cast(item.attributes.get("frame"), int, index)
 
         if self._save_media and item.media:
             self._save_point_cloud(item, subdir=KittiRawPath.PCD_DIR)
 
-            images = sorted(item.media.extra_images, key=lambda img: img.path)
+            images = sorted(
+                item.media.extra_images, key=lambda img: img.path if hasattr(img, "path") else ""
+            )
             for i, image in enumerate(images):
                 if image.has_data:
                     image.save(
                         osp.join(
                             self._save_dir,
                             KittiRawPath.IMG_DIR_PREFIX + ("%02d" % i),
                             "data",
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             item_id = osp.splitext(osp.relpath(item_path, polygons_dir))[0]
             item = items.get(item_id)
             item_info = {}
             item_info = parse_json_file(item_path)
 
             image_size = self._get_image_size(item_info)
             if image_size and item.has_image:
-                item.media = Image.from_file(path=item.image.path, size=image_size)
+                item.media = item.image.from_self(size=image_size)
 
             polygons = item_info["objects"]
             annotations = []
             for polygon in polygons:
                 label = polygon["label"]
                 label_id = self._categories[AnnotationType.label].find(label)[0]
                 if label_id is None:
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mars.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mot.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mots.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,20 @@
         self._objects = {}  # id -> key
 
         self._label_cat = extractor.categories().get(AnnotationType.label, LabelCategories())
 
     def _write_related_images(self, item):
         img_dir = self._related_images_dir
 
-        for img in item.media.extra_images:
-            name = osp.splitext(osp.basename(img.path))[0]
+        for idx, img in enumerate(item.media.extra_images):
+            name = (
+                osp.splitext(osp.basename(img.path))[0]
+                if hasattr(img, "path")
+                else f"extra_image_{idx}"
+            )
             img_path = osp.join(img_dir, item.id + "_pcd", name + self._find_image_ext(img))
             if img.has_data:
                 img.save(img_path)
 
             img_data = {
                 "name": osp.basename(img_path),
                 "meta": {
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/synthia.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/synthia.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/video.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from datumaro.components.annotation import Annotation, AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem, SubsetBase
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     UndeclaredLabelError,
 )
-from datumaro.components.media import Image
+from datumaro.components.media import Image, ImageFromFile
 from datumaro.util.image import (
     DEFAULT_IMAGE_META_FILE_NAME,
     IMAGE_EXTENSIONS,
     ImageMeta,
     load_image_meta_file,
 )
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
@@ -206,15 +206,15 @@
                 f"Can't parse {field_name} from '{value}'. Expected {cls}"
             ) from e
 
     @classmethod
     def _parse_annotations(
         cls,
         anno_path: str,
-        image: Image,
+        image: ImageFromFile,
         *,
         label_categories: LabelCategories,
     ) -> List[Annotation]:
         lines = []
         with open(anno_path, "r", encoding="utf-8") as f:
             for line in f:
                 line = line.strip()
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/ndr.py` & `datumaro-1.2.0rc3/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.2.0rc3/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.2.0rc3/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
             if not item.media or item.media.size is None:
                 raise Exception(f"Item {item.id} does not have image info")
 
             width, height = item.media.size
             data_df["Width"].append(width)
             data_df["Height"].append(height)
-            data_df["ImagePath"].append(item.media.path)
+            data_df["ImagePath"].append(getattr(item.media, "path", None))
 
             if not item.annotations:
                 raise Exception(f"Item {item.id} does not have annotations")
 
             for annotation in item.annotations:
                 if "scores" not in annotation.attributes:
                     raise Exception(
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/searcher.py` & `datumaro-1.2.0rc3/datumaro/plugins/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/shift_analyzer.py` & `datumaro-1.2.0rc3/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/splitter.py` & `datumaro-1.2.0rc3/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.2.0rc3/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/tiling/tile.py` & `datumaro-1.2.0rc3/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/tiling/util.py` & `datumaro-1.2.0rc3/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/transforms.py` & `datumaro-1.2.0rc3/datumaro/plugins/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,19 +510,19 @@
 
 class IdFromImageName(ItemTransform, CliPlugin):
     """
     Renames items in the dataset using image file name (without extension).
     """
 
     def transform_item(self, item):
-        if isinstance(item.media, Image) and item.media.path:
+        if isinstance(item.media, Image) and hasattr(item.media, "path"):
             name = osp.splitext(osp.basename(item.media.path))[0]
             return self.wrap_item(item, id=name)
         else:
-            log.debug("Can't change item id for item '%s': " "item has no image info" % item.id)
+            log.debug("Can't change item id for item '%s': " "item has no path info" % item.id)
             return item
 
 
 class Rename(ItemTransform, CliPlugin):
     r"""
     Renames items in the dataset. Supports regular expressions.
     The first character in the expression is a delimiter for
```

### Comparing `datumaro-1.2.0rc2/datumaro/plugins/validators.py` & `datumaro-1.2.0rc3/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/__init__.py` & `datumaro-1.2.0rc3/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/annotation_util.py` & `datumaro-1.2.0rc3/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/attrs_util.py` & `datumaro-1.2.0rc3/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/file_utils.py` & `datumaro-1.2.0rc3/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/image.py` & `datumaro-1.2.0rc3/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/image_cache.py` & `datumaro-1.2.0rc3/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/log_utils.py` & `datumaro-1.2.0rc3/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/mask_tools.py` & `datumaro-1.2.0rc3/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/meta_file_util.py` & `datumaro-1.2.0rc3/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/os_util.py` & `datumaro-1.2.0rc3/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/pickle_util.py` & `datumaro-1.2.0rc3/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/scope.py` & `datumaro-1.2.0rc3/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/telemetry_stub.py` & `datumaro-1.2.0rc3/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/telemetry_utils.py` & `datumaro-1.2.0rc3/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro/util/tf_util.py` & `datumaro-1.2.0rc3/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/datumaro.egg-info/PKG-INFO` & `datumaro-1.2.0rc3/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc2
+Version: 1.2.0rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc2/datumaro.egg-info/SOURCES.txt` & `datumaro-1.2.0rc3/datumaro.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,18 @@
 datumaro/plugins/data_formats/widerface.py
 datumaro/plugins/data_formats/arrow/__init__.py
 datumaro/plugins/data_formats/arrow/arrow_dataset.py
 datumaro/plugins/data_formats/arrow/base.py
 datumaro/plugins/data_formats/arrow/exporter.py
 datumaro/plugins/data_formats/arrow/format.py
 datumaro/plugins/data_formats/arrow/importer.py
+datumaro/plugins/data_formats/arrow/mapper/__init__.py
+datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+datumaro/plugins/data_formats/arrow/mapper/media.py
+datumaro/plugins/data_formats/arrow/mapper/utils.py
 datumaro/plugins/data_formats/ava/__init__.py
 datumaro/plugins/data_formats/ava/ava.py
 datumaro/plugins/data_formats/ava/ava_label_pb2.py
 datumaro/plugins/data_formats/celeba/__init__.py
 datumaro/plugins/data_formats/celeba/align_celeba.py
 datumaro/plugins/data_formats/celeba/celeba.py
 datumaro/plugins/data_formats/coco/__init__.py
```

### Comparing `datumaro-1.2.0rc2/datumaro.egg-info/requires.txt` & `datumaro-1.2.0rc3/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/pyproject.toml` & `datumaro-1.2.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/requirements-core.txt` & `datumaro-1.2.0rc3/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc2/setup.py` & `datumaro-1.2.0rc3/setup.py`

 * *Files identical despite different names*

