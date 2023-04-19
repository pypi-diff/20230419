# Comparing `tmp/dbt-artifacts-parser-0.2.5.tar.gz` & `tmp/dbt-artifacts-parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-artifacts-parser-0.2.5.tar", last modified: Thu Mar  9 13:32:28 2023, max compression
+gzip compressed data, was "dbt-artifacts-parser-0.3.0.tar", last modified: Wed Apr 19 10:29:21 2023, max compression
```

## Comparing `dbt-artifacts-parser-0.2.5.tar` & `dbt-artifacts-parser-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,90 @@
--rw-r--r--   0        0        0      804 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1824 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2319 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1158 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1896 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.gitignore
--rw-r--r--   0        0        0    14055 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.pylintrc
--rw-r--r--   0        0        0      150 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.pypirc
--rw-r--r--   0        0        0       32 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/.style.yapf
--rw-r--r--   0        0        0    11357 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/LICENSE
--rw-r--r--   0        0        0      159 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/MANIFEST.in
--rw-r--r--   0        0        0      749 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/Makefile
--rw-r--r--   0        0        0     8681 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/README.md
--rw-r--r--   0        0        0      859 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    10980 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    40546 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47751 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48519 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52861 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35031 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     4102 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   135379 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138301 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157234 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159202 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163790 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   115570 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0     4622 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9816 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10271 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     5568 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6789 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7248 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/utils.py
--rwxr-xr-x   0        0        0     1121 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/clean.sh
--rwxr-xr-x   0        0        0     1021 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/format_python.sh
--rw-r--r--   0        0        0     3157 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/generate_parser_classes.sh
--rw-r--r--   0        0        0      978 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/dev/test_python.sh
--rw-r--r--   0        0        0     1518 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      830 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/setup.py
--rw-r--r--   0        0        0      792 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      796 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/parsers/__init__.py
--rw-r--r--   0        0        0     6001 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/parsers/test_utils.py
--rw-r--r--   0        0        0    11587 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/catalog.json
--rw-r--r--   0        0        0   226551 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/manifest.json
--rw-r--r--   0        0        0     4688 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   265840 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v2/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15168 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v2/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   289190 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v3/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15738 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v3/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   269797 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v4/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    14576 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v4/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   817922 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v5/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   352436 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v6/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   412717 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v7/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   394308 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v8/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   401315 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json
--rw-r--r--   0        0        0      938 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/test_basic.py
--rw-r--r--   0        0        0     6555 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/test_parser.py
--rw-r--r--   0        0        0     1090 2023-03-09 13:32:28.000000 dbt-artifacts-parser-0.2.5/tests/test_utils.py
--rw-r--r--   0        0        0    10407 1970-01-01 00:00:00.000000 dbt-artifacts-parser-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1824 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2319 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1158 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1896 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1371 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14055 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pypirc
+-rw-r--r--   0        0        0       32 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0      159 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      879 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/Makefile
+-rw-r--r--   0        0        0     8681 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/README.md
+-rw-r--r--   0        0        0      859 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    11501 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    39709 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    40546 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    41294 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    46633 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    47751 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    48519 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    52861 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    35031 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    39455 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1719 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1755 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3346 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3458 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2044 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2327 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2441 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     4274 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   135379 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138301 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157234 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159202 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163790 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9816 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10271 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     5568 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6789 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7248 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/utils.py
+-rwxr-xr-x   0        0        0     1121 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/clean.sh
+-rwxr-xr-x   0        0        0     1021 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/format_python.sh
+-rw-r--r--   0        0        0     3162 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/generate_parser_classes.sh
+-rw-r--r--   0        0        0      978 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1391 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/publish.sh
+-rwxr-xr-x   0        0        0     1023 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/test_python.sh
+-rw-r--r--   0        0        0     1545 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/setup.py
+-rw-r--r--   0        0        0      792 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     6001 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/parsers/test_utils.py
+-rw-r--r--   0        0        0    11587 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/catalog.json
+-rw-r--r--   0        0        0   226551 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0     4688 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   265840 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    15168 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   289190 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    15738 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   269797 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    14576 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   817922 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v5/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   352436 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v6/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   412717 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v7/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   394308 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   401315 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json
+-rw-r--r--   0        0        0  1234064 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json
+-rw-r--r--   0        0        0      938 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_basic.py
+-rw-r--r--   0        0        0     6671 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_parser.py
+-rw-r--r--   0        0        0     1090 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0    10459 1970-01-01 00:00:00.000000 dbt-artifacts-parser-0.3.0/PKG-INFO
```

### Comparing `dbt-artifacts-parser-0.2.5/.github/CODEOWNERS` & `dbt-artifacts-parser-0.3.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/.github/workflows/publish.yml` & `dbt-artifacts-parser-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/.github/workflows/test-publish.yml` & `dbt-artifacts-parser-0.3.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/.github/workflows/test.yml` & `dbt-artifacts-parser-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/.gitignore` & `dbt-artifacts-parser-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/.pylintrc` & `dbt-artifacts-parser-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/LICENSE` & `dbt-artifacts-parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/Makefile` & `dbt-artifacts-parser-0.3.0/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Set up an environment
 .PHONEY: setup
-setup:
+setup: setup-python setup-pre-commit
+
+.PHONE: setup-python
+setup-python:
 	bash ./dev/setup.sh
 
+.PHONE: setup-pre-commit
+setup-pre-commit:
+	pre-commit install
+
 # Check all the coding style.
 .PHONY: lint
 lint: lint-shell lint-python
 
 # Check the coding style for the shell scripts.
 .PHONY: lint-shell
 lint-shell:
```

### Comparing `dbt-artifacts-parser-0.2.5/README.md` & `dbt-artifacts-parser-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.2.5"
+__version__ = "0.3.0"
```

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parser.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from typing import Union
 
-from dbt_artifacts_parser.parsers.utils import get_dbt_schema_version
-
 from dbt_artifacts_parser.parsers.catalog.catalog_v1 import CatalogV1
 from dbt_artifacts_parser.parsers.manifest.manifest_v1 import ManifestV1
 from dbt_artifacts_parser.parsers.manifest.manifest_v2 import ManifestV2
 from dbt_artifacts_parser.parsers.manifest.manifest_v3 import ManifestV3
 from dbt_artifacts_parser.parsers.manifest.manifest_v4 import ManifestV4
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ManifestV5
 from dbt_artifacts_parser.parsers.manifest.manifest_v6 import ManifestV6
 from dbt_artifacts_parser.parsers.manifest.manifest_v7 import ManifestV7
 from dbt_artifacts_parser.parsers.manifest.manifest_v8 import ManifestV8
+from dbt_artifacts_parser.parsers.manifest.manifest_v9 import ManifestV9
 from dbt_artifacts_parser.parsers.run_results.run_results_v1 import RunResultsV1
 from dbt_artifacts_parser.parsers.run_results.run_results_v2 import RunResultsV2
 from dbt_artifacts_parser.parsers.run_results.run_results_v3 import RunResultsV3
 from dbt_artifacts_parser.parsers.run_results.run_results_v4 import RunResultsV4
 from dbt_artifacts_parser.parsers.sources.sources_v1 import SourcesV1
 from dbt_artifacts_parser.parsers.sources.sources_v2 import SourcesV2
 from dbt_artifacts_parser.parsers.sources.sources_v3 import SourcesV3
-
+from dbt_artifacts_parser.parsers.utils import get_dbt_schema_version
 from dbt_artifacts_parser.parsers.version_map import ArtifactTypes
 
 
 #
 # catalog
 #
 def parse_catalog(catalog: dict) -> Union[CatalogV1]:
@@ -92,14 +91,16 @@
         return ManifestV5(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V6.value.dbt_schema_version:
         return ManifestV6(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V7.value.dbt_schema_version:
         return ManifestV7(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V8.value.dbt_schema_version:
         return ManifestV8(**manifest)
+    elif dbt_schema_version == ArtifactTypes.MANIFEST_V9.value.dbt_schema_version:
+        return ManifestV9(**manifest)
     raise ValueError("Not a soft of manifest.json")
 
 
 def parse_manifest_v1(manifest: dict) -> ManifestV1:
     """Parse manifest.json ver.1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V1.value.dbt_schema_version:
@@ -159,14 +160,22 @@
     """Parse manifest.json ver.8"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V8.value.dbt_schema_version:
         return ManifestV8(**manifest)
     raise ValueError("Not a manifest.json v8")
 
 
+def parse_manifest_v9(manifest: dict) -> ManifestV6:
+    """Parse manifest.json ver.9"""
+    dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
+    if dbt_schema_version == ArtifactTypes.MANIFEST_V9.value.dbt_schema_version:
+        return ManifestV9(**manifest)
+    raise ValueError("Not a manifest.json v9")
+
+
 #
 # run-results
 #
 def parse_run_results(
     run_results: dict
 ) -> Union[RunResultsV1, RunResultsV2, RunResultsV3, RunResultsV4]:
     """Parse run-results.json
```

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/base.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v2.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v3.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v4.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v5.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v6.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v7.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/manifest/manifest_v8.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/sources/sources_v3.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/utils.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/parsers/version_map.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/version_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,36 +10,33 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from typing import Type
-from enum import Enum
 from dataclasses import dataclass
+from enum import Enum
+from typing import Type
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
-
 from dbt_artifacts_parser.parsers.catalog.catalog_v1 import CatalogV1
-
 from dbt_artifacts_parser.parsers.manifest.manifest_v1 import ManifestV1
 from dbt_artifacts_parser.parsers.manifest.manifest_v2 import ManifestV2
 from dbt_artifacts_parser.parsers.manifest.manifest_v3 import ManifestV3
 from dbt_artifacts_parser.parsers.manifest.manifest_v4 import ManifestV4
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ManifestV5
 from dbt_artifacts_parser.parsers.manifest.manifest_v6 import ManifestV6
 from dbt_artifacts_parser.parsers.manifest.manifest_v7 import ManifestV7
 from dbt_artifacts_parser.parsers.manifest.manifest_v8 import ManifestV8
-
+from dbt_artifacts_parser.parsers.manifest.manifest_v9 import ManifestV9
 from dbt_artifacts_parser.parsers.run_results.run_results_v1 import RunResultsV1
 from dbt_artifacts_parser.parsers.run_results.run_results_v2 import RunResultsV2
 from dbt_artifacts_parser.parsers.run_results.run_results_v3 import RunResultsV3
 from dbt_artifacts_parser.parsers.run_results.run_results_v4 import RunResultsV4
-
 from dbt_artifacts_parser.parsers.sources.sources_v1 import SourcesV1
 from dbt_artifacts_parser.parsers.sources.sources_v2 import SourcesV2
 from dbt_artifacts_parser.parsers.sources.sources_v3 import SourcesV3
 
 
 @dataclass
 class ArtifactType:
@@ -65,14 +62,16 @@
         "https://schemas.getdbt.com/dbt/manifest/v5.json", ManifestV5)
     MANIFEST_V6 = ArtifactType(
         "https://schemas.getdbt.com/dbt/manifest/v6.json", ManifestV6)
     MANIFEST_V7 = ArtifactType(
         "https://schemas.getdbt.com/dbt/manifest/v7.json", ManifestV7)
     MANIFEST_V8 = ArtifactType(
         "https://schemas.getdbt.com/dbt/manifest/v8.json", ManifestV8)
+    MANIFEST_V9 = ArtifactType(
+        "https://schemas.getdbt.com/dbt/manifest/v9.json", ManifestV9)
     # RunResults
     RUN_RESULTS_V1 = ArtifactType(
         "https://schemas.getdbt.com/dbt/run-results/v1.json", RunResultsV1)
     RUN_RESULTS_V2 = ArtifactType(
         "https://schemas.getdbt.com/dbt/run-results/v2.json", RunResultsV2)
     RUN_RESULTS_V3 = ArtifactType(
         "https://schemas.getdbt.com/dbt/run-results/v3.json", RunResultsV3)
```

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dbt_artifacts_parser/utils.py` & `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/clean.sh` & `dbt-artifacts-parser-0.3.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/format_python.sh` & `dbt-artifacts-parser-0.3.0/dev/format_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/generate_parser_classes.sh` & `dbt-artifacts-parser-0.3.0/dev/generate_parser_classes.sh`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     --input "${MODULE_ROOT}/dbt_artifacts_parser/resources/catalog/catalog_${ver}.json" \
     --output "${destination}"
 done
 
 #
 # manifest
 #
-manifest_versions=("v1" "v2" "v3" "v4" "v5" "v6" "v7" "v8")
+manifest_versions=("v1" "v2" "v3" "v4" "v5" "v6" "v7" "v8" "v9")
 for ver in "${manifest_versions[@]}"
 do
   # Convert `v1` to `V1`
   upper_ver=${ver^v}
   destination="${MODULE_ROOT}/dbt_artifacts_parser/parsers/manifest/manifest_${ver}.py"
   echo "Generate ${destination}"
   datamodel-codegen  --input-file-type jsonschema \
```

### Comparing `dbt-artifacts-parser-0.2.5/dev/lint_python.sh` & `dbt-artifacts-parser-0.3.0/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/publish.sh` & `dbt-artifacts-parser-0.3.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/setup.sh` & `dbt-artifacts-parser-0.3.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/dev/test_python.sh` & `dbt-artifacts-parser-0.3.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/pyproject.toml` & `dbt-artifacts-parser-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -49,8 +49,9 @@
 ]
 dev = [
     "flit ==3.7.1",
     "build ==0.7.0",
     "yapf >=0.29.0",
     "pyyaml >=5.3",
     "pdoc3 >=0.9.2",
+    "pre-commit >=2.15.0",
 ]
```

### Comparing `dbt-artifacts-parser-0.2.5/setup.py` & `dbt-artifacts-parser-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/__init__.py` & `dbt-artifacts-parser-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/parsers/__init__.py` & `dbt-artifacts-parser-0.3.0/tests/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/parsers/test_utils.py` & `dbt-artifacts-parser-0.3.0/tests/parsers/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/catalog.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/catalog.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v1/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v2/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v2/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v3/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v3/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v4/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v4/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v5/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v5/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v6/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v6/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v7/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v7/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v8/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json` & `dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/test_basic.py` & `dbt-artifacts-parser-0.3.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/tests/test_parser.py` & `dbt-artifacts-parser-0.3.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import os
-import yaml
 
 import pytest
+import yaml
 
 from dbt_artifacts_parser import parser
 from dbt_artifacts_parser.utils import get_project_root
 
 
 @pytest.mark.parametrize("version", ["v1"])
 class TestCatalogParser:
@@ -66,14 +66,15 @@
     ("v3", os.path.join(get_project_root(), "tests", "resources", "v3", "jaffle_shop", "manifest.json")),
     ("v4", os.path.join(get_project_root(), "tests", "resources", "v4", "jaffle_shop", "manifest.json")),
     ("v5", os.path.join(get_project_root(), "tests", "resources", "v5", "jaffle_shop", "manifest.json")),
     ("v6", os.path.join(get_project_root(), "tests", "resources", "v6", "jaffle_shop", "manifest.json")),
     ("v7", os.path.join(get_project_root(), "tests", "resources", "v7", "jaffle_shop", "manifest.json")),
     ("v8", os.path.join(get_project_root(), "tests", "resources", "v8", "jaffle_shop", "manifest.json")),
     ("v8", os.path.join(get_project_root(), "tests", "resources", "v8", "jaffle_shop_at_1_4_3", "manifest.json")),
+    ("v9", os.path.join(get_project_root(), "tests", "resources", "v9", "jaffle_shop_at_1.5rc1", "manifest.json")),
 ])
 class TestManifestParser:
     def test_parse_manifest(self, version, path):
         with open(path, "r", encoding="utf-8") as fp:
             manifest_dict = yaml.safe_load(fp)
             manifest_obj = parser.parse_manifest(manifest_dict)
         assert (
```

### Comparing `dbt-artifacts-parser-0.2.5/tests/test_utils.py` & `dbt-artifacts-parser-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.2.5/PKG-INFO` & `dbt-artifacts-parser-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.2.5
+Version: 0.3.0
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -23,14 +23,15 @@
 Requires-Dist: pydantic >=1.6
 Requires-Dist: datamodel-code-generator >=0.12.0
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
+Requires-Dist: pre-commit >=2.15.0 ; extra == "dev"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
 Requires-Dist: pylint >=2.12.0 ; extra == "test"
 Requires-Dist: mypy ==0.910 ; extra == "test"
 Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
 Requires-Dist: black ==21.9b0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
 Requires-Dist: yapf >=0.29.0 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.2.5 Summary: A dbt
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.3.0 Summary: A dbt
 artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
@@ -10,47 +10,47 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Typing :: Typed Requires-Dist: pydantic >=1.6
 Requires-Dist: datamodel-code-generator >=0.12.0 Requires-Dist: flit ==3.7.1 ;
 extra == "dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist:
 yapf >=0.29.0 ; extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev"
-Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pytest
->=6.2.4,<7.0.0 ; extra == "test" Requires-Dist: pylint >=2.12.0 ; extra ==
-"test" Requires-Dist: mypy ==0.910 ; extra == "test" Requires-Dist: flake8
->=3.8.3,<4.0.0 ; extra == "test" Requires-Dist: black ==21.9b0 ; extra ==
-"test" Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test" Requires-Dist:
-yapf >=0.29.0 ; extra == "test" Project-URL: Home, https://github.com/yu-iskw/
-dbt-artifacts-parser Provides-Extra: dev Provides-Extra: test [![Test python]
-(https://github.com/yu-iskw/dbt-artifacts-parser/actions/workflows/test.yml/
-badge.svg)](https://github.com/yu-iskw/dbt-artifacts-parser/actions/workflows/
-test.yml) [Package_version] [Supported_Python_versions] # dbt-artifacts-parser
-This is a dbt artifacts parse in python. It enables us to deal with
-`catalog.json`, `manifest.json`, `run-results.json` and `sources.json` as
-python objects. ## Installation ```bash pip install -U dbt-artifacts-parser ```
-## Python classes Those are the classes to parse dbt artifacts. ### Catalog -
-[CatalogV1](dbt_artifacts_parser/parsers/catalog/catalog_v1.py) for
-catalog.json v1 ### Manifest - [ManifestV1](dbt_artifacts_parser/parsers/
-manifest/manifest_v1.py) for manifest.json v1 - [ManifestV2]
-(dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for manifest.json v2 -
-[ManifestV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for
-manifest.json v3 - [ManifestV4](dbt_artifacts_parser/parsers/manifest/
-manifest_v4.py) for manifest.json v4 - [ManifestV5](dbt_artifacts_parser/
-parsers/manifest/manifest_v5.py) for manifest.json v5 - [ManifestV6]
-(dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6 -
-[ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for
-manifest.json v7 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/
-manifest_v8.py) for manifest.json v8 ### Run Results - [RunResultsV1]
-(dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
-- [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for
-run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/
-manifest_v3.py) for run_results.json v3 - [RunResultsV4](dbt_artifacts_parser/
-parsers/manifest/manifest_v4.py) for run_results.json v4 ### Sources -
-[SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py) for
-sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
+Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pre-commit
+>=2.15.0 ; extra == "dev" Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra ==
+"test" Requires-Dist: pylint >=2.12.0 ; extra == "test" Requires-Dist: mypy
+==0.910 ; extra == "test" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra ==
+"test" Requires-Dist: black ==21.9b0 ; extra == "test" Requires-Dist: isort
+>=5.0.6,<6.0.0 ; extra == "test" Requires-Dist: yapf >=0.29.0 ; extra == "test"
+Project-URL: Home, https://github.com/yu-iskw/dbt-artifacts-parser Provides-
+Extra: dev Provides-Extra: test [![Test python](https://github.com/yu-iskw/dbt-
+artifacts-parser/actions/workflows/test.yml/badge.svg)](https://github.com/yu-
+iskw/dbt-artifacts-parser/actions/workflows/test.yml) [Package_version]
+[Supported_Python_versions] # dbt-artifacts-parser This is a dbt artifacts
+parse in python. It enables us to deal with `catalog.json`, `manifest.json`,
+`run-results.json` and `sources.json` as python objects. ## Installation
+```bash pip install -U dbt-artifacts-parser ``` ## Python classes Those are the
+classes to parse dbt artifacts. ### Catalog - [CatalogV1](dbt_artifacts_parser/
+parsers/catalog/catalog_v1.py) for catalog.json v1 ### Manifest - [ManifestV1]
+(dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for manifest.json v1 -
+[ManifestV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for
+manifest.json v2 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/
+manifest_v3.py) for manifest.json v3 - [ManifestV4](dbt_artifacts_parser/
+parsers/manifest/manifest_v4.py) for manifest.json v4 - [ManifestV5]
+(dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5 -
+[ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for
+manifest.json v6 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/
+manifest_v7.py) for manifest.json v7 - [ManifestV8](dbt_artifacts_parser/
+parsers/manifest/manifest_v8.py) for manifest.json v8 ### Run Results -
+[RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for
+run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/
+manifest_v2.py) for run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/
+parsers/manifest/manifest_v3.py) for run_results.json v3 - [RunResultsV4]
+(dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
+### Sources - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py)
+for sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
 sources_v2.py) for sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/
 sources/sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json
 ```python import json # parse any version of catalog.json from
 dbt_artifacts_parser.parser import parse_catalog with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog(catalog=catalog_dict) # parse catalog.json v1 from
 dbt_artifacts_parser.parser import parse_catalog_v1 with open("path/to/
```

