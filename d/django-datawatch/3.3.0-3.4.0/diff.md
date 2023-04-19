# Comparing `tmp/django-datawatch-3.3.0.tar.gz` & `tmp/django-datawatch-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-datawatch-3.3.0.tar", last modified: Mon Jan  2 16:56:32 2023, max compression
+gzip compressed data, was "django-datawatch-3.4.0.tar", last modified: Wed Apr 19 16:22:20 2023, max compression
```

## Comparing `django-datawatch-3.3.0.tar` & `django-datawatch-3.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/backends/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/backends/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/datawatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.743073 django-datawatch-3.3.0/django_datawatch/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.743073 django-datawatch-3.3.0/django_datawatch/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/django_datawatch/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_list_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_refresh_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_run_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/django_datawatch/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/migrations/0002_auto_20180807_1508.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/migrations/0003_resultstatushistory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/querysets.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.743073 django-datawatch-3.3.0/django_datawatch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/django_datawatch/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/templatetags/class_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/django_datawatch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/test_base_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/test_post_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/tests/test_trigger_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/django_datawatch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:56:32.747073 django-datawatch-3.3.0/django_datawatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-01-02 16:56:32.000000 django-datawatch-3.3.0/django_datawatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-02 16:56:32.000000 django-datawatch-3.3.0/django_datawatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 16:56:32.000000 django-datawatch-3.3.0/django_datawatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-02 16:56:32.000000 django-datawatch-3.3.0/django_datawatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-02 16:56:32.000000 django-datawatch-3.3.0/django_datawatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-02 16:56:32.751073 django-datawatch-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-01-02 16:56:27.000000 django-datawatch-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/datawatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_list_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_refresh_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_run_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0002_auto_20180807_1508.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0003_resultstatushistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templatetags/class_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_base_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_post_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_trigger_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 16:22:20.627444 django-datawatch-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/setup.py
```

### Comparing `django-datawatch-3.3.0/LICENSE` & `django-datawatch-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/PKG-INFO` & `django-datawatch-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.3.0
+Version: 3.4.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
@@ -239,20 +239,20 @@
 ```bash
 docker-compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint=celery app worker -A example -l DEBUG
+docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint=celery app beat --scheduler django_celery_beat.schedulers:DatabaseScheduler -A example
+docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
```

### Comparing `django-datawatch-3.3.0/README.md` & `django-datawatch-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -213,20 +213,20 @@
 ```bash
 docker-compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint=celery app worker -A example -l DEBUG
+docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint=celery app beat --scheduler django_celery_beat.schedulers:DatabaseScheduler -A example
+docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
```

### Comparing `django-datawatch-3.3.0/django_datawatch/admin.py` & `django-datawatch-3.4.0/django_datawatch/admin.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/backends/celery.py` & `django-datawatch-3.4.0/django_datawatch/backends/celery.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/backends/synchronous.py` & `django-datawatch-3.4.0/django_datawatch/backends/synchronous.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/base.py` & `django-datawatch-3.4.0/django_datawatch/base.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/common/views.py` & `django-datawatch-3.4.0/django_datawatch/common/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/datawatch.py` & `django-datawatch-3.4.0/django_datawatch/datawatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,20 +90,20 @@
         if self._backend is None:
             backend_module = importlib.import_module(
                 getattr(settings, 'DJANGO_DATAWATCH_BACKEND',
                         defaults['BACKEND']))
             self._backend = backend_module.Backend()
         return self._backend
 
-    def delete_results(self, sender, instance):
+    def delete_results(self, sender, instance, db_alias=None):
         from django_datawatch.models import Result
         for check_class in datawatch.get_checks_for_model(model=sender):
             check = check_class()
             identifier = check.get_identifier(instance)
-            Result.objects.filter(slug=check.slug, identifier=identifier).delete()
+            Result.objects.using(db_alias).filter(slug=check.slug, identifier=identifier).delete()
 
     def update_related(self, sender, instance):
         checks = datawatch.get_checks_for_related_model(sender) or []
         for check_class in checks:
             check = check_class()
             backend = datawatch.get_backend()
             model_uid = make_model_uid(instance.__class__)
@@ -185,15 +185,15 @@
     return "%s.%s" % (model._meta.app_label, model.__name__)
 
 
 def delete_results(sender, instance, using, **kwargs):
     if not getattr(settings, 'DJANGO_DATAWATCH_RUN_SIGNALS',
                    defaults['RUN_SIGNALS']):
         return
-    datawatch.delete_results(sender, instance)
+    datawatch.delete_results(sender, instance, using)
 
 
 def run_checks(sender, instance, created, raw, using, **kwargs):
     """
     Re-execute checks related to the given sender model, only for the
     updated instance.
```

### Comparing `django-datawatch-3.3.0/django_datawatch/forms.py` & `django-datawatch-3.4.0/django_datawatch/forms.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/locale/de/LC_MESSAGES/django.mo` & `django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/locale/de/LC_MESSAGES/django.po` & `django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_refresh_results.py` & `django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_refresh_results.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/management/commands/datawatch_run_checks.py` & `django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_run_checks.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/migrations/0001_initial.py` & `django-datawatch-3.4.0/django_datawatch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/migrations/0002_auto_20180807_1508.py` & `django-datawatch-3.4.0/django_datawatch/migrations/0002_auto_20180807_1508.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/migrations/0003_resultstatushistory.py` & `django-datawatch-3.4.0/django_datawatch/migrations/0003_resultstatushistory.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/models.py` & `django-datawatch-3.4.0/django_datawatch/models.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/querysets.py` & `django-datawatch-3.4.0/django_datawatch/querysets.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/base.html` & `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/base.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/dashboard.html` & `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/detail.html` & `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/detail.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/templates/django_datawatch/form.html` & `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/form.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/tests/test_base_check.py` & `django-datawatch-3.4.0/django_datawatch/tests/test_base_check.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/tests/test_integration.py` & `django-datawatch-3.4.0/django_datawatch/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/tests/test_post_delete.py` & `django-datawatch-3.4.0/django_datawatch/tests/test_post_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def test_update_related_calls_backend(self, mock_get_checks_for_model):
         # mock the list of checks
         mock_get_checks_for_model.return_value = [CheckPostDelete]
 
         # mock the manager
         manager = mock.Mock(spec=ResultQuerySet)
         Result.objects = manager
+        manager.using.return_value = manager
         manager_filtered = mock.Mock(spec=ResultQuerySet)
         manager.filter.return_value = manager_filtered
 
         # test if delete has been called
         datawatch.delete_results(sender=Result, instance=Result(pk=1))
         manager.filter.assert_called_with(slug=CheckPostDelete().slug, identifier=1)
         manager_filtered.delete.assert_called_with()
```

### Comparing `django-datawatch-3.3.0/django_datawatch/tests/test_scheduler.py` & `django-datawatch-3.4.0/django_datawatch/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/tests/test_trigger_update.py` & `django-datawatch-3.4.0/django_datawatch/tests/test_trigger_update.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/urls.py` & `django-datawatch-3.4.0/django_datawatch/urls.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch/views.py` & `django-datawatch-3.4.0/django_datawatch/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/django_datawatch.egg-info/PKG-INFO` & `django-datawatch-3.4.0/django_datawatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.3.0
+Version: 3.4.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
@@ -239,20 +239,20 @@
 ```bash
 docker-compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint=celery app worker -A example -l DEBUG
+docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint=celery app beat --scheduler django_celery_beat.schedulers:DatabaseScheduler -A example
+docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
```

### Comparing `django-datawatch-3.3.0/django_datawatch.egg-info/SOURCES.txt` & `django-datawatch-3.4.0/django_datawatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.3.0/setup.py` & `django-datawatch-3.4.0/setup.py`

 * *Files identical despite different names*

