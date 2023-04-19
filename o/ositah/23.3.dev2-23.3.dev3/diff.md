# Comparing `tmp/ositah-23.3.dev2.tar.gz` & `tmp/ositah-23.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ositah-23.3.dev2.tar", last modified: Sat Mar 11 10:29:34 2023, max compression
+gzip compressed data, was "ositah-23.3.dev3.tar", last modified: Sat Mar 11 11:11:49 2023, max compression
```

## Comparing `ositah-23.3.dev2.tar` & `ositah-23.3.dev3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.883361 ositah-23.3.dev2/
--rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-23.3.dev2/.gitignore
--rw-rw-rw-   0        0        0      341 2023-02-13 17:50:27.000000 ositah-23.3.dev2/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-23.3.dev2/LICENSE
--rw-rw-rw-   0        0        0     7693 2023-03-11 10:29:34.882368 ositah-23.3.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-23.3.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.494150 ositah-23.3.dev2/gunicorn.config/
--rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-23.3.dev2/gunicorn.config/README.md
--rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-23.3.dev2/gunicorn.config/gunicorn.ositah
--rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-23.3.dev2/gunicorn.config/gunicorn@.service
--rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-23.3.dev2/gunicorn.config/ositah.conf.py
--rw-rw-rw-   0        0        0     1243 2022-11-13 21:10:36.000000 ositah-23.3.dev2/noxfile.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.516680 ositah-23.3.dev2/ositah/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev2/ositah/__init__.py
--rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-23.3.dev2/ositah/app.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.584255 ositah-23.3.dev2/ositah/apps/
--rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-23.3.dev2/ositah/apps/analysis.py
--rw-rw-rw-   0        0        0    34803 2023-03-11 10:27:03.000000 ositah-23.3.dev2/ositah/apps/configuration.py
--rw-rw-rw-   0        0        0    47246 2023-02-27 19:50:46.000000 ositah-23.3.dev2/ositah/apps/export.py
--rw-rw-rw-   0        0        0    53059 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/apps/validation.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.639073 ositah-23.3.dev2/ositah/assets/
--rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/assets/arrow_down_up.svg
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/assets/ositah.css
--rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/assets/sort_ascending.svg
--rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/assets/sort_descending.svg
--rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/assets/sorttable.js
--rw-rw-rw-   0        0        0    15685 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/main.py
--rw-rw-rw-   0        0        0     7471 2023-02-24 17:01:35.000000 ositah-23.3.dev2/ositah/ositah.example.cfg
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.641752 ositah-23.3.dev2/ositah/static/
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/static/style.css
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.663357 ositah-23.3.dev2/ositah/templates/
--rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/templates/base.html
--rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/templates/bootstrap_login.html
--rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-23.3.dev2/ositah/templates/login_form.html
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.757449 ositah-23.3.dev2/ositah/utils/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev2/ositah/utils/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/agents.py
--rw-rw-rw-   0        0        0     9149 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/authentication.py
--rw-rw-rw-   0        0        0      504 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/cache.py
--rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-23.3.dev2/ositah/utils/core.py
--rw-rw-rw-   0        0        0     1500 2023-02-24 18:11:54.000000 ositah-23.3.dev2/ositah/utils/exceptions.py
--rw-rw-rw-   0        0        0     1510 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/hito_db.py
--rw-rw-rw-   0        0        0     8988 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/hito_db_model.py
--rw-rw-rw-   0        0        0    11127 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/menus.py
--rw-rw-rw-   0        0        0     3617 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/period.py
--rw-rw-rw-   0        0        0    39683 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/projects.py
--rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-23.3.dev2/ositah/utils/teams.py
--rw-rw-rw-   0        0        0    16370 2023-03-10 16:43:58.000000 ositah-23.3.dev2/ositah/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.548690 ositah-23.3.dev2/ositah.egg-info/
--rw-rw-rw-   0        0        0     7693 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      181 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-11 10:29:34.000000 ositah-23.3.dev2/ositah.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-03-10 16:43:58.000000 ositah-23.3.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-11 10:29:34.884361 ositah-23.3.dev2/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-23.3.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.867391 ositah-23.3.dev2/test-dash/
--rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/README.md
--rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/accordion.py
--rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-23.3.dev2/test-dash/authentication.py
--rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/checkbox.py
--rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/checklist.py
--rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/file-selector.py
--rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/file-upload.py
--rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/long_running_callback.py
--rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/pandas_split.py
--rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/pandas_split_bug_report.py
--rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/pattern-matching-callback.py
--rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/progess_bar.py
--rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/reset_table_checkboxes.py
--rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/sortable_table.py
--rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/sqlalchemy_test.py
-drwxrwxrwx   0        0        0        0 2023-03-11 10:29:34.880398 ositah-23.3.dev2/test-dash/templates/
--rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/templates/base.html
--rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-23.3.dev2/test-dash/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.151095 ositah-23.3.dev3/
+-rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-23.3.dev3/.gitignore
+-rw-rw-rw-   0        0        0      341 2023-02-13 17:50:27.000000 ositah-23.3.dev3/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-23.3.dev3/LICENSE
+-rw-rw-rw-   0        0        0     7693 2023-03-11 11:11:49.151095 ositah-23.3.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-23.3.dev3/README.md
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.061528 ositah-23.3.dev3/gunicorn.config/
+-rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/README.md
+-rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/gunicorn.ositah
+-rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/gunicorn@.service
+-rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/ositah.conf.py
+-rw-rw-rw-   0        0        0     1243 2022-11-13 21:10:36.000000 ositah-23.3.dev3/noxfile.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.067523 ositah-23.3.dev3/ositah/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-23.3.dev3/ositah/app.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.091534 ositah-23.3.dev3/ositah/apps/
+-rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-23.3.dev3/ositah/apps/analysis.py
+-rw-rw-rw-   0        0        0    34803 2023-03-11 10:27:03.000000 ositah-23.3.dev3/ositah/apps/configuration.py
+-rw-rw-rw-   0        0        0    47246 2023-02-27 19:50:46.000000 ositah-23.3.dev3/ositah/apps/export.py
+-rw-rw-rw-   0        0        0    53059 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/apps/validation.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.098089 ositah-23.3.dev3/ositah/assets/
+-rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/arrow_down_up.svg
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/ositah.css
+-rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sort_ascending.svg
+-rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sort_descending.svg
+-rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sorttable.js
+-rw-rw-rw-   0        0        0    15685 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/main.py
+-rw-rw-rw-   0        0        0     7471 2023-02-24 17:01:35.000000 ositah-23.3.dev3/ositah/ositah.example.cfg
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.101091 ositah-23.3.dev3/ositah/static/
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/static/style.css
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.105093 ositah-23.3.dev3/ositah/templates/
+-rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/base.html
+-rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/bootstrap_login.html
+-rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.124090 ositah-23.3.dev3/ositah/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/agents.py
+-rw-rw-rw-   0        0        0     9149 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/authentication.py
+-rw-rw-rw-   0        0        0      504 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/cache.py
+-rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-23.3.dev3/ositah/utils/core.py
+-rw-rw-rw-   0        0        0     1500 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1510 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/hito_db.py
+-rw-rw-rw-   0        0        0     8988 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/hito_db_model.py
+-rw-rw-rw-   0        0        0    11127 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/menus.py
+-rw-rw-rw-   0        0        0     3617 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/period.py
+-rw-rw-rw-   0        0        0    39683 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/projects.py
+-rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/teams.py
+-rw-rw-rw-   0        0        0    16370 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.086534 ositah-23.3.dev3/ositah.egg-info/
+-rw-rw-rw-   0        0        0     7693 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2023-03-11 11:11:49.000000 ositah-23.3.dev3/ositah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      181 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-03-11 11:10:11.000000 ositah-23.3.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-11 11:11:49.152094 ositah-23.3.dev3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-23.3.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.145105 ositah-23.3.dev3/test-dash/
+-rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/README.md
+-rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/accordion.py
+-rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-23.3.dev3/test-dash/authentication.py
+-rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/checkbox.py
+-rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/checklist.py
+-rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/file-selector.py
+-rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/file-upload.py
+-rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/long_running_callback.py
+-rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pandas_split.py
+-rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pandas_split_bug_report.py
+-rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pattern-matching-callback.py
+-rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/progess_bar.py
+-rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/reset_table_checkboxes.py
+-rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/sortable_table.py
+-rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/sqlalchemy_test.py
+drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.149097 ositah-23.3.dev3/test-dash/templates/
+-rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/templates/base.html
+-rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/templates/login_form.html
```

### Comparing `ositah-23.3.dev2/LICENSE` & `ositah-23.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/PKG-INFO` & `ositah-23.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 23.3.dev2
+Version: 23.3.dev3
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-23.3.dev2/README.md` & `ositah-23.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/gunicorn.config/README.md` & `ositah-23.3.dev3/gunicorn.config/README.md`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/noxfile.py` & `ositah-23.3.dev3/noxfile.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/apps/analysis.py` & `ositah-23.3.dev3/ositah/apps/analysis.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/apps/configuration.py` & `ositah-23.3.dev3/ositah/apps/configuration.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/apps/export.py` & `ositah-23.3.dev3/ositah/apps/export.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/apps/validation.py` & `ositah-23.3.dev3/ositah/apps/validation.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/assets/ositah.css` & `ositah-23.3.dev3/ositah/assets/ositah.css`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/assets/sort_ascending.svg` & `ositah-23.3.dev3/ositah/assets/sort_ascending.svg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/assets/sort_descending.svg` & `ositah-23.3.dev3/ositah/assets/sort_descending.svg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/assets/sorttable.js` & `ositah-23.3.dev3/ositah/assets/sorttable.js`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/main.py` & `ositah-23.3.dev3/ositah/main.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/ositah.example.cfg` & `ositah-23.3.dev3/ositah/ositah.example.cfg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/static/style.css` & `ositah-23.3.dev3/ositah/static/style.css`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/templates/base.html` & `ositah-23.3.dev3/ositah/templates/base.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/templates/bootstrap_login.html` & `ositah-23.3.dev3/ositah/templates/bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/templates/login_form.html` & `ositah-23.3.dev3/ositah/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/agents.py` & `ositah-23.3.dev3/ositah/utils/agents.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/authentication.py` & `ositah-23.3.dev3/ositah/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/exceptions.py` & `ositah-23.3.dev3/ositah/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/hito_db.py` & `ositah-23.3.dev3/ositah/utils/hito_db.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/hito_db_model.py` & `ositah-23.3.dev3/ositah/utils/hito_db_model.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/menus.py` & `ositah-23.3.dev3/ositah/utils/menus.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/period.py` & `ositah-23.3.dev3/ositah/utils/period.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/projects.py` & `ositah-23.3.dev3/ositah/utils/projects.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/teams.py` & `ositah-23.3.dev3/ositah/utils/teams.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah/utils/utils.py` & `ositah-23.3.dev3/ositah/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/ositah.egg-info/PKG-INFO` & `ositah-23.3.dev3/ositah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 23.3.dev2
+Version: 23.3.dev3
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-23.3.dev2/ositah.egg-info/SOURCES.txt` & `ositah-23.3.dev3/ositah.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/pyproject.toml` & `ositah-23.3.dev3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "setuptools-scm",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ositah"
-version = "23.3.dev2"
+version = "23.3.dev3"
 description = "Outils de Suivi d'Activités basé sur Hito"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
@@ -18,15 +18,15 @@
     "dash",
     "dash-bootstrap-components",
     "flask~=2.2",
     "flask-multipass",
     "flask-sqlalchemy~=3.0",
     "flask-wtf",
     "hito-tools>=23.2",
-    "pandas~=2.0",
+    "pandas==2.*",
     "pymysql",
     "python-ldap",
     "pyyaml",
     "simplejson",
     "sqlalchemy~=2.0",
 ]
 dynamic = []
```

### Comparing `ositah-23.3.dev2/test-dash/accordion.py` & `ositah-23.3.dev3/test-dash/accordion.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/authentication.py` & `ositah-23.3.dev3/test-dash/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/checkbox.py` & `ositah-23.3.dev3/test-dash/checkbox.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/checklist.py` & `ositah-23.3.dev3/test-dash/checklist.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/file-selector.py` & `ositah-23.3.dev3/test-dash/file-selector.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/file-upload.py` & `ositah-23.3.dev3/test-dash/file-upload.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/long_running_callback.py` & `ositah-23.3.dev3/test-dash/long_running_callback.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/pandas_split.py` & `ositah-23.3.dev3/test-dash/pandas_split.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/pandas_split_bug_report.py` & `ositah-23.3.dev3/test-dash/pandas_split_bug_report.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/pattern-matching-callback.py` & `ositah-23.3.dev3/test-dash/pattern-matching-callback.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/progess_bar.py` & `ositah-23.3.dev3/test-dash/progess_bar.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/reset_table_checkboxes.py` & `ositah-23.3.dev3/test-dash/reset_table_checkboxes.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/sortable_table.py` & `ositah-23.3.dev3/test-dash/sortable_table.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/sqlalchemy_test.py` & `ositah-23.3.dev3/test-dash/sqlalchemy_test.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev2/test-dash/templates/login_form.html` & `ositah-23.3.dev3/test-dash/templates/login_form.html`

 * *Files identical despite different names*

