# Comparing `tmp/oarepo-model-builder-drafts-1.0.1.tar.gz` & `tmp/oarepo-model-builder-drafts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-drafts-1.0.1.tar", last modified: Wed Apr 19 09:03:37 2023, max compression
+gzip compressed data, was "oarepo-model-builder-drafts-1.0.2.tar", last modified: Wed Apr 19 13:16:16 2023, max compression
```

## Comparing `oarepo-model-builder-drafts-1.0.1.tar` & `oarepo-model-builder-drafts-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.176254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.176254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_draft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/profiles/drafts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:03:37.176254 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 09:03:37.000000 oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-19 09:03:37.180254 oarepo-model-builder-drafts-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:01:16.000000 oarepo-model-builder-drafts-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.966021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.966021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.966021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/profiles/drafts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:16.966021 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 13:16:16.000000 oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-19 13:16:16.970021 oarepo-model-builder-drafts-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:14:10.000000 oarepo-model-builder-drafts-1.0.2/setup.py
```

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/__init__.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_common.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_common.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_draft.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_draft.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_record.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/model_preprocessors/invenio_drafts_record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts/validation/__init__.py` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/SOURCES.txt` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/oarepo_model_builder_drafts.egg-info/entry_points.txt` & `oarepo-model-builder-drafts-1.0.2/oarepo_model_builder_drafts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-1.0.1/setup.cfg` & `oarepo-model-builder-drafts-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-drafts
-version = 1.0.1
+version = 1.0.2
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

