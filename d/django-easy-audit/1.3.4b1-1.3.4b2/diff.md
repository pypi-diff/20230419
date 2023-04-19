# Comparing `tmp/django-easy-audit-1.3.4b1.tar.gz` & `tmp/django-easy-audit-1.3.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-audit-1.3.4b1.tar", last modified: Mon Mar 20 19:30:58 2023, max compression
+gzip compressed data, was "django-easy-audit-1.3.4b2.tar", last modified: Wed Apr 19 15:38:19 2023, max compression
```

## Comparing `django-easy-audit-1.3.4b1.tar` & `django-easy-audit-1.3.4b2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/
--rw-r--r--   0 jason     (1000) jason     (1000)    35141 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)      112 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/MANIFEST.in
--rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      787 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/README.rst
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.007589 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-03-20 19:30:57.000000 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     1630 2023-03-20 19:30:57.000000 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-03-20 19:30:57.000000 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       32 2023-03-20 19:30:57.000000 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       10 2023-03-20 19:30:57.000000 django-easy-audit-1.3.4b1/django_easy_audit.egg-info/top_level.txt
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.011589 django-easy-audit-1.3.4b1/easyaudit/
--rw-rw-r--   0 jason     (1000) jason     (1000)      101 2022-04-07 03:31:02.000000 django-easy-audit-1.3.4b1/easyaudit/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     4461 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b1/easyaudit/admin.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5159 2022-05-24 18:10:15.000000 django-easy-audit-1.3.4b1/easyaudit/admin_helpers.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      294 2022-02-25 18:56:54.000000 django-easy-audit-1.3.4b1/easyaudit/apps.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      410 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b1/easyaudit/backends.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3693 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b1/easyaudit/crudhistory_admin_mixin.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.011589 django-easy-audit-1.3.4b1/easyaudit/middleware/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/middleware/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1912 2020-08-07 17:56:33.000000 django-easy-audit-1.3.4b1/easyaudit/middleware/easyaudit.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/easyaudit/migrations/
--rw-r--r--   0 jason     (1000) jason     (1000)     2290 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0001_initial.py
--rw-r--r--   0 jason     (1000) jason     (1000)      812 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0002_auto_20170125_0759.py
--rw-r--r--   0 jason     (1000) jason     (1000)      837 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0003_auto_20170228_1505.py
--rw-r--r--   0 jason     (1000) jason     (1000)      496 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0004_auto_20170620_1354.py
--rw-r--r--   0 jason     (1000) jason     (1000)      577 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0005_auto_20170713_1155.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1563 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0006_auto_20171018_1242.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1020 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0007_auto_20180105_0838.py
--rw-r--r--   0 jason     (1000) jason     (1000)      704 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0008_auto_20180220_1908.py
--rw-r--r--   0 jason     (1000) jason     (1000)      634 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0009_auto_20180314_2225.py
--rw-r--r--   0 jason     (1000) jason     (1000)      404 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0010_repr_text.py
--rw-r--r--   0 jason     (1000) jason     (1000)      432 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0011_auto_20181101_1339.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1519 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0012_auto_20181018_0012.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      700 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0013_auto_20190723_0126.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      395 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0014_auto_20200513_0008.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5081 2020-11-07 19:27:56.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0015_auto_20201019_1217.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      721 2022-02-12 03:50:51.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0016_alter_crudevent_event_type.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      453 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/0017_alter_requestevent_datetime.py
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/migrations/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     4221 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b1/easyaudit/models.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     6277 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b1/easyaudit/settings.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/easyaudit/signals/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/signals/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     2121 2022-09-04 03:25:59.000000 django-easy-audit-1.3.4b1/easyaudit/signals/auth_signals.py
--rw-rw-r--   0 jason     (1000) jason     (1000)    14466 2022-09-04 03:25:59.000000 django-easy-audit-1.3.4b1/easyaudit/signals/model_signals.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3267 2022-09-04 03:25:59.000000 django-easy-audit-1.3.4b1/easyaudit/signals/request_signals.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.007589 django-easy-audit-1.3.4b1/easyaudit/templates/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.007589 django-easy-audit-1.3.4b1/easyaudit/templates/admin/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/easyaudit/templates/admin/easyaudit/
--rw-r--r--   0 jason     (1000) jason     (1000)      508 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/templates/admin/easyaudit/change_list.html
--rw-r--r--   0 jason     (1000) jason     (1000)     1215 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/templates/admin/easyaudit/purge_confirmation.html
--rw-rw-r--   0 jason     (1000) jason     (1000)     2679 2023-03-20 19:29:30.000000 django-easy-audit-1.3.4b1/easyaudit/utils.py
--rw-r--r--   0 jason     (1000) jason     (1000)       63 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b1/easyaudit/views.py
--rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-03-20 19:30:58.015589 django-easy-audit-1.3.4b1/setup.cfg
--rw-rw-r--   0 jason     (1000) jason     (1000)     1719 2023-03-20 19:29:55.000000 django-easy-audit-1.3.4b1/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/
+-rw-r--r--   0 jason     (1000) jason     (1000)    35141 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)      112 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/MANIFEST.in
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)      787 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/README.rst
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1630 2023-04-19 15:38:19.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       32 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       10 2023-04-19 15:38:19.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      101 2022-04-07 03:31:02.000000 django-easy-audit-1.3.4b2/easyaudit/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4461 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/admin.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5159 2022-05-24 18:10:15.000000 django-easy-audit-1.3.4b2/easyaudit/admin_helpers.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      294 2022-02-25 18:56:54.000000 django-easy-audit-1.3.4b2/easyaudit/apps.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      410 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/backends.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3693 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b2/easyaudit/crudhistory_admin_mixin.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/middleware/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/middleware/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1912 2020-08-07 17:56:33.000000 django-easy-audit-1.3.4b2/easyaudit/middleware/easyaudit.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/migrations/
+-rw-r--r--   0 jason     (1000) jason     (1000)     2290 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0001_initial.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      812 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0002_auto_20170125_0759.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      837 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0003_auto_20170228_1505.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      496 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0004_auto_20170620_1354.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      577 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0005_auto_20170713_1155.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1563 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0006_auto_20171018_1242.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1020 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0007_auto_20180105_0838.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      704 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0008_auto_20180220_1908.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      634 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0009_auto_20180314_2225.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      404 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0010_repr_text.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      432 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0011_auto_20181101_1339.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1519 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0012_auto_20181018_0012.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      700 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0013_auto_20190723_0126.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      395 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0014_auto_20200513_0008.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5081 2020-11-07 19:27:56.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0015_auto_20201019_1217.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      721 2022-02-12 03:50:51.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0016_alter_crudevent_event_type.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      453 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0017_alter_requestevent_datetime.py
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4221 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b2/easyaudit/models.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6277 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/settings.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/signals/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2348 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/auth_signals.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    14865 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/model_signals.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3267 2022-09-04 03:25:59.000000 django-easy-audit-1.3.4b2/easyaudit/signals/request_signals.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/templates/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/templates/admin/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/
+-rw-r--r--   0 jason     (1000) jason     (1000)      508 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/change_list.html
+-rw-r--r--   0 jason     (1000) jason     (1000)     1215 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/purge_confirmation.html
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2893 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/utils.py
+-rw-r--r--   0 jason     (1000) jason     (1000)       63 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/views.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/setup.cfg
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1719 2023-04-19 15:37:59.000000 django-easy-audit-1.3.4b2/setup.py
```

### Comparing `django-easy-audit-1.3.4b1/LICENSE` & `django-easy-audit-1.3.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/PKG-INFO` & `django-easy-audit-1.3.4b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-audit
-Version: 1.3.4b1
+Version: 1.3.4b2
 Summary: Yet another Django audit log app, hopefully the simplest one.
 Home-page: https://github.com/soynatan/django-easy-audit
 Author: Natán Calzolari
 Author-email: natancalzolari@gmail.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Environment :: Plugins
```

### Comparing `django-easy-audit-1.3.4b1/README.rst` & `django-easy-audit-1.3.4b2/README.rst`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/django_easy_audit.egg-info/PKG-INFO` & `django-easy-audit-1.3.4b2/django_easy_audit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-audit
-Version: 1.3.4b1
+Version: 1.3.4b2
 Summary: Yet another Django audit log app, hopefully the simplest one.
 Home-page: https://github.com/soynatan/django-easy-audit
 Author: Natán Calzolari
 Author-email: natancalzolari@gmail.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Environment :: Plugins
```

### Comparing `django-easy-audit-1.3.4b1/django_easy_audit.egg-info/SOURCES.txt` & `django-easy-audit-1.3.4b2/django_easy_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/admin.py` & `django-easy-audit-1.3.4b2/easyaudit/admin.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/admin_helpers.py` & `django-easy-audit-1.3.4b2/easyaudit/admin_helpers.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/crudhistory_admin_mixin.py` & `django-easy-audit-1.3.4b2/easyaudit/crudhistory_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/middleware/easyaudit.py` & `django-easy-audit-1.3.4b2/easyaudit/middleware/easyaudit.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0001_initial.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0002_auto_20170125_0759.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0002_auto_20170125_0759.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0003_auto_20170228_1505.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0003_auto_20170228_1505.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0005_auto_20170713_1155.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0005_auto_20170713_1155.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0006_auto_20171018_1242.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0006_auto_20171018_1242.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0007_auto_20180105_0838.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0007_auto_20180105_0838.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0008_auto_20180220_1908.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0008_auto_20180220_1908.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0009_auto_20180314_2225.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0009_auto_20180314_2225.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0012_auto_20181018_0012.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0012_auto_20181018_0012.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0013_auto_20190723_0126.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0013_auto_20190723_0126.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0015_auto_20201019_1217.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0015_auto_20201019_1217.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/migrations/0016_alter_crudevent_event_type.py` & `django-easy-audit-1.3.4b2/easyaudit/migrations/0016_alter_crudevent_event_type.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/models.py` & `django-easy-audit-1.3.4b2/easyaudit/models.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/settings.py` & `django-easy-audit-1.3.4b2/easyaudit/settings.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/signals/auth_signals.py` & `django-easy-audit-1.3.4b2/easyaudit/signals/auth_signals.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,55 +2,59 @@
 from django.db import transaction
 from django.utils.module_loading import import_string
 
 from easyaudit.middleware.easyaudit import get_current_request
 from easyaudit.models import LoginEvent
 from easyaudit.settings import REMOTE_ADDR_HEADER, WATCH_AUTH_EVENTS, LOGGING_BACKEND, \
     DATABASE_ALIAS
+from easyaudit.utils import should_propagate_exceptions
 
 audit_logger = import_string(LOGGING_BACKEND)()
 
 
 def user_logged_in(sender, request, user, **kwargs):
     try:
         with transaction.atomic(using=DATABASE_ALIAS):
             login_event = audit_logger.login({
                 'login_type': LoginEvent.LOGIN,
                 'username': getattr(user, user.USERNAME_FIELD),
                 'user_id': getattr(user, 'id', None),
                 'remote_ip': request.META[REMOTE_ADDR_HEADER]
             })
-    except:
-        pass
+    except Exception:
+        if should_propagate_exceptions():
+            raise
 
 
 def user_logged_out(sender, request, user, **kwargs):
     try:
         with transaction.atomic(using=DATABASE_ALIAS):
             login_event = audit_logger.login({
                 'login_type': LoginEvent.LOGOUT,
                 'username': getattr(user, user.USERNAME_FIELD),
                 'user_id': getattr(user, 'id', None),
                 'remote_ip': request.META[REMOTE_ADDR_HEADER]
             })
-    except:
-        pass
+    except Exception:
+        if should_propagate_exceptions():
+            raise
 
 
 def user_login_failed(sender, credentials, **kwargs):
     try:
         with transaction.atomic(using=DATABASE_ALIAS):
             request = get_current_request() # request argument not available in django < 1.11
             user_model = get_user_model()
             login_event = audit_logger.login({
                 'login_type': LoginEvent.FAILED,
                 'username': credentials[user_model.USERNAME_FIELD],
                 'remote_ip': request.META[REMOTE_ADDR_HEADER]
             })
-    except:
-        pass
+    except Exception:
+        if should_propagate_exceptions():
+            raise
 
 
 if WATCH_AUTH_EVENTS:
     signals.user_logged_in.connect(user_logged_in, dispatch_uid='easy_audit_signals_logged_in')
     signals.user_logged_out.connect(user_logged_out, dispatch_uid='easy_audit_signals_logged_out')
     signals.user_login_failed.connect(user_login_failed, dispatch_uid='easy_audit_signals_login_failed')
```

### Comparing `django-easy-audit-1.3.4b1/easyaudit/signals/model_signals.py` & `django-easy-audit-1.3.4b2/easyaudit/signals/model_signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from easyaudit.middleware.easyaudit import get_current_request, \
     get_current_user
 from easyaudit.models import CRUDEvent
 from easyaudit.settings import REGISTERED_CLASSES, UNREGISTERED_CLASSES, \
     WATCH_MODEL_EVENTS, CRUD_DIFFERENCE_CALLBACKS, LOGGING_BACKEND, \
     DATABASE_ALIAS
-from easyaudit.utils import get_m2m_field_name, model_delta
+from easyaudit.utils import get_m2m_field_name, model_delta, should_propagate_exceptions
 
 logger = logging.getLogger(__name__)
 audit_logger = import_string(LOGGING_BACKEND)()
 
 
 def should_audit(instance):
     """Returns True or False to indicate whether the instance
@@ -123,21 +123,27 @@
                     except Exception as e:
                         try:
                             logger.exception(
                                 "easy audit had a pre_save exception on CRUDEvent creation. instance: {}, instance pk: {}".format(
                                     instance, instance.pk))
                         except Exception:
                             pass
+
+                        raise e
+
                 if getattr(settings, "TEST", False):
                     crud_flow()
                 else:
                     transaction.on_commit(crud_flow, using=using)
     except Exception:
         logger.exception('easy audit had a pre-save exception.')
 
+        if should_propagate_exceptions():
+            raise
+
 
 def post_save(sender, instance, created, raw, using, update_fields, **kwargs):
     """https://docs.djangoproject.com/es/1.10/ref/signals/#post-save"""
     if raw:
         # Return if loading Fixtures
         return
 
@@ -182,21 +188,27 @@
                     except Exception as e:
                         try:
                             logger.exception(
                                 "easy audit had a post_save exception on CRUDEvent creation. instance: {}, instance pk: {}".format(
                                     instance, instance.pk))
                         except Exception:
                             pass
+
+                        raise e
+
                 if getattr(settings, "TEST", False):
                     crud_flow()
                 else:
                     transaction.on_commit(crud_flow, using=using)
     except Exception:
         logger.exception('easy audit had a post-save exception.')
 
+        if should_propagate_exceptions():
+            raise
+
 
 def _m2m_rev_field_name(model1, model2):
     """Gets the name of the reverse m2m accessor from `model1` to `model2`
 
     For example, if User has a ManyToManyField connected to Group,
     `_m2m_rev_field_name(Group, User)` retrieves the name of the field on
     Group that lists a group's Users. (By default, this field is called
@@ -281,21 +293,26 @@
                     try:
                         logger.exception(
                             "easy audit had a m2m_changed exception on CRUDEvent creation. instance: {}, instance pk: {}".format(
                                 instance, instance.pk))
                     except Exception:
                         pass
 
+                    raise e
+
             if getattr(settings, "TEST", False):
                 crud_flow()
             else:
                 transaction.on_commit(crud_flow, using=using)
     except Exception:
         logger.exception('easy audit had an m2m-changed exception.')
 
+        if should_propagate_exceptions():
+            raise
+
 
 def post_delete(sender, instance, using, **kwargs):
     """https://docs.djangoproject.com/es/1.10/ref/signals/#post-delete"""
     try:
         if not should_audit(instance):
             return False
 
@@ -329,20 +346,25 @@
                     try:
                         logger.exception(
                             "easy audit had a post_delete exception on CRUDEvent creation. instance: {}, instance pk: {}".format(
                                 instance, instance.pk))
                     except Exception:
                         pass
 
+                    raise e
+
             if getattr(settings, "TEST", False):
                 crud_flow()
             else:
                 transaction.on_commit(crud_flow, using=using)
     except Exception:
         logger.exception('easy audit had a post-delete exception.')
 
+        if should_propagate_exceptions():
+            raise
+
 
 if WATCH_MODEL_EVENTS:
     signals.post_save.connect(post_save, dispatch_uid='easy_audit_signals_post_save')
     signals.pre_save.connect(pre_save, dispatch_uid='easy_audit_signals_pre_save')
     signals.m2m_changed.connect(m2m_changed, dispatch_uid='easy_audit_signals_m2m_changed')
     signals.post_delete.connect(post_delete, dispatch_uid='easy_audit_signals_post_delete')
```

### Comparing `django-easy-audit-1.3.4b1/easyaudit/signals/request_signals.py` & `django-easy-audit-1.3.4b2/easyaudit/signals/request_signals.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/templates/admin/easyaudit/purge_confirmation.html` & `django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/purge_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b1/easyaudit/utils.py` & `django-easy-audit-1.3.4b2/easyaudit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,7 +75,15 @@
     :type new: Model
     :return: ManyToManyField name of instance related to model.
     :rtype: str
     """
     for x in model._meta.related_objects:
         if x.related_model().__class__ == instance.__class__:
             return x.remote_field.name
+
+
+def should_propagate_exceptions():
+    """
+    Should Django Easy Audit propagate signal handler exceptions.
+    :rtype: bool
+    """
+    return getattr(settings, 'DJANGO_EASY_AUDIT_PROPAGATE_EXCEPTIONS', False)
```

### Comparing `django-easy-audit-1.3.4b1/setup.py` & `django-easy-audit-1.3.4b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-easy-audit',
-    version='1.3.4.b1',
+    version='1.3.4.b2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "django>=2.2,<5.0"
     ],
     python_requires=">=3.5",
```

