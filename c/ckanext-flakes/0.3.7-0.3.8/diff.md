# Comparing `tmp/ckanext-flakes-0.3.7.tar.gz` & `tmp/ckanext-flakes-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-flakes-0.3.7.tar", last modified: Thu Mar 23 22:49:31 2023, max compression
+gzip compressed data, was "ckanext-flakes-0.3.8.tar", last modified: Wed Apr 19 15:25:55 2023, max compression
```

## Comparing `ckanext-flakes-0.3.7.tar` & `ckanext-flakes-0.3.8.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.012009 ckanext-flakes-0.3.7/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2023-03-11 13:04:37.000000 ckanext-flakes-0.3.7/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13114 2023-03-23 22:49:31.012009 ckanext-flakes-0.3.7/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12494 2023-03-12 09:07:40.000000 ckanext-flakes-0.3.7/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      430 2023-03-11 10:05:29.000000 ckanext-flakes-0.3.7/ckanext/flakes/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1263 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12927 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2932 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.7/ckanext/flakes/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4241 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:30.992009 ckanext-flakes-0.3.7/ckanext/flakes/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1780 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      439 2023-03-11 04:52:30.000000 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/versions/a7384c7e0e27_nullable_author.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1114 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3028 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/model/flake.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1934 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       84 2023-03-23 14:32:10.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      159 2023-03-23 14:34:44.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      261 2023-03-23 18:29:13.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/config_declaration.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-23 18:32:20.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3038 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      844 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      895 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1130 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      704 2023-03-23 22:16:21.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1632 2023-03-23 22:46:16.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1314 2023-03-23 22:21:28.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      267 2023-03-23 14:52:52.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/package/read_base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4183 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       80 2023-03-11 13:07:23.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1234 2023-03-12 12:19:39.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2022-11-07 20:13:24.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      638 2023-03-23 14:47:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-03-23 14:46:56.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-07 20:13:24.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3401 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      903 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1286 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/flakes_rating/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1306 2023-03-01 18:07:56.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      530 2023-03-23 14:45:35.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/package/read_base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1376 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/plugins/scheming.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/conftest.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/flake_dataset.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      130 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/flake_group.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      144 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/flake_organization.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17166 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6713 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1606 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.002009 ckanext-flakes-0.3.7/ckanext/flakes/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5762 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/model/test_flake.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      311 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.012009 ckanext-flakes-0.3.7/ckanext/flakes/tests/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/plugins/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2254 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/plugins/test_scheming.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      449 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2513 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.7/ckanext/flakes/types.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-23 22:49:31.012009 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13114 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3065 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-23 22:49:30.000000 ckanext-flakes-0.3.7/ckanext_flakes.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2820 2023-03-11 09:14:51.000000 ckanext-flakes-0.3.7/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1927 2023-03-23 22:49:31.012009 ckanext-flakes-0.3.7/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.7/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2023-03-11 13:04:37.000000 ckanext-flakes-0.3.8/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13078 2023-04-12 09:35:34.000000 ckanext-flakes-0.3.8/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      430 2023-03-11 10:05:29.000000 ckanext-flakes-0.3.8/ckanext/flakes/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1263 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12927 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2932 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.8/ckanext/flakes/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4241 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1780 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      439 2023-03-11 04:52:30.000000 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/versions/a7384c7e0e27_nullable_author.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1114 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3028 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/model/flake.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1934 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       84 2023-03-23 14:32:10.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      159 2023-03-23 14:34:44.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      261 2023-03-23 18:29:13.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/config_declaration.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-23 18:32:20.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3038 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      844 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      895 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1130 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      704 2023-03-23 22:16:21.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1632 2023-03-23 22:46:16.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1314 2023-03-23 22:21:28.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      269 2023-04-12 09:33:57.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/package/read_base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4183 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       80 2023-03-11 13:07:23.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1402 2023-04-19 13:34:29.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2022-11-07 20:13:24.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      638 2023-03-23 14:47:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-03-23 14:46:56.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-07 20:13:24.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3401 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      903 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1286 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2023-03-23 22:28:12.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.891189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/flakes_rating/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1469 2023-04-19 13:33:00.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      530 2023-03-23 14:45:35.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/package/read_base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1376 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/plugins/scheming.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/conftest.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/flake_dataset.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      130 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/flake_group.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      144 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/flake_organization.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17166 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6713 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1606 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5762 2023-03-11 09:14:54.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/model/test_flake.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      311 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext/flakes/tests/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/plugins/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2254 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/plugins/test_scheming.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      449 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2513 2023-03-09 06:46:46.000000 ckanext-flakes-0.3.8/ckanext/flakes/types.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3065 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-19 15:25:55.000000 ckanext-flakes-0.3.8/ckanext_flakes.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2820 2023-03-11 09:14:51.000000 ckanext-flakes-0.3.8/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1927 2023-04-19 15:25:55.901189 ckanext-flakes-0.3.8/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-25 15:10:26.000000 ckanext-flakes-0.3.8/setup.py
```

### Comparing `ckanext-flakes-0.3.7/LICENSE` & `ckanext-flakes-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/PKG-INFO` & `ckanext-flakes-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: ckanext-flakes
-Version: 0.3.7
-Home-page: https://github.com/DataShades/ckanext-flakes
-Author: Sergey Motornyuk
-Author-email: sergey.motornyuk@linkdigital.com.au
-License: AGPL
-Keywords: CKAN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Tests](https://github.com/DataShades/ckanext-flakes/workflows/Tests/badge.svg)](https://github.com/DataShades/ckanext-flakes/actions/workflows/test.yml)
 
 # ckanext-flakes
 
 Tools for creating and managing independent chunks of data.
 
 This extension provides a base entity for storing arbitrary data. It can be
@@ -29,14 +12,15 @@
 dictionary-like objects(anything, that can be serialized into JSON). If you are
 using it and want to add an extra action, feel free to create a PR or an issue
 with your suggestion.
 
 ## Structure
 
 * [Examples](#examples)
+* [Example plugins](#example-plugins)
 * [Requirements](#definition)
 * [Installation](#installation)
 * [Configuration](#configuration)
 * [Interfaces](#interfaces)
 * [API](#api)
   * [`flakes_flake_create`](#flakes_flake_create)
   * [`flakes_flake_show`](#flakes_flake_show)
@@ -183,14 +167,31 @@
 value = tk.get_action("flakes_flake_lookup")(
     {"ignore_auth": True},
     {"name": "global:config:value", "author_id": None}
 )["data"]["value"]
 ```
 
 
+## Example plugins
+
+These plugins implement basic features that can be used as a real-life example
+of `ckanext-flakes` usage.
+
+### `flakes_rating`
+
+User can rate a package via API action. Add
+`ckanext.flakes_rating.show_package_widget = true` to the config and default
+widget will be added to the sidebar on `dataset.read` page.
+
+### `flakes_feedback`
+
+User can leave a feedback for package via API action. Add
+`ckanext.flakes_feedback.enable_views = true` to the config and default page
+will be added to navigation tabs on `dataset.read` page.
+
 ## Requirements
 
 Requires python v3.7 or greater. Python v2 support doesn't require much effort,
 but it neither worth the time you'll spend on it.
 
 
 Compatibility with core CKAN versions:
```

### Comparing `ckanext-flakes-0.3.7/README.md` & `ckanext-flakes-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: ckanext-flakes
+Version: 0.3.8
+Home-page: https://github.com/DataShades/ckanext-flakes
+Author: Sergey Motornyuk
+Author-email: sergey.motornyuk@linkdigital.com.au
+License: AGPL
+Keywords: CKAN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Tests](https://github.com/DataShades/ckanext-flakes/workflows/Tests/badge.svg)](https://github.com/DataShades/ckanext-flakes/actions/workflows/test.yml)
 
 # ckanext-flakes
 
 Tools for creating and managing independent chunks of data.
 
 This extension provides a base entity for storing arbitrary data. It can be
@@ -12,14 +29,15 @@
 dictionary-like objects(anything, that can be serialized into JSON). If you are
 using it and want to add an extra action, feel free to create a PR or an issue
 with your suggestion.
 
 ## Structure
 
 * [Examples](#examples)
+* [Example plugins](#example-plugins)
 * [Requirements](#definition)
 * [Installation](#installation)
 * [Configuration](#configuration)
 * [Interfaces](#interfaces)
 * [API](#api)
   * [`flakes_flake_create`](#flakes_flake_create)
   * [`flakes_flake_show`](#flakes_flake_show)
@@ -166,14 +184,31 @@
 value = tk.get_action("flakes_flake_lookup")(
     {"ignore_auth": True},
     {"name": "global:config:value", "author_id": None}
 )["data"]["value"]
 ```
 
 
+## Example plugins
+
+These plugins implement basic features that can be used as a real-life example
+of `ckanext-flakes` usage.
+
+### `flakes_rating`
+
+User can rate a package via API action. Add
+`ckanext.flakes_rating.show_package_widget = true` to the config and default
+widget will be added to the sidebar on `dataset.read` page.
+
+### `flakes_feedback`
+
+User can leave a feedback for package via API action. Add
+`ckanext.flakes_feedback.enable_views = true` to the config and default page
+will be added to navigation tabs on `dataset.read` page.
+
 ## Requirements
 
 Requires python v3.7 or greater. Python v2 support doesn't require much effort,
 but it neither worth the time you'll spend on it.
 
 
 Compatibility with core CKAN versions:
```

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/interfaces.py` & `ckanext-flakes-0.3.8/ckanext/flakes/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/logic/action.py` & `ckanext-flakes-0.3.8/ckanext/flakes/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/logic/auth.py` & `ckanext-flakes-0.3.8/ckanext/flakes/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/logic/schema.py` & `ckanext-flakes-0.3.8/ckanext/flakes/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/logic/validators.py` & `ckanext-flakes-0.3.8/ckanext/flakes/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/alembic.ini` & `ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/env.py` & `ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py` & `ckanext-flakes-0.3.8/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/model/flake.py` & `ckanext-flakes-0.3.8/ckanext/flakes/model/flake.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugin.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/action.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/auth.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/logic/schema.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/plugin.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/feedback/views.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/feedback/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,16 @@
     "use strict";
 
     return {
         options: {
             type: null,
             id: null,
             current: 0,
+            starClass: "fa-star-o",
+            starFilledClass: "fa-star",
         },
         initialize: function() {
             $.proxyAll(this, /_on/);
             this.el.find(".star").on({
                 click: this._onClick,
                 mouseover: this._onOver,
                 mouseout: this._onOut,
@@ -18,17 +20,18 @@
                 this.setStars(this.options.current);
             }
         },
         setStars: function(n) {
             var el = this.$(".star").eq(n - 1);
             el.prevAll()
                 .add(el)
-                .removeClass("star-empty fa-star-o")
-                .addClass("fa-star");
-            el.nextAll().addClass("star-empty fa-star-o").removeClass("fa-star");
+                .removeClass("star-empty")
+                .removeClass(this.options.starClass)
+                .addClass(this.options.starFilledClass);
+            el.nextAll().addClass("star-empty").addClass(this.options.starClass).removeClass(this.options.starFilledClass);
         },
 
         _onClick: function(e) {
             var rating = this.$(".star").index(e.target) + 1;
             this.setStars(rating);
             this.sandbox.client.call("POST", "flakes_rating_rate", {
                 target_type: this.options.type,
```

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/config.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/config_declaration.yaml` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/helpers.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/action.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/auth.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/logic/schema.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/plugin.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 id
 fa_star - FontAwesome class of the star icon
 #}
 {% asset "flakes_rating/rate" %}
 
 {% set rating = h.flakes_rating_get_rating(type, id) %}
 {% set fa_star = fa_star|default("fa-star-o") %}
+{% set fa_filled_star = fa_filled_star|default("fa-star") %}
 
 
 <style>
  .flakes-rating--rate-widget .star-holder {
      display: flex;
      justify-content: space-around;
  }
@@ -36,14 +37,16 @@
 </p>
 
 <div class="flakes-rating--rate-widget m-bottom"
      {% if h.check_access("flakes_rating_rate", {"target_type": type, "target_id": id}) %} data-module="flakes-rating-rate"{% endif %}
      data-module-type="{{ type }}"
      data-module-id="{{ id }}"
      data-module-current="{{ rating.own }}"
+     data-module-star-class="{{ fa_star }}"
+     data-module-star-filled-class="{{ fa_filled_star }}"
 >
     <div class="star-holder">
         {% for i in range(5) %}
             <i class="fa star-empty star {{ fa_star }}"></i>
         {% endfor %}
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 {# type id fa_star - FontAwesome class of the star icon #} {% asset
 "flakes_rating/rate" %} {% set rating = h.flakes_rating_get_rating(type, id) %}
-{% set fa_star = fa_star|default("fa-star-o") %}
+{% set fa_star = fa_star|default("fa-star-o") %} {% set fa_filled_star =
+fa_filled_star|default("fa-star") %}
 {{ _("Current rating(based on {count} votes):").format(count=rating.count) }} {
 { "{average:.2f}".format(average=rating.average) }}
 % if h.check_access("flakes_rating_rate", {"target_type": type, "target_id":
 id}) %} data-module="flakes-rating-rate"{% endif %} data-module-type="{{ type
-}}" data-module-id="{{ id }}" data-module-current="{{ rating.own }}" >
+}}" data-module-id="{{ id }}" data-module-current="{{ rating.own }}" data-
+module-star-class="{{ fa_star }}" data-module-star-filled-class="{
+{ fa_filled_star }}" >
 {% for i in range(5) %}  {% endfor %}
```

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/rating/templates/package/read_base.html` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/rating/templates/package/read_base.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/plugins/scheming.py` & `ckanext-flakes-0.3.8/ckanext/flakes/plugins/scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_action.py` & `ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_auth.py` & `ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/tests/logic/test_validators.py` & `ckanext-flakes-0.3.8/ckanext/flakes/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/tests/model/test_flake.py` & `ckanext-flakes-0.3.8/ckanext/flakes/tests/model/test_flake.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/tests/plugins/test_scheming.py` & `ckanext-flakes-0.3.8/ckanext/flakes/tests/plugins/test_scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext/flakes/types.py` & `ckanext-flakes-0.3.8/ckanext/flakes/types.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/ckanext_flakes.egg-info/PKG-INFO` & `ckanext-flakes-0.3.8/ckanext_flakes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-flakes
-Version: 0.3.7
+Version: 0.3.8
 Home-page: https://github.com/DataShades/ckanext-flakes
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -29,14 +29,15 @@
 dictionary-like objects(anything, that can be serialized into JSON). If you are
 using it and want to add an extra action, feel free to create a PR or an issue
 with your suggestion.
 
 ## Structure
 
 * [Examples](#examples)
+* [Example plugins](#example-plugins)
 * [Requirements](#definition)
 * [Installation](#installation)
 * [Configuration](#configuration)
 * [Interfaces](#interfaces)
 * [API](#api)
   * [`flakes_flake_create`](#flakes_flake_create)
   * [`flakes_flake_show`](#flakes_flake_show)
@@ -183,14 +184,31 @@
 value = tk.get_action("flakes_flake_lookup")(
     {"ignore_auth": True},
     {"name": "global:config:value", "author_id": None}
 )["data"]["value"]
 ```
 
 
+## Example plugins
+
+These plugins implement basic features that can be used as a real-life example
+of `ckanext-flakes` usage.
+
+### `flakes_rating`
+
+User can rate a package via API action. Add
+`ckanext.flakes_rating.show_package_widget = true` to the config and default
+widget will be added to the sidebar on `dataset.read` page.
+
+### `flakes_feedback`
+
+User can leave a feedback for package via API action. Add
+`ckanext.flakes_feedback.enable_views = true` to the config and default page
+will be added to navigation tabs on `dataset.read` page.
+
 ## Requirements
 
 Requires python v3.7 or greater. Python v2 support doesn't require much effort,
 but it neither worth the time you'll spend on it.
 
 
 Compatibility with core CKAN versions:
```

### Comparing `ckanext-flakes-0.3.7/ckanext_flakes.egg-info/SOURCES.txt` & `ckanext-flakes-0.3.8/ckanext_flakes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/pyproject.toml` & `ckanext-flakes-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.3.7/setup.cfg` & `ckanext-flakes-0.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-flakes
-version = 0.3.7
+version = 0.3.8
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-flakes
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-flakes-0.3.7/setup.py` & `ckanext-flakes-0.3.8/setup.py`

 * *Files identical despite different names*

