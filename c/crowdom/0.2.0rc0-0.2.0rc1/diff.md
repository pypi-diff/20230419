# Comparing `tmp/crowdom-0.2.0rc0.tar.gz` & `tmp/crowdom-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/o-gulyaev/arc/arcadia/dataforge/dist/.tmp-or5_h7l0/crowdom-0.2.0rc0.tar", last modified: Wed Mar 29 10:24:24 2023, max compression
+gzip compressed data, was "/Users/o-gulyaev/arc/arcadia/dataforge/dist/.tmp-j97smmkc/crowdom-0.2.0rc1.tar", last modified: Wed Mar 29 12:08:09 2023, max compression
```

## Comparing `crowdom-0.2.0rc0.tar` & `crowdom-0.2.0rc1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.198766 crowdom-0.2.0rc0/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      578 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/LICENSE
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7958 2023-03-29 10:24:24.198219 crowdom-0.2.0rc0/PKG-INFO
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7719 2022-11-11 11:38:27.000000 crowdom-0.2.0rc0/README.md
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.059660 crowdom-0.2.0rc0/crowdom.egg-info/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7958 2023-03-29 10:24:23.000000 crowdom-0.2.0rc0/crowdom.egg-info/PKG-INFO
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2819 2023-03-29 10:24:24.000000 crowdom-0.2.0rc0/crowdom.egg-info/SOURCES.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2023-03-29 10:24:23.000000 crowdom-0.2.0rc0/crowdom.egg-info/dependency_links.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2023-03-29 10:24:23.000000 crowdom-0.2.0rc0/crowdom.egg-info/requires.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        8 2023-03-29 10:24:23.000000 crowdom-0.2.0rc0/crowdom.egg-info/top_level.txt
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-02-15 08:42:43.000000 crowdom-0.2.0rc0/pyproject.toml
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2023-03-29 10:24:24.199254 crowdom-0.2.0rc0/setup.cfg
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1083 2023-03-29 10:18:27.000000 crowdom-0.2.0rc0/setup.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.068803 crowdom-0.2.0rc0/src/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       74 2023-03-29 10:15:15.000000 crowdom-0.2.0rc0/src/__version__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.077641 crowdom-0.2.0rc0/src/base/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      183 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/base/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1591 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/base/common.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2957 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/base/conditions.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6442 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/base/functions.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2682 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/base/metas.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      656 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/base/task.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4506 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/base/types.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.082615 crowdom-0.2.0rc0/src/bots/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       88 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/bots/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8023 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/bots/client.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7835 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/bots/util.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12660 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/bots/worker.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.084047 crowdom-0.2.0rc0/src/classification/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5991 2023-01-26 15:48:39.000000 crowdom-0.2.0rc0/src/classification/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.085211 crowdom-0.2.0rc0/src/classification_loop/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18175 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/classification_loop/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.095146 crowdom-0.2.0rc0/src/client/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      209 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/client/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19987 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/client/display.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21065 2023-03-29 10:03:32.000000 crowdom-0.2.0rc0/src/client/launch.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      599 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/client/relaunch.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3310 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/client/sbs.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10812 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/client/task.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4268 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/client/training.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4222 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/client/utils.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.097373 crowdom-0.2.0rc0/src/contrib/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       32 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/contrib/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15123 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/contrib/lzstring.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.100947 crowdom-0.2.0rc0/src/control/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       64 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/control/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10924 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/control/rule.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9233 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/control/rule_builder.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.105066 crowdom-0.2.0rc0/src/datasource/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       58 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/datasource/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4883 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/datasource/media.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3341 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/datasource/tasks.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      344 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/duration.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.106183 crowdom-0.2.0rc0/src/evaluation/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22945 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/evaluation/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.113554 crowdom-0.2.0rc0/src/experts/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      128 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      698 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/base.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2179 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/lzy.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5778 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/pipeline.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7223 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/registration.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4608 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/experts/training.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.119404 crowdom-0.2.0rc0/src/feedback_loop/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      124 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/feedback_loop/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4925 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/feedback_loop/metrics.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      861 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/feedback_loop/params.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13175 2023-03-29 08:34:56.000000 crowdom-0.2.0rc0/src/feedback_loop/pipeline.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3725 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/feedback_loop/results.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.125747 crowdom-0.2.0rc0/src/instruction/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      132 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/instruction/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10312 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/instruction/acceptance.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1253 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/instruction/annotation_check.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1371 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/instruction/css.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    33002 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/instruction/experts.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.126972 crowdom-0.2.0rc0/src/lzy/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       70 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/lzy/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.143471 crowdom-0.2.0rc0/src/lzy/serialization/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      390 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1834 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/annotation.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22068 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/base.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3803 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/classification.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2599 2022-11-11 11:38:27.000000 crowdom-0.2.0rc0/src/lzy/serialization/classification_loop.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5688 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/lzy/serialization/client.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3273 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/lzy/serialization/common.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7804 2022-11-11 11:38:27.000000 crowdom-0.2.0rc0/src/lzy/serialization/control.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1788 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/evaluation.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1118 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/serialization/mapping.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1848 2022-11-11 11:38:27.000000 crowdom-0.2.0rc0/src/lzy/serialization/pricing.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1717 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/lzy/serialization/toloka.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6782 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/lzy/serialization/worker.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.147169 crowdom-0.2.0rc0/src/lzy/workflows/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      553 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/workflows/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2204 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/workflows/annotation.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2050 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/lzy/workflows/classification.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.148343 crowdom-0.2.0rc0/src/mapping/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15290 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/mapping/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.149523 crowdom-0.2.0rc0/src/metrics/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15604 2023-03-28 08:44:49.000000 crowdom-0.2.0rc0/src/metrics/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.150688 crowdom-0.2.0rc0/src/mos/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17649 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/mos/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.154966 crowdom-0.2.0rc0/src/objects/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       60 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/objects/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3557 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/objects/questions.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      957 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/objects/std.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.165145 crowdom-0.2.0rc0/src/params/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      215 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/params/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2303 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/params/base.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14888 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/params/characteristics.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5598 2023-01-26 15:48:43.000000 crowdom-0.2.0rc0/src/params/client.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18538 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/params/event_loop.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    40759 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/params/params.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22531 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/params/ui.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1639 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/params/util.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8987 2023-02-06 16:57:08.000000 crowdom-0.2.0rc0/src/pool.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.166272 crowdom-0.2.0rc0/src/precision/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       28 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/precision/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    38127 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/pricing.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.169875 crowdom-0.2.0rc0/src/project/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       63 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/project/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18532 2022-10-31 11:43:07.000000 crowdom-0.2.0rc0/src/project/builders.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11360 2022-11-10 11:56:07.000000 crowdom-0.2.0rc0/src/project/viewers.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3151 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/src/task_spec.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1585 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/utils.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.175310 crowdom-0.2.0rc0/src/worker/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       88 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/worker/__init__.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      180 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/src/worker/common.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5262 2023-02-08 16:48:46.000000 crowdom-0.2.0rc0/src/worker/human.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3255 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/src/worker/model.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 10:24:24.196696 crowdom-0.2.0rc0/tests/
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12351 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/tests/test_base.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6100 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_classification.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    46828 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_classification_loop.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23719 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_control.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10649 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_datasource.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    50093 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_evaluation.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17719 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_feedback_loop.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)   146211 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/tests/test_instruction.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20132 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_mapping.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2917 2022-10-24 14:39:42.000000 crowdom-0.2.0rc0/tests/test_objects.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36460 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/tests/test_params.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20144 2023-02-08 16:48:46.000000 crowdom-0.2.0rc0/tests/test_pool.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18630 2022-12-12 14:42:34.000000 crowdom-0.2.0rc0/tests/test_pricing.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    74461 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/tests/test_project.py
--rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7874 2023-03-27 07:29:42.000000 crowdom-0.2.0rc0/tests/test_worker.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.267252 crowdom-0.2.0rc1/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      578 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/LICENSE
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7958 2023-03-29 12:08:09.266420 crowdom-0.2.0rc1/PKG-INFO
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7719 2022-11-11 11:38:27.000000 crowdom-0.2.0rc1/README.md
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.120861 crowdom-0.2.0rc1/crowdom.egg-info/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7958 2023-03-29 12:08:09.000000 crowdom-0.2.0rc1/crowdom.egg-info/PKG-INFO
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2819 2023-03-29 12:08:09.000000 crowdom-0.2.0rc1/crowdom.egg-info/SOURCES.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2023-03-29 12:08:09.000000 crowdom-0.2.0rc1/crowdom.egg-info/dependency_links.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2023-03-29 12:08:09.000000 crowdom-0.2.0rc1/crowdom.egg-info/requires.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        8 2023-03-29 12:08:09.000000 crowdom-0.2.0rc1/crowdom.egg-info/top_level.txt
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-02-15 08:42:43.000000 crowdom-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2023-03-29 12:08:09.268404 crowdom-0.2.0rc1/setup.cfg
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1083 2023-03-29 12:04:31.000000 crowdom-0.2.0rc1/setup.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.129878 crowdom-0.2.0rc1/src/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       74 2023-03-29 12:04:37.000000 crowdom-0.2.0rc1/src/__version__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.139058 crowdom-0.2.0rc1/src/base/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      183 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/base/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1591 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/base/common.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2957 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/base/conditions.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6442 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/base/functions.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2682 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/base/metas.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      656 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/base/task.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4822 2023-03-29 11:37:55.000000 crowdom-0.2.0rc1/src/base/types.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.144593 crowdom-0.2.0rc1/src/bots/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       88 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/bots/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8023 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/bots/client.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7835 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/bots/util.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12660 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/bots/worker.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.145750 crowdom-0.2.0rc1/src/classification/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5991 2023-01-26 15:48:39.000000 crowdom-0.2.0rc1/src/classification/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.146927 crowdom-0.2.0rc1/src/classification_loop/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18175 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/classification_loop/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.157731 crowdom-0.2.0rc1/src/client/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      209 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/client/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19987 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/client/display.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21065 2023-03-29 12:04:31.000000 crowdom-0.2.0rc1/src/client/launch.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      599 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/client/relaunch.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3310 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/client/sbs.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10812 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/client/task.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4268 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/client/training.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4222 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/client/utils.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.160430 crowdom-0.2.0rc1/src/contrib/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       32 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/contrib/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15123 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/contrib/lzstring.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.163968 crowdom-0.2.0rc1/src/control/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       64 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/control/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10924 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/control/rule.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9233 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/control/rule_builder.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.167405 crowdom-0.2.0rc1/src/datasource/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       58 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/datasource/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4883 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/datasource/media.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3341 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/datasource/tasks.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      344 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/duration.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.168902 crowdom-0.2.0rc1/src/evaluation/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22954 2023-03-29 11:37:55.000000 crowdom-0.2.0rc1/src/evaluation/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.177047 crowdom-0.2.0rc1/src/experts/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      128 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      698 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/base.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2179 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/lzy.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5778 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/pipeline.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7223 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/registration.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4608 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/experts/training.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.183317 crowdom-0.2.0rc1/src/feedback_loop/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      124 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/feedback_loop/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4925 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/feedback_loop/metrics.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      861 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/feedback_loop/params.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13175 2023-03-29 08:34:56.000000 crowdom-0.2.0rc1/src/feedback_loop/pipeline.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3725 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/feedback_loop/results.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.189411 crowdom-0.2.0rc1/src/instruction/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      132 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/instruction/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10312 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/instruction/acceptance.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1253 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/instruction/annotation_check.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1371 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/instruction/css.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    33002 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/instruction/experts.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.190623 crowdom-0.2.0rc1/src/lzy/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       70 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/lzy/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.207662 crowdom-0.2.0rc1/src/lzy/serialization/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      390 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1834 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/annotation.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22068 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/base.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3803 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/classification.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2599 2022-11-11 11:38:27.000000 crowdom-0.2.0rc1/src/lzy/serialization/classification_loop.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5688 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/lzy/serialization/client.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3273 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/lzy/serialization/common.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7804 2022-11-11 11:38:27.000000 crowdom-0.2.0rc1/src/lzy/serialization/control.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1788 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/evaluation.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1118 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/serialization/mapping.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1848 2022-11-11 11:38:27.000000 crowdom-0.2.0rc1/src/lzy/serialization/pricing.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1717 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/lzy/serialization/toloka.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6782 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/lzy/serialization/worker.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.211451 crowdom-0.2.0rc1/src/lzy/workflows/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      553 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/workflows/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2204 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/workflows/annotation.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2050 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/lzy/workflows/classification.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.212597 crowdom-0.2.0rc1/src/mapping/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15290 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/mapping/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.213936 crowdom-0.2.0rc1/src/metrics/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15604 2023-03-29 12:04:31.000000 crowdom-0.2.0rc1/src/metrics/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.215007 crowdom-0.2.0rc1/src/mos/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17649 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/mos/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.219217 crowdom-0.2.0rc1/src/objects/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       60 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/objects/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3557 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/objects/questions.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      957 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/objects/std.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.231917 crowdom-0.2.0rc1/src/params/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      215 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/params/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2303 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/params/base.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14888 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/params/characteristics.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5598 2023-01-26 15:48:43.000000 crowdom-0.2.0rc1/src/params/client.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18538 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/params/event_loop.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    40759 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/params/params.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22531 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/params/ui.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1639 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/params/util.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8987 2023-02-06 16:57:08.000000 crowdom-0.2.0rc1/src/pool.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.233292 crowdom-0.2.0rc1/src/precision/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       28 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/precision/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    38127 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/pricing.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.237641 crowdom-0.2.0rc1/src/project/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       63 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/project/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18532 2022-10-31 11:43:07.000000 crowdom-0.2.0rc1/src/project/builders.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11360 2022-11-10 11:56:07.000000 crowdom-0.2.0rc1/src/project/viewers.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3151 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/src/task_spec.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1585 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/utils.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.242720 crowdom-0.2.0rc1/src/worker/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       88 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/worker/__init__.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      180 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/src/worker/common.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5262 2023-02-08 16:48:46.000000 crowdom-0.2.0rc1/src/worker/human.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3255 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/src/worker/model.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-03-29 12:08:09.264658 crowdom-0.2.0rc1/tests/
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12351 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/tests/test_base.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6100 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_classification.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    46828 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_classification_loop.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23719 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_control.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10649 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_datasource.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    50093 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_evaluation.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17719 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_feedback_loop.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)   146211 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/tests/test_instruction.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20132 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_mapping.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2917 2022-10-24 14:39:42.000000 crowdom-0.2.0rc1/tests/test_objects.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36460 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/tests/test_params.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20144 2023-02-08 16:48:46.000000 crowdom-0.2.0rc1/tests/test_pool.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18630 2022-12-12 14:42:34.000000 crowdom-0.2.0rc1/tests/test_pricing.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    74461 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/tests/test_project.py
+-rw-rw-r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7874 2023-03-27 07:29:42.000000 crowdom-0.2.0rc1/tests/test_worker.py
```

### Comparing `crowdom-0.2.0rc0/LICENSE` & `crowdom-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/PKG-INFO` & `crowdom-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdom
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Crowdom
 Author: Oleg Gulyaev
 Author-email: o-gulyaev@yandex-team.ru
 License: Apache 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crowdom-0.2.0rc0/README.md` & `crowdom-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/crowdom.egg-info/PKG-INFO` & `crowdom-0.2.0rc1/crowdom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdom
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Crowdom
 Author: Oleg Gulyaev
 Author-email: o-gulyaev@yandex-team.ru
 License: Apache 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crowdom-0.2.0rc0/crowdom.egg-info/SOURCES.txt` & `crowdom-0.2.0rc1/crowdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/setup.py` & `crowdom-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/common.py` & `crowdom-0.2.0rc1/src/base/common.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/conditions.py` & `crowdom-0.2.0rc1/src/base/conditions.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/functions.py` & `crowdom-0.2.0rc1/src/base/functions.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/metas.py` & `crowdom-0.2.0rc1/src/base/metas.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/task.py` & `crowdom-0.2.0rc1/src/base/task.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/base/types.py` & `crowdom-0.2.0rc1/src/base/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -117,14 +117,21 @@
     @staticmethod
     def get_display_labels() -> List[LocalizedString]:
         return [
             LocalizedString({'EN': 'Yes', 'RU': 'Да', 'TR': 'Evet', 'KK': 'Иә'}),
             LocalizedString({'EN': 'No', 'RU': 'Нет', 'TR': 'Hayır', 'KK': 'Жоқ'}),
         ]
 
+    @staticmethod
+    def get_ok_confidence(probas: Dict['BinaryEvaluation', float]) -> float:
+        assert len(probas), 'empty probas for binary evaluation'
+        if BinaryEvaluation(ok=True) in probas:
+            return probas[BinaryEvaluation(ok=True)]
+        return 1 - probas[BinaryEvaluation(ok=False)]
+
 
 class ScoreEvaluation(Evaluation, Class):
     ...
 
 
 @dataclass(frozen=True)
 class Metadata(Object):
```

### Comparing `crowdom-0.2.0rc0/src/bots/client.py` & `crowdom-0.2.0rc1/src/bots/client.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/bots/util.py` & `crowdom-0.2.0rc1/src/bots/util.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/bots/worker.py` & `crowdom-0.2.0rc1/src/bots/worker.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/classification/__init__.py` & `crowdom-0.2.0rc1/src/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/classification_loop/__init__.py` & `crowdom-0.2.0rc1/src/classification_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/display.py` & `crowdom-0.2.0rc1/src/client/display.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/launch.py` & `crowdom-0.2.0rc1/src/client/launch.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/relaunch.py` & `crowdom-0.2.0rc1/src/client/relaunch.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/sbs.py` & `crowdom-0.2.0rc1/src/client/sbs.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/task.py` & `crowdom-0.2.0rc1/src/client/task.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/training.py` & `crowdom-0.2.0rc1/src/client/training.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/client/utils.py` & `crowdom-0.2.0rc1/src/client/utils.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/contrib/lzstring.py` & `crowdom-0.2.0rc1/src/contrib/lzstring.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/control/rule.py` & `crowdom-0.2.0rc1/src/control/rule.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/control/rule_builder.py` & `crowdom-0.2.0rc1/src/control/rule_builder.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/datasource/media.py` & `crowdom-0.2.0rc1/src/datasource/media.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/datasource/tasks.py` & `crowdom-0.2.0rc1/src/datasource/tasks.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/evaluation/__init__.py` & `crowdom-0.2.0rc1/src/evaluation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         aggregation_algorithm,
         worker_weights,
     ):
         # TODO: support other evaluation types
         # TODO: add individual workers evaluations like in base loop
         # TODO: may be None
         assert task_labels_probas is not None
-        confidence = task_labels_probas[base.BinaryEvaluation(ok=True)]
+        confidence = base.BinaryEvaluation.get_ok_confidence(task_labels_probas)
         assert worker_labels
         evaluations.append(
             SolutionEvaluation(
                 ok=bool(confidence >= confidence_threshold),  # to convert from numpy bool
                 confidence=confidence,
                 worker_labels=worker_labels,
             )
```

### Comparing `crowdom-0.2.0rc0/src/experts/base.py` & `crowdom-0.2.0rc1/src/experts/base.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/experts/lzy.py` & `crowdom-0.2.0rc1/src/experts/lzy.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/experts/pipeline.py` & `crowdom-0.2.0rc1/src/experts/pipeline.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/experts/registration.py` & `crowdom-0.2.0rc1/src/experts/registration.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/experts/training.py` & `crowdom-0.2.0rc1/src/experts/training.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/feedback_loop/metrics.py` & `crowdom-0.2.0rc1/src/feedback_loop/metrics.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/feedback_loop/params.py` & `crowdom-0.2.0rc1/src/feedback_loop/params.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/feedback_loop/pipeline.py` & `crowdom-0.2.0rc1/src/feedback_loop/pipeline.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/feedback_loop/results.py` & `crowdom-0.2.0rc1/src/feedback_loop/results.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/instruction/acceptance.py` & `crowdom-0.2.0rc1/src/instruction/acceptance.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/instruction/annotation_check.py` & `crowdom-0.2.0rc1/src/instruction/annotation_check.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/instruction/css.py` & `crowdom-0.2.0rc1/src/instruction/css.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/instruction/experts.py` & `crowdom-0.2.0rc1/src/instruction/experts.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/annotation.py` & `crowdom-0.2.0rc1/src/lzy/serialization/annotation.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/base.py` & `crowdom-0.2.0rc1/src/lzy/serialization/base.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/classification.py` & `crowdom-0.2.0rc1/src/lzy/serialization/classification.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/classification_loop.py` & `crowdom-0.2.0rc1/src/lzy/serialization/classification_loop.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/client.py` & `crowdom-0.2.0rc1/src/lzy/serialization/client.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/common.py` & `crowdom-0.2.0rc1/src/lzy/serialization/common.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/control.py` & `crowdom-0.2.0rc1/src/lzy/serialization/control.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/evaluation.py` & `crowdom-0.2.0rc1/src/lzy/serialization/evaluation.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/mapping.py` & `crowdom-0.2.0rc1/src/lzy/serialization/mapping.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/pricing.py` & `crowdom-0.2.0rc1/src/lzy/serialization/pricing.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/toloka.py` & `crowdom-0.2.0rc1/src/lzy/serialization/toloka.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/serialization/worker.py` & `crowdom-0.2.0rc1/src/lzy/serialization/worker.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/workflows/__init__.py` & `crowdom-0.2.0rc1/src/lzy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/workflows/annotation.py` & `crowdom-0.2.0rc1/src/lzy/workflows/annotation.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/lzy/workflows/classification.py` & `crowdom-0.2.0rc1/src/lzy/workflows/classification.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/mapping/__init__.py` & `crowdom-0.2.0rc1/src/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/metrics/__init__.py` & `crowdom-0.2.0rc1/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/mos/__init__.py` & `crowdom-0.2.0rc1/src/mos/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/objects/questions.py` & `crowdom-0.2.0rc1/src/objects/questions.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/objects/std.py` & `crowdom-0.2.0rc1/src/objects/std.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/base.py` & `crowdom-0.2.0rc1/src/params/base.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/characteristics.py` & `crowdom-0.2.0rc1/src/params/characteristics.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/client.py` & `crowdom-0.2.0rc1/src/params/client.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/event_loop.py` & `crowdom-0.2.0rc1/src/params/event_loop.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/params.py` & `crowdom-0.2.0rc1/src/params/params.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/ui.py` & `crowdom-0.2.0rc1/src/params/ui.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/params/util.py` & `crowdom-0.2.0rc1/src/params/util.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/pool.py` & `crowdom-0.2.0rc1/src/pool.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/pricing.py` & `crowdom-0.2.0rc1/src/pricing.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/project/builders.py` & `crowdom-0.2.0rc1/src/project/builders.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/project/viewers.py` & `crowdom-0.2.0rc1/src/project/viewers.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/task_spec.py` & `crowdom-0.2.0rc1/src/task_spec.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/utils.py` & `crowdom-0.2.0rc1/src/utils.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/worker/human.py` & `crowdom-0.2.0rc1/src/worker/human.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/src/worker/model.py` & `crowdom-0.2.0rc1/src/worker/model.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_base.py` & `crowdom-0.2.0rc1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_classification.py` & `crowdom-0.2.0rc1/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_classification_loop.py` & `crowdom-0.2.0rc1/tests/test_classification_loop.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_control.py` & `crowdom-0.2.0rc1/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_datasource.py` & `crowdom-0.2.0rc1/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_evaluation.py` & `crowdom-0.2.0rc1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_feedback_loop.py` & `crowdom-0.2.0rc1/tests/test_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_instruction.py` & `crowdom-0.2.0rc1/tests/test_instruction.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_mapping.py` & `crowdom-0.2.0rc1/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_objects.py` & `crowdom-0.2.0rc1/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_params.py` & `crowdom-0.2.0rc1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_pool.py` & `crowdom-0.2.0rc1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_pricing.py` & `crowdom-0.2.0rc1/tests/test_pricing.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_project.py` & `crowdom-0.2.0rc1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `crowdom-0.2.0rc0/tests/test_worker.py` & `crowdom-0.2.0rc1/tests/test_worker.py`

 * *Files identical despite different names*

