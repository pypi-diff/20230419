# Comparing `tmp/django-common-task-system-1.1.8.tar.gz` & `tmp/django-common-task-system-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.8.tar", last modified: Tue Apr 18 06:28:24 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.9.tar", last modified: Wed Apr 19 07:40:38 2023, max compression
```

## Comparing `django-common-task-system-1.1.8.tar` & `django-common-task-system-1.1.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.086859 django-common-task-system-1.1.8/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.8/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     9800 2023-04-17 08:40:58.000000 django-common-task-system-1.1.8/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.8/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.8/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.8/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.8/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.098240 django-common-task-system-1.1.8/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.1.8/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    34023 2023-04-18 02:49:48.000000 django-common-task-system-1.1.8/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.8/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.8/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.070854 django-common-task-system-1.1.8/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.070854 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.099247 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.101249 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.108444 django-common-task-system-1.1.8/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.113959 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    17147 2023-04-18 02:49:48.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.114958 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.116958 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.120527 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.072862 django-common-task-system-1.1.8/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.072862 django-common-task-system-1.1.8/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.121534 django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     6709 2023-04-14 09:00:33.000000 django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.124535 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.8/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.8/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.128534 django-common-task-system-1.1.8/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.8/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.8/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.8/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.8/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.8/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.8/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.093549 django-common-task-system-1.1.8/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4253 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-18 06:24:58.000000 django-common-task-system-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.128534 django-common-task-system-1.1.8/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.817973 django-common-task-system-1.1.9/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.9/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    10500 2023-04-19 07:34:32.000000 django-common-task-system-1.1.9/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.9/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.9/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.9/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.9/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.885397 django-common-task-system-1.1.9/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.1.9/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    34061 2023-04-18 07:40:32.000000 django-common-task-system-1.1.9/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.9/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.9/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.729770 django-common-task-system-1.1.9/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.729770 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.888471 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.890480 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.954847 django-common-task-system-1.1.9/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.999563 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    17296 2023-04-18 07:39:59.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.006346 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.014357 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2660 2023-04-18 07:30:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.049153 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.732264 django-common-task-system-1.1.9/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.732264 django-common-task-system-1.1.9/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.050665 django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.059873 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.9/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.9/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.084087 django-common-task-system-1.1.9/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.9/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.9/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.9/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.9/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.9/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.9/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.838748 django-common-task-system-1.1.9/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4253 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-19 07:38:37.000000 django-common-task-system-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.085086 django-common-task-system-1.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.9/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.8/LICENSE` & `django-common-task-system-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/__init__.py` & `django-common-task-system-1.1.9/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/admin.py` & `django-common-task-system-1.1.9/django_common_task_system/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -136,47 +136,62 @@
             return "每%s秒" % type_config.get('period', '')
         elif schedule_type == TaskScheduleType.TIMINGS:
             return ScheduleTimingType[config[schedule_type]['type']].label
         return '-'
     schedule_sub_type.short_description = '详细'
 
     def put(self, obj):
-        url = reverse(self.schedule_put_name) + '?i=%s' % obj.id
-        templates = ""
         now = datetime.now()
+        url = reverse(self.schedule_put_name) + '?i=%s' % obj.id
+        templates = '''
+            <div style="padding: 10px; border-bottom: 1px solid black">
+                <div>
+                    <span>计划日期</span>
+                    <input type="text" value="%s" class="vDateField">
+                </div>
+                <span>计划时间</span>
+                <input type="text" value="%s" class="vTimeField">
+            </div>
+        ''' % (now.strftime('%Y-%m-%d'), now.strftime('%H:%M:%S'))
         for queue in self.queues.values():
-            queue_url = url + '&q=%s&t=%s' % (queue.code, now.strftime('%Y-%m-%d %H:%M:%S'))
+            queue_url = url + '&q=%s' % queue.code
             templates += """
                 <li>
-                    <a href="%s" target="_blank"><div>%s</div></a>
+                    <a href="javascript:void(0);" onclick="put_schedule('%s', %s)"><div>%s</div></a>
                 </li>
-            """ % (queue_url, queue.name)
+            """ % (queue_url, obj.id, queue.name,)
         return mark_safe(
             '''
-                <div class="schedule_box">
+            
+                <div class="schedule_box" id="schedule_box_%s">
                     <span class="pop_ctrl" style="padding:5px;border:none;color: var(--secondary)">加入队列</span>
                     <ul>%s</ul>
                 </div>
                 
-            ''' % templates
+            ''' % (obj.id, templates)
         )
     put.allow_tags = True
     put.short_description = '调度'
 
     class Media:
         js = (
             'https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js',
             'https://cdn.bootcss.com/popper.js/1.14.3/umd/popper.min.js',
             'https://cdn.bootcss.com/bootstrap/4.1.3/js/bootstrap.min.js',
             # reverse('admin:jsi18n'),
             'common_task_system/js/task_schedule_admin.js',
+            'common_task_system/js/calendar.js',
+            'admin/js/calendar.js',
+            'admin/js/admin/DateTimeShortcuts.js'
         )
         css = {
             'all': (
                 'common_task_system/css/task_schedule_admin.css',
+                'admin/css/base.css',
+                'admin/css/forms.css',
             )
         }
 
 
 class TaskScheduleLogAdmin(UserAdmin):
     schedule_retry_name = 'task_schedule_retry'
     list_display = ('id', 'schedule', 'status', 'retry', 'schedule_time', 'create_time')
```

### Comparing `django-common-task-system-1.1.8/django_common_task_system/choices.py` & `django-common-task-system-1.1.9/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/fields.py` & `django-common-task-system-1.1.9/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/forms.py` & `django-common-task-system-1.1.9/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.9/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.1.9/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.1.9/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.1.9/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/mixin.py` & `django-common-task-system-1.1.9/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/models.py` & `django-common-task-system-1.1.9/django_common_task_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,15 @@
     result = common_fields.ConfigField(blank=True, null=True, verbose_name='结果')
     schedule_time = models.DateTimeField(verbose_name='计划时间')
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
 
     class Meta:
         db_table = 'task_schedule_log'
         verbose_name = verbose_name_plural = '任务日志'
+        ordering = ('-create_time',)
         abstract = True
 
     def __str__(self):
         return "schedule: %s, status: %s" % (self.schedule, self.status)
 
     __repr__ = __str__
```

### Comparing `django-common-task-system-1.1.8/django_common_task_system/permissions.py` & `django-common-task-system-1.1.9/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/serializers.py` & `django-common-task-system-1.1.9/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/models.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             },
         )[0]
 
         interval = 1
         unit = 'month'
         self.system_log_cleaning = SystemTask.objects.get_or_create(
             name='系统日志清理',
-            parent=self.shell_execution_parent_task,
+            parent=self.sql_execution_parent_task,
             category=self.system_default_category,
             user=user,
             defaults={
                 'config': {
                     'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
                            (SystemScheduleLog._meta.db_table, interval, unit)
                 },
@@ -242,15 +242,15 @@
 
         interval = 1
         unit = 'month'
         self.task_log_cleaning = SystemTask.objects.get_or_create(
             name='任务日志清理',
             user=user,
             category=self.system_default_category,
-            parent=self.shell_execution_parent_task,
+            parent=self.sql_execution_parent_task,
             defaults={
                 'config': {
                     'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
                            (TaskScheduleLog._meta.db_table, interval, unit)
                 },
             }
         )[0]
@@ -377,24 +377,27 @@
                 "schedule_type": "S"
             }
         }
 
         self.test_sql_execution = SystemSchedule.objects.get_or_create(
             task=tasks.test_sql_execution,
             user=user,
+            status=TaskScheduleStatus.TEST.value,
             defaults=defaults
         )[0]
         self.test_sql_produce = SystemSchedule.objects.get_or_create(
             task=tasks.test_sql_produce,
             user=user,
+            status=TaskScheduleStatus.TEST.value,
             defaults=defaults
         )[0]
         self.test_shell_execution = SystemSchedule.objects.get_or_create(
             task=tasks.test_shell_execution,
             user=user,
+            status=TaskScheduleStatus.TEST.value,
             defaults=defaults
         )[0]
 
 
 class BuiltinConsumerPermissions(BaseConsumerPermissions):
     model = SystemConsumerPermission
```

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/process.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task/views.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,32 +4,22 @@
 import requests
 from queue import Queue, Empty
 from datetime import datetime
 from django.urls import reverse
 from .executors import Executors
 from . import settings
 from urllib.parse import urljoin
-from django_common_task_system.system_task.models import SystemSchedule, SystemTask, builtins
+from django_common_task_system.system_task.models import SystemSchedule, SystemTask
 from django_common_task_system.models import TaskScheduleCallback
-from django_common_task_system.choices import TaskScheduleStatus
+
 
 system_task_queue = Queue()
 logger = settings.logger
 
 
-def query_system_schedule():
-
-    now = datetime.now()
-    queryset = SystemSchedule.objects.filter(next_schedule_time__lte=now, status=TaskScheduleStatus.OPENING.value)
-    for schedule in queryset:
-        system_task_queue.put(copy.deepcopy(schedule))
-        schedule.generate_next_schedule()
-    return queryset
-
-
 def request_system_schedule():
 
     url = urljoin(settings.HOST, reverse('system_schedule_get', args=('opening', )))
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
         callback = result.pop('callback')
@@ -58,22 +48,14 @@
 
 def get_system_schedule():
     while True:
         schedule = request_system_schedule()
         if schedule:
             return schedule
         time.sleep(1)
-    # try:
-    #     return system_task_queue.get(timeout=2)
-    # except Empty:
-    #     logger.debug('\r[%s]%s' % (time.strftime('%Y-%m-%d %H:%M:%S'), 'waiting for system schedule...'))
-    #     query_system_schedule()
-    #     if system_task_queue.empty():
-    #         request_system_schedule()
-    # return get_system_schedule()
 
 
 def get_schedule_executor(schedule):
     try:
         if not schedule.task.parent:
             raise KeyError
         cls = Executors[schedule.task.parent.name]
```

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     </style>
   {% endif %}
 {% endblock %}
 
 
 {% block extrahead %}
 {{ block.super }}
+<script type="text/javascript">window.__admin_media_prefix__ = "{% filter escapejs %}{% static 'admin/' %}{% endfilter %}";</script>
 {{ media.js }}
 <script src="{% static 'admin/js/filters.js' %}" defer></script>
 {% endblock %}
 
 {% block bodyclass %}{{ block.super }} app-{{ opts.app_label }} model-{{ opts.model_name }} change-list{% endblock %}
 
 {% if not is_popup %}
@@ -36,14 +37,15 @@
 </div>
 {% endblock %}
 {% endif %}
 
 {% block coltype %}{% endblock %}
 
 {% block content %}
+  <div id="option-msg" style="text-align: center; color: red"></div>
   <div id="content-main">
     {% block object-tools %}
         <ul class="object-tools">
           {% block object-tools-items %}
             {% change_list_object_tools %}
           {% endblock %}
         </ul>
@@ -83,16 +85,47 @@
           </div>
         {% endif %}
       {% endblock %}
     </div>
   </div>
 
     <script>
-        (function ($) {
+        function put_schedule(base_url, schedule_id){
+            const schedule_box = $('#schedule_box_' + schedule_id);
+            let date = schedule_box.find('input[class="vDateField"]').val();
+            let time = schedule_box.find('input[class="vTimeField"]').val();
+            if(date === ""){
+                date = new Date().toLocaleDateString();
+            }
+            if (time === ""){
+                time = new Date().toLocaleTimeString();
+            }
+            if(time.split(':').length === 2){
+                time = time + ':00'
+            }
+            const url = base_url + '&t=' + date.replaceAll('/', '-') + ' ' + time;
+            $.ajax({
+                url: url,
+                dataType: 'json',
+                contentType: 'application/json; charset=utf-8',
+                success: function(data){
+                    $('#option-msg').text("加入成功");
+                    $(document).trigger('mouseup');
+                    setTimeout(function(){
+                        $('#option-msg').text("");
+                    }, 1000);
+                },
+                error: function(data){
+                    console.debug(data);
+                    alert(JSON.stringify(JSON.parse(data.responseText)));
+                }}
+            );
+        }
 
+        (function ($) {
             $.fn.popmenu = function (options) {
                 var settings = $.extend({
                     'controller': true,
                     'width': '300px',
                     'background': '#34495e',
                     'focusColor': '#1abc9c',
                     'borderRadius': '10px',
@@ -166,12 +199,12 @@
                     });
                 }
                 return setIt();
 
             };
         }(jQuery));
         $('.schedule_box').each(function () {
-            $(this).popmenu();
+            $(this).popmenu({background: '#79aec8', color: 'black'});
         });
     </script>
 {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/urls.py` & `django-common-task-system-1.1.9/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.9/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.9/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.9/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system/views.py` & `django-common-task-system-1.1.9/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.9/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.8/setup.py` & `django-common-task-system-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.8',
+    version='1.1.9',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

