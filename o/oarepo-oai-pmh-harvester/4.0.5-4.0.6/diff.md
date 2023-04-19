# Comparing `tmp/oarepo-oai-pmh-harvester-4.0.5.tar.gz` & `tmp/oarepo-oai-pmh-harvester-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-oai-pmh-harvester-4.0.5.tar", last modified: Tue Apr 18 08:51:55 2023, max compression
+gzip compressed data, was "oarepo-oai-pmh-harvester-4.0.6.tar", last modified: Wed Apr 19 15:22:59 2023, max compression
```

## Comparing `oarepo-oai-pmh-harvester-4.0.5.tar` & `oarepo-oai-pmh-harvester-4.0.6.tar`

### file list

```diff
@@ -1,212 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/cecc281d2938_create_oarepo_oaipmh_harvester_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/harvester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29797 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/oai_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/sickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/marcxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.391404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 15:22:59.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/alembic/cecc281d2938_create_oarepo_oaipmh_harvester_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.395404 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.399405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22227 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.403405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.407405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.411405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/oai_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/sickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/marcxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:59.415405 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/oai_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-19 15:22:59.419405 oarepo-oai-pmh-harvester-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:21:40.000000 oarepo-oai-pmh-harvester-4.0.6/setup.py
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/PKG-INFO` & `oarepo-oai-pmh-harvester-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-oai-pmh-harvester
-Version: 4.0.5
+Version: 4.0.6
 Summary: OAIPMH harvester
 Description-Content-Type: text/markdown
 
 # OARepo OAI-PMH harvester
 
 An OAI-PMH harvesing library for Invenio 3.5+. The library provides initial transformation 
 of OAI-PMH payload to an intermediary json representation which is later on transformed by
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/README.md` & `oarepo-oai-pmh-harvester-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/PKG-INFO` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-oai-pmh-harvester
-Version: 4.0.5
+Version: 4.0.6
 Summary: OAIPMH harvester
 Description-Content-Type: text/markdown
 
 # OARepo OAI-PMH harvester
 
 An OAI-PMH harvesing library for Invenio 3.5+. The library provides initial transformation 
 of OAI-PMH payload to an intermediary json representation which is later on transformed by
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 oarepo_oaipmh_harvester/oai_batch/config.py
 oarepo_oaipmh_harvester/oai_batch/ext.py
 oarepo_oaipmh_harvester/oai_batch/proxies.py
 oarepo_oaipmh_harvester/oai_batch/version.py
 oarepo_oaipmh_harvester/oai_batch/views.py
 oarepo_oaipmh_harvester/oai_batch/models/__init__.py
 oarepo_oaipmh_harvester/oai_batch/models/model.json
+oarepo_oaipmh_harvester/oai_batch/models/ui.json
 oarepo_oaipmh_harvester/oai_batch/records/__init__.py
 oarepo_oaipmh_harvester/oai_batch/records/api.py
 oarepo_oaipmh_harvester/oai_batch/records/dumper.py
 oarepo_oaipmh_harvester/oai_batch/records/models.py
 oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/__init__.py
 oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json
 oarepo_oaipmh_harvester/oai_batch/records/mappings/__init__.py
@@ -56,14 +57,15 @@
 oarepo_oaipmh_harvester/oai_harvester/config.py
 oarepo_oaipmh_harvester/oai_harvester/ext.py
 oarepo_oaipmh_harvester/oai_harvester/proxies.py
 oarepo_oaipmh_harvester/oai_harvester/version.py
 oarepo_oaipmh_harvester/oai_harvester/views.py
 oarepo_oaipmh_harvester/oai_harvester/models/__init__.py
 oarepo_oaipmh_harvester/oai_harvester/models/model.json
+oarepo_oaipmh_harvester/oai_harvester/models/ui.json
 oarepo_oaipmh_harvester/oai_harvester/records/__init__.py
 oarepo_oaipmh_harvester/oai_harvester/records/api.py
 oarepo_oaipmh_harvester/oai_harvester/records/dumper.py
 oarepo_oaipmh_harvester/oai_harvester/records/models.py
 oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/__init__.py
 oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json
 oarepo_oaipmh_harvester/oai_harvester/records/mappings/__init__.py
@@ -88,14 +90,15 @@
 oarepo_oaipmh_harvester/oai_record/config.py
 oarepo_oaipmh_harvester/oai_record/ext.py
 oarepo_oaipmh_harvester/oai_record/proxies.py
 oarepo_oaipmh_harvester/oai_record/version.py
 oarepo_oaipmh_harvester/oai_record/views.py
 oarepo_oaipmh_harvester/oai_record/models/__init__.py
 oarepo_oaipmh_harvester/oai_record/models/model.json
+oarepo_oaipmh_harvester/oai_record/models/ui.json
 oarepo_oaipmh_harvester/oai_record/records/__init__.py
 oarepo_oaipmh_harvester/oai_record/records/api.py
 oarepo_oaipmh_harvester/oai_record/records/dumper.py
 oarepo_oaipmh_harvester/oai_record/records/models.py
 oarepo_oaipmh_harvester/oai_record/records/jsonschemas/__init__.py
 oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json
 oarepo_oaipmh_harvester/oai_record/records/mappings/__init__.py
@@ -120,14 +123,15 @@
 oarepo_oaipmh_harvester/oai_run/config.py
 oarepo_oaipmh_harvester/oai_run/ext.py
 oarepo_oaipmh_harvester/oai_run/proxies.py
 oarepo_oaipmh_harvester/oai_run/version.py
 oarepo_oaipmh_harvester/oai_run/views.py
 oarepo_oaipmh_harvester/oai_run/models/__init__.py
 oarepo_oaipmh_harvester/oai_run/models/model.json
+oarepo_oaipmh_harvester/oai_run/models/ui.json
 oarepo_oaipmh_harvester/oai_run/records/__init__.py
 oarepo_oaipmh_harvester/oai_run/records/api.py
 oarepo_oaipmh_harvester/oai_run/records/dumper.py
 oarepo_oaipmh_harvester/oai_run/records/models.py
 oarepo_oaipmh_harvester/oai_run/records/jsonschemas/__init__.py
 oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json
 oarepo_oaipmh_harvester/oai_run/records/mappings/__init__.py
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/cli.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/ext.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/harvester.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/harvester.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/ext.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/model.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/models/model.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9464451650943396%*

 * *Differences: {"'model'": "{'properties': {'id': {'ui': {'marshmallow': {'read': False, 'write': False}}}, "*

 * *            "'created': {'marshmallow': {'validators': ['validate_datetime'], 'read': False, "*

 * *            "'imports': {0: {'import': 'oarepo_runtime.validation.validate_datetime'}, 2: "*

 * *            "{'import': 'oarepo_runtime.validation.validate_datetime'}}}, 'ui': {'marshmallow': "*

 * *            "{'field-class': 'l10n.LocalizedDateTime', 'read': False, 'write': False}}, 'type': "*

 * *            "'datetime'}, 'updated […]*

```diff
@@ -51,14 +51,32 @@
         "package-base-upper": "OAI_BATCH",
         "package-path": "oarepo_oaipmh_harvester/oai_batch",
         "permissions": {
             "presets": [
                 "oai_harvester"
             ]
         },
+        "pid-field-args": [
+            "create=True"
+        ],
+        "pid-field-cls": "PIDField",
+        "pid-field-context": "PIDFieldContext",
+        "pid-field-imports": [
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDField"
+            },
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDFieldContext"
+            },
+            {
+                "import": "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+            }
+        ],
+        "pid-field-provider": "RecordIdProviderV2",
+        "pid-type": "_btch",
         "plugins": {
             "builder": {
                 "disable": [
                     "script_sample_data",
                     "invenio_cli_setup_cfg",
                     "invenio_cli",
                     "invenio_record_metadata_alembic_setup_cfg"
@@ -80,53 +98,57 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "created": {
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "errors": {
                 "items": {
                     "marshmallow": {
                         "field-class": "ma_fields.Nested",
@@ -225,15 +247,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "identifiers": {
                 "items": {
                     "marshmallow": {
                         "field-class": "ma_fields.String",
@@ -407,41 +431,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             }
         },
         "proxies-current-resource": "oarepo_oaipmh_harvester.oai_batch.proxies.current_resource",
         "proxies-current-service": "oarepo_oaipmh_harvester.oai_batch.proxies.current_service",
         "record-api-blueprints-setup-cfg": "oai_batch",
@@ -451,17 +477,24 @@
         "record-blueprints-setup-cfg": "oai_batch",
         "record-class": "oarepo_oaipmh_harvester.oai_batch.records.api.OaiBatchRecord",
         "record-dumper-class": "oarepo_oaipmh_harvester.oai_batch.records.dumper.OaiBatchDumper",
         "record-dumper-extensions": [],
         "record-facets-class": "oarepo_oaipmh_harvester.oai_batch.services.records.facets.Test",
         "record-jsonschemas-setup-cfg": "oai_batch",
         "record-mapping-setup-cfg": "oai_batch",
+        "record-metadata-bases": [
+            "invenio_records.models.RecordMetadataBase"
+        ],
         "record-metadata-class": "oarepo_oaipmh_harvester.oai_batch.records.models.OaiBatchMetadata",
         "record-metadata-table-name": "oaibatch_metadata",
         "record-permissions-class": "oarepo_oaipmh_harvester.oai_batch.services.records.permissions.OaiBatchPermissionPolicy",
+        "record-pid-provider-bases": [
+            "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+        ],
+        "record-pid-provider-class": "oarepo_oaipmh_harvester.oai_batch.records.api.OaiBatchIdProvider",
         "record-prefix": "OaiBatch",
         "record-prefix-snake": "oai_batch",
         "record-records-package": "oarepo_oaipmh_harvester.oai_batch.records",
         "record-resource-bases": [
             "invenio_records_resources.resources.RecordResource"
         ],
         "record-resource-blueprint-name": "OaiBatch",
@@ -481,33 +514,41 @@
         ],
         "record-service-class": "oarepo_oaipmh_harvester.oai_batch.services.records.service.OaiBatchService",
         "record-service-config-bases": [
             "invenio_records_resources.services.RecordServiceConfig"
         ],
         "record-service-config-class": "oarepo_oaipmh_harvester.oai_batch.services.records.config.OaiBatchServiceConfig",
         "record-service-config-components": [
-            "invenio_records_resources.services.records.components.DataComponent"
+            "invenio_records_resources.services.records.components.DataComponent",
+            "oarepo_runtime.relations.components.CachingRelationsComponent"
         ],
         "record-service-config-generate-links": true,
         "record-services-package": "oarepo_oaipmh_harvester.oai_batch.services.records",
         "record-ui-schema-class": "oarepo_oaipmh_harvester.oai_batch.services.records.ui_schema.OaiBatchUISchema",
         "record-ui-schema-metadata-class": "oarepo_oaipmh_harvester.oai_batch.services.records.ui_schema.OaiBatchMetadataUISchema",
         "record-ui-serializer-class": "oarepo_oaipmh_harvester.oai_batch.resources.records.ui.OaiBatchUIJSONSerializer",
         "saved-model-file": "oarepo_oaipmh_harvester/oai_batch/models/model.json",
         "schema-file": "oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json",
         "schema-name": "oai_batch-1.0.0.json",
         "schema-server": "local://",
         "schema-version": "1.0.0",
         "script-import-sample-data": "data/sample_data.yaml",
         "service-id": "oarepo-oaipmh-batch",
+        "translations-setup-cfg": "oarepo_oaipmh_harvester.oai_batch",
         "type": "object",
         "ui": {
             "marshmallow": {
                 "base-classes": [
-                    "ma.Schema"
+                    "InvenioUISchema"
                 ],
                 "generate": true,
+                "imports": [
+                    {
+                        "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                    }
+                ],
                 "schema-class": "oarepo_oaipmh_harvester.oai_batch.services.records.ui_schema.OaiBatchUISchema"
             }
-        }
+        },
+        "ui-layout": "oarepo_oaipmh_harvester/oai_batch/models/ui.json"
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/api.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from invenio_pidstore.providers.recordid_v2 import RecordIdProviderV2
 from invenio_records.systemfields import ConstantField, RelationsField
 from invenio_records_resources.records.api import Record
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.records.systemfields.pid import PIDField, PIDFieldContext
-from oarepo_runtime.relations import InternalRelation, PIDRelation, RelationsField
+from oarepo_runtime.relations import PIDRelation, RelationsField
 
 from oarepo_oaipmh_harvester.oai_batch.records.dumper import OaiBatchDumper
 from oarepo_oaipmh_harvester.oai_batch.records.models import OaiBatchMetadata
 from oarepo_oaipmh_harvester.oai_run.records.api import OaiRunRecord
 
 
+class OaiBatchIdProvider(RecordIdProviderV2):
+    pid_type = "_btch"
+
+
 class OaiBatchRecord(Record):
     model_cls = OaiBatchMetadata
 
     schema = ConstantField("$schema", "local://oai_batch-1.0.0.json")
 
     index = IndexField("oai_batch-oai_batch-1.0.0")
 
     pid = PIDField(
-        create=True, provider=RecordIdProviderV2, context_cls=PIDFieldContext
+        provider=OaiBatchIdProvider, context_cls=PIDFieldContext, create=True
     )
 
     dumper_extensions = []
     dumper = OaiBatchDumper(extensions=dumper_extensions)
 
     relations = RelationsField(
         run=PIDRelation(
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7946428571428572%*

 * *Differences: {"'properties'": "{'created': {'format': 'date-time'}, 'updated': {'format': 'date-time'}, 'code': "*

 * *                 "OrderedDict([('type', 'string')]), 'baseurl': OrderedDict([('type', 'string')]), "*

 * *                 "'metadataprefix': OrderedDict([('type', 'string')]), 'comment': "*

 * *                 "OrderedDict([('type', 'string')]), 'name': OrderedDict([('type', 'string')]), "*

 * *                 "'setspecs': OrderedDict([('type', 'string')]), 'loader': OrderedDict([('type', "*

 * *                 "'string')]) […]*

```diff
@@ -1,68 +1,55 @@
 {
     "properties": {
         "$schema": {
             "type": "string"
         },
-        "created": {
-            "format": "date",
+        "baseurl": {
             "type": "string"
         },
-        "errors": {
-            "items": {
-                "properties": {
-                    "error": {
-                        "type": "string"
-                    },
-                    "oai_identifier": {
-                        "type": "string"
-                    }
-                },
-                "type": "object"
-            },
-            "type": "array"
+        "batch_size": {
+            "type": "integer"
+        },
+        "code": {
+            "type": "string"
         },
-        "finished": {
+        "comment": {
+            "type": "string"
+        },
+        "created": {
             "format": "date-time",
             "type": "string"
         },
         "id": {
             "type": "string"
         },
-        "identifiers": {
+        "loader": {
+            "type": "string"
+        },
+        "max_records": {
+            "type": "integer"
+        },
+        "metadataprefix": {
+            "type": "string"
+        },
+        "name": {
+            "type": "string"
+        },
+        "setspecs": {
+            "type": "string"
+        },
+        "transformers": {
             "items": {
                 "type": "string"
             },
             "type": "array"
         },
-        "run": {
-            "properties": {
-                "@v": {
-                    "type": "string"
-                },
-                "id": {
-                    "type": "string"
-                }
-            },
-            "type": "object"
-        },
-        "started": {
+        "updated": {
             "format": "date-time",
             "type": "string"
         },
-        "status": {
-            "enum": [
-                "R",
-                "O",
-                "W",
-                "E",
-                "I"
-            ],
-            "type": "string"
-        },
-        "updated": {
-            "format": "date",
+        "writer": {
             "type": "string"
         }
     },
     "type": "object"
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7976190476190477%*

 * *Differences: {"'mappings'": "{'properties': {'code': OrderedDict([('type', 'keyword')]), 'baseurl': "*

 * *               "OrderedDict([('type', 'keyword')]), 'metadataprefix': OrderedDict([('type', "*

 * *               "'keyword')]), 'comment': OrderedDict([('type', 'text')]), 'name': "*

 * *               "OrderedDict([('type', 'keyword')]), 'setspecs': OrderedDict([('type', "*

 * *               "'keyword')]), 'loader': OrderedDict([('type', 'keyword')]), 'transformers': "*

 * *               "OrderedDict([('type', 'keyword')]), 'writer': O […]*

```diff
@@ -1,57 +1,51 @@
 {
     "mappings": {
         "properties": {
             "$schema": {
                 "type": "keyword"
             },
-            "created": {
-                "type": "date"
+            "baseurl": {
+                "type": "keyword"
+            },
+            "batch_size": {
+                "type": "integer"
             },
-            "errors": {
-                "properties": {
-                    "error": {
-                        "fields": {
-                            "keyword": {
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "text"
-                    },
-                    "oai_identifier": {
-                        "type": "keyword"
-                    }
-                },
-                "type": "object"
+            "code": {
+                "type": "keyword"
+            },
+            "comment": {
+                "type": "text"
             },
-            "finished": {
+            "created": {
                 "type": "date"
             },
             "id": {
                 "type": "keyword"
             },
-            "identifiers": {
+            "loader": {
                 "type": "keyword"
             },
-            "run": {
-                "properties": {
-                    "@v": {
-                        "type": "keyword"
-                    },
-                    "id": {
-                        "type": "keyword"
-                    }
-                },
-                "type": "object"
+            "max_records": {
+                "type": "integer"
             },
-            "started": {
-                "type": "date"
+            "metadataprefix": {
+                "type": "keyword"
+            },
+            "name": {
+                "type": "keyword"
             },
-            "status": {
+            "setspecs": {
+                "type": "keyword"
+            },
+            "transformers": {
                 "type": "keyword"
             },
             "updated": {
                 "type": "date"
+            },
+            "writer": {
+                "type": "keyword"
             }
         }
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import RecordServiceConfig
-from invenio_records_resources.services import (
-    RecordServiceConfig as InvenioRecordServiceConfig,
-)
 from invenio_records_resources.services import pagination_links
 from invenio_records_resources.services.records.components import DataComponent
 from oarepo_runtime.config.service import PermissionsPresetsConfigMixin
+from oarepo_runtime.relations.components import CachingRelationsComponent
 
 from oarepo_oaipmh_harvester.oai_batch.records.api import OaiBatchRecord
-from oarepo_oaipmh_harvester.oai_batch.services.records.permissions import (
-    OaiBatchPermissionPolicy,
-)
 from oarepo_oaipmh_harvester.oai_batch.services.records.schema import OaiBatchSchema
 from oarepo_oaipmh_harvester.oai_batch.services.records.search import (
     OaiBatchSearchOptions,
 )
 
 
 class OaiBatchServiceConfig(PermissionsPresetsConfigMixin, RecordServiceConfig):
     """OaiBatchRecord service config."""
 
     url_prefix = "/oarepo-oaipmh-harvester.oai-batch/"
 
     PERMISSIONS_PRESETS = ["oai_harvester"]
 
+
     schema = OaiBatchSchema
 
     search = OaiBatchSearchOptions
 
     record_cls = OaiBatchRecord
-    # todo should i leave this here?
     service_id = "oarepo-oaipmh-batch"
 
-    components = [*RecordServiceConfig.components, DataComponent]
+    components = [
+        *RecordServiceConfig.components,
+        DataComponent,
+        CachingRelationsComponent,
+    ]
 
     model = "oai_batch"
 
     @property
     def links_item(self):
         return {
             "self": RecordLink("{self.url_prefix}{id}"),
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/facets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 """Facet definitions."""
 
+from flask_babelex import lazy_gettext as _
 from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
+from oarepo_runtime.facets.date import DateTimeFacet
+from oarepo_runtime.facets.enum import EnumTermsFacet
 
-run_id = TermsFacet(field="run.id")
+batch_id = TermsFacet(field="batch.id", label=_("batch/id.label"))
 
 
-run__version = TermsFacet(field="run.@v")
+batch__version = TermsFacet(field="batch.@v", label=_("batch/@v.label"))
 
 
-status = TermsFacet(field="status")
+local_identifier = TermsFacet(
+    field="local_identifier", label=_("local_identifier.label")
+)
 
 
-identifiers = TermsFacet(field="identifiers")
+oai_identifier = TermsFacet(field="oai_identifier", label=_("oai_identifier.label"))
 
 
-errors_oai_identifier = TermsFacet(field="errors.oai_identifier")
+datestamp = DateTimeFacet(field="datestamp", label=_("datestamp.label"))
 
 
-errors_error_keyword = TermsFacet(field="errors.error.keyword")
+status = EnumTermsFacet(field="status", label=_("status.label"))
 
 
-started = TermsFacet(field="started")
+warnings_keyword = TermsFacet(
+    field="warnings.keyword", label=_("warnings/keyword.label")
+)
 
 
-finished = TermsFacet(field="finished")
+errors_keyword = TermsFacet(field="errors.keyword", label=_("errors/keyword.label"))
 
 
-_id = TermsFacet(field="id")
+_id = TermsFacet(field="id", label=_("id.label"))
 
 
-created = TermsFacet(field="created")
+created = DateTimeFacet(field="created", label=_("created.label"))
 
 
-updated = TermsFacet(field="updated")
+updated = DateTimeFacet(field="updated", label=_("updated.label"))
 
 
-_schema = TermsFacet(field="$schema")
+_schema = TermsFacet(field="$schema", label=_("$schema.label"))
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import marshmallow as ma
 from invenio_records_resources.services.records.schema import (
     BaseRecordSchema as InvenioBaseRecordSchema,
 )
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
 from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
-from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date, validate_datetime
+from oarepo_runtime.validation import validate_datetime
 
 
 class RunSchema(ma.Schema):
     """RunSchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
     _version = ma_fields.String(data_key="@v", attribute="@v")
@@ -30,9 +26,7 @@
 
     run = ma_fields.Nested(lambda: RunSchema())
     status = ma_fields.String(validate=[ma_validate.OneOf(["R", "O", "W", "E", "I"])])
     identifiers = ma_fields.List(ma_fields.String())
     errors = ma_fields.List(ma_fields.Nested(lambda: ErrorsItemSchema()))
     started = ma_fields.String(validate=[validate_datetime])
     finished = ma_fields.String(validate=[validate_datetime])
-    created = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/search.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-def _(x):
-    """Identity function for string extraction."""
-    return x
-
-
-class OaiBatchSearchOptions(InvenioSearchOptions):
-    """OaiBatchRecord search options."""
+class OaiRecordSearchOptions(InvenioSearchOptions):
+    """OaiRecordRecord search options."""
 
     facets = {
-        "run_id": facets.run_id,
-        "run__version": facets.run__version,
+        "batch_id": facets.batch_id,
+        "batch__version": facets.batch__version,
+        "local_identifier": facets.local_identifier,
+        "oai_identifier": facets.oai_identifier,
+        "datestamp": facets.datestamp,
         "status": facets.status,
-        "identifiers": facets.identifiers,
-        "errors_oai_identifier": facets.errors_oai_identifier,
-        "errors_error_keyword": facets.errors_error_keyword,
-        "started": facets.started,
-        "finished": facets.finished,
+        "warnings_keyword": facets.warnings_keyword,
+        "errors_keyword": facets.errors_keyword,
         "_id": facets._id,
         "created": facets.created,
         "updated": facets.updated,
         "_schema": facets._schema,
     }
     sort_options = {
         **InvenioSearchOptions.sort_options,
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import marshmallow as ma
-from invenio_records_resources.services.records.schema import (
-    BaseRecordSchema as InvenioBaseRecordSchema,
-)
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
-from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
 from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date, validate_datetime
+from oarepo_runtime.ui.marshmallow import InvenioUISchema
 
 
-class RunUISchema(ma.Schema):
-    """RunUISchema schema."""
+class HarvesterUISchema(ma.Schema):
+    """HarvesterUISchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
-    _version = ma_fields.String(data_key="@v", attribute="@v")
-
-
-class ErrorsItemUISchema(ma.Schema):
-    """ErrorsItemUISchema schema."""
-
-    oai_identifier = ma_fields.String()
+    code = ma_fields.String()
+    baseurl = ma_fields.String()
+    metadataprefix = ma_fields.String()
+    comment = ma_fields.String()
+    name = ma_fields.String()
+    setspecs = ma_fields.String()
+    loader = ma_fields.String()
+    transformers = ma_fields.List(ma_fields.String())
+    writer = ma_fields.String()
+    max_records = ma_fields.Integer()
+    batch_size = ma_fields.Integer()
+
+
+class OaiRunUISchema(InvenioUISchema):
+    """OaiRunUISchema schema."""
+
+    harvester = ma_fields.Nested(lambda: HarvesterUISchema())
+    batches = ma_fields.Integer()
+    status = l10n.LocalizedEnum(value_prefix="oarepo_oaipmh_harvester.oai_run")
+    warning = ma_fields.String()
     error = ma_fields.String()
-
-
-class OaiBatchUISchema(ma.Schema):
-    """OaiBatchUISchema schema."""
-
-    run = ma_fields.Nested(lambda: RunUISchema())
-    status = l10n.LocalizedEnum(value_prefix="oarepo_oaipmh_harvester.oai_batch")
-    identifiers = ma_fields.List(ma_fields.String())
-    errors = ma_fields.List(ma_fields.Nested(lambda: ErrorsItemUISchema()))
     started = l10n.LocalizedDateTime()
     finished = l10n.LocalizedDateTime()
-    _id = ma_fields.String(data_key="id", attribute="id")
-    created = l10n.LocalizedDate()
-    updated = l10n.LocalizedDate()
-    _schema = ma_fields.String(data_key="$schema", attribute="$schema")
+    duration = ma_fields.Float()
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/views.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/ext.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/model.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/models/model.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9464606918238994%*

 * *Differences: {"'model'": "{'ui': {'marshmallow': {'base-classes': ['InvenioUISchema'], 'imports': "*

 * *            "[OrderedDict([('import', 'oarepo_runtime.ui.marshmallow.InvenioUISchema')])]}}, "*

 * *            "'properties': {'id': {'ui': {'marshmallow': {'write': False, 'read': False}}}, "*

 * *            "'created': {'marshmallow': {'read': False, 'validators': ['validate_datetime'], "*

 * *            "'imports': {0: {'import': 'oarepo_runtime.validation.validate_datetime'}, 2: "*

 * *            "{'import': 'oarepo_runtime.validatio […]*

```diff
@@ -51,14 +51,32 @@
         "package-base-upper": "OAI_HARVESTER",
         "package-path": "oarepo_oaipmh_harvester/oai_harvester",
         "permissions": {
             "presets": [
                 "oai_harvester"
             ]
         },
+        "pid-field-args": [
+            "create=True"
+        ],
+        "pid-field-cls": "PIDField",
+        "pid-field-context": "PIDFieldContext",
+        "pid-field-imports": [
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDField"
+            },
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDFieldContext"
+            },
+            {
+                "import": "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+            }
+        ],
+        "pid-field-provider": "RecordIdProviderV2",
+        "pid-type": "_hrstr",
         "plugins": {
             "builder": {
                 "disable": [
                     "script_sample_data",
                     "invenio_cli_setup_cfg",
                     "invenio_cli",
                     "invenio_record_metadata_alembic_setup_cfg"
@@ -80,15 +98,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "baseurl": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [],
@@ -146,41 +166,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "id": {
                 "facets": {
                     "searchable": true
                 },
@@ -193,15 +215,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "loader": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [],
@@ -300,41 +324,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "writer": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [],
@@ -357,17 +383,24 @@
         "record-blueprints-setup-cfg": "oai_harvester",
         "record-class": "oarepo_oaipmh_harvester.oai_harvester.records.api.OaiHarvesterRecord",
         "record-dumper-class": "oarepo_oaipmh_harvester.oai_harvester.records.dumper.OaiHarvesterDumper",
         "record-dumper-extensions": [],
         "record-facets-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.facets.Test",
         "record-jsonschemas-setup-cfg": "oai_harvester",
         "record-mapping-setup-cfg": "oai_harvester",
+        "record-metadata-bases": [
+            "invenio_records.models.RecordMetadataBase"
+        ],
         "record-metadata-class": "oarepo_oaipmh_harvester.oai_harvester.records.models.OaiHarvesterMetadata",
         "record-metadata-table-name": "oaiharvester_metadata",
         "record-permissions-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.permissions.OaiHarvesterPermissionPolicy",
+        "record-pid-provider-bases": [
+            "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+        ],
+        "record-pid-provider-class": "oarepo_oaipmh_harvester.oai_harvester.records.api.OaiHarvesterIdProvider",
         "record-prefix": "OaiHarvester",
         "record-prefix-snake": "oai_harvester",
         "record-records-package": "oarepo_oaipmh_harvester.oai_harvester.records",
         "record-resource-bases": [
             "invenio_records_resources.resources.RecordResource"
         ],
         "record-resource-blueprint-name": "OaiHarvester",
@@ -387,33 +420,41 @@
         ],
         "record-service-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.service.OaiHarvesterService",
         "record-service-config-bases": [
             "invenio_records_resources.services.RecordServiceConfig"
         ],
         "record-service-config-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.config.OaiHarvesterServiceConfig",
         "record-service-config-components": [
-            "invenio_records_resources.services.records.components.DataComponent"
+            "invenio_records_resources.services.records.components.DataComponent",
+            "oarepo_runtime.relations.components.CachingRelationsComponent"
         ],
         "record-service-config-generate-links": true,
         "record-services-package": "oarepo_oaipmh_harvester.oai_harvester.services.records",
         "record-ui-schema-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.ui_schema.OaiHarvesterUISchema",
         "record-ui-schema-metadata-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.ui_schema.OaiHarvesterMetadataUISchema",
         "record-ui-serializer-class": "oarepo_oaipmh_harvester.oai_harvester.resources.records.ui.OaiHarvesterUIJSONSerializer",
         "saved-model-file": "oarepo_oaipmh_harvester/oai_harvester/models/model.json",
         "schema-file": "oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json",
         "schema-name": "oai_harvester-1.0.0.json",
         "schema-server": "local://",
         "schema-version": "1.0.0",
         "script-import-sample-data": "data/sample_data.yaml",
         "service-id": "oarepo-oaipmh-harvester",
+        "translations-setup-cfg": "oarepo_oaipmh_harvester.oai_harvester",
         "type": "object",
         "ui": {
             "marshmallow": {
                 "base-classes": [
-                    "ma.Schema"
+                    "InvenioUISchema"
                 ],
                 "generate": true,
+                "imports": [
+                    {
+                        "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                    }
+                ],
                 "schema-class": "oarepo_oaipmh_harvester.oai_harvester.services.records.ui_schema.OaiHarvesterUISchema"
             }
-        }
+        },
+        "ui-layout": "oarepo_oaipmh_harvester/oai_harvester/models/ui.json"
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/api.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/records/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.records.systemfields.pid import PIDField, PIDFieldContext
 
 from oarepo_oaipmh_harvester.oai_harvester.records.dumper import OaiHarvesterDumper
 from oarepo_oaipmh_harvester.oai_harvester.records.models import OaiHarvesterMetadata
 
 
+class OaiHarvesterIdProvider(RecordIdProviderV2):
+    pid_type = "_hrstr"
+
+
 class OaiHarvesterRecord(Record):
     model_cls = OaiHarvesterMetadata
 
     schema = ConstantField("$schema", "local://oai_harvester-1.0.0.json")
 
     index = IndexField("oai_harvester-oai_harvester-1.0.0")
 
     pid = PIDField(
-        create=True, provider=RecordIdProviderV2, context_cls=PIDFieldContext
+        provider=OaiHarvesterIdProvider, context_cls=PIDFieldContext, create=True
     )
 
     dumper_extensions = []
     dumper = OaiHarvesterDumper(extensions=dumper_extensions)
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666667%*

 * *Differences: {"'mappings'": "{'properties': {'batch': OrderedDict([('properties', OrderedDict([('id', "*

 * *               "OrderedDict([('type', 'keyword')])), ('@v', OrderedDict([('type', "*

 * *               "'keyword')]))])), ('type', 'object')]), 'local_identifier': OrderedDict([('type', "*

 * *               "'keyword')]), 'oai_identifier': OrderedDict([('type', 'keyword')]), 'datestamp': "*

 * *               "OrderedDict([('type', 'date')]), 'status': OrderedDict([('type', 'keyword')]), "*

 * *               "'warnings': OrderedDict([ […]*

```diff
@@ -1,51 +1,65 @@
 {
     "mappings": {
         "properties": {
             "$schema": {
                 "type": "keyword"
             },
-            "baseurl": {
-                "type": "keyword"
-            },
-            "batch_size": {
-                "type": "integer"
-            },
-            "code": {
-                "type": "keyword"
-            },
-            "comment": {
-                "type": "text"
+            "batch": {
+                "properties": {
+                    "@v": {
+                        "type": "keyword"
+                    },
+                    "id": {
+                        "type": "keyword"
+                    }
+                },
+                "type": "object"
+            },
+            "context": {
+                "enabled": false,
+                "type": "object"
             },
             "created": {
                 "type": "date"
             },
-            "id": {
-                "type": "keyword"
-            },
-            "loader": {
-                "type": "keyword"
+            "datestamp": {
+                "type": "date"
             },
-            "max_records": {
-                "type": "integer"
+            "entry": {
+                "enabled": false,
+                "type": "object"
+            },
+            "errors": {
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                },
+                "type": "text"
             },
-            "metadataprefix": {
+            "id": {
                 "type": "keyword"
             },
-            "name": {
+            "local_identifier": {
                 "type": "keyword"
             },
-            "setspecs": {
+            "oai_identifier": {
                 "type": "keyword"
             },
-            "transformers": {
+            "status": {
                 "type": "keyword"
             },
             "updated": {
                 "type": "date"
             },
-            "writer": {
-                "type": "keyword"
+            "warnings": {
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                },
+                "type": "text"
             }
         }
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import RecordServiceConfig
-from invenio_records_resources.services import (
-    RecordServiceConfig as InvenioRecordServiceConfig,
-)
 from invenio_records_resources.services import pagination_links
 from invenio_records_resources.services.records.components import DataComponent
 from oarepo_runtime.config.service import PermissionsPresetsConfigMixin
+from oarepo_runtime.relations.components import CachingRelationsComponent
 
-from oarepo_oaipmh_harvester.oai_harvester.records.api import OaiHarvesterRecord
-from oarepo_oaipmh_harvester.oai_harvester.services.records.permissions import (
-    OaiHarvesterPermissionPolicy,
-)
-from oarepo_oaipmh_harvester.oai_harvester.services.records.schema import (
-    OaiHarvesterSchema,
-)
-from oarepo_oaipmh_harvester.oai_harvester.services.records.search import (
-    OaiHarvesterSearchOptions,
+from oarepo_oaipmh_harvester.oai_record.records.api import OaiRecordRecord
+from oarepo_oaipmh_harvester.oai_record.services.records.schema import OaiRecordSchema
+from oarepo_oaipmh_harvester.oai_record.services.records.search import (
+    OaiRecordSearchOptions,
 )
 
 
-class OaiHarvesterServiceConfig(PermissionsPresetsConfigMixin, RecordServiceConfig):
-    """OaiHarvesterRecord service config."""
+class OaiRecordServiceConfig(PermissionsPresetsConfigMixin, RecordServiceConfig):
+    """OaiRecordRecord service config."""
 
-    url_prefix = "/oarepo-oaipmh-harvester.oai-harvester/"
+    url_prefix = "/oarepo-oaipmh-harvester.oai-record/"
 
     PERMISSIONS_PRESETS = ["oai_harvester"]
 
-    schema = OaiHarvesterSchema
+    schema = OaiRecordSchema
 
-    search = OaiHarvesterSearchOptions
+    search = OaiRecordSearchOptions
 
-    record_cls = OaiHarvesterRecord
-    # todo should i leave this here?
-    service_id = "oarepo-oaipmh-harvester"
+    record_cls = OaiRecordRecord
+    service_id = "oarepo-oaipmh-record"
 
-    components = [*RecordServiceConfig.components, DataComponent]
+    components = [
+        *RecordServiceConfig.components,
+        DataComponent,
+        CachingRelationsComponent,
+    ]
 
-    model = "oai_harvester"
+    model = "oai_record"
 
     @property
     def links_item(self):
         return {
             "self": RecordLink("{self.url_prefix}{id}"),
         }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import marshmallow as ma
 from invenio_records_resources.services.records.schema import (
     BaseRecordSchema as InvenioBaseRecordSchema,
 )
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
 from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
-from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date
-
-
-class OaiHarvesterSchema(InvenioBaseRecordSchema):
-    """OaiHarvesterSchema schema."""
-
-    code = ma_fields.String()
-    baseurl = ma_fields.String()
-    metadataprefix = ma_fields.String()
-    comment = ma_fields.String()
-    name = ma_fields.String()
-    setspecs = ma_fields.String()
-    loader = ma_fields.String()
-    transformers = ma_fields.List(ma_fields.String())
-    writer = ma_fields.String()
-    max_records = ma_fields.Integer()
-    batch_size = ma_fields.Integer()
-    created = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
+from oarepo_runtime.validation import validate_datetime
+
+
+class BatchSchema(ma.Schema):
+    """BatchSchema schema."""
+
+    _id = ma_fields.String(data_key="id", attribute="id")
+    _version = ma_fields.String(data_key="@v", attribute="@v")
+
+
+class OaiRecordSchema(InvenioBaseRecordSchema):
+    """OaiRecordSchema schema."""
+
+    batch = ma_fields.Nested(lambda: BatchSchema())
+    local_identifier = ma_fields.String()
+    oai_identifier = ma_fields.String()
+    datestamp = ma_fields.String(validate=[validate_datetime])
+    status = ma_fields.String(validate=[ma_validate.OneOf(["O", "W", "E", "S"])])
+    warnings = ma_fields.List(ma_fields.String())
+    errors = ma_fields.List(ma_fields.String())
+    entry = ma_fields.Raw()
+    context = ma_fields.Raw()
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-def _(x):
-    """Identity function for string extraction."""
-    return x
-
-
 class OaiHarvesterSearchOptions(InvenioSearchOptions):
     """OaiHarvesterRecord search options."""
 
     facets = {
         "code": facets.code,
         "baseurl": facets.baseurl,
         "metadataprefix": facets.metadataprefix,
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import marshmallow as ma
-from invenio_records_resources.services.records.schema import (
-    BaseRecordSchema as InvenioBaseRecordSchema,
-)
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
-from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
 from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date
+from oarepo_runtime.ui.marshmallow import InvenioUISchema
 
 
-class OaiHarvesterUISchema(ma.Schema):
-    """OaiHarvesterUISchema schema."""
+class BatchUISchema(ma.Schema):
+    """BatchUISchema schema."""
 
-    code = ma_fields.String()
-    baseurl = ma_fields.String()
-    metadataprefix = ma_fields.String()
-    comment = ma_fields.String()
-    name = ma_fields.String()
-    setspecs = ma_fields.String()
-    loader = ma_fields.String()
-    transformers = ma_fields.List(ma_fields.String())
-    writer = ma_fields.String()
-    max_records = ma_fields.Integer()
-    batch_size = ma_fields.Integer()
     _id = ma_fields.String(data_key="id", attribute="id")
-    created = l10n.LocalizedDate()
-    updated = l10n.LocalizedDate()
-    _schema = ma_fields.String(data_key="$schema", attribute="$schema")
+    _version = ma_fields.String(data_key="@v", attribute="@v")
+
+
+class OaiRecordUISchema(InvenioUISchema):
+    """OaiRecordUISchema schema."""
+
+    batch = ma_fields.Nested(lambda: BatchUISchema())
+    local_identifier = ma_fields.String()
+    oai_identifier = ma_fields.String()
+    datestamp = l10n.LocalizedDateTime()
+    status = l10n.LocalizedEnum(value_prefix="oarepo_oaipmh_harvester.oai_record")
+    warnings = ma_fields.List(ma_fields.String())
+    errors = ma_fields.List(ma_fields.String())
+    entry = ma_fields.Raw()
+    context = ma_fields.Raw()
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/views.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_harvester/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/ext.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/model.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/models/model.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9464559143686502%*

 * *Differences: {"'model'": "{'record-service-config-components': {insert: [(1, "*

 * *            "'oarepo_runtime.relations.components.CachingRelationsComponent')]}, 'ui': "*

 * *            "{'marshmallow': {'base-classes': ['InvenioUISchema'], 'imports': "*

 * *            "[OrderedDict([('import', 'oarepo_runtime.ui.marshmallow.InvenioUISchema')])]}}, "*

 * *            "'properties': {'id': {'ui': {'marshmallow': {'read': False, 'write': False}}}, "*

 * *            "'created': {'marshmallow': {'validators': ['validate_datetime'], 'read': Fa […]*

```diff
@@ -51,14 +51,32 @@
         "package-base-upper": "OAI_RECORD",
         "package-path": "oarepo_oaipmh_harvester/oai_record",
         "permissions": {
             "presets": [
                 "oai_harvester"
             ]
         },
+        "pid-field-args": [
+            "create=True"
+        ],
+        "pid-field-cls": "PIDField",
+        "pid-field-context": "PIDFieldContext",
+        "pid-field-imports": [
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDField"
+            },
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDFieldContext"
+            },
+            {
+                "import": "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+            }
+        ],
+        "pid-field-provider": "RecordIdProviderV2",
+        "pid-type": "_rcrd",
         "plugins": {
             "builder": {
                 "disable": [
                     "invenio_cli_setup_cfg",
                     "invenio_cli",
                     "script_sample_data",
                     "invenio_record_metadata_alembic_setup_cfg"
@@ -80,15 +98,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "batch": {
                 "imports": [
                     {
                         "import": "oarepo_runtime.relations.RelationsField"
@@ -187,41 +207,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "datestamp": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
@@ -306,15 +328,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "local_identifier": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [],
@@ -377,41 +401,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "warnings": {
                 "items": {
                     "marshmallow": {
                         "field-class": "ma_fields.String",
@@ -447,17 +473,24 @@
         "record-blueprints-setup-cfg": "oai_record",
         "record-class": "oarepo_oaipmh_harvester.oai_record.records.api.OaiRecordRecord",
         "record-dumper-class": "oarepo_oaipmh_harvester.oai_record.records.dumper.OaiRecordDumper",
         "record-dumper-extensions": [],
         "record-facets-class": "oarepo_oaipmh_harvester.oai_record.services.records.facets.Test",
         "record-jsonschemas-setup-cfg": "oai_record",
         "record-mapping-setup-cfg": "oai_record",
+        "record-metadata-bases": [
+            "invenio_records.models.RecordMetadataBase"
+        ],
         "record-metadata-class": "oarepo_oaipmh_harvester.oai_record.records.models.OaiRecordMetadata",
         "record-metadata-table-name": "oairecord_metadata",
         "record-permissions-class": "oarepo_oaipmh_harvester.oai_record.services.records.permissions.OaiRecordPermissionPolicy",
+        "record-pid-provider-bases": [
+            "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+        ],
+        "record-pid-provider-class": "oarepo_oaipmh_harvester.oai_record.records.api.OaiRecordIdProvider",
         "record-prefix": "OaiRecord",
         "record-prefix-snake": "oai_record",
         "record-records-package": "oarepo_oaipmh_harvester.oai_record.records",
         "record-resource-bases": [
             "invenio_records_resources.resources.RecordResource"
         ],
         "record-resource-blueprint-name": "OaiRecord",
@@ -477,33 +510,41 @@
         ],
         "record-service-class": "oarepo_oaipmh_harvester.oai_record.services.records.service.OaiRecordService",
         "record-service-config-bases": [
             "invenio_records_resources.services.RecordServiceConfig"
         ],
         "record-service-config-class": "oarepo_oaipmh_harvester.oai_record.services.records.config.OaiRecordServiceConfig",
         "record-service-config-components": [
-            "invenio_records_resources.services.records.components.DataComponent"
+            "invenio_records_resources.services.records.components.DataComponent",
+            "oarepo_runtime.relations.components.CachingRelationsComponent"
         ],
         "record-service-config-generate-links": true,
         "record-services-package": "oarepo_oaipmh_harvester.oai_record.services.records",
         "record-ui-schema-class": "oarepo_oaipmh_harvester.oai_record.services.records.ui_schema.OaiRecordUISchema",
         "record-ui-schema-metadata-class": "oarepo_oaipmh_harvester.oai_record.services.records.ui_schema.OaiRecordMetadataUISchema",
         "record-ui-serializer-class": "oarepo_oaipmh_harvester.oai_record.resources.records.ui.OaiRecordUIJSONSerializer",
         "saved-model-file": "oarepo_oaipmh_harvester/oai_record/models/model.json",
         "schema-file": "oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json",
         "schema-name": "oai_record-1.0.0.json",
         "schema-server": "local://",
         "schema-version": "1.0.0",
         "script-import-sample-data": "data/sample_data.yaml",
         "service-id": "oarepo-oaipmh-record",
+        "translations-setup-cfg": "oarepo_oaipmh_harvester.oai_record",
         "type": "object",
         "ui": {
             "marshmallow": {
                 "base-classes": [
-                    "ma.Schema"
+                    "InvenioUISchema"
                 ],
                 "generate": true,
+                "imports": [
+                    {
+                        "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                    }
+                ],
                 "schema-class": "oarepo_oaipmh_harvester.oai_record.services.records.ui_schema.OaiRecordUISchema"
             }
-        }
+        },
+        "ui-layout": "oarepo_oaipmh_harvester/oai_record/models/ui.json"
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/api.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from invenio_pidstore.providers.recordid_v2 import RecordIdProviderV2
 from invenio_records.systemfields import ConstantField, RelationsField
 from invenio_records_resources.records.api import Record
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.records.systemfields.pid import PIDField, PIDFieldContext
-from oarepo_runtime.relations import InternalRelation, PIDRelation, RelationsField
+from oarepo_runtime.relations import PIDRelation, RelationsField
 
 from oarepo_oaipmh_harvester.oai_batch.records.api import OaiBatchRecord
 from oarepo_oaipmh_harvester.oai_record.records.dumper import OaiRecordDumper
 from oarepo_oaipmh_harvester.oai_record.records.models import OaiRecordMetadata
 
 
+class OaiRecordIdProvider(RecordIdProviderV2):
+    pid_type = "_rcrd"
+
+
 class OaiRecordRecord(Record):
     model_cls = OaiRecordMetadata
 
     schema = ConstantField("$schema", "local://oai_record-1.0.0.json")
 
     index = IndexField("oai_record-oai_record-1.0.0")
 
     pid = PIDField(
-        create=True, provider=RecordIdProviderV2, context_cls=PIDFieldContext
+        provider=OaiRecordIdProvider, context_cls=PIDFieldContext, create=True
     )
 
     dumper_extensions = []
     dumper = OaiRecordDumper(extensions=dumper_extensions)
 
     relations = RelationsField(
         batch=PIDRelation(
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'properties'": "{'created': {'format': 'date-time'}, 'updated': {'format': 'date-time'}}"}*

```diff
@@ -14,15 +14,15 @@
             },
             "type": "object"
         },
         "context": {
             "type": "object"
         },
         "created": {
-            "format": "date",
+            "format": "date-time",
             "type": "string"
         },
         "datestamp": {
             "format": "date-time",
             "type": "string"
         },
         "entry": {
@@ -49,15 +49,15 @@
                 "W",
                 "E",
                 "S"
             ],
             "type": "string"
         },
         "updated": {
-            "format": "date",
+            "format": "date-time",
             "type": "string"
         },
         "warnings": {
             "items": {
                 "type": "string"
             },
             "type": "array"
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {"'mappings'": "{'properties': {'harvester': OrderedDict([('properties', OrderedDict([('id', "*

 * *               "OrderedDict([('type', 'keyword')])), ('code', OrderedDict([('type', 'keyword')])), "*

 * *               "('baseurl', OrderedDict([('type', 'keyword')])), ('metadataprefix', "*

 * *               "OrderedDict([('type', 'keyword')])), ('comment', OrderedDict([('type', 'text')])), "*

 * *               "('name', OrderedDict([('type', 'keyword')])), ('setspecs', OrderedDict([('type', "*

 * *               "'keyword')])), […]*

```diff
@@ -1,65 +1,89 @@
 {
     "mappings": {
         "properties": {
             "$schema": {
                 "type": "keyword"
             },
-            "batch": {
-                "properties": {
-                    "@v": {
-                        "type": "keyword"
-                    },
-                    "id": {
-                        "type": "keyword"
-                    }
-                },
-                "type": "object"
-            },
-            "context": {
-                "enabled": false,
-                "type": "object"
+            "batches": {
+                "type": "integer"
             },
             "created": {
                 "type": "date"
             },
-            "datestamp": {
-                "type": "date"
+            "duration": {
+                "type": "double"
             },
-            "entry": {
-                "enabled": false,
-                "type": "object"
+            "error": {
+                "type": "keyword"
             },
-            "errors": {
-                "fields": {
-                    "keyword": {
+            "finished": {
+                "type": "date"
+            },
+            "harvester": {
+                "properties": {
+                    "$schema": {
+                        "type": "keyword"
+                    },
+                    "baseurl": {
+                        "type": "keyword"
+                    },
+                    "batch_size": {
+                        "type": "integer"
+                    },
+                    "code": {
+                        "type": "keyword"
+                    },
+                    "comment": {
+                        "type": "text"
+                    },
+                    "created": {
+                        "type": "date"
+                    },
+                    "id": {
+                        "type": "keyword"
+                    },
+                    "loader": {
+                        "type": "keyword"
+                    },
+                    "max_records": {
+                        "type": "integer"
+                    },
+                    "metadataprefix": {
+                        "type": "keyword"
+                    },
+                    "name": {
+                        "type": "keyword"
+                    },
+                    "setspecs": {
+                        "type": "keyword"
+                    },
+                    "transformers": {
+                        "type": "keyword"
+                    },
+                    "updated": {
+                        "type": "date"
+                    },
+                    "writer": {
                         "type": "keyword"
                     }
                 },
-                "type": "text"
+                "type": "object"
             },
             "id": {
                 "type": "keyword"
             },
-            "local_identifier": {
-                "type": "keyword"
-            },
-            "oai_identifier": {
-                "type": "keyword"
+            "started": {
+                "type": "date"
             },
             "status": {
                 "type": "keyword"
             },
             "updated": {
                 "type": "date"
             },
-            "warnings": {
-                "fields": {
-                    "keyword": {
-                        "type": "keyword"
-                    }
-                },
-                "type": "text"
+            "warning": {
+                "type": "keyword"
             }
         }
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import marshmallow as ma
 from invenio_records_resources.services.records.schema import (
     BaseRecordSchema as InvenioBaseRecordSchema,
 )
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
 from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
-from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date, validate_datetime
+from oarepo_runtime.validation import validate_datetime
 
 
-class BatchSchema(ma.Schema):
-    """BatchSchema schema."""
+class HarvesterSchema(ma.Schema):
+    """HarvesterSchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
-    _version = ma_fields.String(data_key="@v", attribute="@v")
-
-
-class OaiRecordSchema(InvenioBaseRecordSchema):
-    """OaiRecordSchema schema."""
-
-    batch = ma_fields.Nested(lambda: BatchSchema())
-    local_identifier = ma_fields.String()
-    oai_identifier = ma_fields.String()
-    datestamp = ma_fields.String(validate=[validate_datetime])
-    status = ma_fields.String(validate=[ma_validate.OneOf(["O", "W", "E", "S"])])
-    warnings = ma_fields.List(ma_fields.String())
-    errors = ma_fields.List(ma_fields.String())
-    entry = ma_fields.Raw()
-    context = ma_fields.Raw()
-    created = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date("%Y-%m-%d")], dump_only=True)
+    code = ma_fields.String()
+    baseurl = ma_fields.String()
+    metadataprefix = ma_fields.String()
+    comment = ma_fields.String()
+    name = ma_fields.String()
+    setspecs = ma_fields.String()
+    loader = ma_fields.String()
+    transformers = ma_fields.List(ma_fields.String())
+    writer = ma_fields.String()
+    max_records = ma_fields.Integer()
+    batch_size = ma_fields.Integer()
+
+
+class OaiRunSchema(InvenioBaseRecordSchema):
+    """OaiRunSchema schema."""
+
+    harvester = ma_fields.Nested(lambda: HarvesterSchema())
+    batches = ma_fields.Integer()
+    status = ma_fields.String(validate=[ma_validate.OneOf(["R", "O", "W", "E", "I"])])
+    warning = ma_fields.String()
+    error = ma_fields.String()
+    started = ma_fields.String(validate=[validate_datetime])
+    finished = ma_fields.String(validate=[validate_datetime])
+    duration = ma_fields.Float()
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/search.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-def _(x):
-    """Identity function for string extraction."""
-    return x
-
-
-class OaiRecordSearchOptions(InvenioSearchOptions):
-    """OaiRecordRecord search options."""
+class OaiBatchSearchOptions(InvenioSearchOptions):
+    """OaiBatchRecord search options."""
 
     facets = {
-        "batch_id": facets.batch_id,
-        "batch__version": facets.batch__version,
-        "local_identifier": facets.local_identifier,
-        "oai_identifier": facets.oai_identifier,
-        "datestamp": facets.datestamp,
+        "run_id": facets.run_id,
+        "run__version": facets.run__version,
         "status": facets.status,
-        "warnings_keyword": facets.warnings_keyword,
-        "errors_keyword": facets.errors_keyword,
+        "identifiers": facets.identifiers,
+        "errors_oai_identifier": facets.errors_oai_identifier,
+        "errors_error_keyword": facets.errors_error_keyword,
+        "started": facets.started,
+        "finished": facets.finished,
         "_id": facets._id,
         "created": facets.created,
         "updated": facets.updated,
         "_schema": facets._schema,
     }
     sort_options = {
         **InvenioSearchOptions.sort_options,
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/views.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_record/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/ext.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/model.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/models/model.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9464528099886442%*

 * *Differences: {"'model'": "{'properties': {'harvester': {'properties': {'created': {'marshmallow': "*

 * *            "{'validators': ['validate_datetime', 'validate_datetime'], 'read': False, 'imports': "*

 * *            "{0: {'import': 'oarepo_runtime.validation.validate_datetime'}, 2: {'import': "*

 * *            "'oarepo_runtime.validation.validate_datetime'}, 4: {'import': "*

 * *            "'oarepo_runtime.validation.validate_datetime'}, 6: {'import': "*

 * *            "'oarepo_runtime.validation.validate_datetime'}}}, 'ui': {'marshmal […]*

```diff
@@ -51,14 +51,32 @@
         "package-base-upper": "OAI_RUN",
         "package-path": "oarepo_oaipmh_harvester/oai_run",
         "permissions": {
             "presets": [
                 "oai_harvester"
             ]
         },
+        "pid-field-args": [
+            "create=True"
+        ],
+        "pid-field-cls": "PIDField",
+        "pid-field-context": "PIDFieldContext",
+        "pid-field-imports": [
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDField"
+            },
+            {
+                "import": "invenio_records_resources.records.systemfields.pid.PIDFieldContext"
+            },
+            {
+                "import": "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+            }
+        ],
+        "pid-field-provider": "RecordIdProviderV2",
+        "pid-type": "_rn",
         "plugins": {
             "builder": {
                 "disable": [
                     "invenio_cli_setup_cfg",
                     "invenio_cli",
                     "script_sample_data",
                     "invenio_record_metadata_alembic_setup_cfg"
@@ -80,15 +98,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "batches": {
                 "marshmallow": {
                     "field-class": "ma_fields.Integer",
                     "imports": [],
@@ -105,41 +125,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "duration": {
                 "marshmallow": {
                     "field-class": "ma_fields.Float",
                     "imports": [],
@@ -216,15 +238,17 @@
                         },
                         "sample": {
                             "skip": true
                         },
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String"
+                                "field-class": "ma_fields.String",
+                                "read": false,
+                                "write": false
                             }
                         }
                     },
                     "baseurl": {
                         "marshmallow": {
                             "field-class": "ma_fields.String",
                             "imports": [],
@@ -282,56 +306,58 @@
                         "facets": {
                             "searchable": true
                         },
                         "marshmallow": {
                             "field-class": "ma_fields.String",
                             "imports": [
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 }
                             ],
-                            "read": true,
+                            "read": false,
                             "validators": [
-                                "validate_date('%Y-%m-%d')",
-                                "validate_date('%Y-%m-%d')"
+                                "validate_datetime",
+                                "validate_datetime"
                             ],
                             "write": false
                         },
                         "sample": {
                             "skip": true
                         },
-                        "type": "date",
+                        "type": "datetime",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "l10n.LocalizedDate"
+                                "field-class": "l10n.LocalizedDateTime",
+                                "read": false,
+                                "write": false
                             }
                         }
                     },
                     "id": {
                         "marshmallow": {
                             "field-class": "ma_fields.String",
                             "imports": [],
@@ -443,56 +469,58 @@
                         "facets": {
                             "searchable": true
                         },
                         "marshmallow": {
                             "field-class": "ma_fields.String",
                             "imports": [
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 },
                                 {
-                                    "import": "oarepo_runtime.validation.validate_date"
+                                    "import": "oarepo_runtime.validation.validate_datetime"
                                 },
                                 {
                                     "alias": "l10n",
                                     "import": "oarepo_runtime.ui.marshmallow"
                                 }
                             ],
-                            "read": true,
+                            "read": false,
                             "validators": [
-                                "validate_date('%Y-%m-%d')",
-                                "validate_date('%Y-%m-%d')"
+                                "validate_datetime",
+                                "validate_datetime"
                             ],
                             "write": false
                         },
                         "sample": {
                             "skip": true
                         },
-                        "type": "date",
+                        "type": "datetime",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "l10n.LocalizedDate"
+                                "field-class": "l10n.LocalizedDateTime",
+                                "read": false,
+                                "write": false
                             }
                         }
                     },
                     "writer": {
                         "marshmallow": {
                             "field-class": "ma_fields.String",
                             "imports": [],
@@ -528,15 +556,17 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String"
+                        "field-class": "ma_fields.String",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "started": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
@@ -604,41 +634,43 @@
                 "facets": {
                     "searchable": true
                 },
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         },
                         {
-                            "import": "oarepo_runtime.validation.validate_date"
+                            "import": "oarepo_runtime.validation.validate_datetime"
                         },
                         {
                             "alias": "l10n",
                             "import": "oarepo_runtime.ui.marshmallow"
                         }
                     ],
-                    "read": true,
+                    "read": false,
                     "validators": [
-                        "validate_date('%Y-%m-%d')"
+                        "validate_datetime"
                     ],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
-                "type": "date",
+                "type": "datetime",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "l10n.LocalizedDate"
+                        "field-class": "l10n.LocalizedDateTime",
+                        "read": false,
+                        "write": false
                     }
                 }
             },
             "warning": {
                 "marshmallow": {
                     "field-class": "ma_fields.String",
                     "imports": [],
@@ -661,17 +693,24 @@
         "record-blueprints-setup-cfg": "oai_run",
         "record-class": "oarepo_oaipmh_harvester.oai_run.records.api.OaiRunRecord",
         "record-dumper-class": "oarepo_oaipmh_harvester.oai_run.records.dumper.OaiRunDumper",
         "record-dumper-extensions": [],
         "record-facets-class": "oarepo_oaipmh_harvester.oai_run.services.records.facets.Test",
         "record-jsonschemas-setup-cfg": "oai_run",
         "record-mapping-setup-cfg": "oai_run",
+        "record-metadata-bases": [
+            "invenio_records.models.RecordMetadataBase"
+        ],
         "record-metadata-class": "oarepo_oaipmh_harvester.oai_run.records.models.OaiRunMetadata",
         "record-metadata-table-name": "oairun_metadata",
         "record-permissions-class": "oarepo_oaipmh_harvester.oai_run.services.records.permissions.OaiRunPermissionPolicy",
+        "record-pid-provider-bases": [
+            "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
+        ],
+        "record-pid-provider-class": "oarepo_oaipmh_harvester.oai_run.records.api.OaiRunIdProvider",
         "record-prefix": "OaiRun",
         "record-prefix-snake": "oai_run",
         "record-records-package": "oarepo_oaipmh_harvester.oai_run.records",
         "record-resource-bases": [
             "invenio_records_resources.resources.RecordResource"
         ],
         "record-resource-blueprint-name": "OaiRun",
@@ -691,33 +730,41 @@
         ],
         "record-service-class": "oarepo_oaipmh_harvester.oai_run.services.records.service.OaiRunService",
         "record-service-config-bases": [
             "invenio_records_resources.services.RecordServiceConfig"
         ],
         "record-service-config-class": "oarepo_oaipmh_harvester.oai_run.services.records.config.OaiRunServiceConfig",
         "record-service-config-components": [
-            "invenio_records_resources.services.records.components.DataComponent"
+            "invenio_records_resources.services.records.components.DataComponent",
+            "oarepo_runtime.relations.components.CachingRelationsComponent"
         ],
         "record-service-config-generate-links": true,
         "record-services-package": "oarepo_oaipmh_harvester.oai_run.services.records",
         "record-ui-schema-class": "oarepo_oaipmh_harvester.oai_run.services.records.ui_schema.OaiRunUISchema",
         "record-ui-schema-metadata-class": "oarepo_oaipmh_harvester.oai_run.services.records.ui_schema.OaiRunMetadataUISchema",
         "record-ui-serializer-class": "oarepo_oaipmh_harvester.oai_run.resources.records.ui.OaiRunUIJSONSerializer",
         "saved-model-file": "oarepo_oaipmh_harvester/oai_run/models/model.json",
         "schema-file": "oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json",
         "schema-name": "oai_run-1.0.0.json",
         "schema-server": "local://",
         "schema-version": "1.0.0",
         "script-import-sample-data": "data/sample_data.yaml",
         "service-id": "oarepo-oaipmh-run",
+        "translations-setup-cfg": "oarepo_oaipmh_harvester.oai_run",
         "type": "object",
         "ui": {
             "marshmallow": {
                 "base-classes": [
-                    "ma.Schema"
+                    "InvenioUISchema"
                 ],
                 "generate": true,
+                "imports": [
+                    {
+                        "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                    }
+                ],
                 "schema-class": "oarepo_oaipmh_harvester.oai_run.services.records.ui_schema.OaiRunUISchema"
             }
-        }
+        },
+        "ui-layout": "oarepo_oaipmh_harvester/oai_run/models/ui.json"
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/api.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.records.systemfields.pid import PIDField, PIDFieldContext
 
 from oarepo_oaipmh_harvester.oai_run.records.dumper import OaiRunDumper
 from oarepo_oaipmh_harvester.oai_run.records.models import OaiRunMetadata
 
 
+class OaiRunIdProvider(RecordIdProviderV2):
+    pid_type = "_rn"
+
+
 class OaiRunRecord(Record):
     model_cls = OaiRunMetadata
 
     schema = ConstantField("$schema", "local://oai_run-1.0.0.json")
 
     index = IndexField("oai_run-oai_run-1.0.0")
 
-    pid = PIDField(
-        create=True, provider=RecordIdProviderV2, context_cls=PIDFieldContext
-    )
+    pid = PIDField(provider=OaiRunIdProvider, context_cls=PIDFieldContext, create=True)
 
     dumper_extensions = []
     dumper = OaiRunDumper(extensions=dumper_extensions)
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947482638888889%*

 * *Differences: {"'properties'": "{'harvester': {'properties': {'created': {'format': 'date-time'}, 'updated': "*

 * *                 "{'format': 'date-time'}}}, 'created': {'format': 'date-time'}, 'updated': "*

 * *                 "{'format': 'date-time'}}"}*

```diff
@@ -3,15 +3,15 @@
         "$schema": {
             "type": "string"
         },
         "batches": {
             "type": "integer"
         },
         "created": {
-            "format": "date",
+            "format": "date-time",
             "type": "string"
         },
         "duration": {
             "type": "number"
         },
         "error": {
             "type": "string"
@@ -34,15 +34,15 @@
                 "code": {
                     "type": "string"
                 },
                 "comment": {
                     "type": "string"
                 },
                 "created": {
-                    "format": "date",
+                    "format": "date-time",
                     "type": "string"
                 },
                 "id": {
                     "type": "string"
                 },
                 "loader": {
                     "type": "string"
@@ -62,15 +62,15 @@
                 "transformers": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "updated": {
-                    "format": "date",
+                    "format": "date-time",
                     "type": "string"
                 },
                 "writer": {
                     "type": "string"
                 }
             },
             "type": "object"
@@ -89,15 +89,15 @@
                 "W",
                 "E",
                 "I"
             ],
             "type": "string"
         },
         "updated": {
-            "format": "date",
+            "format": "date-time",
             "type": "string"
         },
         "warning": {
             "type": "string"
         }
     },
     "type": "object"
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8666666666666667%*

 * *Differences: {"'mappings'": "{'properties': {'run': OrderedDict([('properties', OrderedDict([('id', "*

 * *               "OrderedDict([('type', 'keyword')])), ('@v', OrderedDict([('type', "*

 * *               "'keyword')]))])), ('type', 'object')]), 'identifiers': OrderedDict([('type', "*

 * *               "'keyword')]), 'errors': OrderedDict([('properties', "*

 * *               "OrderedDict([('oai_identifier', OrderedDict([('type', 'keyword')])), ('error', "*

 * *               "OrderedDict([('type', 'text'), ('fields', OrderedDict([('keyw […]*

```diff
@@ -1,89 +1,57 @@
 {
     "mappings": {
         "properties": {
             "$schema": {
                 "type": "keyword"
             },
-            "batches": {
-                "type": "integer"
-            },
             "created": {
                 "type": "date"
             },
-            "duration": {
-                "type": "double"
-            },
-            "error": {
-                "type": "keyword"
+            "errors": {
+                "properties": {
+                    "error": {
+                        "fields": {
+                            "keyword": {
+                                "type": "keyword"
+                            }
+                        },
+                        "type": "text"
+                    },
+                    "oai_identifier": {
+                        "type": "keyword"
+                    }
+                },
+                "type": "object"
             },
             "finished": {
                 "type": "date"
             },
-            "harvester": {
+            "id": {
+                "type": "keyword"
+            },
+            "identifiers": {
+                "type": "keyword"
+            },
+            "run": {
                 "properties": {
-                    "$schema": {
-                        "type": "keyword"
-                    },
-                    "baseurl": {
+                    "@v": {
                         "type": "keyword"
                     },
-                    "batch_size": {
-                        "type": "integer"
-                    },
-                    "code": {
-                        "type": "keyword"
-                    },
-                    "comment": {
-                        "type": "text"
-                    },
-                    "created": {
-                        "type": "date"
-                    },
                     "id": {
                         "type": "keyword"
-                    },
-                    "loader": {
-                        "type": "keyword"
-                    },
-                    "max_records": {
-                        "type": "integer"
-                    },
-                    "metadataprefix": {
-                        "type": "keyword"
-                    },
-                    "name": {
-                        "type": "keyword"
-                    },
-                    "setspecs": {
-                        "type": "keyword"
-                    },
-                    "transformers": {
-                        "type": "keyword"
-                    },
-                    "updated": {
-                        "type": "date"
-                    },
-                    "writer": {
-                        "type": "keyword"
                     }
                 },
                 "type": "object"
             },
-            "id": {
-                "type": "keyword"
-            },
             "started": {
                 "type": "date"
             },
             "status": {
                 "type": "keyword"
             },
             "updated": {
                 "type": "date"
-            },
-            "warning": {
-                "type": "keyword"
             }
         }
     }
 }
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import RecordServiceConfig
-from invenio_records_resources.services import (
-    RecordServiceConfig as InvenioRecordServiceConfig,
-)
 from invenio_records_resources.services import pagination_links
 from invenio_records_resources.services.records.components import DataComponent
 from oarepo_runtime.config.service import PermissionsPresetsConfigMixin
+from oarepo_runtime.relations.components import CachingRelationsComponent
 
 from oarepo_oaipmh_harvester.oai_run.records.api import OaiRunRecord
-from oarepo_oaipmh_harvester.oai_run.services.records.permissions import (
-    OaiRunPermissionPolicy,
-)
 from oarepo_oaipmh_harvester.oai_run.services.records.schema import OaiRunSchema
 from oarepo_oaipmh_harvester.oai_run.services.records.search import OaiRunSearchOptions
 
 
 class OaiRunServiceConfig(PermissionsPresetsConfigMixin, RecordServiceConfig):
     """OaiRunRecord service config."""
 
@@ -23,18 +18,21 @@
     PERMISSIONS_PRESETS = ["oai_harvester"]
 
     schema = OaiRunSchema
 
     search = OaiRunSearchOptions
 
     record_cls = OaiRunRecord
-    # todo should i leave this here?
     service_id = "oarepo-oaipmh-run"
 
-    components = [*RecordServiceConfig.components, DataComponent]
+    components = [
+        *RecordServiceConfig.components,
+        DataComponent,
+        CachingRelationsComponent,
+    ]
 
     model = "oai_run"
 
     @property
     def links_item(self):
         return {
             "self": RecordLink("{self.url_prefix}{id}"),
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/services/records/search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-def _(x):
-    """Identity function for string extraction."""
-    return x
-
-
 class OaiRunSearchOptions(InvenioSearchOptions):
     """OaiRunRecord search options."""
 
     facets = {
         "harvester_id": facets.harvester_id,
         "harvester_code": facets.harvester_code,
         "harvester_baseurl": facets.harvester_baseurl,
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,29 @@
 import marshmallow as ma
-from invenio_records_resources.services.records.schema import (
-    BaseRecordSchema as InvenioBaseRecordSchema,
-)
-from marshmallow import ValidationError
 from marshmallow import fields as ma_fields
-from marshmallow import validate as ma_validate
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
 from oarepo_runtime.ui import marshmallow as l10n
-from oarepo_runtime.validation import validate_date, validate_datetime
+from oarepo_runtime.ui.marshmallow import InvenioUISchema
 
 
-class HarvesterUISchema(ma.Schema):
-    """HarvesterUISchema schema."""
+class RunUISchema(ma.Schema):
+    """RunUISchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
-    code = ma_fields.String()
-    baseurl = ma_fields.String()
-    metadataprefix = ma_fields.String()
-    comment = ma_fields.String()
-    name = ma_fields.String()
-    setspecs = ma_fields.String()
-    loader = ma_fields.String()
-    transformers = ma_fields.List(ma_fields.String())
-    writer = ma_fields.String()
-    max_records = ma_fields.Integer()
-    batch_size = ma_fields.Integer()
-    created = l10n.LocalizedDate()
-    updated = l10n.LocalizedDate()
-    _schema = ma_fields.String(data_key="$schema", attribute="$schema")
-
-
-class OaiRunUISchema(ma.Schema):
-    """OaiRunUISchema schema."""
-
-    harvester = ma_fields.Nested(lambda: HarvesterUISchema())
-    batches = ma_fields.Integer()
-    status = l10n.LocalizedEnum(value_prefix="oarepo_oaipmh_harvester.oai_run")
-    warning = ma_fields.String()
+    _version = ma_fields.String(data_key="@v", attribute="@v")
+
+
+class ErrorsItemUISchema(ma.Schema):
+    """ErrorsItemUISchema schema."""
+
+    oai_identifier = ma_fields.String()
     error = ma_fields.String()
+
+
+class OaiBatchUISchema(InvenioUISchema):
+    """OaiBatchUISchema schema."""
+
+    run = ma_fields.Nested(lambda: RunUISchema())
+    status = l10n.LocalizedEnum(value_prefix="oarepo_oaipmh_harvester.oai_batch")
+    identifiers = ma_fields.List(ma_fields.String())
+    errors = ma_fields.List(ma_fields.Nested(lambda: ErrorsItemUISchema()))
     started = l10n.LocalizedDateTime()
     finished = l10n.LocalizedDateTime()
-    duration = ma_fields.Float()
-    _id = ma_fields.String(data_key="id", attribute="id")
-    created = l10n.LocalizedDate()
-    updated = l10n.LocalizedDate()
-    _schema = ma_fields.String(data_key="$schema", attribute="$schema")
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/views.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/oai_run/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/permissions.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/permissions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from invenio_records_permissions import RecordPermissionPolicy
 from invenio_records_permissions.generators import SystemProcess
 
 
-# TODO: change the permissions for oaipmh group
+from invenio_records_permissions.generators import AnyUser
+
 class OAIHarvesterPermissions(RecordPermissionPolicy):
     """record policy for read only repository"""
 
-    can_search = [SystemProcess()]
-    can_read = [SystemProcess()]
+    can_search = [SystemProcess(), AnyUser()]
+    can_read = [SystemProcess(), AnyUser()]
     can_create = [SystemProcess()]
     can_update = [SystemProcess()]
     can_delete = [SystemProcess()]
     can_manage = [SystemProcess()]
 
     can_create_files = [SystemProcess()]
     can_set_content_files = [SystemProcess()]
```

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/oai_dir.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/oai_dir.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/sickle.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/readers/sickle.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/batch.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/batch.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/marcxml.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/marcxml.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/rule.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/transformers/rule.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/uow.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/uow.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/utils.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/oai.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai_dir.py` & `oarepo-oai-pmh-harvester-4.0.6/oarepo_oaipmh_harvester/writers/oai_dir.py`

 * *Files identical despite different names*

