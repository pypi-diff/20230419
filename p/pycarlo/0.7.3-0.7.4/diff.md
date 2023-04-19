# Comparing `tmp/pycarlo-0.7.3.tar.gz` & `tmp/pycarlo-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycarlo-0.7.3.tar", last modified: Thu Apr  6 20:47:30 2023, max compression
+gzip compressed data, was "dist/pycarlo-0.7.4.tar", last modified: Wed Apr 19 19:05:46 2023, max compression
```

## Comparing `pycarlo-0.7.3.tar` & `pycarlo-0.7.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:30.002324 pycarlo-0.7.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.986324 pycarlo-0.7.3/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-06 20:47:14.000000 pycarlo-0.7.3/.circleci/README.md
--rw-r--r--   0 root         (0) root         (0)     3101 2023-04-06 20:47:14.000000 pycarlo-0.7.3/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.986324 pycarlo-0.7.3/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-04-06 20:47:14.000000 pycarlo-0.7.3/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-06 20:47:14.000000 pycarlo-0.7.3/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1832 2023-04-06 20:47:14.000000 pycarlo-0.7.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-06 20:47:14.000000 pycarlo-0.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1986 2023-04-06 20:47:14.000000 pycarlo-0.7.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     7803 2023-04-06 20:47:30.002324 pycarlo-0.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7026 2023-04-06 20:47:14.000000 pycarlo-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/examples/
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-06 20:47:14.000000 pycarlo-0.7.3/examples/sample_circuit_breaker.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-06 20:47:14.000000 pycarlo-0.7.3/examples/sample_insight_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/common/
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/errors.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/files.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/http.py
--rw-r--r--   0 root         (0) root         (0)      622 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/mcon.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/retries.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/settings.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/core/
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/core/client.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/core/endpoint.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/core/operations.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/core/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/features/
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/features/circuit_breakers/
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/circuit_breakers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/circuit_breakers/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    11391 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/circuit_breakers/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo/features/dbt/
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/dbt/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17849 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/dbt/dbt_importer.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/dbt/queries.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.994324 pycarlo-0.7.3/pycarlo/features/metadata/
--rw-r--r--   0 root         (0) root         (0)      206 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/metadata/allow_block_list.py
--rw-r--r--   0 root         (0) root         (0)    11893 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/metadata/metadata_filters_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.994324 pycarlo-0.7.3/pycarlo/features/pii/
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/pii/__init__.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/pii/constants.py
--rw-r--r--   0 root         (0) root         (0)     6051 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/pii/pii_filterer.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/pii/queries.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/pii/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.994324 pycarlo-0.7.3/pycarlo/features/user/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/user/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/user/models.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/user/queries.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/features/user/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.994324 pycarlo-0.7.3/pycarlo/lib/
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/lib/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2587692 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/lib/schema.json
--rw-r--r--   0 root         (0) root         (0)   927818 2023-04-06 20:47:14.000000 pycarlo-0.7.3/pycarlo/lib/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.990324 pycarlo-0.7.3/pycarlo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7803 2023-04-06 20:47:29.000000 pycarlo-0.7.3/pycarlo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2554 2023-04-06 20:47:29.000000 pycarlo-0.7.3/pycarlo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 20:47:29.000000 pycarlo-0.7.3/pycarlo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-06 20:47:29.000000 pycarlo-0.7.3/pycarlo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-06 20:47:29.000000 pycarlo-0.7.3/pycarlo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-06 20:47:14.000000 pycarlo-0.7.3/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-06 20:47:14.000000 pycarlo-0.7.3/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-06 20:47:14.000000 pycarlo-0.7.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-06 20:47:30.002324 pycarlo-0.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1477 2023-04-06 20:47:14.000000 pycarlo-0.7.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/common/data.json
--rw-r--r--   0 root         (0) root         (0)      912 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/common/test_files.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/common/test_http.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/common/test_mcon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/features/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/features/circuit_breakers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/circuit_breakers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/circuit_breakers/test_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/features/dbt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/dbt/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/dbt/sample_logs.txt
--rw-r--r--   0 root         (0) root         (0)    16826 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/dbt/sample_manifest.json
--rw-r--r--   0 root         (0) root         (0)     3237 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/dbt/sample_run_results.json
--rw-r--r--   0 root         (0) root         (0)    15115 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/dbt/test_dbt_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/features/metadata/
--rw-r--r--   0 root         (0) root         (0)    15717 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/metadata/test_dataset_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:29.998324 pycarlo-0.7.3/tests/features/pii/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:30.002324 pycarlo-0.7.3/tests/features/pii/sample_events/
--rw-r--r--   0 root         (0) root         (0)  1638574 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/pii/sample_events/sample_md_events_01.json
--rw-r--r--   0 root         (0) root         (0)   125065 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/pii/sample_events/sample_md_events_02.json
--rw-r--r--   0 root         (0) root         (0)    11340 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/pii/test_pii_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:30.002324 pycarlo-0.7.3/tests/features/user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/features/user/test_user_service.py
--rw-r--r--   0 root         (0) root         (0)    10305 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/test_operations.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/test_retry_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-04-06 20:47:14.000000 pycarlo-0.7.3/tests/test_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:47:30.002324 pycarlo-0.7.3/utils/
--rw-r--r--   0 root         (0) root         (0)      565 2023-04-06 20:47:14.000000 pycarlo-0.7.3/utils/env.sh
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-06 20:47:14.000000 pycarlo-0.7.3/utils/generate.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-06 20:47:14.000000 pycarlo-0.7.3/utils/sample.env
--rw-r--r--   0 root         (0) root         (0)     1759 2023-04-06 20:47:14.000000 pycarlo-0.7.3/utils/sanity.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-06 20:47:14.000000 pycarlo-0.7.3/utils/vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.419406 pycarlo-0.7.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.403406 pycarlo-0.7.4/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-19 19:05:27.000000 pycarlo-0.7.4/.circleci/README.md
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-04-19 19:05:27.000000 pycarlo-0.7.4/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.403406 pycarlo-0.7.4/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-04-19 19:05:27.000000 pycarlo-0.7.4/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 19:05:27.000000 pycarlo-0.7.4/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-04-19 19:05:27.000000 pycarlo-0.7.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 19:05:27.000000 pycarlo-0.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-04-19 19:05:27.000000 pycarlo-0.7.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-04-19 19:05:46.419406 pycarlo-0.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-04-19 19:05:27.000000 pycarlo-0.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.403406 pycarlo-0.7.4/examples/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-19 19:05:27.000000 pycarlo-0.7.4/examples/sample_circuit_breaker.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-19 19:05:27.000000 pycarlo-0.7.4/examples/sample_insight_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/common/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/files.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/http.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/mcon.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/retries.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/core/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/core/client.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/core/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/core/operations.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/core/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/features/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/features/circuit_breakers/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/circuit_breakers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/circuit_breakers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/circuit_breakers/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo/features/dbt/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17849 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/dbt/dbt_importer.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/dbt/queries.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.411406 pycarlo-0.7.4/pycarlo/features/metadata/
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/metadata/allow_block_list.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/metadata/metadata_filters_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.411406 pycarlo-0.7.4/pycarlo/features/pii/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/pii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/pii/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/pii/pii_filterer.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/pii/queries.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/pii/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.411406 pycarlo-0.7.4/pycarlo/features/user/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/user/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/user/models.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/user/queries.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/features/user/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/pycarlo/lib/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/lib/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2587692 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/lib/schema.json
+-rw-r--r--   0 root         (0) root         (0)   927818 2023-04-19 19:05:27.000000 pycarlo-0.7.4/pycarlo/lib/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.407406 pycarlo-0.7.4/pycarlo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-04-19 19:05:46.000000 pycarlo-0.7.4/pycarlo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-04-19 19:05:46.000000 pycarlo-0.7.4/pycarlo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:05:46.000000 pycarlo-0.7.4/pycarlo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 19:05:46.000000 pycarlo-0.7.4/pycarlo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:05:46.000000 pycarlo-0.7.4/pycarlo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-19 19:05:27.000000 pycarlo-0.7.4/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-19 19:05:27.000000 pycarlo-0.7.4/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 19:05:27.000000 pycarlo-0.7.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-19 19:05:46.419406 pycarlo-0.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-04-19 19:05:27.000000 pycarlo-0.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/common/data.json
+-rw-r--r--   0 root         (0) root         (0)      912 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/common/test_files.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/common/test_http.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/common/test_mcon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/features/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/features/circuit_breakers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/circuit_breakers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/circuit_breakers/test_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/features/dbt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/dbt/sample_logs.txt
+-rw-r--r--   0 root         (0) root         (0)    16826 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/dbt/sample_manifest.json
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/dbt/sample_run_results.json
+-rw-r--r--   0 root         (0) root         (0)    15115 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/dbt/test_dbt_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/features/metadata/
+-rw-r--r--   0 root         (0) root         (0)    18130 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/metadata/test_dataset_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.415406 pycarlo-0.7.4/tests/features/pii/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.419406 pycarlo-0.7.4/tests/features/pii/sample_events/
+-rw-r--r--   0 root         (0) root         (0)  1638574 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/pii/sample_events/sample_md_events_01.json
+-rw-r--r--   0 root         (0) root         (0)   125065 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/pii/sample_events/sample_md_events_02.json
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/pii/test_pii_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.419406 pycarlo-0.7.4/tests/features/user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/features/user/test_user_service.py
+-rw-r--r--   0 root         (0) root         (0)    10305 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/test_operations.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/test_retry_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-04-19 19:05:27.000000 pycarlo-0.7.4/tests/test_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:05:46.419406 pycarlo-0.7.4/utils/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-04-19 19:05:27.000000 pycarlo-0.7.4/utils/env.sh
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-19 19:05:27.000000 pycarlo-0.7.4/utils/generate.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-04-19 19:05:27.000000 pycarlo-0.7.4/utils/sample.env
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-04-19 19:05:27.000000 pycarlo-0.7.4/utils/sanity.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-19 19:05:27.000000 pycarlo-0.7.4/utils/vars.py
```

### Comparing `pycarlo-0.7.3/.circleci/config.yml` & `pycarlo-0.7.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/.gitignore` & `pycarlo-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/LICENSE` & `pycarlo-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/Makefile` & `pycarlo-0.7.4/Makefile`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/PKG-INFO` & `pycarlo-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycarlo
-Version: 0.7.3
+Version: 0.7.4
 Summary: Monte Carlo's Python SDK
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pycarlo-0.7.3/README.md` & `pycarlo-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/examples/sample_insight_upload.py` & `pycarlo-0.7.4/examples/sample_insight_upload.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/__init__.py` & `pycarlo-0.7.4/pycarlo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/errors.py` & `pycarlo-0.7.4/pycarlo/common/errors.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/files.py` & `pycarlo-0.7.4/pycarlo/common/files.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/http.py` & `pycarlo-0.7.4/pycarlo/common/http.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/mcon.py` & `pycarlo-0.7.4/pycarlo/common/mcon.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/retries.py` & `pycarlo-0.7.4/pycarlo/common/retries.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/settings.py` & `pycarlo-0.7.4/pycarlo/common/settings.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/common/utils.py` & `pycarlo-0.7.4/pycarlo/common/utils.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/core/client.py` & `pycarlo-0.7.4/pycarlo/core/client.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/core/endpoint.py` & `pycarlo-0.7.4/pycarlo/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/core/operations.py` & `pycarlo-0.7.4/pycarlo/core/operations.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/core/session.py` & `pycarlo-0.7.4/pycarlo/core/session.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/circuit_breakers/service.py` & `pycarlo-0.7.4/pycarlo/features/circuit_breakers/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/dbt/dbt_importer.py` & `pycarlo-0.7.4/pycarlo/features/dbt/dbt_importer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/dbt/queries.py` & `pycarlo-0.7.4/pycarlo/features/dbt/queries.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/metadata/allow_block_list.py` & `pycarlo-0.7.4/pycarlo/features/metadata/allow_block_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         # Field not specified on this object, e.g. self.dataset=None, which matches everything
         if component is None:
             return True
         # The value in kwargs is empty, it does not match the condition.
         if value is None:
             return False
 
+        # Convert it in lowercase. In the normalizer we are converting identifiers (like project/dataset) to lowercase
+        # so the metadata filters may be defined with lowercase on the UI, however on Snowflake the identifiers
+        # are usually in uppercase. Therefore, we perform the evaluation case-insensitive.
+        component = component.lower()
+        value = value.lower()
+
         if force_regexp or filter_type == FilterType.REGEXP:
             regexp = f'^{component}$'  # Anchor the regexp to be more strict about what to match.
             return re.match(regexp, value) is not None
         elif filter_type == FilterType.PREFIX:
             return value.startswith(component)
         else:
             return component == value
```

### Comparing `pycarlo-0.7.3/pycarlo/features/metadata/metadata_filters_container.py` & `pycarlo-0.7.4/pycarlo/features/metadata/metadata_filters_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,12 +203,16 @@
             conditions = other_effect_conditions
         return f'({conditions})' if conditions else ''
 
     @staticmethod
     def _get_sql_field_condition(mf: MetadataFilter,
                                  column_mapping: Dict,
                                  encoder: Callable[[str, FilterType, bool], str]):
+        # The comparison is performed case-insensitive (check MetadataFilter._safe_match)
+        # We can use LOWER here since it is part of standard SQL (like AND/OR/NOT), so including it here
+        # is a way to make sure that all comparisons are case-insensitive in the SQL sentences for all
+        # engines
         conditions = ' AND '.join([
-            encoder(column, getattr(mf, field), mf.type)
+            encoder(f"LOWER({column})", getattr(mf, field).lower(), mf.type)
             for (field, column) in column_mapping.items() if getattr(mf, field)
         ])
         return f'NOT({conditions})' if mf.effect == FilterEffectType.BLOCK else f'({conditions})'
```

### Comparing `pycarlo-0.7.3/pycarlo/features/pii/pii_filterer.py` & `pycarlo-0.7.4/pycarlo/features/pii/pii_filterer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/pii/service.py` & `pycarlo-0.7.4/pycarlo/features/pii/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/features/user/service.py` & `pycarlo-0.7.4/pycarlo/features/user/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/lib/schema.json` & `pycarlo-0.7.4/pycarlo/lib/schema.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo/lib/schema.py` & `pycarlo-0.7.4/pycarlo/lib/schema.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/pycarlo.egg-info/PKG-INFO` & `pycarlo-0.7.4/pycarlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycarlo
-Version: 0.7.3
+Version: 0.7.4
 Summary: Monte Carlo's Python SDK
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pycarlo-0.7.3/pycarlo.egg-info/SOURCES.txt` & `pycarlo-0.7.4/pycarlo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/setup.py` & `pycarlo-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/common/test_files.py` & `pycarlo-0.7.4/tests/common/test_files.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/common/test_http.py` & `pycarlo-0.7.4/tests/common/test_http.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/common/test_mcon.py` & `pycarlo-0.7.4/tests/common/test_mcon.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/circuit_breakers/test_service.py` & `pycarlo-0.7.4/tests/features/circuit_breakers/test_service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/dbt/sample_manifest.json` & `pycarlo-0.7.4/tests/features/dbt/sample_manifest.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/dbt/sample_run_results.json` & `pycarlo-0.7.4/tests/features/dbt/sample_run_results.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/dbt/test_dbt_importer.py` & `pycarlo-0.7.4/tests/features/dbt/test_dbt_importer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/metadata/test_dataset_filtering.py` & `pycarlo-0.7.4/tests/features/metadata/test_dataset_filtering.py`

 * *Files 18% similar despite different names*

```diff
@@ -157,28 +157,28 @@
         limits = MetadataFiltersContainer(metadata_filters=filters)
         self.assertTrue(limits.is_metadata_filtered)
 
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(NOT(database='project_2'))", conditions)
+        self.assertEqual("(NOT(LOWER(database)='project_2'))", conditions)
 
     def test_sql_query_block_project_prefix(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='prj_', type=FilterType.PREFIX, effect=FilterEffectType.BLOCK),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         self.assertTrue(limits.is_metadata_filtered)
 
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(NOT(database LIKE 'prj_%'))", conditions)
+        self.assertEqual("(NOT(LOWER(database) LIKE 'prj_%'))", conditions)
 
     def test_sql_query_block_project_dataset_prefix(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_name',
                            dataset='ds_',
                            type=FilterType.PREFIX,
                            effect=FilterEffectType.BLOCK
@@ -187,41 +187,41 @@
         limits = MetadataFiltersContainer(metadata_filters=filters)
         self.assertTrue(limits.is_metadata_filtered)
 
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(NOT(database LIKE 'project_name%' AND schema LIKE 'ds_%'))", conditions)
+        self.assertEqual("(NOT(LOWER(database) LIKE 'project_name%' AND LOWER(schema) LIKE 'ds_%'))", conditions)
 
     def test_sql_query_block_single_dataset(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2', dataset='dataset_1', effect=FilterEffectType.BLOCK),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(NOT(database='project_2' AND schema='dataset_1'))", conditions)
+        self.assertEqual("(NOT(LOWER(database)='project_2' AND LOWER(schema)='dataset_1'))", conditions)
 
     def test_sql_query_block_datasets_regexp(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2',
                            dataset='dataset_.+',
                            type=FilterType.REGEXP,
                            effect=FilterEffectType.BLOCK
                            ),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(NOT(database~'^(project_2)$' AND schema~'^(dataset_.+)$'))", conditions)
+        self.assertEqual("(NOT(LOWER(database)~'^(project_2)$' AND LOWER(schema)~'^(dataset_.+)$'))", conditions)
 
     def test_sql_query_block_datasets_regexp_with_exception(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2',
                            dataset='dataset_.+',
                            type=FilterType.REGEXP,
                            effect=FilterEffectType.BLOCK
@@ -232,16 +232,16 @@
                            ),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
-        self.assertEqual("(((database='project_2' AND schema='dataset_10')) OR "
-                         "(NOT(database~'^(project_2)$' AND schema~'^(dataset_.+)$')))", conditions)
+        self.assertEqual("(((LOWER(database)='project_2' AND LOWER(schema)='dataset_10')) OR "
+                         "(NOT(LOWER(database)~'^(project_2)$' AND LOWER(schema)~'^(dataset_.+)$')))", conditions)
 
     def test_sql_query_project_block_single_dataset(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2', dataset='dataset_1', effect=FilterEffectType.BLOCK),
             MetadataFilter(project='project_1', dataset='dataset_2', effect=FilterEffectType.BLOCK),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
@@ -249,15 +249,15 @@
             project='project_2',
             column_mapping={
                 'project': 'database',
                 'dataset': 'schema'
             },
             encoder=_redshift_encoder
         )
-        self.assertEqual("(NOT(database='project_2' AND schema='dataset_1'))", conditions)
+        self.assertEqual("(NOT(LOWER(database)='project_2' AND LOWER(schema)='dataset_1'))", conditions)
 
     def test_sql_query_project_block_nothing(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_1', dataset='dataset_2', effect=FilterEffectType.BLOCK),
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         self.assertFalse(limits.is_project_with_datasets_filtered('project_2'))
@@ -278,47 +278,93 @@
         ])
         limits = MetadataFiltersContainer(metadata_filters=filters)
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
         self.assertEqual("("
-                         "NOT(database='project_2' AND schema='dataset_1') AND "
-                         "NOT(database='project_1' AND schema='dataset_2')"
+                         "NOT(LOWER(database)='project_2' AND LOWER(schema)='dataset_1') AND "
+                         "NOT(LOWER(database)='project_1' AND LOWER(schema)='dataset_2')"
                          ")", conditions)
 
     def test_sql_query_allow_multi_datasets(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2', dataset='dataset_1', effect=FilterEffectType.ALLOW),
             MetadataFilter(project='project_1', dataset='dataset_2', effect=FilterEffectType.ALLOW),
         ], default_effect=FilterEffectType.BLOCK)
         limits = MetadataFiltersContainer(metadata_filters=filters)
         conditions = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
         self.assertEqual("("
-                         "(database='project_2' AND schema='dataset_1') OR "
-                         "(database='project_1' AND schema='dataset_2')"
+                         "(LOWER(database)='project_2' AND LOWER(schema)='dataset_1') OR "
+                         "(LOWER(database)='project_1' AND LOWER(schema)='dataset_2')"
                          ")", conditions)
 
+    def test_sql_query_block_case_insensitive(self):
+        filters = AllowBlockList(filters=[
+            MetadataFilter(project='SOME_PROJECT', effect=FilterEffectType.BLOCK, type=FilterType.EXACT_MATCH),
+            MetadataFilter(project='PROJECT_', effect=FilterEffectType.BLOCK, type=FilterType.PREFIX),
+            MetadataFilter(project='[A-Z]+[1-9]+', effect=FilterEffectType.BLOCK, type=FilterType.REGEXP),
+        ])
+        limits = MetadataFiltersContainer(metadata_filters=filters)
+        self.assertTrue(limits.is_metadata_filtered)
+
+        conditions = limits.get_sql_conditions({
+            'project': 'database',
+            'dataset': 'schema'
+        }, _redshift_encoder)
+        self.assertEqual("(NOT(LOWER(database)='some_project') AND "
+                         "NOT(LOWER(database) LIKE 'project_%') AND "
+                         "NOT(LOWER(database)~'^([a-z]+[1-9]+)$')"
+                         ")"
+                         , conditions)
+
     def test_whole_project_blocked(self):
         filters = AllowBlockList(filters=[
             MetadataFilter(project='project_2', dataset='dataset_1', effect=FilterEffectType.BLOCK),
         ], default_effect=FilterEffectType.BLOCK)
         limits = MetadataFiltersContainer(metadata_filters=filters)
         self.assertTrue(limits.is_metadata_blocked)
         self.assertTrue(limits.is_whole_project_blocked('project_2'))
 
         query = limits.get_sql_conditions({
             'project': 'database',
             'dataset': 'schema'
         }, _redshift_encoder)
         self.assertTrue(query)
 
+    def test_case_insensitive_comparison_exact_match(self):
+        filters = AllowBlockList(filters=[
+            MetadataFilter(project='project_2', effect=FilterEffectType.BLOCK, type=FilterType.EXACT_MATCH),
+        ])
+
+        limits = MetadataFiltersContainer(metadata_filters=filters)
+        self.assertTrue(limits.is_whole_project_blocked('PROJECT_2'))
+        self.assertFalse(limits.is_whole_project_blocked('PROJECT_3'))
+
+    def test_case_insensitive_comparison_prefix(self):
+        filters = AllowBlockList(filters=[
+            MetadataFilter(project='project_', effect=FilterEffectType.BLOCK, type=FilterType.PREFIX),
+        ])
+
+        limits = MetadataFiltersContainer(metadata_filters=filters)
+        self.assertTrue(limits.is_whole_project_blocked('PROJECT_1'))
+        self.assertFalse(limits.is_whole_project_blocked('OTHER_PROJECT'))
+
+    def test_case_insensitive_comparison_regex(self):
+        filters = AllowBlockList(filters=[
+            MetadataFilter(project='[a-z]+_[1-9]+', effect=FilterEffectType.BLOCK, type=FilterType.REGEXP),
+        ])
+
+        limits = MetadataFiltersContainer(metadata_filters=filters)
+        self.assertTrue(limits.is_whole_project_blocked('PROJECT_1'))
+        self.assertFalse(limits.is_whole_project_blocked('PROJECT_'))
+
     def _validate_allowed_datasets(self,
                                    filters: AllowBlockList,
                                    expected_datasets: List,
                                    datasets: Optional[List] = None
                           ) -> MetadataFiltersContainer:
         limits = MetadataFiltersContainer(metadata_filters=filters)
         filtered_datasets = self._filter_datasets(datasets or self.DATASETS, limits)
```

### Comparing `pycarlo-0.7.3/tests/features/pii/sample_events/sample_md_events_01.json` & `pycarlo-0.7.4/tests/features/pii/sample_events/sample_md_events_01.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/pii/sample_events/sample_md_events_02.json` & `pycarlo-0.7.4/tests/features/pii/sample_events/sample_md_events_02.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/pii/test_pii_filtering.py` & `pycarlo-0.7.4/tests/features/pii/test_pii_filtering.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/features/user/test_user_service.py` & `pycarlo-0.7.4/tests/features/user/test_user_service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/test_client.py` & `pycarlo-0.7.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/test_operations.py` & `pycarlo-0.7.4/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/test_retry_decorator.py` & `pycarlo-0.7.4/tests/test_retry_decorator.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/tests/test_session.py` & `pycarlo-0.7.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/utils/env.sh` & `pycarlo-0.7.4/utils/env.sh`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/utils/generate.py` & `pycarlo-0.7.4/utils/generate.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/utils/sanity.py` & `pycarlo-0.7.4/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.3/utils/vars.py` & `pycarlo-0.7.4/utils/vars.py`

 * *Files identical despite different names*

