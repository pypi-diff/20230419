# Comparing `tmp/cbcflow-0.1.2a4.tar.gz` & `tmp/cbcflow-0.1.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.1.2a4.tar", last modified: Tue Apr 18 03:42:04 2023, max compression
+gzip compressed data, was "cbcflow-0.1.2a6.tar", last modified: Tue Apr 18 14:12:07 2023, max compression
```

## Comparing `cbcflow-0.1.2a4.tar` & `cbcflow-0.1.2a6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.955842 cbcflow-0.1.2a4/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/library-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88880 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1503 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a4/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.955842 cbcflow-0.1.2a4/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/_version.py
--rw-r--r--   0 greg      (1000) greg      (1000)    12180 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/src/cbcflow/asimov.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88880 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5044 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3082 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      481 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a4/tests/test_parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/tests/test_schema.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/
+-rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/.gitattributes
+-rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/.gitignore
+-rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/.gitlab-ci.yml
+-rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/.pre-commit-config.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/CHANGELOG.md
+-rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/LICENSE.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/README.md
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.824520 cbcflow-0.1.2a6/docs/
+-rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/Makefile
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/requirements.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/_templates/
+-rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/actionitems.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/adding-to-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/asimov.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/conf.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/configuration.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/development-setup.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/example_mini_schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/example.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.min.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/gwosc.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/index.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/docs/source/libraries_images/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_1.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_2.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_3.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_4.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_5.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_6.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_7.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_8.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/library-index-labelling.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/library-indices.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/library-setup.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/monitor-usage.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/reading-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/schema-visualization.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/updating-metadata-from-the-command-line.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/updating-metadata-with-the-python-api.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/what-is-metadata.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/examples/
+-rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/examples/initial_example.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/pyproject.toml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-18 14:11:16.000000 cbcflow-0.1.2a6/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     1503 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a6/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.813687 cbcflow-0.1.2a6/src/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/_version.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    12824 2023-04-18 14:11:16.000000 cbcflow-0.1.2a6/src/cbcflow/asimov.py
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/cbcflow.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/configuration.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/gracedb.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/monitor.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/process.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/schema.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     5044 2023-04-18 14:11:05.000000 cbcflow-0.1.2a6/src/cbcflow/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3082 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      481 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/top_level.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/tests/files_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/cbc-meta-data-example.json
+-rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_json_1.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_json_2.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_1.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_2.yaml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/tests/library_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/library_for_testing/library.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/library_for_testing/testing-library-index.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/test_database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/test_metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a6/tests/test_parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/tests/test_schema.py
```

### Comparing `cbcflow-0.1.2a4/.gitlab-ci.yml` & `cbcflow-0.1.2a6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/.pre-commit-config.yaml` & `cbcflow-0.1.2a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/LICENSE.md` & `cbcflow-0.1.2a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/PKG-INFO` & `cbcflow-0.1.2a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a4
+Version: 0.1.2a6
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.2a4/README.md` & `cbcflow-0.1.2a6/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/Makefile` & `cbcflow-0.1.2a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.1.2a6/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.1.2a6/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/actionitems.rst` & `cbcflow-0.1.2a6/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/adding-to-the-schema.rst` & `cbcflow-0.1.2a6/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/conf.py` & `cbcflow-0.1.2a6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/configuration.rst` & `cbcflow-0.1.2a6/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/development-setup.rst` & `cbcflow-0.1.2a6/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/example_mini_schema/example.schema` & `cbcflow-0.1.2a6/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/index.rst` & `cbcflow-0.1.2a6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries.rst` & `cbcflow-0.1.2a6/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_1.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_2.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_3.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_4.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_5.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_6.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_7.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/libraries_images/part_8.png` & `cbcflow-0.1.2a6/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/library-index-labelling.rst` & `cbcflow-0.1.2a6/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/library-indices.rst` & `cbcflow-0.1.2a6/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/library-setup.rst` & `cbcflow-0.1.2a6/docs/source/library-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/monitor-usage.rst` & `cbcflow-0.1.2a6/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/reading-the-schema.rst` & `cbcflow-0.1.2a6/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.1.2a6/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.1.2a6/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/docs/source/what-is-metadata.rst` & `cbcflow-0.1.2a6/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/examples/initial_example.md` & `cbcflow-0.1.2a6/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/pyproject.toml` & `cbcflow-0.1.2a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a6/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a6/schema/cbc-meta-data-v2.schema`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997456247457%*

 * *Differences: {"'$defs'": "{'PEResult': {'properties': {'RunStatus': {'enum': {insert: [(3, 'unstarted'), (4, "*

 * *            "'cancelled')]}}}}}"}*

```diff
@@ -1277,15 +1277,17 @@
                     "type": "string"
                 },
                 "RunStatus": {
                     "description": "Status of the run",
                     "enum": [
                         "complete",
                         "running",
-                        "stuck"
+                        "stuck",
+                        "unstarted",
+                        "cancelled"
                     ],
                     "type": "string"
                 },
                 "UID": {
                     "description": "The name of the analysis",
                     "type": "string"
                 },
```

### Comparing `cbcflow-0.1.2a4/schema/index-v1.schema` & `cbcflow-0.1.2a6/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/setup.cfg` & `cbcflow-0.1.2a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/setup.py` & `cbcflow-0.1.2a6/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/__init__.py` & `cbcflow-0.1.2a6/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/asimov.py` & `cbcflow-0.1.2a6/src/cbcflow/asimov.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Collector:
     status_map = {
         "ready": "unstarted",
-        "processing": "ongoing",
-        "running": "ongoing",
-        "stuck": "ongoing",
-        "restart": "ongoing",
+        "processing": "running",
+        "running": "running",
+        "stuck": "running",
+        "restart": "running",
         "stopped": "cancelled",
-        "finished": "ongoing",
+        "finished": "running",
         "uploaded": "complete",
     }
 
     def __init__(self, ledger):
         """
         Collect data from the asimov ledger and write it to a CBCFlow library.
         """
@@ -61,14 +61,28 @@
                         analysis.pipeline.production.name, analysis.pipeline.category
                     )[0]
                     analysis_output["ConfigFile"] = {}
                     analysis_output["ConfigFile"]["Path"] = ini
                 except IndexError:
                     logger.warning("Could not find ini file for this analysis")
                 analysis_output["Notes"] = [analysis.comment]
+                if analysis.review.status:
+                    if analysis.review.status.lower() == "approved":
+                        analysis_output["ReviewStatus"] = "pass"
+                    elif analysis.review.status.lower() == "rejected":
+                        analysis_output["ReviewStatus"] = "fail"
+                    elif analysis.review.status.lower() == "deprecated":
+                        analysis_output["Deprecated"] = True
+                    messages = sorted(
+                        analysis.review.messages, key=lambda k: k.timestamp
+                    )
+                    if len(messages) > 0:
+                        analysis_output["Notes"].append(
+                            f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
+                        )
                 if analysis.finished:
                     # Get the results
                     results = analysis.pipeline.collect_assets()
                     if str(analysis.pipeline).lower() == "bayeswave":
                         # If the pipeline is Bayeswave, we slot each psd into its designated spot
                         analysis_output["BayeswaveResults"] = {}
                         for ifo, psd in results["psds"].items():
@@ -204,34 +218,35 @@
         data = {}
         channels = data["channels"] = {}
         frame_types = data["frame types"] = {}
         data["segment length"] = detchar["RecommendedDuration"]
         # NOTE there are also detector specific quantities "RecommendedStart/EndTime"
         # but it is not clear how these should be reconciled with
 
+        ifo_list = []
+
         for ifo in ifos:
             # Grab IFO specific quantities
             ifo_name = ifo["UID"]
-            if ifo_name in participating_detectors:
-                # Tracking which detectors are participating and also recommended
-                participating_detectors.remove(ifo_name)
+            ifo_list.append(ifo_name)
             if "RecommendedMaximumFrequency" in ifo.keys():
                 max_f[ifo_name] = ifo["RecommendedMaximumFrequency"]
             if "RecommendedMinimumFrequency" in ifo.keys():
                 min_f[ifo_name] = ifo["RecommendedMinimumFrequency"]
             if "RecommendedChannel" in ifo.keys():
                 channels[ifo_name] = ifo["RecommendedChannel"]
             if "FrameType" in ifo.keys():
                 frame_types[ifo_name] = ifo["FrameType"]
 
-        if len(participating_detectors) != 0:
+        if ifo_list != []:
+            data["interferometers"] = ifo_list
+        else:
+            data["interferometers"] = participating_detectors
             logger.info(
-                f"Detectors {participating_detectors} were not in recommended list\
-                        either because validation is still pending\
-                        or because they are rejected upon validation"
+                "No detchar recommended IFOs provided, falling back to participating detectors"
             )
 
         # GraceDB Settings
         ligo = {}
         for event in grace["Events"]:
             if event["State"] == "preferred":
                 ligo["preferred event"] = event["UID"]
```

### Comparing `cbcflow-0.1.2a4/src/cbcflow/cbcflow.py` & `cbcflow-0.1.2a6/src/cbcflow/cbcflow.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/configuration.py` & `cbcflow-0.1.2a6/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/database.py` & `cbcflow-0.1.2a6/src/cbcflow/database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/gracedb.py` & `cbcflow-0.1.2a6/src/cbcflow/gracedb.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/metadata.py` & `cbcflow-0.1.2a6/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/monitor.py` & `cbcflow-0.1.2a6/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/parser.py` & `cbcflow-0.1.2a6/src/cbcflow/parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/process.py` & `cbcflow-0.1.2a6/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997456247457%*

 * *Differences: {"'$defs'": "{'PEResult': {'properties': {'RunStatus': {'enum': {insert: [(3, 'unstarted'), (4, "*

 * *            "'cancelled')]}}}}}"}*

```diff
@@ -1277,15 +1277,17 @@
                     "type": "string"
                 },
                 "RunStatus": {
                     "description": "Status of the run",
                     "enum": [
                         "complete",
                         "running",
-                        "stuck"
+                        "stuck",
+                        "unstarted",
+                        "cancelled"
                     ],
                     "type": "string"
                 },
                 "UID": {
                     "description": "The name of the analysis",
                     "type": "string"
                 },
```

### Comparing `cbcflow-0.1.2a4/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.1.2a6/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/schema.py` & `cbcflow-0.1.2a6/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow/utils.py` & `cbcflow-0.1.2a6/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.1.2a6/src/cbcflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a4
+Version: 0.1.2a6
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.2a4/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.1.2a6/src/cbcflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.1.2a6/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/files_for_testing/update_json_1.json` & `cbcflow-0.1.2a6/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/files_for_testing/update_json_2.json` & `cbcflow-0.1.2a6/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.1.2a6/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/test_database.py` & `cbcflow-0.1.2a6/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/test_metadata.py` & `cbcflow-0.1.2a6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/test_parser.py` & `cbcflow-0.1.2a6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a4/tests/test_schema.py` & `cbcflow-0.1.2a6/tests/test_schema.py`

 * *Files identical despite different names*

