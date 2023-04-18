# Comparing `tmp/kolena_client-0.0.1.tar.gz` & `tmp/kolena_client-0.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.0.1.tar", max compression
+gzip compressed data, was "kolena_client-0.64.0.tar", max compression
```

## Comparing `kolena_client-0.0.1.tar` & `kolena_client-0.64.0.tar`

### file list

```diff
@@ -1,4 +1,105 @@
--rw-r--r--   0        0        0       30 2023-03-30 20:02:31.319969 kolena_client-0.0.1/README.md
--rw-r--r--   0        0        0       39 2023-03-30 20:03:59.384846 kolena_client-0.0.1/kolena/hi.py
--rw-r--r--   0        0        0      306 2023-03-30 20:03:16.633655 kolena_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 kolena_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-18 22:03:41.350605 kolena_client-0.64.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-04-18 22:03:41.350605 kolena_client-0.64.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1492 2023-04-18 22:03:41.350605 kolena_client-0.64.0/README.md
+-rw-r--r--   0        0        0     1356 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1725 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     7578 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7480 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5507 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      690 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/samples.py
+-rw-r--r--   0        0        0      833 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0      784 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/_consts.py
+-rw-r--r--   0        0        0     1604 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     6883 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     2774 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1260 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/futures.py
+-rw-r--r--   0        0        0     1183 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2646 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4161 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0      997 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     4768 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     6672 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/stratification.py
+-rw-r--r--   0        0        0     1942 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3005 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    14006 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3578 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     2541 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4138 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8415 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13650 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    12938 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     4707 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0      689 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/_consts.py
+-rw-r--r--   0        0        0    20512 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9248 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14560 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12177 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    17008 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15219 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     4134 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4454 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     6423 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    14664 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0     9312 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      625 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2738 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7436 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13248 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22814 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     8817 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    11379 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9293 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     1927 2023-04-18 22:03:53.818579 kolena_client-0.64.0/pyproject.toml
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 kolena_client-0.64.0/setup.py
+-rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 kolena_client-0.64.0/PKG-INFO
```

