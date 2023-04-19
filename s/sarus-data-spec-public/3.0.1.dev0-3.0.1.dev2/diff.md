# Comparing `tmp/sarus_data_spec_public-3.0.1.dev0.tar.gz` & `tmp/sarus_data_spec_public-3.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.0.1.dev0.tar", last modified: Mon Apr 17 16:16:48 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.0.1.dev2.tar", last modified: Wed Apr 19 07:18:40 2023, max compression
```

## Comparing `sarus_data_spec_public-3.0.1.dev0.tar` & `sarus_data_spec_public-3.0.1.dev2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.707583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.710583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5582 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     2795 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9709 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.711583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2744 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6687 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/routing.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3587 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.712583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18537 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.714583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12691 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.716584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4470 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.717584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28484 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.718584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8138 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.719584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.720584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.721584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.721584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.726585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15727 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.727585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28988 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    28830 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/protection_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     9271 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10449 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.732585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13739 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11529 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    10747 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6519 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    10991 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.733585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    12588 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.756588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    73431 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28800 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10611 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17816 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.758588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31051 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   136116 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6787 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4878 2023-04-17 16:16:48.761588 sarus_data_spec_public-3.0.1.dev0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.894037 sarus_data_spec_public-3.0.1.dev2/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-19 07:18:40.895038 sarus_data_spec_public-3.0.1.dev2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.845032 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.847032 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9709 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.848033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2744 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6687 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/routing.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.850033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18537 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.852033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.854033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4470 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.855033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28484 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.856033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8138 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.857033 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.858034 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.858034 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.859034 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.864034 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15727 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.865034 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28988 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    28830 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/protection_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     9271 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10449 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.869035 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13739 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11529 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10703 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    10747 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6519 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.871035 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    12588 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.891037 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    73431 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28800 2023-04-19 07:18:30.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10611 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17816 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.892037 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:18:40.894037 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6787 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 07:18:40.000000 sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4878 2023-04-19 07:18:40.896038 sarus_data_spec_public-3.0.1.dev2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-04-19 07:18:17.000000 sarus_data_spec_public-3.0.1.dev2/setup.py
```

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.0.1.dev0'
+VERSION: Final[str] = '3.0.1.dev2'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.DataFrame:
     arrow_batches = [batch async for batch in batches_async_iterator]
     # follow advices in
     # https://arrow.apache.org/docs/python/pandas.html#reducing
     # -memory-use-in-table-to-pandas
     tab = pa.Table.from_batches(arrow_batches)
-    df = tab.to_pandas(split_blocks=True, self_destruct=True)
+    df = tab.to_pandas(split_blocks=False, self_destruct=True)
     del tab  # not necessary, but a good practice
     return df
 
 
 async def async_arrow_batches_to_series(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
```

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/__init__.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/routing.yaml` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/config/routing.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/protection_utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/protection_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/signature.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/path.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/size.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/status.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/type.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.0.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/setup.cfg` & `sarus_data_spec_public-3.0.1.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.1.dev0/setup.py` & `sarus_data_spec_public-3.0.1.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.0.1.dev0')
+    setup(version='3.0.1.dev2')
```

