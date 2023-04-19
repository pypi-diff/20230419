# Comparing `tmp/simple_parsing-0.1.1.tar.gz` & `tmp/simple_parsing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_parsing-0.1.1.tar", last modified: Tue Mar 14 14:54:09 2023, max compression
+gzip compressed data, was "simple_parsing-0.1.2.tar", last modified: Wed Apr 19 15:30:25 2023, max compression
```

## Comparing `simple_parsing-0.1.1.tar` & `simple_parsing-0.1.2.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/simple_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/simple_parsing/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.951315 simple_parsing-0.1.1/simple_parsing/annotation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/annotation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/annotation_utils/get_field_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/help_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.951315 simple_parsing-0.1.1/simple_parsing/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/flatten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.955315 simple_parsing-0.1.1/simple_parsing/helpers/hparams/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/hparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/hyperparameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/priors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/hparams/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.955315 simple_parsing-0.1.1/simple_parsing/helpers/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/serialization/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/serialization/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/serialization/yaml_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/helpers/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    49343 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/replace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.955315 simple_parsing-0.1.1/simple_parsing/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/field_metavar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/field_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/field_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/simple_parsing/wrappers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.951315 simple_parsing-0.1.1/simple_parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-03-14 14:54:09.000000 simple_parsing-0.1.1/simple_parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-14 14:54:09.000000 simple_parsing-0.1.1/simple_parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:54:09.000000 simple_parsing-0.1.1/simple_parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-14 14:54:09.000000 simple_parsing-0.1.1/simple_parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 14:54:09.000000 simple_parsing-0.1.1/simple_parsing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:54:09.963315 simple_parsing-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_bools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_custom_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_default_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_future_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_generation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_huggingface_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_initvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue64.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_107.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_132.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_144.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_46.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_48.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_issue_96.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_optional_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_optional_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_positional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_set_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_suppress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-03-14 14:53:45.000000 simple_parsing-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/simple_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/simple_parsing/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing/annotation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/annotation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/annotation_utils/get_field_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/help_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/flatten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/helpers/hparams/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/nested_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/helpers/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/yaml_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_metavar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_bools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_custom_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_default_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_future_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_generation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_huggingface_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_46.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_positional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_set_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_suppress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/versioneer.py
```

### Comparing `simple_parsing-0.1.1/LICENSE` & `simple_parsing-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/PKG-INFO` & `simple_parsing-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_parsing
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.1/README.md` & `simple_parsing-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/setup.py` & `simple_parsing-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/__init__.py` & `simple_parsing-0.1.2/simple_parsing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 @author: Fabrice Normandin
 """
 from . import helpers, utils, wrappers
 from .conflicts import ConflictResolution
 from .decorators import main
 from .help_formatter import SimpleHelpFormatter
 from .helpers import (
+    Partial,
     Serializable,
     choice,
+    config_for,
     field,
     flag,
     list_field,
     mutable_field,
     subgroups,
     subparsers,
 )
@@ -27,27 +29,29 @@
 from .replace import replace
 from .utils import InconsistentArgumentError
 
 __all__ = [
     "ArgumentGenerationMode",
     "ArgumentParser",
     "choice",
+    "config_for",
     "ConflictResolution",
     "DashVariant",
     "field",
     "flag",
     "helpers",
     "InconsistentArgumentError",
     "list_field",
     "main",
     "mutable_field",
     "NestedMode",
     "parse_known_args",
     "parse",
     "ParsingError",
+    "Partial",
     "replace",
     "Serializable",
     "SimpleHelpFormatter",
     "subgroups",
     "subparsers",
     "utils",
     "wrappers",
```

### Comparing `simple_parsing-0.1.1/simple_parsing/annotation_utils/get_field_annotations.py` & `simple_parsing-0.1.2/simple_parsing/annotation_utils/get_field_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 import inspect
 import sys
 import types
 import typing
 from contextlib import contextmanager
 from dataclasses import InitVar
+from itertools import dropwhile
 from logging import getLogger as get_logger
 from typing import Any, Dict, Iterator, Optional, get_type_hints
 
 logger = get_logger(__name__)
 
 # NOTE: This dict is used to enable forward compatibility with things such as `tuple[int, str]`,
 # `list[float]`, etc. when using `from __future__ import annotations`.
@@ -186,21 +187,22 @@
         # stack.append(frame)
         frame = frame.f_back
     # Found the frame with the dataclass definition. Update the locals. This makes it possible to
     # use dataclasses defined in local scopes!
     if frame is not None:
         local_ns.update(frame.f_locals)
 
-    # Get the global_ns in the module starting from the deepest base until the module where the field_name is defined.
+    # Get the global_ns in the module starting from the deepest base until the module with the field_name last definition.
     global_ns = {}
-    for base_cls in reversed(some_class.mro()):
+    classes_to_iterate = list(dropwhile(
+        lambda cls: field_name not in getattr(cls, "__annotations__", {}),
+        some_class.mro()
+    ))
+    for base_cls in reversed(classes_to_iterate):
         global_ns.update(sys.modules[base_cls.__module__].__dict__)
-        annotations = getattr(base_cls, "__annotations__", None)
-        if annotations and field_name in annotations:
-            break
 
     try:
         with _initvar_patcher():
             annotations_dict = get_type_hints(some_class, localns=local_ns, globalns=global_ns)
     except TypeError:
         annotations_dict = collections.ChainMap(
             *[getattr(cls, "__annotations__", {}) for cls in some_class.mro()]
```

### Comparing `simple_parsing-0.1.1/simple_parsing/conflicts.py` & `simple_parsing-0.1.2/simple_parsing/conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/decorators.py` & `simple_parsing-0.1.2/simple_parsing/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/docstring.py` & `simple_parsing-0.1.2/simple_parsing/docstring.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/help_formatter.py` & `simple_parsing-0.1.2/simple_parsing/help_formatter.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/custom_actions.py` & `simple_parsing-0.1.2/simple_parsing/helpers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/fields.py` & `simple_parsing-0.1.2/simple_parsing/helpers/fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/flatten.py` & `simple_parsing-0.1.2/simple_parsing/helpers/flatten.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/hparams/hparam.py` & `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hparam.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/hparams/hyperparameters.py` & `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/hparams/hyperparameters_test.py` & `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/hparams/priors.py` & `simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/hparams/priors_test.py` & `simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/serialization/decoding.py` & `simple_parsing-0.1.2/simple_parsing/helpers/serialization/decoding.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ Functions for decoding dataclass fields from "raw" values (e.g. from json).
 """
 from __future__ import annotations
 
 import inspect
+import sys
 import warnings
 from collections import OrderedDict
 from collections.abc import Mapping
 from dataclasses import Field
 from enum import Enum
 from functools import partial
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Callable, TypeVar
-from typing_extensions import Literal
 
 from simple_parsing.annotation_utils.get_field_annotations import (
     evaluate_string_annotation,
 )
 from simple_parsing.utils import (
     get_bound,
     get_forward_arg,
@@ -40,25 +40,74 @@
 K = TypeVar("K")
 V = TypeVar("V")
 
 # Dictionary mapping from types/type annotations to their decoding functions.
 _decoding_fns: dict[type[T], Callable[[Any], T]] = {
     # the 'primitive' types are decoded using the type fn as a constructor.
     t: t
-    for t in [str, float, int, bytes]
+    for t in [str, bytes]
 }
 
 
-def decode_bool(v: Any) -> bool:
-    if isinstance(v, str):
-        return str2bool(v)
-    return bool(v)
+def register_decoding_fn(
+    some_type: type[T], function: Callable[[Any], T], overwrite: bool = False
+) -> None:
+    """Register a decoding function for the type `some_type`."""
+    _register(some_type, function, overwrite=overwrite)
+
+
+def _register(t: type, func: Callable, overwrite: bool = False) -> None:
+    if t not in _decoding_fns or overwrite:
+        # logger.debug(f"Registering the type {t} with decoding function {func}")
+        _decoding_fns[t] = func
+
 
+C = TypeVar("C", bound=Callable[[Any], Any])
 
-_decoding_fns[bool] = decode_bool
+
+def decoding_fn_for_type(some_type: type) -> Callable[[C], C]:
+    """Registers a function to be used to convert a serialized value to the given type.
+
+    The function should accept one argument (the serialized value) and return the decoded value.
+    """
+
+    def _wrapper(fn: C) -> C:
+        register_decoding_fn(some_type, fn, overwrite=True)
+        return fn
+
+    return _wrapper
+
+
+@decoding_fn_for_type(int)
+def _decode_int(v: str) -> int:
+    int_v = int(v)
+    if isinstance(v, bool):
+        warnings.warn(UnsafeCastingWarning(raw_value=v, decoded_value=int_v))
+    elif int_v != float(v):
+        warnings.warn(UnsafeCastingWarning(raw_value=v, decoded_value=int_v))
+    return int_v
+
+
+@decoding_fn_for_type(float)
+def _decode_float(v: Any) -> float:
+    float_v = float(v)
+    if isinstance(v, bool):
+        warnings.warn(UnsafeCastingWarning(raw_value=v, decoded_value=float_v))
+    return float_v
+
+
+@decoding_fn_for_type(bool)
+def _decode_bool(v: Any) -> bool:
+    if isinstance(v, str):
+        bool_v = str2bool(v)
+    else:
+        bool_v = bool(v)
+        if isinstance(v, (int, float)) and v not in (0, 1, 0.0, 1.0):
+            warnings.warn(UnsafeCastingWarning(raw_value=v, decoded_value=bool_v))
+    return bool_v
 
 
 def decode_field(
     field: Field,
     raw_value: Any,
     containing_dataclass: type | None = None,
     drop_extra_fields: bool | None = None,
@@ -89,19 +138,44 @@
         return custom_decoding_fn(raw_value)
 
     if isinstance(field_type, str) and containing_dataclass:
         field_type = evaluate_string_annotation(field_type, containing_dataclass)
 
     decoding_function = get_decoding_fn(field_type)
 
-    if is_dataclass_type(field_type) and drop_extra_fields is not None:
-        # Pass the drop_extra_fields argument to the decoding function.
-        return decoding_function(raw_value, drop_extra_fields=drop_extra_fields)
+    _kwargs = dict(category=UnsafeCastingWarning) if sys.version_info >= (3, 11) else {}
 
-    return decoding_function(raw_value)
+    with warnings.catch_warnings(record=True, **_kwargs) as warning_messages:
+        if is_dataclass_type(field_type) and drop_extra_fields is not None:
+            # Pass the drop_extra_fields argument to the decoding function.
+            decoded_value = decoding_function(raw_value, drop_extra_fields=drop_extra_fields)
+        else:
+            decoded_value = decoding_function(raw_value)
+
+    for warning_message in warning_messages.copy():
+        if not isinstance(warning_message.message, UnsafeCastingWarning):
+            warnings.warn_explicit(
+                message=warning_message.message,
+                category=warning_message.category,
+                filename=warning_message.filename,
+                lineno=warning_message.lineno,
+                # module=warning_message.module,
+                # registry=warning_message.registry,
+                # module_globals=warning_message.module_globals,
+            )
+            warning_messages.remove(warning_message)
+
+    if warning_messages:
+        warnings.warn(
+            RuntimeWarning(
+                f"Unsafe casting occurred when deserializing field '{name}' of type {field_type}: "
+                f"raw value: {raw_value!r}, decoded value: {decoded_value!r}."
+            )
+        )
+    return decoded_value
 
 
 # NOTE: Disabling the caching here might help avoid some bugs, and it's unclear if this has that
 # much of a performance impact.
 def get_decoding_fn(type_annotation: type[T] | str) -> Callable[..., T]:
     """Fetches/Creates a decoding function for the given type annotation.
 
@@ -220,15 +294,15 @@
         return decode_enum(t)
 
     if is_typevar(t):
         bound = get_bound(t)
         logger.debug(f"Decoding a typevar: {t}, bound type is {bound}.")
         if bound is not None:
             return get_decoding_fn(bound)
-    
+
     if is_literal(t):
         logger.debug(f"Decoding a Literal field: {t}")
         possible_vals = get_type_arguments(t)
         return decode_literal(*possible_vals)
 
     # Unknown type.
     warnings.warn(
@@ -237,27 +311,14 @@
             f"Will try to use the type as a constructor. Consider registering a decoding function "
             f"using `register_decoding_fn`, or posting an issue on GitHub. "
         )
     )
     return try_constructor(t)
 
 
-def _register(t: type, func: Callable, overwrite: bool = False) -> None:
-    if t not in _decoding_fns or overwrite:
-        # logger.debug(f"Registering the type {t} with decoding function {func}")
-        _decoding_fns[t] = func
-
-
-def register_decoding_fn(
-    some_type: type[T], function: Callable[[Any], T], overwrite: bool = False
-) -> None:
-    """Register a decoding function for the type `some_type`."""
-    _register(some_type, function, overwrite=overwrite)
-
-
 def decode_optional(t: type[T]) -> Callable[[Any | None], T | None]:
     decode = get_decoding_fn(t)
 
     def _decode_optional(val: Any | None) -> T | None:
         return val if val is None else decode(val)
 
     return _decode_optional
@@ -277,23 +338,29 @@
             logger.debug(f"Couldn't parse value {val}, returning it as-is. (exception: {e})")
         return val
 
     return _try_functions
 
 
 def decode_union(*types: type[T]) -> Callable[[Any], T | Any]:
-    types = list(types)
-    optional = type(None) in types
+    types_list = list(types)
+    optional = type(None) in types_list
+
     # Partition the Union into None and non-None types.
-    while type(None) in types:
-        types.remove(type(None))
+    while type(None) in types_list:
+        types_list.remove(type(None))
 
     decoding_fns: list[Callable[[Any], T]] = [
-        decode_optional(t) if optional else get_decoding_fn(t) for t in types
+        decode_optional(t) if optional else get_decoding_fn(t) for t in types_list
     ]
+
+    # TODO: We could be a bit smarter about the order in which we try the functions, but for now,
+    # we just try the functions in the same order as the annotation, and return the result from the
+    # first function that doesn't raise an exception.
+
     # Try using each of the non-None types, in succession. Worst case, return the value.
     return try_functions(*decoding_fns)
 
 
 def decode_list(t: type[T]) -> Callable[[list[Any]], list[T]]:
     decode_item = get_decoding_fn(t)
 
@@ -451,7 +518,14 @@
         else:
             return t(val)
 
     return try_functions(constructor)
 
 
 register_decoding_fn(Path, Path)
+
+
+class UnsafeCastingWarning(RuntimeWarning):
+    def __init__(self, raw_value: Any, decoded_value: Any) -> None:
+        super().__init__()
+        self.raw_value = raw_value
+        self.decoded_value = decoded_value
```

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/serialization/encoding.py` & `simple_parsing-0.1.2/simple_parsing/helpers/serialization/encoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/serialization/serializable.py` & `simple_parsing-0.1.2/simple_parsing/helpers/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/serialization/yaml_serialization.py` & `simple_parsing-0.1.2/simple_parsing/helpers/serialization/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/helpers/subgroups.py` & `simple_parsing-0.1.2/simple_parsing/helpers/subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/parsing.py` & `simple_parsing-0.1.2/simple_parsing/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,21 @@
                 config_paths = [self.config_path]
             else:
                 config_paths = self.config_path
             for config_file in config_paths:
                 self.set_defaults(config_file)
 
         if self.add_config_path_arg:
-            temp_parser = ArgumentParser(add_config_path_arg=False, add_help=False)
+            temp_parser = ArgumentParser(
+                add_config_path_arg=False,
+                add_help=False,
+                add_option_string_dash_variants=FieldWrapper.add_dash_variants,
+                argument_generation_mode=FieldWrapper.argument_generation_mode,
+                nested_mode=FieldWrapper.nested_mode,
+            )
             temp_parser.add_argument(
                 "--config_path",
                 type=Path,
                 nargs="*",
                 default=self.config_path,
                 help="Path to a config file containing default values to use.",
             )
```

### Comparing `simple_parsing-0.1.1/simple_parsing/replace.py` & `simple_parsing-0.1.2/simple_parsing/replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/utils.py` & `simple_parsing-0.1.2/simple_parsing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -913,15 +913,21 @@
             sub_dictionary = sub_dictionary.setdefault(part, {})
         assert isinstance(sub_dictionary, dict)
         sub_dictionary[keys[-1]] = value
     return nested
 
 
 def flatten_join(nested: PossiblyNestedMapping[str, V], sep: str = ".") -> dict[str, V]:
-    """Flatten a dictionary of dictionaries. When collisions occur, joins the keys with `sep`."""
+    """Flatten a dictionary of dictionaries. Joins different nesting levels with `sep` as separator.
+
+    >>> flatten_join({'a': {'b': 2, 'c': 3}, 'c': {'d': 3, 'e': 4}})
+    {'a.b': 2, 'a.c': 3, 'c.d': 3, 'c.e': 4}
+    >>> flatten_join({'a': {'b': 2, 'c': 3}, 'c': {'d': 3, 'e': 4}}, sep="/")
+    {'a/b': 2, 'a/c': 3, 'c/d': 3, 'c/e': 4}
+    """
     return {sep.join(keys): value for keys, value in flatten(nested).items()}
 
 
 def unflatten_split(
     flattened: Mapping[str, V], sep: str = ".", recursive: bool = False
 ) -> PossiblyNestedDict[str, V]:
     """Unflatten a dict into a possibly nested dict. Keys are split using `sep`.
```

### Comparing `simple_parsing-0.1.1/simple_parsing/wrappers/dataclass_wrapper.py` & `simple_parsing-0.1.2/simple_parsing/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/wrappers/field_metavar.py` & `simple_parsing-0.1.2/simple_parsing/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/wrappers/field_parsing.py` & `simple_parsing-0.1.2/simple_parsing/wrappers/field_parsing.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/wrappers/field_wrapper.py` & `simple_parsing-0.1.2/simple_parsing/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing/wrappers/wrapper.py` & `simple_parsing-0.1.2/simple_parsing/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/simple_parsing.egg-info/PKG-INFO` & `simple_parsing-0.1.2/simple_parsing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-parsing
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.1/simple_parsing.egg-info/SOURCES.txt` & `simple_parsing-0.1.2/simple_parsing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 simple_parsing.egg-info/top_level.txt
 simple_parsing/annotation_utils/__init__.py
 simple_parsing/annotation_utils/get_field_annotations.py
 simple_parsing/helpers/__init__.py
 simple_parsing/helpers/custom_actions.py
 simple_parsing/helpers/fields.py
 simple_parsing/helpers/flatten.py
+simple_parsing/helpers/nested_partial.py
+simple_parsing/helpers/partial.py
 simple_parsing/helpers/subgroups.py
 simple_parsing/helpers/hparams/__init__.py
 simple_parsing/helpers/hparams/hparam.py
 simple_parsing/helpers/hparams/hyperparameters.py
 simple_parsing/helpers/hparams/hyperparameters_test.py
 simple_parsing/helpers/hparams/priors.py
 simple_parsing/helpers/hparams/priors_test.py
```

### Comparing `simple_parsing-0.1.1/test/test_aliases.py` & `simple_parsing-0.1.2/test/test_aliases.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_base.py` & `simple_parsing-0.1.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_bools.py` & `simple_parsing-0.1.2/test/test_bools.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_choice.py` & `simple_parsing-0.1.2/test/test_choice.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_conflicts.py` & `simple_parsing-0.1.2/test/test_conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_custom_args.py` & `simple_parsing-0.1.2/test/test_custom_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_decoding.py` & `simple_parsing-0.1.2/test/test_decoding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import textwrap
 from dataclasses import dataclass, field
 from pathlib import Path
 from test.testutils import Generic, TypeVar
-from typing import Any, Dict, List, Optional, Tuple, Type
-from typing_extensions import Literal
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import pytest
-import warnings
+from typing_extensions import Literal
 
 from simple_parsing.helpers import Serializable, dict_field, list_field
 from simple_parsing.helpers.serialization.decoding import (
     get_decoding_fn,
     register_decoding_fn,
 )
+from simple_parsing.helpers.serialization.serializable import loads_json
+from simple_parsing.utils import DataclassT
 
 
 def test_encode_something(simple_attribute):
 
     some_type, passed_value, expected_value = simple_attribute
 
     @dataclass
@@ -117,20 +118,35 @@
     [
         # (Tuple[int, float], json.loads(json.dumps([1, 2])), (1, 2.0)),
         (
             List[Tuple[int, float]],
             json.loads(json.dumps([[1, 2], [3, 4]])),
             [(1, 2.0), (3, 4.0)],
         ),
+        (Union[int, float], "1", 1),
+        (Union[int, float], "1.2", 1.2),
+        pytest.param(
+            Union[int, float],
+            1.2,
+            1.2,
+            marks=[
+                pytest.mark.xfail(reason="decoding an int works (but raises a warning)"),
+            ],
+        ),
+        # NOTE: Here we expect a float, since it's the first type that will work.
+        (Union[float, int], "1", 1.0),
+        (Union[float, int], "1.2", 1.2),
+        (Union[float, int], 1.2, 1.2),
     ],
 )
-def test_decode_tuple(some_type: Type, encoded_value: Any, expected_value: Any):
+def test_decode(some_type: Type, encoded_value: Any, expected_value: Any):
     decoding_function = get_decoding_fn(some_type)
     actual = decoding_function(encoded_value)
     assert actual == expected_value
+    assert type(actual) == type(expected_value)
 
 
 @dataclass
 class Hparams:
     use_log: int = 1
     severity: int = 2
     probs: List[int] = field(default_factory=lambda: [1, 2])
@@ -138,32 +154,53 @@
 
 @dataclass
 class Parameters(Serializable):
     hparams: Hparams = field(default_factory=Hparams)
 
 
 def test_implicit_int_casting(tmp_path: Path):
-    """Test for 'issue' #227: https://github.com/lebrice/SimpleParsing/issues/227"""
-    assert get_decoding_fn(int) is int
+    """Test that we do in fact perform the unsafe casting as described in #227:
+    https://github.com/lebrice/SimpleParsing/issues/227
+    """
     with open(tmp_path / "conf.yaml", "w") as f:
         f.write(
             textwrap.dedent(
                 """\
                 hparams:
                     use_log: 1
                     severity: 0.1
                     probs: [0.1, 0.2]
                 """
             )
         )
-
-    file_config = Parameters.load(tmp_path / "conf.yaml")
+    with pytest.warns(RuntimeWarning, match="Unsafe casting"):
+        file_config = Parameters.load(tmp_path / "conf.yaml")
     assert file_config == Parameters(hparams=Hparams(severity=0, probs=[0, 0]))
 
 
+@pytest.fixture(autouse=True)
+def reset_int_decoding_fns_after_test():
+    """Reset the decoding function for `int` to the default after each test."""
+    from simple_parsing.helpers.serialization.decoding import _decoding_fns
+
+    backup = _decoding_fns.copy()
+    yield
+    for key, value in _decoding_fns.items():
+        if key not in backup:
+            # print(f"Test added a decoding function for {key} with value {value}.")
+            pass
+        elif value != backup[key]:
+            # print(
+            #     f"Test changed the decoding function for {key} from {backup[key]} to {value}.",
+            # )
+            pass
+    _decoding_fns.clear()
+    _decoding_fns.update(backup)
+
+
 def test_registering_safe_casting_decoding_fn():
     """Test the solution to 'issue' #227: https://github.com/lebrice/SimpleParsing/issues/227"""
 
     # Solution: register a decoding function for `int` that casts to int, but raises an error if
     # the value would lose precision.
 
     def _safe_cast(v: Any) -> int:
@@ -208,16 +245,14 @@
                 use_log: 1
                 severity: 1
                 probs: [0.2, 0.3]
             """
             )
         )
 
-    register_decoding_fn(int, int, overwrite=True)
-
 
 @pytest.mark.xfail(strict=True, match="DID NOT RAISE <class 'ValueError'>")
 def test_optional_list_type_doesnt_use_type_decoding_fn():
     """BUG: Parsing an Optional[list[int]] doesn't work correctly."""
 
     def _safe_cast(v: Any) -> int:
         int_v = int(v)
@@ -230,8 +265,58 @@
     with pytest.raises(ValueError):
         get_decoding_fn(List[int])([0.1, 0.2])
 
     # BUG: This doesn't work correctly.
     with pytest.raises(ValueError):
         get_decoding_fn(Optional[List[int]])([0.1, 0.2])
 
-    register_decoding_fn(int, int, overwrite=True)
+
+@dataclass
+class ClassWithInt:
+    a: int = 1
+
+
+@dataclass
+class ClassWithIntList:
+    values: List[int] = field(default_factory=[1, 2, 3].copy)
+
+
+@pytest.mark.parametrize(
+    ("class_to_use", "serialized_dict", "expected_message", "expected_result"),
+    [
+        pytest.param(
+            ClassWithInt,
+            {"a": 1.1},
+            r"Unsafe casting occurred when deserializing field 'a' of type <class 'int'>: raw value: 1.1, decoded value: 1",
+            ClassWithInt(a=int(1.1)),
+            id="float to int",
+        ),
+        pytest.param(
+            ClassWithInt,
+            {"a": True},
+            r"Unsafe casting occurred when deserializing field 'a' of type <class 'int'>: raw value: True, decoded value: 1",
+            ClassWithInt(a=int(True)),
+            id="bool to int",
+        ),
+        pytest.param(
+            ClassWithIntList,
+            {"values": [1.1, 2.2, 3.3]},
+            r"Unsafe casting occurred when deserializing field 'values' of type typing.List\[int\]: raw value: \[1.1, 2.2, 3.3\], decoded value: \[1, 2, 3\].",
+            ClassWithIntList(values=[int(1.1), int(2.2), int(3.3)]),
+            id="List of floats",
+        ),
+    ],
+)
+def test_issue_227_unsafe_int_casting_on_load(
+    class_to_use: Type[DataclassT],
+    serialized_dict: dict,
+    expected_message: str,
+    expected_result: DataclassT,
+):
+    """Test that a warning is raised when performing a lossy cast when deserializing a dataclass."""
+    with pytest.warns(
+        RuntimeWarning,
+        match=expected_message,
+    ) as record:
+        obj = loads_json(class_to_use, json.dumps(serialized_dict))
+        assert obj == expected_result
+    assert len(record.list) == 1
```

### Comparing `simple_parsing-0.1.1/test/test_decorator.py` & `simple_parsing-0.1.2/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_default_args.py` & `simple_parsing-0.1.2/test/test_default_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_docstrings.py` & `simple_parsing-0.1.2/test/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_examples.py` & `simple_parsing-0.1.2/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_fields.py` & `simple_parsing-0.1.2/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_forward_ref.py` & `simple_parsing-0.1.2/test/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_future_annotations.py` & `simple_parsing-0.1.2/test/test_future_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_generation_mode.py` & `simple_parsing-0.1.2/test/test_generation_mode.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_huggingface_compat.py` & `simple_parsing-0.1.2/test/test_huggingface_compat.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_inheritance.py` & `simple_parsing-0.1.2/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_initvar.py` & `simple_parsing-0.1.2/test/test_initvar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue64.py` & `simple_parsing-0.1.2/test/test_issue64.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_107.py` & `simple_parsing-0.1.2/test/test_issue_107.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_132.py` & `simple_parsing-0.1.2/test/test_issue_132.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_144.py` & `simple_parsing-0.1.2/test/test_issue_144.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_46.py` & `simple_parsing-0.1.2/test/test_issue_46.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_48.py` & `simple_parsing-0.1.2/test/test_issue_48.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_issue_96.py` & `simple_parsing-0.1.2/test/test_issue_96.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_lists.py` & `simple_parsing-0.1.2/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_literal.py` & `simple_parsing-0.1.2/test/test_literal.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_multiple.py` & `simple_parsing-0.1.2/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_optional.py` & `simple_parsing-0.1.2/test/test_optional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_optional_subparsers.py` & `simple_parsing-0.1.2/test/test_optional_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_positional.py` & `simple_parsing-0.1.2/test/test_positional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_replace.py` & `simple_parsing-0.1.2/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_set_defaults.py` & `simple_parsing-0.1.2/test/test_set_defaults.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_subgroups.py` & `simple_parsing-0.1.2/test/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_subparsers.py` & `simple_parsing-0.1.2/test/test_subparsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import dataclasses
 from argparse import Namespace
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Union
 
+import pytest
+
 import simple_parsing
 from simple_parsing import ArgumentParser, choice
 from simple_parsing.helpers import subparsers
 
 from .testutils import TestSetup, raises, xfail
 
 
@@ -287,14 +289,15 @@
     args = parser.parse_args("--foo 1 boo --bar 2 --baz 3".split())
     assert args == Namespace(foo=1, bar=2, baz=3)
 
     args = parser.parse_known_args("boo --bar 2 --baz 3 --foo 1".split())
     assert args == (Namespace(foo=3, bar=2, baz=3), ["--foo", "1"])
 
 
+@pytest.mark.filterwarnings("ignore:Unparsed arguments")
 def test_simpleparse_version_giving_extra_args_to_parent():
     parser = simple_parsing.ArgumentParser()
     parser.add_argument("--foo", type=int, default=3)
     assert not parser._subparsers
     subparsers = parser.add_subparsers(title="foo_command")
 
     subparser = subparsers.add_parser("boo")
```

### Comparing `simple_parsing-0.1.1/test/test_suppress.py` & `simple_parsing-0.1.2/test/test_suppress.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_tuples.py` & `simple_parsing-0.1.2/test/test_tuples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_union.py` & `simple_parsing-0.1.2/test/test_union.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/test_utils.py` & `simple_parsing-0.1.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/test/testutils.py` & `simple_parsing-0.1.2/test/testutils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.1/versioneer.py` & `simple_parsing-0.1.2/versioneer.py`

 * *Files identical despite different names*

